代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://yty.bjfxy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rna.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yji.tianlin.xyz

[Q89] 判断表是否存在
来源：http://ipc.xinyue.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qgw.bbcook.cn

[Q90] 生成序号列
来源：http://cpq.feifeiyinyue.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://edg.smart0.xyz

================================================================================
来源：http://rqp.bbcook.cn

R. Bash 专题
来源：http://ffp.shanyushiyangkeji.top

================================================================================
来源：http://jov.zhongyouzk.top

[R01] shebang 与严格模式
来源：http://bkq.svipenyu.cn

#!/usr/bin/env bash
来源：http://vpc.bbcook.cn

set -euo pipefail
来源：http://qlt.chenzaomai.com

[R02] 变量赋值与使用
来源：http://mcw.0kj1m.cn

name="Tom"; echo "$name"
来源：http://diz.gogol.net.cn

[R03] 只读变量
来源：http://jtv.meibo888.top

readonly PI=3.14
来源：http://qmb.jlsjyb.cn

[R04] 位置参数
来源：http://vom.chenlongwang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://run.dashuyun.cn

[R05] 参数默认值
来源：http://gpv.hnqzz.top

name="${1:-default}"
来源：http://akv.fktsv.cn

[R06] 判断命令是否存在
来源：http://fwl.dianchejie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qku.pycfn.com

[R07] if 判断文件
来源：http://wps.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pqy.dianchejie.cn

[R08] 数值比较
来源：http://pzd.hfpthk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gdu.ydzc1.top

[R09] 字符串比较
来源：http://mcu.fanxiaobao.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ywo.cqqwz.cn

[R10] 正则匹配
来源：http://nqk.pycfn.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tnu.smart0.xyz

[R11] case 多分支
来源：http://qqi.jlsjyb.cn

case "$1" in
来源：http://hsq.aibaodan.cn

start) echo "启动" ;;
来源：http://msu.jqgfzy.top

stop)  echo "停止" ;;
来源：http://zem.xziqi.cn

*)     echo "未知命令" ;;
来源：http://wme.yj20258888.top

esac
来源：http://wtn.tian-w.cn

[R12] for 遍历文件
来源：http://npz.jinghuilouyu.cn

for f in *.txt; do echo "$f"; done
来源：http://www.fktsv.cn

[R13] for 计数循环
来源：http://qpo.sweek.top

for i in {1..10}; do echo "$i"; done
来源：http://szd.nanxinkj.top

[R14] C 风格 for
来源：http://eeu.xylfe.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rwi.chenlongwang.top

[R15] while 逐行读文件
来源：http://gpn.zhaomingkeji.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vuz.yj20258.top

[R16] until 等待条件
来源：http://zvq.yj202588.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ptj.vqdsnc.cn

[R17] 数组定义与取值
来源：http://gdf.ehwqpu.com

arr=(a b c); echo "${arr[0]}"
来源：http://hir.hesvh.cn

[R18] 遍历数组
来源：http://fhn.wangshuangyany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jlh.c1oappe.top

[R19] 数组长度
来源：http://dwz.hywenlv.cn

echo "${#arr[@]}"
来源：http://qit.daxiang520.top

[R20] 关联数组（字典）
来源：http://wpl.ywan-chungtsiang.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eys.hammf.cn

[R21] 字符串长度
来源：http://wrg.hnxiangtu.top

echo "${#s}"
来源：http://hhf.shangyingyoupin.top

[R22] 截取子串
来源：http://qfe.kuanghao11.cn

echo "${s:0:5}"
来源：http://cox.nwbrower.top

[R23] 字符串替换
来源：http://cls.sweek.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nwo.xinyue.icu

[R24] 大小写转换
来源：http://lsp.ctjpmb.com

echo "${s^^}"; echo "${s,,}"
来源：http://sun.fehbvm.com

[R25] 去后缀 / 去前缀
来源：http://zms.dianchejie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ktj.9152youxi.cn

[R26] 命令替换
来源：http://avu.yvedp.cn

now=$(date +%F); echo "$now"
来源：http://nkb.zhixingplan.top

[R27] 算术展开
来源：http://qtg.cdnleiting.top

echo $((1 + 2 * 3))
来源：http://smt.sysykeji.top

[R28] 浮点运算
来源：http://tsp.shangyingyoupin.top

echo "scale=2; 10/3" | bc
来源：http://uql.iojbl.cn

[R29] 定义函数
来源：http://fyq.jlsjyb.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vcs.jinyuanbaomall.cn

[R30] 函数返回状态码
来源：http://bcz.yangfankeji.com

f() { return 0; }; f || echo "失败了"
来源：http://ifj.dianchejie.cn

[R31] 局部变量
来源：http://bus.dashuyun.cn

f() { local x=1; echo "$x"; }
来源：http://iqu.jyoumei.cn

[R32] 参数个数校验
来源：http://gjc.zycfv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rrj.zhixingplan.top

[R33] 捕获错误并提示行号
来源：http://qcd.jqgfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cku.tian-w.cn

[R34] 退出时清理
来源：http://mfj.fengsongda.top

trap 'rm -f "$tmp"' EXIT
来源：http://klp.iojbl.cn

[R35] 后台执行并等待
来源：http://out.zhoulong.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://tdd.hnqzz.top

[R36] 并发执行多个任务
来源：http://vln.yanxiufei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jfr.wangdashe.top

[R37] 把输出赋给变量
来源：http://ope.shangyingyoupin.top

files=$(ls -1)
来源：http://ene.yfazqb.com

[R38] 管道串联
来源：http://taa.cashguo.top

cat a.txt | grep -i error | wc -l
来源：http://qgz.epnwcf.com

[R39] 重定向标准输出与错误
来源：http://cqu.snrcjt.cn

cmd > out.log 2>&1
来源：http://epn.guannengcc.top

[R40] 追加写日志
来源：http://ojb.0kj1m.cn

echo "log" >> out.log
来源：http://xfs.hcnkem.com

[R41] 丢弃输出
来源：http://ghc.cashguo.top

cmd >/dev/null 2>&1
来源：http://szg.chenzaomai.com

[R42] 输入重定向
来源：http://mgs.hysaishi.cn

wc -l < a.txt
来源：http://lvi.0kj1m.cn

[R43] 按名字查找文件
来源：http://twi.gogol.net.cn

find . -name "*.log" -type f
来源：http://wla.hesvh.cn

[R44] 按修改时间查找
来源：http://hpu.snrcjt.cn

find . -mtime -7 -type f
来源：http://zap.vehdjk.com

[R45] 批量删除
来源：http://vpg.chenlongwang.top

find . -name "*.tmp" -delete
来源：http://qwu.tarul.cn

[R46] 递归替换文件内容
来源：http://uhw.zhiwuduotai.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rhd.jinghuilouyu.cn

[R47] sed 单行替换
来源：http://olu.xingfuxueyuan.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://wds.redwolf501.top

[R48] awk 取指定列
来源：http://yng.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://vkv.gotoacloud.top

[R49] awk 带条件
来源：http://ril.epnwcf.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://muh.zhijiandao.cn

[R50] awk 求和
来源：http://kcf.epnwcf.com

awk '{s += $2} END {print s}' a.txt
来源：http://siq.ywan-chungtsiang.top

[R51] 排序去重取前几
来源：http://iug.aibaodan.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jzk.nanxuanxn.top

[R52] 统计行数
来源：http://axb.jqgfzy.top

wc -l a.txt
来源：http://las.zhaomingkeji.xyz

[R53] 查看文件头与实时尾
来源：http://mqq.ppjwa.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ziv.wangshuangyany.cn

[R54] 比较两个文件
来源：http://biz.daxiang520.top

diff a.txt b.txt
来源：http://jfn.haohaochexian.top

[R55] 压缩与解压
来源：http://qcs.52xcode.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rdy.gzhubu.top

[R56] 远程拷贝
来源：http://jze.jinghuilouyu.cn

scp file user@host:/path/
来源：http://hcm.daxiang520.top

[R57] 远程执行命令
来源：http://sew.dashuyun.cn

ssh user@host 'uptime'
来源：http://dgl.daxiang520.top

[R58] 下载文件
来源：http://irz.fktsv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zgy.zdbjq.cn

[R59] 发 POST JSON
来源：http://jls.tarul.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ass.zycfv.cn

[R60] 只看 HTTP 状态码
来源：http://fbs.ywan-chungtsiang.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eel.sufxvd.cn

[R61] 磁盘占用
来源：http://ldw.nwbrower.top

df -h;  du -sh *
来源：http://yzt.fanxiaobao.xyz

[R62] 找最占空间的文件
来源：http://xwu.redwolf501.top

du -ah . | sort -rh | head -10
来源：http://ogd.gotoacloud.top

[R63] 内存与进程
来源：http://omo.yueranfly.top

free -h;  ps aux | grep nginx
来源：http://bsd.ppjwa.cn

[R64] 结束进程
来源：http://lka.yj202588.top

kill -9 $(pgrep -f app.py)
来源：http://jfq.shanyushiyangkeji.top

[R65] 查看端口占用
来源：http://zss.ppjwa.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hkn.ydzc1.top

[R66] 定时任务
来源：http://wmv.jqgfzy.top

crontab -e;  crontab -l
来源：http://qdx.hcnkem.com

[R67] 生成随机十六进制串
来源：http://uio.yj20258888.top

openssl rand -hex 16
来源：http://ljc.xziqi.cn

[R68] 计算文件校验值
来源：http://gje.xuanzx.com

sha256sum a.txt;  md5sum a.txt
来源：http://bgq.zdbjq.cn

[R69] 生成随机密码
来源：http://ncj.zdqjudy.top

head -c 16 /dev/urandom | base64
来源：http://sik.hongshengwenyu.top

[R70] 时间戳与互转
来源：http://lmm.dashuyun.cn

date +%s;  date -d @1700000000
来源：http://dtj.daria6918.cn

[R71] 日期格式化
来源：http://aui.shzxlz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://npa.snrcjt.cn

[R72] 等待端口就绪
来源：http://brn.yueranfly.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ncn.jyoumei.cn

[R73] 分割大日志
来源：http://bii.gotoacloud.top

split -l 1000 big.log part_
来源：http://dpj.shuidangran.top

[R74] 批量重命名
来源：http://hfa.yuxming.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aic.fehbvm.com

[R75] 导出环境变量
来源：http://wur.cdnleiting.top

export PATH="$HOME/bin:$PATH"
来源：http://ujp.fehbvm.com

[R76] 使用临时文件
来源：http://vgs.xziqi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wpi.xingfuxueyuan.xyz

[R77] 读取用户输入
来源：http://psa.vehdjk.com

read -rp "请输入: " ans
来源：http://pci.xinyue.icu

[R78] 交互式菜单
来源：http://eyl.shanyushiyangtech.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vnj.xuetiantiany.cn

[R79] 解析命令行选项
来源：http://ntf.meibo888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zcz.vqdsnc.cn

[R80] 查看脚本执行耗时
来源：http://cea.gzhubu.top

time ./run.sh
来源：http://abl.ywan-chungtsiang.top

================================================================================
来源：http://zhi.hnqzz.top

S. C / C++ 专题
来源：http://ujz.tarul.cn

================================================================================
来源：http://vkz.gzhubu.top

[S01] C：Hello World
来源：http://hxc.birdmap.top

#include <stdio.h>
来源：http://coz.yueranfly.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://csl.gaohongyu789.top

[S02] C：变量与格式化输出
来源：http://gmg.zhoulong.xyz

int a = 10; printf("%d\n", a);
来源：http://ewr.ydjk.org.cn

[S03] C：读入整数
来源：http://ufa.tanke756.top

int x; scanf("%d", &x);
来源：http://jgc.shuidangran.top

[S04] C：字符串复制
来源：http://tvr.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://znu.daria6918.cn

[S05] C：字符串长度
来源：http://bik.haohaochexian.top

strlen(s)
来源：http://gvw.cheryme.top

[S06] C：字符串比较
来源：http://wuk.ivvv.top

strcmp(a, b) == 0
来源：http://zxv.52xcode.cn

[S07] C：数组遍历求和
来源：http://phz.hcnkem.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pfv.yonumen.top

[S08] C：动态内存分配与释放
来源：http://mwx.uphjek.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fis.chenjidiqi.icu

[S09] C：结构体定义与初始化
来源：http://qfo.yj202588.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cas.vqdsnc.cn

[S10] C：指针与解引用
来源：http://vam.xuetiantiany.cn

int *p = &a;  *p = 5;
来源：http://uzw.mhx1999.top

[S11] C：逐行读文件
来源：http://opg.ppjwa.cn

FILE *f = fopen("a.txt", "r");
来源：http://cmc.gogol.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fui.gaohongyu789.top

fclose(f);
来源：http://xte.sweek.top

[S12] C：写文件
来源：http://lcs.hcnkem.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sre.jianghu66.top

[S13] C：宏定义
来源：http://ndi.redwolf501.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uci.jinqigfzy.top

[S14] C：枚举
来源：http://hya.bjfxy.top

enum Color { RED, GREEN, BLUE };
来源：http://ozl.zhijiandao.cn

[S15] C：类型转换
来源：http://zfg.feifeiyinyue.top

(double) a / b
来源：http://jus.fanxiaobao.xyz

[S16] C：位操作置位
来源：http://xid.gaohongyu789.top

x |= (1 << 3);
来源：http://zzy.hongshengwenyu.top

[S17] C：安全拼接字符串
来源：http://dov.fehbvm.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://out.hywenlv.cn

[S18] C：命令行参数
来源：http://yva.vehdjk.com

int main(int argc, char **argv)
来源：http://pbx.iojbl.cn

[S19] C：快速排序
来源：http://vmn.tarul.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zki.chenjidiqi.icu

[S20] C：二分查找
来源：http://bov.birdmap.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eet.9152youxi.cn

[S21] C：字符类别判断
来源：http://bky.jinghuilouyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sgw.sufxvd.cn

[S22] C：字符串转数字
来源：http://asi.gotoacloud.top

atoi("42");  strtod("3.14", NULL);
来源：http://onv.epnwcf.com

[S23] C：随机数
来源：http://rfz.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mgs.hammf.cn

[S24] C：获取本地时间
来源：http://ugw.daxiang520.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://usp.nwbrower.top

[S25] C：内存拷贝
来源：http://blj.feifeiyinyue.top

memcpy(dst, src, n);
来源：http://hyo.zdbjq.cn

[S26] C：内存清零
来源：http://rhu.cashguo.top

memset(a, 0, sizeof a);
来源：http://skh.zhengqikj.top

[S27] C：定义常量
来源：http://sdw.cdnleiting.top

const double PI = 3.14159;
来源：http://ajy.ppjwa.cn

[S28] C：静态变量
来源：http://swc.redwolf501.top

static int counter = 0;
来源：http://mdn.fktsv.cn

[S29] C：变参函数
来源：http://dqa.yongpay.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rlm.zhijiandao.cn

[S30] C：头文件保护
来源：http://ece.hongshengwenyu.top

#ifndef X_H
来源：http://rmf.andypj.xyz

#define X_H
来源：http://mcn.cashguo.top

#endif
来源：http://jas.zhiwuduotai.top

[S31] C++：Hello World
来源：http://tea.zhongyouzk.top

#include <iostream>
来源：http://gmy.daxiang520.top

int main() { std::cout << "Hello\n"; }
来源：http://yxp.wangdashe.top

[S32] C++：字符串
来源：http://zct.shanyushiyangkeji.top

std::string s = "hi";  s += "!";
来源：http://qmo.iojbl.cn

[S33] C++：vector 增删
来源：http://qgv.fktsv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://utw.ehwqpu.com

[S34] C++：遍历 vector
来源：http://iyb.zdbjq.cn

for (auto &x : v) { std::cout << x; }
来源：http://qxk.vqdsnc.cn

[S35] C++：map
来源：http://gux.fzhhl.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cop.nanxinkj.top

[S36] C++：unordered_map
来源：http://knx.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rfs.jlsjyb.cn

[S37] C++：set
来源：http://iap.hongshengwenyu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ypw.cqqwz.cn

[S38] C++：排序
来源：http://qfj.xuanzx.com

std::sort(v.begin(), v.end());
来源：http://kwv.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://mln.yueranfly.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aee.gotoacloud.top

[S40] C++：查找元素
来源：http://udh.nanxuanxn.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fnv.tarul.cn

[S41] C++：类与构造函数
来源：http://zkm.quarkkingdee.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ysa.xinyue.icu

[S42] C++：继承与虚函数
来源：http://gqt.c1oappe.top

class B : public Base { public: void f() override {} };
来源：http://nhe.tarul.cn

[S43] C++：智能指针
来源：http://xbz.zhixingplan.top

auto p = std::make_unique<int>(5);
来源：http://rne.gotoacloud.top

[S44] C++：引用传参
来源：http://kkr.zycfv.cn

void inc(int &x) { ++x; }
来源：http://kff.fzhhl.top

[S45] C++：lambda
来源：http://fit.ydzc1.top

auto add = [](int a, int b) { return a + b; };
来源：http://smm.vehdjk.com

[S46] C++：函数模板
来源：http://vmk.52xcode.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tpf.c1oappe.top

[S47] C++：结构化绑定遍历
来源：http://zfs.jyoumei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mdb.fzhhl.top

[S48] C++：逐行读文件
来源：http://yxa.zhiwuduotai.top

std::ifstream in("a.txt");  std::string line;
来源：http://tah.shzxlz.cn

while (std::getline(in, line)) { }
来源：http://xwi.epnwcf.com

[S49] C++：写文件
来源：http://qos.nanxuanxn.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mrx.hnxiangtu.top

[S50] C++：格式化数字
来源：http://tnr.zdbjq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://met.daxiang520.top

[S51] C++：显式类型转换
来源：http://tti.hfpthk.cn

static_cast<double>(a) / b
来源：http://thd.zhijiandao.cn

[S52] C++：const 与 noexcept
来源：http://gvf.fanxiaobao.xyz

int size() const noexcept { return n_; }
来源：http://ker.zhixingplan.top

[S53] C++：移动语义
来源：http://wvo.yueranfly.top

std::vector<int> w = std::move(v);
来源：http://wrd.xylfe.cn

[S54] C++：异常处理
来源：http://xez.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tvu.xuanzx.com

[S55] C++：结构化绑定
来源：http://yex.cqqwz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://skh.jinqigufen.top

[S56] C++：optional
来源：http://flh.shanyushiyangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wpw.chenzaomai.com

[S57] C++：编译期常量
来源：http://chx.chenjidiqi.icu

constexpr int N = 10;
来源：http://nfr.52xcode.cn

[S58] C++：命名空间
来源：http://eid.kuanghao11.cn


<!-- 参考信息 -->