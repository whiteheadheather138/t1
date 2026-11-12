代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://ehb.mhx1999.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zrb.cashguo.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pcy.sxryk.cn

[Q89] 判断表是否存在
来源：http://nsn.9152youxi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fdz.0kj1m.cn

[Q90] 生成序号列
来源：http://xle.gzhubu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ipv.zhengqikj.top

================================================================================
来源：http://cps.yvedp.cn

R. Bash 专题
来源：http://zll.shanyushiyangtech.top

================================================================================
来源：http://hin.andypj.xyz

[R01] shebang 与严格模式
来源：http://sdf.gzhubu.top

#!/usr/bin/env bash
来源：http://utm.zhaomingkeji.xyz

set -euo pipefail
来源：http://bfv.wangdashe.top

[R02] 变量赋值与使用
来源：http://bvo.fengsongda.top

name="Tom"; echo "$name"
来源：http://xch.fzhhl.top

[R03] 只读变量
来源：http://dbi.aizwys.cn

readonly PI=3.14
来源：http://qqb.9152youxi.cn

[R04] 位置参数
来源：http://hmu.fzhhl.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rsh.xuanzx.com

[R05] 参数默认值
来源：http://nev.316326.xyz

name="${1:-default}"
来源：http://jzg.tanke756.top

[R06] 判断命令是否存在
来源：http://meb.quarkkingdee.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wxb.jinghuilouyu.cn

[R07] if 判断文件
来源：http://qyz.shangyingyoupin.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hvn.zycfv.cn

[R08] 数值比较
来源：http://syy.ppjwa.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ljw.hfpthk.cn

[R09] 字符串比较
来源：http://jsa.wangdashe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zwx.andypj.xyz

[R10] 正则匹配
来源：http://kcf.9152youxi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zob.tarul.cn

[R11] case 多分支
来源：http://ork.jinyuanbaomall.cn

case "$1" in
来源：http://wtj.feifeiyinyue.top

start) echo "启动" ;;
来源：http://bty.sweek.top

stop)  echo "停止" ;;
来源：http://wsk.tianlin.xyz

*)     echo "未知命令" ;;
来源：http://ryf.haohaochexian.top

esac
来源：http://zrj.hnqzz.top

[R12] for 遍历文件
来源：http://wbg.redwolf501.top

for f in *.txt; do echo "$f"; done
来源：http://tnp.haohaochexian.top

[R13] for 计数循环
来源：http://dog.zycfv.cn

for i in {1..10}; do echo "$i"; done
来源：http://lpi.hcnkem.com

[R14] C 风格 for
来源：http://bjc.yfazqb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bpn.cashguo.top

[R15] while 逐行读文件
来源：http://qdl.dianchejie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ofu.zhijiandao.cn

[R16] until 等待条件
来源：http://tyq.yuxming.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ltd.gzhubu.top

[R17] 数组定义与取值
来源：http://anq.cheryme.top

arr=(a b c); echo "${arr[0]}"
来源：http://icu.ctjpmb.com

[R18] 遍历数组
来源：http://flh.wangshuangyany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ipx.jqgufenzy.top

[R19] 数组长度
来源：http://sek.xziqi.cn

echo "${#arr[@]}"
来源：http://gzi.hnqzz.top

[R20] 关联数组（字典）
来源：http://idw.jinqigufen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://olq.yj20258.top

[R21] 字符串长度
来源：http://kwt.yfazqb.com

echo "${#s}"
来源：http://kio.316326.xyz

[R22] 截取子串
来源：http://vng.zhixingplan.top

echo "${s:0:5}"
来源：http://kvo.hammf.cn

[R23] 字符串替换
来源：http://uwf.gaohongyu789.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tgz.yj20258.top

[R24] 大小写转换
来源：http://kls.fzhhl.top

echo "${s^^}"; echo "${s,,}"
来源：http://ylo.guowangkeji.top

[R25] 去后缀 / 去前缀
来源：http://pot.yuxming.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dgj.sufxvd.cn

[R26] 命令替换
来源：http://yla.aizwys.cn

now=$(date +%F); echo "$now"
来源：http://sdt.wangdashe.top

[R27] 算术展开
来源：http://xad.zycfv.cn

echo $((1 + 2 * 3))
来源：http://nqk.shzxlz.cn

[R28] 浮点运算
来源：http://ewz.zhixingplan.top

echo "scale=2; 10/3" | bc
来源：http://iwj.nwbrower.top

[R29] 定义函数
来源：http://psd.ydzc1.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kcf.xylfe.cn

[R30] 函数返回状态码
来源：http://ppp.tanke756.top

f() { return 0; }; f || echo "失败了"
来源：http://luj.xziqi.cn

[R31] 局部变量
来源：http://obg.andypj.xyz

f() { local x=1; echo "$x"; }
来源：http://tea.ivvv.top

[R32] 参数个数校验
来源：http://vvu.shzxlz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eok.guannengcc.top

[R33] 捕获错误并提示行号
来源：http://kwe.zhengqikj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://emh.cashguo.top

[R34] 退出时清理
来源：http://esv.cashguo.top

trap 'rm -f "$tmp"' EXIT
来源：http://sqi.tianlin.xyz

[R35] 后台执行并等待
来源：http://xpv.xinyue.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://kqx.zdbjq.cn

[R36] 并发执行多个任务
来源：http://vrg.bbcook.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hes.ydjk.org.cn

[R37] 把输出赋给变量
来源：http://cjk.jinghuilouyu.cn

files=$(ls -1)
来源：http://vdh.pycfn.com

[R38] 管道串联
来源：http://amj.jinghuilouyu.cn

cat a.txt | grep -i error | wc -l
来源：http://zpc.ctjpmb.com

[R39] 重定向标准输出与错误
来源：http://rso.jianghu66.top

cmd > out.log 2>&1
来源：http://jof.yj20258.top

[R40] 追加写日志
来源：http://tli.0kj1m.cn

echo "log" >> out.log
来源：http://ojs.bbcook.cn

[R41] 丢弃输出
来源：http://zah.cashguo.top

cmd >/dev/null 2>&1
来源：http://hqt.hongshengwenyu.top

[R42] 输入重定向
来源：http://wxz.yanxiufei.cn

wc -l < a.txt
来源：http://ifd.sufxvd.cn

[R43] 按名字查找文件
来源：http://juq.fzhhl.top

find . -name "*.log" -type f
来源：http://qgm.yueranfly.top

[R44] 按修改时间查找
来源：http://koo.andypj.xyz

find . -mtime -7 -type f
来源：http://dqs.wangshuangyany.cn

[R45] 批量删除
来源：http://ark.xuanzx.com

find . -name "*.tmp" -delete
来源：http://zfs.quarkkingdee.top

[R46] 递归替换文件内容
来源：http://icx.uphjek.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iwo.ehwqpu.com

[R47] sed 单行替换
来源：http://anl.meibo888.top

sed -i 's/foo/bar/g' a.txt
来源：http://qkh.zhoulong.xyz

[R48] awk 取指定列
来源：http://hwv.daria6918.cn

awk '{print $1, $3}' a.txt
来源：http://zqj.jiagoushi.top

[R49] awk 带条件
来源：http://keh.svipenyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://che.daxiang520.top

[R50] awk 求和
来源：http://kcc.yj20258888.top

awk '{s += $2} END {print s}' a.txt
来源：http://adt.tanke756.top

[R51] 排序去重取前几
来源：http://jbv.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://djx.zdbjq.cn

[R52] 统计行数
来源：http://nyj.jyoumei.cn

wc -l a.txt
来源：http://fka.hesvh.cn

[R53] 查看文件头与实时尾
来源：http://erq.pycfn.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://avi.pycfn.com

[R54] 比较两个文件
来源：http://xtk.zhongyouzk.top

diff a.txt b.txt
来源：http://zgu.ehwqpu.com

[R55] 压缩与解压
来源：http://rui.cashguo.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jpc.daria6918.cn

[R56] 远程拷贝
来源：http://tma.cdnleiting.top

scp file user@host:/path/
来源：http://vvw.chenzaomai.com

[R57] 远程执行命令
来源：http://mok.jianghu66.top

ssh user@host 'uptime'
来源：http://tkm.smart0.xyz

[R58] 下载文件
来源：http://qju.quarkkingdee.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ggi.shanyushiyangtech.top

[R59] 发 POST JSON
来源：http://kev.shangyingyoupin.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ujc.yueranfly.top

[R60] 只看 HTTP 状态码
来源：http://eul.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kqa.xuanzx.com

[R61] 磁盘占用
来源：http://alx.dashuyun.cn

df -h;  du -sh *
来源：http://xkv.zdbjq.cn

[R62] 找最占空间的文件
来源：http://ynh.pengpengdd.cyou

du -ah . | sort -rh | head -10
来源：http://afv.zhengqikj.top

[R63] 内存与进程
来源：http://vvo.ivvv.top

free -h;  ps aux | grep nginx
来源：http://syl.zhongyouzk.top

[R64] 结束进程
来源：http://ove.yanxiufei.cn

kill -9 $(pgrep -f app.py)
来源：http://sry.jinyuanbaomall.cn

[R65] 查看端口占用
来源：http://hvw.hcnkem.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://chr.gzhubu.top

[R66] 定时任务
来源：http://lkz.fzhhl.top

crontab -e;  crontab -l
来源：http://bdw.zhoulong.xyz

[R67] 生成随机十六进制串
来源：http://dyp.tanke756.top

openssl rand -hex 16
来源：http://ycc.jqgufenzy.top

[R68] 计算文件校验值
来源：http://veu.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nyi.xuanzx.com

[R69] 生成随机密码
来源：http://oht.fengsongda.top

head -c 16 /dev/urandom | base64
来源：http://cgn.shangyingyoupin.top

[R70] 时间戳与互转
来源：http://olh.hywenlv.cn

date +%s;  date -d @1700000000
来源：http://zbm.fengsongda.top

[R71] 日期格式化
来源：http://mkl.cdnleiting.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vqm.zdqjudy.top

[R72] 等待端口就绪
来源：http://egs.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qcj.iojbl.cn

[R73] 分割大日志
来源：http://znv.fanxiaobao.xyz

split -l 1000 big.log part_
来源：http://gav.gzhubu.top

[R74] 批量重命名
来源：http://cta.zdqjudy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zww.yonumen.top

[R75] 导出环境变量
来源：http://pvj.jinyuanbaomall.cn

export PATH="$HOME/bin:$PATH"
来源：http://vdl.sweek.top

[R76] 使用临时文件
来源：http://upb.yj202588.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cxk.zhiwuduotai.top

[R77] 读取用户输入
来源：http://qfs.cashguo.top

read -rp "请输入: " ans
来源：http://cqc.dashuyun.cn

[R78] 交互式菜单
来源：http://agb.hnqzz.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qzl.yj202588.top

[R79] 解析命令行选项
来源：http://cik.smart0.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jhc.cqqwz.cn

[R80] 查看脚本执行耗时
来源：http://qus.ybcxt.top

time ./run.sh
来源：http://jzs.mhx1999.top

================================================================================
来源：http://rzd.fanxiaobao.xyz

S. C / C++ 专题
来源：http://duq.smart0.xyz

================================================================================
来源：http://dcx.guowangkeji.top

[S01] C：Hello World
来源：http://nal.hammf.cn

#include <stdio.h>
来源：http://jmh.ehwqpu.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://fdb.quarkkingdee.top

[S02] C：变量与格式化输出
来源：http://vri.zhaomingkeji.xyz

int a = 10; printf("%d\n", a);
来源：http://vnj.jiagoushi.top

[S03] C：读入整数
来源：http://zoc.birdmap.top

int x; scanf("%d", &x);
来源：http://osd.yuanzhike.top

[S04] C：字符串复制
来源：http://zjs.316326.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://jeh.redwolf501.top

[S05] C：字符串长度
来源：http://xkd.yfazqb.com

strlen(s)
来源：http://mxa.haohaochexian.top

[S06] C：字符串比较
来源：http://hgx.fktsv.cn

strcmp(a, b) == 0
来源：http://eml.pengpengdd.cyou

[S07] C：数组遍历求和
来源：http://ugt.shanyushiyangkeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wez.316326.xyz

[S08] C：动态内存分配与释放
来源：http://jkc.yvedp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yrx.ehwqpu.com

[S09] C：结构体定义与初始化
来源：http://kqj.hnxiangtu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zho.yj20258.top

[S10] C：指针与解引用
来源：http://rah.c1oappe.top

int *p = &a;  *p = 5;
来源：http://uhn.xylfe.cn

[S11] C：逐行读文件
来源：http://uvn.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://aqp.yuanzhike.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://izw.iojbl.cn

fclose(f);
来源：http://soy.sufxvd.cn

[S12] C：写文件
来源：http://vnc.zhoulong.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ytb.shanyushiyangkeji.top

[S13] C：宏定义
来源：http://zbt.fanxiaobao.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wbf.daxiang520.top

[S14] C：枚举
来源：http://ouz.gaohongyu789.top

enum Color { RED, GREEN, BLUE };
来源：http://fhe.zhiwuduotai.top

[S15] C：类型转换
来源：http://mbo.fengsongda.top

(double) a / b
来源：http://dod.zycfv.cn

[S16] C：位操作置位
来源：http://mxw.ehwqpu.com

x |= (1 << 3);
来源：http://rcs.jinqigfzy.top

[S17] C：安全拼接字符串
来源：http://pyf.xinyue.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zyx.shzxlz.cn

[S18] C：命令行参数
来源：http://oys.daxiang520.top

int main(int argc, char **argv)
来源：http://ecq.yj202588.top

[S19] C：快速排序
来源：http://wte.gzhubu.top

qsort(a, n, sizeof(int), cmp);
来源：http://fvl.shangyingyoupin.top

[S20] C：二分查找
来源：http://kjg.fehbvm.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qyy.bbcook.cn

[S21] C：字符类别判断
来源：http://rsz.shanyushiyangtech.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bdw.sweek.top

[S22] C：字符串转数字
来源：http://rvx.cqqwz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sfm.sxryk.cn

[S23] C：随机数
来源：http://crq.jyoumei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tyt.9152youxi.cn

[S24] C：获取本地时间
来源：http://bfl.jinqigfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wkg.dashuyun.cn

[S25] C：内存拷贝
来源：http://zoy.zhoulong.xyz

memcpy(dst, src, n);
来源：http://ngt.bjfxy.top

[S26] C：内存清零
来源：http://jhy.snrcjt.cn

memset(a, 0, sizeof a);
来源：http://djh.tianlin.xyz

[S27] C：定义常量
来源：http://xih.yanxiufei.cn

const double PI = 3.14159;
来源：http://zfw.jiagoushi.top

[S28] C：静态变量
来源：http://frq.vehdjk.com

static int counter = 0;
来源：http://szx.nanxinkj.top

[S29] C：变参函数
来源：http://fpr.yj202588.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vui.yuxming.cn

[S30] C：头文件保护
来源：http://qxc.yuanzhike.top

#ifndef X_H
来源：http://ufe.hesvh.cn

#define X_H
来源：http://ivn.sweek.top

#endif
来源：http://gep.aizwys.cn

[S31] C++：Hello World
来源：http://etc.zycfv.cn

#include <iostream>
来源：http://qhd.ppjwa.cn

int main() { std::cout << "Hello\n"; }
来源：http://sci.xziqi.cn

[S32] C++：字符串
来源：http://uiv.tian-w.cn

std::string s = "hi";  s += "!";
来源：http://smr.yonumen.top

[S33] C++：vector 增删
来源：http://ydu.shzxlz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oip.jinqigfzy.top

[S34] C++：遍历 vector
来源：http://mcy.shzxlz.cn

for (auto &x : v) { std::cout << x; }
来源：http://bru.cdnleiting.top

[S35] C++：map
来源：http://vyc.xziqi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ryy.yj20258.top

[S36] C++：unordered_map
来源：http://wpk.fzhhl.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vjh.hnqzz.top

[S37] C++：set
来源：http://dek.sxryk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sij.ybcxt.top

[S38] C++：排序
来源：http://xxt.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://asq.fanxiaobao.xyz

[S39] C++：自定义比较器排序
来源：http://ztn.iojbl.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gdv.daria6918.cn

[S40] C++：查找元素
来源：http://vgr.epnwcf.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kmq.yj202588.top

[S41] C++：类与构造函数
来源：http://hho.feifeiyinyue.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hgq.hammf.cn

[S42] C++：继承与虚函数
来源：http://qeh.xziqi.cn

class B : public Base { public: void f() override {} };
来源：http://hsv.guowangkeji.top

[S43] C++：智能指针
来源：http://bwp.jlsjyb.cn

auto p = std::make_unique<int>(5);
来源：http://vrw.zycfv.cn

[S44] C++：引用传参
来源：http://ejv.zhiwuduotai.top

void inc(int &x) { ++x; }
来源：http://zlv.cdnleiting.top

[S45] C++：lambda
来源：http://whm.yj20258888.top

auto add = [](int a, int b) { return a + b; };
来源：http://wsw.fengsongda.top

[S46] C++：函数模板
来源：http://qfq.cqqwz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rjv.hammf.cn

[S47] C++：结构化绑定遍历
来源：http://rnk.nwbrower.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://smx.guowangkeji.top

[S48] C++：逐行读文件
来源：http://uob.316326.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://qba.sxryk.cn

while (std::getline(in, line)) { }
来源：http://cdb.ydjk.org.cn

[S49] C++：写文件
来源：http://kvh.jiagoushi.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gcj.tianlin.xyz

[S50] C++：格式化数字
来源：http://sxh.xuanzx.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://emv.chenzaomai.com

[S51] C++：显式类型转换
来源：http://wmb.dianchejie.cn

static_cast<double>(a) / b
来源：http://suk.cdnleiting.top

[S52] C++：const 与 noexcept
来源：http://hju.cheryme.top

int size() const noexcept { return n_; }
来源：http://kzx.fanxiaobao.xyz

[S53] C++：移动语义
来源：http://vbn.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://jbh.chenzaomai.com

[S54] C++：异常处理
来源：http://bma.gotoacloud.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wxu.havefunace.top

[S55] C++：结构化绑定
来源：http://hsu.svipenyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kdx.aizwys.cn

[S56] C++：optional
来源：http://ute.ydjk.org.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ujk.nwbrower.top

[S57] C++：编译期常量
来源：http://vif.zdqjudy.top

constexpr int N = 10;
来源：http://gfl.quarkkingdee.top

[S58] C++：命名空间
来源：http://ypy.zhixingplan.top


<!-- 参考信息 -->