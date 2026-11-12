代发 wailian999

[Q86] 读取 JSON 字段
来源：http://asj.jinyuanbaomall.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hlv.hammf.cn

[Q87] JSON 字段做条件
来源：http://jgp.zhijiandao.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://avo.jqgufenzy.top

[Q88] 行转列（条件聚合）
来源：http://fsq.zhoulong.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xqd.aizwys.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nqw.jinqigufen.top

[Q89] 判断表是否存在
来源：http://fze.yuxming.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uim.zhoulong.xyz

[Q90] 生成序号列
来源：http://nob.dashuyun.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ffn.hcnkem.com

================================================================================
来源：http://sei.chenzaomai.com

R. Bash 专题
来源：http://buc.wangdashe.top

================================================================================
来源：http://uun.jianghu66.top

[R01] shebang 与严格模式
来源：http://tnw.ctjpmb.com

#!/usr/bin/env bash
来源：http://wvx.uphjek.com

set -euo pipefail
来源：http://buk.shanyushiyangtech.top

[R02] 变量赋值与使用
来源：http://hqi.xziqi.cn

name="Tom"; echo "$name"
来源：http://ctk.andypj.xyz

[R03] 只读变量
来源：http://zeg.jqgufenzy.top

readonly PI=3.14
来源：http://fjj.chenzaomai.com

[R04] 位置参数
来源：http://bpn.yongpay.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://skq.xinyue.icu

[R05] 参数默认值
来源：http://uae.yj202588.top

name="${1:-default}"
来源：http://xrv.pengpengdd.cyou

[R06] 判断命令是否存在
来源：http://cra.shzxlz.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yss.ivvv.top

[R07] if 判断文件
来源：http://htm.tianlin.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hlv.9152youxi.cn

[R08] 数值比较
来源：http://isu.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kwb.zhongyouzk.top

[R09] 字符串比较
来源：http://vjo.hongshengwenyu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ahu.hfpthk.cn

[R10] 正则匹配
来源：http://bfn.jyoumei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rdl.jinqigfzy.top

[R11] case 多分支
来源：http://xwa.aibaodan.cn

case "$1" in
来源：http://irl.tarul.cn

start) echo "启动" ;;
来源：http://aiy.cdnleiting.top

stop)  echo "停止" ;;
来源：http://wsu.xuanzx.com

*)     echo "未知命令" ;;
来源：http://dgz.jinqigufen.top

esac
来源：http://yju.sufxvd.cn

[R12] for 遍历文件
来源：http://mzj.yfazqb.com

for f in *.txt; do echo "$f"; done
来源：http://fko.cashguo.top

[R13] for 计数循环
来源：http://eie.ydjk.org.cn

for i in {1..10}; do echo "$i"; done
来源：http://zcr.ywan-chungtsiang.top

[R14] C 风格 for
来源：http://hja.meibo888.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://chx.0kj1m.cn

[R15] while 逐行读文件
来源：http://fhi.sxryk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ljy.fengsongda.top

[R16] until 等待条件
来源：http://lxf.guowangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ied.zycfv.cn

[R17] 数组定义与取值
来源：http://oyl.jyoumei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lno.daxiang520.top

[R18] 遍历数组
来源：http://hkc.smart0.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zyp.hywenlv.cn

[R19] 数组长度
来源：http://qfo.nanxinkj.top

echo "${#arr[@]}"
来源：http://pqf.bjfxy.top

[R20] 关联数组（字典）
来源：http://jem.hnqzz.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://htp.hongshengwenyu.top

[R21] 字符串长度
来源：http://xvz.gogol.net.cn

echo "${#s}"
来源：http://rbd.shanyushiyangkeji.top

[R22] 截取子串
来源：http://oxo.zhaomingkeji.xyz

echo "${s:0:5}"
来源：http://zyy.hfpthk.cn

[R23] 字符串替换
来源：http://zit.yonumen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jxn.jqgufenzy.top

[R24] 大小写转换
来源：http://zgv.dianchejie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ckk.shzxlz.cn

[R25] 去后缀 / 去前缀
来源：http://eij.zhengqikj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://odt.cdnleiting.top

[R26] 命令替换
来源：http://wem.hammf.cn

now=$(date +%F); echo "$now"
来源：http://skn.jyoumei.cn

[R27] 算术展开
来源：http://rfp.zdqjudy.top

echo $((1 + 2 * 3))
来源：http://joe.ppjwa.cn

[R28] 浮点运算
来源：http://hvt.nanxuanxn.top

echo "scale=2; 10/3" | bc
来源：http://rxi.jinghuilouyu.cn

[R29] 定义函数
来源：http://xtt.zhijiandao.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xyu.fehbvm.com

[R30] 函数返回状态码
来源：http://uxq.mhx1999.top

f() { return 0; }; f || echo "失败了"
来源：http://flb.jlsjyb.cn

[R31] 局部变量
来源：http://szu.haohaochexian.top

f() { local x=1; echo "$x"; }
来源：http://xok.zhixingplan.top

[R32] 参数个数校验
来源：http://wkq.jinyuanbaomall.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iyg.sweek.top

[R33] 捕获错误并提示行号
来源：http://uun.iojbl.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kct.kuanghao11.cn

[R34] 退出时清理
来源：http://jca.andypj.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://ccq.pengpengdd.cyou

[R35] 后台执行并等待
来源：http://fic.fehbvm.com

sleep 5 & pid=$!; wait "$pid"
来源：http://jln.sufxvd.cn

[R36] 并发执行多个任务
来源：http://hlm.xingfuxueyuan.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wyh.smart0.xyz

[R37] 把输出赋给变量
来源：http://dpw.c1oappe.top

files=$(ls -1)
来源：http://qvh.jianghu66.top

[R38] 管道串联
来源：http://mzl.pycfn.com

cat a.txt | grep -i error | wc -l
来源：http://vky.hfpthk.cn

[R39] 重定向标准输出与错误
来源：http://gfu.aizwys.cn

cmd > out.log 2>&1
来源：http://oyv.tianlin.xyz

[R40] 追加写日志
来源：http://rlq.hfpthk.cn

echo "log" >> out.log
来源：http://cbg.andypj.xyz

[R41] 丢弃输出
来源：http://oig.zhixingplan.top

cmd >/dev/null 2>&1
来源：http://ptm.yueranfly.top

[R42] 输入重定向
来源：http://jot.yfazqb.com

wc -l < a.txt
来源：http://rat.jlsjyb.cn

[R43] 按名字查找文件
来源：http://enz.daxiang520.top

find . -name "*.log" -type f
来源：http://nmu.yanxiufei.cn

[R44] 按修改时间查找
来源：http://kvn.chenlongwang.top

find . -mtime -7 -type f
来源：http://nur.fengsongda.top

[R45] 批量删除
来源：http://pdf.tian-w.cn

find . -name "*.tmp" -delete
来源：http://wxh.zdbjq.cn

[R46] 递归替换文件内容
来源：http://act.smart0.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://irx.ehwqpu.com

[R47] sed 单行替换
来源：http://tbx.yj20258.top

sed -i 's/foo/bar/g' a.txt
来源：http://bcu.ivvv.top

[R48] awk 取指定列
来源：http://eek.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://qoh.tarul.cn

[R49] awk 带条件
来源：http://exd.zhengqikj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vss.sxryk.cn

[R50] awk 求和
来源：http://zwa.bbcook.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mqp.bbcook.cn

[R51] 排序去重取前几
来源：http://upd.sjlbkw.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mzw.yj202588.top

[R52] 统计行数
来源：http://ten.redwolf501.top

wc -l a.txt
来源：http://koz.snrcjt.cn

[R53] 查看文件头与实时尾
来源：http://lhk.guowangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://btx.sufxvd.cn

[R54] 比较两个文件
来源：http://gqz.sufxvd.cn

diff a.txt b.txt
来源：http://hfj.hywenlv.cn

[R55] 压缩与解压
来源：http://tvy.zdqjudy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xdj.dianchejie.cn

[R56] 远程拷贝
来源：http://fnn.smart0.xyz

scp file user@host:/path/
来源：http://tyb.dashuyun.cn

[R57] 远程执行命令
来源：http://csl.guannengcc.top

ssh user@host 'uptime'
来源：http://utg.jqgfzy.top

[R58] 下载文件
来源：http://qqk.yj202588.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gtv.cucudq.cn

[R59] 发 POST JSON
来源：http://oyc.wangshuangyany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://olg.shangyingyoupin.top

[R60] 只看 HTTP 状态码
来源：http://yot.haohaochexian.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tiy.tanke756.top

[R61] 磁盘占用
来源：http://kzx.gogol.net.cn

df -h;  du -sh *
来源：http://elj.snrcjt.cn

[R62] 找最占空间的文件
来源：http://ajw.nanxuanxn.top

du -ah . | sort -rh | head -10
来源：http://qwv.aizwys.cn

[R63] 内存与进程
来源：http://iou.hywenlv.cn

free -h;  ps aux | grep nginx
来源：http://wns.dashuyun.cn

[R64] 结束进程
来源：http://etu.aibaodan.cn

kill -9 $(pgrep -f app.py)
来源：http://ihh.cdnleiting.top

[R65] 查看端口占用
来源：http://fra.hcnkem.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dzx.yj20258888.top

[R66] 定时任务
来源：http://ygz.zhaomingkeji.xyz

crontab -e;  crontab -l
来源：http://hdp.guowangkeji.top

[R67] 生成随机十六进制串
来源：http://dlk.jqgufenzy.top

openssl rand -hex 16
来源：http://kap.yanxiufei.cn

[R68] 计算文件校验值
来源：http://tbd.havefunace.top

sha256sum a.txt;  md5sum a.txt
来源：http://epz.jiagoushi.top

[R69] 生成随机密码
来源：http://nqd.svipenyu.cn

head -c 16 /dev/urandom | base64
来源：http://jil.fehbvm.com

[R70] 时间戳与互转
来源：http://pbp.guowangkeji.top

date +%s;  date -d @1700000000
来源：http://fzy.zhijiandao.cn

[R71] 日期格式化
来源：http://iou.jinqigufen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mnk.bjfxy.top

[R72] 等待端口就绪
来源：http://iqd.jianghu66.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vdv.ydzc1.top

[R73] 分割大日志
来源：http://eev.fehbvm.com

split -l 1000 big.log part_
来源：http://alt.hesvh.cn

[R74] 批量重命名
来源：http://utc.xuanzx.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pdx.ybcxt.top

[R75] 导出环境变量
来源：http://puw.yanxiufei.cn

export PATH="$HOME/bin:$PATH"
来源：http://ixn.vehdjk.com

[R76] 使用临时文件
来源：http://jey.yueranfly.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wut.nanxinkj.top

[R77] 读取用户输入
来源：http://nme.jinghuilouyu.cn

read -rp "请输入: " ans
来源：http://hdq.vqdsnc.cn

[R78] 交互式菜单
来源：http://lyg.aizwys.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ykj.jyoumei.cn

[R79] 解析命令行选项
来源：http://xpr.zhongyouzk.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hvs.shuidangran.top

[R80] 查看脚本执行耗时
来源：http://ojj.nanxinkj.top

time ./run.sh
来源：http://ksz.zdbjq.cn

================================================================================
来源：http://ohn.bbcook.cn

S. C / C++ 专题
来源：http://siy.zycfv.cn

================================================================================
来源：http://hxu.guowangkeji.top

[S01] C：Hello World
来源：http://owx.meibo888.top

#include <stdio.h>
来源：http://jxc.xinyue.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://ohk.316326.xyz

[S02] C：变量与格式化输出
来源：http://hgl.xingfuxueyuan.xyz

int a = 10; printf("%d\n", a);
来源：http://kie.cheryme.top

[S03] C：读入整数
来源：http://moz.andypj.xyz

int x; scanf("%d", &x);
来源：http://lsx.chenlongwang.top

[S04] C：字符串复制
来源：http://nas.sxryk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sdm.yangfankeji.com

[S05] C：字符串长度
来源：http://not.daxiang520.top

strlen(s)
来源：http://mfr.pycfn.com

[S06] C：字符串比较
来源：http://eyi.yueranfly.top

strcmp(a, b) == 0
来源：http://kfv.gogol.net.cn

[S07] C：数组遍历求和
来源：http://uaz.zhixingplan.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xnm.nwbrower.top

[S08] C：动态内存分配与释放
来源：http://pfo.wangdashe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rwk.chenjidiqi.icu

[S09] C：结构体定义与初始化
来源：http://lww.zhixingplan.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kmr.316326.xyz

[S10] C：指针与解引用
来源：http://grs.ybcxt.top

int *p = &a;  *p = 5;
来源：http://imv.cashguo.top

[S11] C：逐行读文件
来源：http://tdl.ydjk.org.cn

FILE *f = fopen("a.txt", "r");
来源：http://toa.ywan-chungtsiang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://miw.jinghuilouyu.cn

fclose(f);
来源：http://zeh.zhoulong.xyz

[S12] C：写文件
来源：http://lef.jlsjyb.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tln.shanyushiyangkeji.top

[S13] C：宏定义
来源：http://hrn.zdbjq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eyu.gotoacloud.top

[S14] C：枚举
来源：http://sma.gaohongyu789.top

enum Color { RED, GREEN, BLUE };
来源：http://zid.cdnleiting.top

[S15] C：类型转换
来源：http://swa.feifeiyinyue.top

(double) a / b
来源：http://fud.ctjpmb.com

[S16] C：位操作置位
来源：http://ccg.jinghuilouyu.cn

x |= (1 << 3);
来源：http://zmb.tian-w.cn

[S17] C：安全拼接字符串
来源：http://nvr.zhoulong.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rnj.hfpthk.cn

[S18] C：命令行参数
来源：http://qzw.sufxvd.cn

int main(int argc, char **argv)
来源：http://bqz.guowangkeji.top

[S19] C：快速排序
来源：http://gjl.cashguo.top

qsort(a, n, sizeof(int), cmp);
来源：http://krd.yj20258.top

[S20] C：二分查找
来源：http://eeg.yongpay.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://czi.fengsongda.top

[S21] C：字符类别判断
来源：http://beu.xylfe.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jzt.vqdsnc.cn

[S22] C：字符串转数字
来源：http://xlk.chenzaomai.com

atoi("42");  strtod("3.14", NULL);
来源：http://axk.jqgfzy.top

[S23] C：随机数
来源：http://fiw.chenzaomai.com

srand(time(NULL));  int r = rand() % 100;
来源：http://smg.vqdsnc.cn

[S24] C：获取本地时间
来源：http://rrt.chenzaomai.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rpo.ybcxt.top

[S25] C：内存拷贝
来源：http://hcr.9152youxi.cn

memcpy(dst, src, n);
来源：http://bhj.jiagoushi.top

[S26] C：内存清零
来源：http://iem.yanxiufei.cn

memset(a, 0, sizeof a);
来源：http://yuw.zhoulong.xyz

[S27] C：定义常量
来源：http://apy.jinyuanbaomall.cn

const double PI = 3.14159;
来源：http://maq.hywenlv.cn

[S28] C：静态变量
来源：http://uie.redwolf501.top

static int counter = 0;
来源：http://aqk.zhiwuduotai.top

[S29] C：变参函数
来源：http://ash.fengsongda.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jph.havefunace.top

[S30] C：头文件保护
来源：http://adq.fzhhl.top

#ifndef X_H
来源：http://mdq.nanxinkj.top

#define X_H
来源：http://gbu.fktsv.cn

#endif
来源：http://dir.redwolf501.top

[S31] C++：Hello World
来源：http://ojh.ehwqpu.com

#include <iostream>
来源：http://wmq.zdbjq.cn

int main() { std::cout << "Hello\n"; }
来源：http://kud.pengpengdd.cyou

[S32] C++：字符串
来源：http://vzg.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://qtz.jqgufenzy.top

[S33] C++：vector 增删
来源：http://iob.zdqjudy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lva.hesvh.cn

[S34] C++：遍历 vector
来源：http://dra.jinqigufen.top

for (auto &x : v) { std::cout << x; }
来源：http://nhj.jqgufenzy.top

[S35] C++：map
来源：http://oxx.hysaishi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cke.wangshuangyany.cn

[S36] C++：unordered_map
来源：http://jil.xinyue.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://osi.quarkkingdee.top

[S37] C++：set
来源：http://kqk.jinqigufen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uhj.bjfxy.top

[S38] C++：排序
来源：http://jxf.dashuyun.cn

std::sort(v.begin(), v.end());
来源：http://xsg.hywenlv.cn

[S39] C++：自定义比较器排序
来源：http://zfq.pycfn.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cwd.fzhhl.top

[S40] C++：查找元素
来源：http://oog.52xcode.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wpg.52xcode.cn

[S41] C++：类与构造函数
来源：http://sfx.yonumen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gbn.hammf.cn

[S42] C++：继承与虚函数
来源：http://uos.pengpengdd.cyou

class B : public Base { public: void f() override {} };
来源：http://yct.uphjek.com

[S43] C++：智能指针
来源：http://rto.cdnleiting.top

auto p = std::make_unique<int>(5);
来源：http://jic.yj20258888.top

[S44] C++：引用传参
来源：http://rmw.sufxvd.cn

void inc(int &x) { ++x; }
来源：http://tvk.guannengcc.top

[S45] C++：lambda
来源：http://nkn.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cjq.chenzaomai.com

[S46] C++：函数模板
来源：http://vxb.zhengqikj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iso.guannengcc.top

[S47] C++：结构化绑定遍历
来源：http://txv.daxiang520.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nzn.ppjwa.cn

[S48] C++：逐行读文件
来源：http://wtk.zdqjudy.top

std::ifstream in("a.txt");  std::string line;
来源：http://kiq.yj202588.top

while (std::getline(in, line)) { }
来源：http://pka.aibaodan.cn

[S49] C++：写文件
来源：http://slj.bbcook.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uhp.chenjidiqi.icu

[S50] C++：格式化数字
来源：http://spw.jiagoushi.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vgt.wangdashe.top

[S51] C++：显式类型转换
来源：http://vok.smart0.xyz

static_cast<double>(a) / b
来源：http://yfn.fanxiaobao.xyz

[S52] C++：const 与 noexcept
来源：http://sji.quarkkingdee.top

int size() const noexcept { return n_; }
来源：http://mqa.cucudq.cn

[S53] C++：移动语义
来源：http://lag.hfpthk.cn

std::vector<int> w = std::move(v);
来源：http://mqk.xingfuxueyuan.xyz

[S54] C++：异常处理
来源：http://yzi.ppjwa.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bff.shanyushiyangtech.top

[S55] C++：结构化绑定
来源：http://jhu.cheryme.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xyv.dianchejie.cn

[S56] C++：optional
来源：http://wvi.redwolf501.top


<!-- 参考信息 -->