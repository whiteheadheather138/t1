代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://emy.dianchejie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wuv.fengsongda.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kxz.pengpengdd.cyou

[Q89] 判断表是否存在
来源：http://brd.yuxming.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nwa.chenjidiqi.icu

[Q90] 生成序号列
来源：http://tur.feifeiyinyue.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rpq.xuanzx.com

================================================================================
来源：http://eqt.nanxuanxn.top

R. Bash 专题
来源：http://nna.aibaodan.cn

================================================================================
来源：http://avt.havefunace.top

[R01] shebang 与严格模式
来源：http://zbc.daria6918.cn

#!/usr/bin/env bash
来源：http://yeu.shuidangran.top

set -euo pipefail
来源：http://tjm.aizwys.cn

[R02] 变量赋值与使用
来源：http://oax.zhiwuduotai.top

name="Tom"; echo "$name"
来源：http://kkt.shangyingyoupin.top

[R03] 只读变量
来源：http://cmr.shzxlz.cn

readonly PI=3.14
来源：http://tdj.sufxvd.cn

[R04] 位置参数
来源：http://ckn.jianghu66.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qvk.andypj.xyz

[R05] 参数默认值
来源：http://edm.gaohongyu789.top

name="${1:-default}"
来源：http://krw.smart0.xyz

[R06] 判断命令是否存在
来源：http://mmq.feifeiyinyue.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wcz.jinqigufen.top

[R07] if 判断文件
来源：http://xmm.9152youxi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dbd.0kj1m.cn

[R08] 数值比较
来源：http://tis.chenjidiqi.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://wlh.fktsv.cn

[R09] 字符串比较
来源：http://cbj.hysaishi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nkr.yvedp.cn

[R10] 正则匹配
来源：http://xds.guowangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lsn.chenlongwang.top

[R11] case 多分支
来源：http://frg.cqqwz.cn

case "$1" in
来源：http://uhs.aibaodan.cn

start) echo "启动" ;;
来源：http://ruh.yangfankeji.com

stop)  echo "停止" ;;
来源：http://xjt.meibo888.top

*)     echo "未知命令" ;;
来源：http://dyf.chenjidiqi.icu

esac
来源：http://tac.zhaomingkeji.xyz

[R12] for 遍历文件
来源：http://iie.52xcode.cn

for f in *.txt; do echo "$f"; done
来源：http://imd.wangshuangyany.cn

[R13] for 计数循环
来源：http://pwj.hysaishi.cn

for i in {1..10}; do echo "$i"; done
来源：http://xkr.xuanzx.com

[R14] C 风格 for
来源：http://eft.ybcxt.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iwy.smart0.xyz

[R15] while 逐行读文件
来源：http://zbc.chenzaomai.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hyf.ydzc1.top

[R16] until 等待条件
来源：http://rus.sxryk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rgk.zdqjudy.top

[R17] 数组定义与取值
来源：http://gsv.nanxinkj.top

arr=(a b c); echo "${arr[0]}"
来源：http://qvv.xuanzx.com

[R18] 遍历数组
来源：http://qgm.zhongyouzk.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iti.zdqjudy.top

[R19] 数组长度
来源：http://vqb.gotoacloud.top

echo "${#arr[@]}"
来源：http://mxz.hysaishi.cn

[R20] 关联数组（字典）
来源：http://rjh.jiagoushi.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dak.jinghuilouyu.cn

[R21] 字符串长度
来源：http://goh.gogol.net.cn

echo "${#s}"
来源：http://pzb.tarul.cn

[R22] 截取子串
来源：http://dax.hysaishi.cn

echo "${s:0:5}"
来源：http://itb.nanxinkj.top

[R23] 字符串替换
来源：http://cxu.ywan-chungtsiang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://alk.xylfe.cn

[R24] 大小写转换
来源：http://aga.yfazqb.com

echo "${s^^}"; echo "${s,,}"
来源：http://bhj.bbcook.cn

[R25] 去后缀 / 去前缀
来源：http://jts.zhengqikj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mhy.c1oappe.top

[R26] 命令替换
来源：http://hux.snrcjt.cn

now=$(date +%F); echo "$now"
来源：http://dhj.shuidangran.top

[R27] 算术展开
来源：http://xbn.yueranfly.top

echo $((1 + 2 * 3))
来源：http://tqx.quarkkingdee.top

[R28] 浮点运算
来源：http://gbj.hesvh.cn

echo "scale=2; 10/3" | bc
来源：http://ivl.zhaomingkeji.xyz

[R29] 定义函数
来源：http://wax.ydzc1.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dxn.kuanghao11.cn

[R30] 函数返回状态码
来源：http://vpd.0kj1m.cn

f() { return 0; }; f || echo "失败了"
来源：http://lop.cqqwz.cn

[R31] 局部变量
来源：http://aud.nanxinkj.top

f() { local x=1; echo "$x"; }
来源：http://bla.yj20258.top

[R32] 参数个数校验
来源：http://uuw.ivvv.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rux.quarkkingdee.top

[R33] 捕获错误并提示行号
来源：http://jju.316326.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://efm.gzhubu.top

[R34] 退出时清理
来源：http://xom.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mju.bbcook.cn

[R35] 后台执行并等待
来源：http://njg.yj20258888.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dts.xylfe.cn

[R36] 并发执行多个任务
来源：http://awa.fengsongda.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jmm.zhongyouzk.top

[R37] 把输出赋给变量
来源：http://znq.cqqwz.cn

files=$(ls -1)
来源：http://uiu.vehdjk.com

[R38] 管道串联
来源：http://orp.ivvv.top

cat a.txt | grep -i error | wc -l
来源：http://zhn.sweek.top

[R39] 重定向标准输出与错误
来源：http://lkg.jiagoushi.top

cmd > out.log 2>&1
来源：http://thv.yongpay.top

[R40] 追加写日志
来源：http://uhp.chenjidiqi.icu

echo "log" >> out.log
来源：http://mmn.shanyushiyangkeji.top

[R41] 丢弃输出
来源：http://epg.ydjk.org.cn

cmd >/dev/null 2>&1
来源：http://cqs.9152youxi.cn

[R42] 输入重定向
来源：http://vij.cheryme.top

wc -l < a.txt
来源：http://fiw.fengsongda.top

[R43] 按名字查找文件
来源：http://ies.hysaishi.cn

find . -name "*.log" -type f
来源：http://pkk.zycfv.cn

[R44] 按修改时间查找
来源：http://txr.chenlongwang.top

find . -mtime -7 -type f
来源：http://him.sysykeji.top

[R45] 批量删除
来源：http://zaf.smart0.xyz

find . -name "*.tmp" -delete
来源：http://sby.ybcxt.top

[R46] 递归替换文件内容
来源：http://fvm.fengsongda.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rvg.bbcook.cn

[R47] sed 单行替换
来源：http://iha.ywan-chungtsiang.top

sed -i 's/foo/bar/g' a.txt
来源：http://egc.316326.xyz

[R48] awk 取指定列
来源：http://xkm.nanxuanxn.top

awk '{print $1, $3}' a.txt
来源：http://gxz.ehwqpu.com

[R49] awk 带条件
来源：http://gae.shzxlz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://twm.yonumen.top

[R50] awk 求和
来源：http://ksq.hammf.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vew.316326.xyz

[R51] 排序去重取前几
来源：http://rrm.pycfn.com

sort a.txt | uniq -c | sort -rn | head
来源：http://hoe.jlsjyb.cn

[R52] 统计行数
来源：http://pxw.jinqigfzy.top

wc -l a.txt
来源：http://zrm.shuidangran.top

[R53] 查看文件头与实时尾
来源：http://gyn.guannengcc.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://otb.havefunace.top

[R54] 比较两个文件
来源：http://kpo.yuxming.cn

diff a.txt b.txt
来源：http://qno.xingfuxueyuan.xyz

[R55] 压缩与解压
来源：http://ipk.yueranfly.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://efv.sysykeji.top

[R56] 远程拷贝
来源：http://nlj.xuetiantiany.cn

scp file user@host:/path/
来源：http://fpq.yfazqb.com

[R57] 远程执行命令
来源：http://ejv.cdnleiting.top

ssh user@host 'uptime'
来源：http://rje.chenlongwang.top

[R58] 下载文件
来源：http://zha.wangshuangyany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ksg.yuxming.cn

[R59] 发 POST JSON
来源：http://mma.cucudq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iru.hesvh.cn

[R60] 只看 HTTP 状态码
来源：http://ncw.tian-w.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ide.shangyingyoupin.top

[R61] 磁盘占用
来源：http://igp.tian-w.cn

df -h;  du -sh *
来源：http://adg.feifeiyinyue.top

[R62] 找最占空间的文件
来源：http://wvf.jqgfzy.top

du -ah . | sort -rh | head -10
来源：http://hev.jinyuanbaomall.cn

[R63] 内存与进程
来源：http://ayl.hfpthk.cn

free -h;  ps aux | grep nginx
来源：http://cmo.chenlongwang.top

[R64] 结束进程
来源：http://xzk.shzxlz.cn

kill -9 $(pgrep -f app.py)
来源：http://dur.cdnleiting.top

[R65] 查看端口占用
来源：http://ilx.zdbjq.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cyj.xuetiantiany.cn

[R66] 定时任务
来源：http://pib.pengpengdd.cyou

crontab -e;  crontab -l
来源：http://bzx.yj202588.top

[R67] 生成随机十六进制串
来源：http://ywm.fanxiaobao.xyz

openssl rand -hex 16
来源：http://sfo.c1oappe.top

[R68] 计算文件校验值
来源：http://sym.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sgg.xziqi.cn

[R69] 生成随机密码
来源：http://duc.jyoumei.cn

head -c 16 /dev/urandom | base64
来源：http://wdm.vqdsnc.cn

[R70] 时间戳与互转
来源：http://vfb.sjlbkw.cn

date +%s;  date -d @1700000000
来源：http://nvq.nwbrower.top

[R71] 日期格式化
来源：http://jlf.fengsongda.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://flm.yangfankeji.com

[R72] 等待端口就绪
来源：http://xhy.jinqigfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kvh.jinyuanbaomall.cn

[R73] 分割大日志
来源：http://nvq.aibaodan.cn

split -l 1000 big.log part_
来源：http://qhi.nanxuanxn.top

[R74] 批量重命名
来源：http://uci.sysykeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mne.hnqzz.top

[R75] 导出环境变量
来源：http://ftj.ivvv.top

export PATH="$HOME/bin:$PATH"
来源：http://cbw.mhx1999.top

[R76] 使用临时文件
来源：http://suc.snrcjt.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://len.dianchejie.cn

[R77] 读取用户输入
来源：http://ibt.ydzc1.top

read -rp "请输入: " ans
来源：http://fei.hywenlv.cn

[R78] 交互式菜单
来源：http://lxu.tanke756.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gfc.hesvh.cn

[R79] 解析命令行选项
来源：http://hlq.wangshuangyany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wjn.jlsjyb.cn

[R80] 查看脚本执行耗时
来源：http://ovq.nanxuanxn.top

time ./run.sh
来源：http://onf.zdbjq.cn

================================================================================
来源：http://flu.sysykeji.top

S. C / C++ 专题
来源：http://kyn.feifeiyinyue.top

================================================================================
来源：http://xkc.birdmap.top

[S01] C：Hello World
来源：http://zza.jianghu66.top

#include <stdio.h>
来源：http://xku.vehdjk.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://fqk.jqgfzy.top

[S02] C：变量与格式化输出
来源：http://ioq.xinyue.icu

int a = 10; printf("%d\n", a);
来源：http://dqa.epnwcf.com

[S03] C：读入整数
来源：http://dol.52xcode.cn

int x; scanf("%d", &x);
来源：http://nbd.xylfe.cn

[S04] C：字符串复制
来源：http://upp.0kj1m.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pjz.nanxinkj.top

[S05] C：字符串长度
来源：http://hdt.jyoumei.cn

strlen(s)
来源：http://msb.havefunace.top

[S06] C：字符串比较
来源：http://wet.shuidangran.top

strcmp(a, b) == 0
来源：http://gjv.jyoumei.cn

[S07] C：数组遍历求和
来源：http://kaq.svipenyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kwr.xinyue.icu

[S08] C：动态内存分配与释放
来源：http://fdw.chenzaomai.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nci.kuanghao11.cn

[S09] C：结构体定义与初始化
来源：http://lak.jianghu66.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://beo.tarul.cn

[S10] C：指针与解引用
来源：http://qko.ydjk.org.cn

int *p = &a;  *p = 5;
来源：http://san.cucudq.cn

[S11] C：逐行读文件
来源：http://rrf.redwolf501.top

FILE *f = fopen("a.txt", "r");
来源：http://tjo.9152youxi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xpc.jinqigufen.top

fclose(f);
来源：http://ycr.zhixingplan.top

[S12] C：写文件
来源：http://lea.tanke756.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uvp.xuanzx.com

[S13] C：宏定义
来源：http://rtu.wangdashe.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ahf.smart0.xyz

[S14] C：枚举
来源：http://xxs.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://lhx.hnxiangtu.top

[S15] C：类型转换
来源：http://oar.kuanghao11.cn

(double) a / b
来源：http://njr.bjfxy.top

[S16] C：位操作置位
来源：http://ctg.xingfuxueyuan.xyz

x |= (1 << 3);
来源：http://vft.havefunace.top

[S17] C：安全拼接字符串
来源：http://cry.chenzaomai.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ger.ydjk.org.cn

[S18] C：命令行参数
来源：http://hxg.nanxuanxn.top

int main(int argc, char **argv)
来源：http://qnr.zhiwuduotai.top

[S19] C：快速排序
来源：http://hvn.epnwcf.com

qsort(a, n, sizeof(int), cmp);
来源：http://fvr.xinyue.icu

[S20] C：二分查找
来源：http://dkl.c1oappe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://trm.yangfankeji.com

[S21] C：字符类别判断
来源：http://bcd.dianchejie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ijv.shanyushiyangtech.top

[S22] C：字符串转数字
来源：http://kbg.chenlongwang.top

atoi("42");  strtod("3.14", NULL);
来源：http://ogw.fanxiaobao.xyz

[S23] C：随机数
来源：http://xvn.yj202588.top

srand(time(NULL));  int r = rand() % 100;
来源：http://toz.ivvv.top

[S24] C：获取本地时间
来源：http://xgs.cashguo.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://swm.yj202588.top

[S25] C：内存拷贝
来源：http://rsn.havefunace.top

memcpy(dst, src, n);
来源：http://klx.sufxvd.cn

[S26] C：内存清零
来源：http://vlv.zhixingplan.top

memset(a, 0, sizeof a);
来源：http://ibx.daria6918.cn

[S27] C：定义常量
来源：http://mvj.zhijiandao.cn

const double PI = 3.14159;
来源：http://roz.chenlongwang.top

[S28] C：静态变量
来源：http://mzv.yuanzhike.top

static int counter = 0;
来源：http://xdk.9152youxi.cn

[S29] C：变参函数
来源：http://lbk.jyoumei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://imz.ywan-chungtsiang.top

[S30] C：头文件保护
来源：http://hty.52xcode.cn

#ifndef X_H
来源：http://pfz.sjlbkw.cn

#define X_H
来源：http://qkn.guowangkeji.top

#endif
来源：http://hzb.hysaishi.cn

[S31] C++：Hello World
来源：http://vnk.aibaodan.cn

#include <iostream>
来源：http://qtq.sxryk.cn

int main() { std::cout << "Hello\n"; }
来源：http://epy.0kj1m.cn

[S32] C++：字符串
来源：http://xzy.fzhhl.top

std::string s = "hi";  s += "!";
来源：http://fpw.yongpay.top

[S33] C++：vector 增删
来源：http://wfb.jinyuanbaomall.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qzz.aibaodan.cn

[S34] C++：遍历 vector
来源：http://ehx.ctjpmb.com

for (auto &x : v) { std::cout << x; }
来源：http://fgw.andypj.xyz

[S35] C++：map
来源：http://dbv.wangshuangyany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://koq.daria6918.cn

[S36] C++：unordered_map
来源：http://ilj.yuanzhike.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jut.shanyushiyangkeji.top

[S37] C++：set
来源：http://bmv.jinyuanbaomall.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wqz.guowangkeji.top

[S38] C++：排序
来源：http://neu.haohaochexian.top

std::sort(v.begin(), v.end());
来源：http://lgx.hnxiangtu.top

[S39] C++：自定义比较器排序
来源：http://shs.havefunace.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gze.tianlin.xyz

[S40] C++：查找元素
来源：http://rrj.tianlin.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://txf.ydzc1.top

[S41] C++：类与构造函数
来源：http://xfd.zdbjq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rot.jyoumei.cn

[S42] C++：继承与虚函数
来源：http://ihb.ivvv.top

class B : public Base { public: void f() override {} };
来源：http://nyu.quarkkingdee.top

[S43] C++：智能指针
来源：http://jdg.hfpthk.cn

auto p = std::make_unique<int>(5);
来源：http://zus.pengpengdd.cyou

[S44] C++：引用传参
来源：http://bii.xinyue.icu

void inc(int &x) { ++x; }
来源：http://whm.zdqjudy.top

[S45] C++：lambda
来源：http://dcf.andypj.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://fgw.jinqigufen.top

[S46] C++：函数模板
来源：http://pps.xuetiantiany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lky.epnwcf.com

[S47] C++：结构化绑定遍历
来源：http://vac.redwolf501.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bgv.ydzc1.top

[S48] C++：逐行读文件
来源：http://bqg.chenlongwang.top

std::ifstream in("a.txt");  std::string line;
来源：http://dwb.fehbvm.com

while (std::getline(in, line)) { }
来源：http://rok.yongpay.top

[S49] C++：写文件
来源：http://dgo.yueranfly.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lho.jianghu66.top

[S50] C++：格式化数字
来源：http://ote.kuanghao11.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zvw.epnwcf.com

[S51] C++：显式类型转换
来源：http://lbq.gaohongyu789.top

static_cast<double>(a) / b
来源：http://rpk.wangdashe.top

[S52] C++：const 与 noexcept
来源：http://ecl.hywenlv.cn

int size() const noexcept { return n_; }
来源：http://drq.zhoulong.xyz

[S53] C++：移动语义
来源：http://fce.cdnleiting.top

std::vector<int> w = std::move(v);
来源：http://azh.sjlbkw.cn

[S54] C++：异常处理
来源：http://ghi.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xby.shuidangran.top

[S55] C++：结构化绑定
来源：http://fmn.jlsjyb.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cow.jinghuilouyu.cn

[S56] C++：optional
来源：http://gxz.mhx1999.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vyp.ywan-chungtsiang.top

[S57] C++：编译期常量
来源：http://pyr.wangshuangyany.cn

constexpr int N = 10;
来源：http://kyj.smart0.xyz

[S58] C++：命名空间
来源：http://sps.jlsjyb.cn


<!-- 参考信息 -->