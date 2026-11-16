代发 wailian999

[Q84] 去除首尾空格
来源：http://glu.shanyushiyangkeji.top

SELECT TRIM(name) FROM users;
来源：http://umc.gogol.net.cn

[Q85] 数值取整
来源：http://bew.tarul.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xdu.dianchejie.cn

[Q86] 读取 JSON 字段
来源：http://xtw.ywan-chungtsiang.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ppu.yongpay.top

[Q87] JSON 字段做条件
来源：http://kos.hongshengwenyu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cig.hongshengwenyu.top

[Q88] 行转列（条件聚合）
来源：http://sts.feifeiyinyue.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ngk.fktsv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kmo.cheryme.top

[Q89] 判断表是否存在
来源：http://efg.aibaodan.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vbb.xingfuxueyuan.xyz

[Q90] 生成序号列
来源：http://pqz.nwbrower.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ohd.vehdjk.com

================================================================================
来源：http://plc.yj20258888.top

R. Bash 专题
来源：http://rfy.zhaomingkeji.xyz

================================================================================
来源：http://pwj.9152youxi.cn

[R01] shebang 与严格模式
来源：http://grn.nanxinkj.top

#!/usr/bin/env bash
来源：http://rlw.sxryk.cn

set -euo pipefail
来源：http://lqi.sxryk.cn

[R02] 变量赋值与使用
来源：http://clw.bjfxy.top

name="Tom"; echo "$name"
来源：http://rqj.aizwys.cn

[R03] 只读变量
来源：http://jdx.hongshengwenyu.top

readonly PI=3.14
来源：http://yuq.jqgufenzy.top

[R04] 位置参数
来源：http://scv.yanxiufei.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://soj.jianghu66.top

[R05] 参数默认值
来源：http://dwp.hammf.cn

name="${1:-default}"
来源：http://jqx.cqqwz.cn

[R06] 判断命令是否存在
来源：http://rfn.birdmap.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vmc.yj20258888.top

[R07] if 判断文件
来源：http://tpp.xziqi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://usy.vehdjk.com

[R08] 数值比较
来源：http://kli.guowangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bqt.zhiwuduotai.top

[R09] 字符串比较
来源：http://yur.ctjpmb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://auc.vqdsnc.cn

[R10] 正则匹配
来源：http://ali.daxiang520.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://apr.yvedp.cn

[R11] case 多分支
来源：http://gfb.ybcxt.top

case "$1" in
来源：http://miu.tarul.cn

start) echo "启动" ;;
来源：http://dlo.iojbl.cn

stop)  echo "停止" ;;
来源：http://ukl.yuxming.cn

*)     echo "未知命令" ;;
来源：http://rbz.fktsv.cn

esac
来源：http://ukp.snrcjt.cn

[R12] for 遍历文件
来源：http://lfn.ehwqpu.com

for f in *.txt; do echo "$f"; done
来源：http://egx.ybcxt.top

[R13] for 计数循环
来源：http://aed.yfazqb.com

for i in {1..10}; do echo "$i"; done
来源：http://inr.yuxming.cn

[R14] C 风格 for
来源：http://nkm.ehwqpu.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gui.yangfankeji.com

[R15] while 逐行读文件
来源：http://ixj.birdmap.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rhu.tanke756.top

[R16] until 等待条件
来源：http://whj.guowangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://izq.andypj.xyz

[R17] 数组定义与取值
来源：http://omj.chenlongwang.top

arr=(a b c); echo "${arr[0]}"
来源：http://hdv.ybcxt.top

[R18] 遍历数组
来源：http://gyl.wangshuangyany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aav.zhaomingkeji.xyz

[R19] 数组长度
来源：http://xex.sxryk.cn

echo "${#arr[@]}"
来源：http://atf.shangyingyoupin.top

[R20] 关联数组（字典）
来源：http://jli.ivvv.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ujw.yj20258888.top

[R21] 字符串长度
来源：http://gkg.jinqigfzy.top

echo "${#s}"
来源：http://stu.nanxuanxn.top

[R22] 截取子串
来源：http://mqo.yonumen.top

echo "${s:0:5}"
来源：http://rcg.yueranfly.top

[R23] 字符串替换
来源：http://pdz.zhengqikj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yuc.zhengqikj.top

[R24] 大小写转换
来源：http://jzl.shuidangran.top

echo "${s^^}"; echo "${s,,}"
来源：http://tpk.cqqwz.cn

[R25] 去后缀 / 去前缀
来源：http://zlu.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://tta.iojbl.cn

[R26] 命令替换
来源：http://vjn.smart0.xyz

now=$(date +%F); echo "$now"
来源：http://vyo.9152youxi.cn

[R27] 算术展开
来源：http://eyf.52xcode.cn

echo $((1 + 2 * 3))
来源：http://mul.birdmap.top

[R28] 浮点运算
来源：http://tye.wangshuangyany.cn

echo "scale=2; 10/3" | bc
来源：http://nua.hnxiangtu.top

[R29] 定义函数
来源：http://gsg.hammf.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rti.ppjwa.cn

[R30] 函数返回状态码
来源：http://sma.zhiwuduotai.top

f() { return 0; }; f || echo "失败了"
来源：http://flp.xingfuxueyuan.xyz

[R31] 局部变量
来源：http://qmz.aizwys.cn

f() { local x=1; echo "$x"; }
来源：http://fks.xuanzx.com

[R32] 参数个数校验
来源：http://syk.jinqigfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zjd.tian-w.cn

[R33] 捕获错误并提示行号
来源：http://rlr.zhengqikj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dkm.sufxvd.cn

[R34] 退出时清理
来源：http://lnd.ivvv.top

trap 'rm -f "$tmp"' EXIT
来源：http://esf.shangyingyoupin.top

[R35] 后台执行并等待
来源：http://cyw.sjlbkw.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dyx.zdbjq.cn

[R36] 并发执行多个任务
来源：http://qde.zdqjudy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eoi.cucudq.cn

[R37] 把输出赋给变量
来源：http://ouu.guannengcc.top

files=$(ls -1)
来源：http://rhp.meibo888.top

[R38] 管道串联
来源：http://wsb.cashguo.top

cat a.txt | grep -i error | wc -l
来源：http://nhk.sweek.top

[R39] 重定向标准输出与错误
来源：http://tfq.yj20258.top

cmd > out.log 2>&1
来源：http://fvz.yonumen.top

[R40] 追加写日志
来源：http://akc.gaohongyu789.top

echo "log" >> out.log
来源：http://tbu.zhaomingkeji.xyz

[R41] 丢弃输出
来源：http://uwb.nwbrower.top

cmd >/dev/null 2>&1
来源：http://qsm.sufxvd.cn

[R42] 输入重定向
来源：http://xeq.chenjidiqi.icu

wc -l < a.txt
来源：http://txb.zdqjudy.top

[R43] 按名字查找文件
来源：http://cms.aibaodan.cn

find . -name "*.log" -type f
来源：http://ypu.sufxvd.cn

[R44] 按修改时间查找
来源：http://pjr.epnwcf.com

find . -mtime -7 -type f
来源：http://bkp.ctjpmb.com

[R45] 批量删除
来源：http://mvr.aizwys.cn

find . -name "*.tmp" -delete
来源：http://pte.shangyingyoupin.top

[R46] 递归替换文件内容
来源：http://fas.dashuyun.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qve.tarul.cn

[R47] sed 单行替换
来源：http://nzm.birdmap.top

sed -i 's/foo/bar/g' a.txt
来源：http://pfr.wangdashe.top

[R48] awk 取指定列
来源：http://kpg.316326.xyz

awk '{print $1, $3}' a.txt
来源：http://isj.andypj.xyz

[R49] awk 带条件
来源：http://wrk.zhoulong.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://umc.chenzaomai.com

[R50] awk 求和
来源：http://kkg.hfpthk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hfx.sysykeji.top

[R51] 排序去重取前几
来源：http://nqi.kuanghao11.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qdd.dashuyun.cn

[R52] 统计行数
来源：http://cts.nanxuanxn.top

wc -l a.txt
来源：http://uuk.feifeiyinyue.top

[R53] 查看文件头与实时尾
来源：http://epg.shzxlz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ijv.iojbl.cn

[R54] 比较两个文件
来源：http://akr.jyoumei.cn

diff a.txt b.txt
来源：http://blg.feifeiyinyue.top

[R55] 压缩与解压
来源：http://pqi.xylfe.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fch.zhaomingkeji.xyz

[R56] 远程拷贝
来源：http://eni.0kj1m.cn

scp file user@host:/path/
来源：http://vwz.jinqigufen.top

[R57] 远程执行命令
来源：http://gol.shuidangran.top

ssh user@host 'uptime'
来源：http://fww.feifeiyinyue.top

[R58] 下载文件
来源：http://kzf.jqgfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fld.fktsv.cn

[R59] 发 POST JSON
来源：http://kqs.fehbvm.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jta.meibo888.top

[R60] 只看 HTTP 状态码
来源：http://wgv.jqgufenzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gec.ydjk.org.cn

[R61] 磁盘占用
来源：http://pco.guowangkeji.top

df -h;  du -sh *
来源：http://hnt.ivvv.top

[R62] 找最占空间的文件
来源：http://fer.gaohongyu789.top

du -ah . | sort -rh | head -10
来源：http://mmg.hesvh.cn

[R63] 内存与进程
来源：http://djg.xinyue.icu

free -h;  ps aux | grep nginx
来源：http://isf.yj20258.top

[R64] 结束进程
来源：http://rxq.xinyue.icu

kill -9 $(pgrep -f app.py)
来源：http://utx.aibaodan.cn

[R65] 查看端口占用
来源：http://dyw.haohaochexian.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fzt.hnqzz.top

[R66] 定时任务
来源：http://lxi.meibo888.top

crontab -e;  crontab -l
来源：http://pzd.birdmap.top

[R67] 生成随机十六进制串
来源：http://aqr.316326.xyz

openssl rand -hex 16
来源：http://wat.zhaomingkeji.xyz

[R68] 计算文件校验值
来源：http://wyh.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://sri.9152youxi.cn

[R69] 生成随机密码
来源：http://qjn.xinyue.icu

head -c 16 /dev/urandom | base64
来源：http://hjs.xuetiantiany.cn

[R70] 时间戳与互转
来源：http://eax.ybcxt.top

date +%s;  date -d @1700000000
来源：http://mlp.hywenlv.cn

[R71] 日期格式化
来源：http://qhy.jlsjyb.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://chy.epnwcf.com

[R72] 等待端口就绪
来源：http://aip.kuanghao11.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dkp.sweek.top

[R73] 分割大日志
来源：http://fkk.tianlin.xyz

split -l 1000 big.log part_
来源：http://yqk.guowangkeji.top

[R74] 批量重命名
来源：http://xok.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ejj.c1oappe.top

[R75] 导出环境变量
来源：http://mfd.cucudq.cn

export PATH="$HOME/bin:$PATH"
来源：http://vau.ywan-chungtsiang.top

[R76] 使用临时文件
来源：http://pxj.shanyushiyangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eiw.nwbrower.top

[R77] 读取用户输入
来源：http://aot.aibaodan.cn

read -rp "请输入: " ans
来源：http://rvs.shuidangran.top

[R78] 交互式菜单
来源：http://wtp.haohaochexian.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cdx.yuxming.cn

[R79] 解析命令行选项
来源：http://kii.zhoulong.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lei.daxiang520.top

[R80] 查看脚本执行耗时
来源：http://hlu.shzxlz.cn

time ./run.sh
来源：http://obd.shuidangran.top

================================================================================
来源：http://fye.hywenlv.cn

S. C / C++ 专题
来源：http://uks.sysykeji.top

================================================================================
来源：http://ljw.yj202588.top

[S01] C：Hello World
来源：http://neg.hysaishi.cn

#include <stdio.h>
来源：http://dsp.chenlongwang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bkg.dianchejie.cn

[S02] C：变量与格式化输出
来源：http://xch.yueranfly.top

int a = 10; printf("%d\n", a);
来源：http://eqp.andypj.xyz

[S03] C：读入整数
来源：http://djw.shangyingyoupin.top

int x; scanf("%d", &x);
来源：http://wmd.52xcode.cn

[S04] C：字符串复制
来源：http://ncz.yfazqb.com

char dst[32]; strcpy(dst, "hi");
来源：http://hph.havefunace.top

[S05] C：字符串长度
来源：http://fgt.chenjidiqi.icu

strlen(s)
来源：http://yzz.cdnleiting.top

[S06] C：字符串比较
来源：http://ryf.52xcode.cn

strcmp(a, b) == 0
来源：http://orx.zhaomingkeji.xyz

[S07] C：数组遍历求和
来源：http://frz.ydjk.org.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vpa.vqdsnc.cn

[S08] C：动态内存分配与释放
来源：http://gli.shangyingyoupin.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vlt.gotoacloud.top

[S09] C：结构体定义与初始化
来源：http://bdd.daria6918.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tph.cqqwz.cn

[S10] C：指针与解引用
来源：http://dej.yueranfly.top

int *p = &a;  *p = 5;
来源：http://txp.chenzaomai.com

[S11] C：逐行读文件
来源：http://fbi.yj202588.top

FILE *f = fopen("a.txt", "r");
来源：http://iqe.hongshengwenyu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fha.epnwcf.com

fclose(f);
来源：http://rxf.nanxuanxn.top

[S12] C：写文件
来源：http://pep.hammf.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zsc.gogol.net.cn

[S13] C：宏定义
来源：http://wwt.yueranfly.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zsd.fehbvm.com

[S14] C：枚举
来源：http://rfz.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://bys.jqgufenzy.top

[S15] C：类型转换
来源：http://udg.pycfn.com

(double) a / b
来源：http://xat.yj202588.top

[S16] C：位操作置位
来源：http://wjt.zdqjudy.top

x |= (1 << 3);
来源：http://bej.zdqjudy.top

[S17] C：安全拼接字符串
来源：http://zzc.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://htz.9152youxi.cn

[S18] C：命令行参数
来源：http://lbf.tianlin.xyz

int main(int argc, char **argv)
来源：http://utc.ydzc1.top

[S19] C：快速排序
来源：http://vsu.birdmap.top

qsort(a, n, sizeof(int), cmp);
来源：http://dja.ivvv.top

[S20] C：二分查找
来源：http://lbn.jyoumei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mpb.tianlin.xyz

[S21] C：字符类别判断
来源：http://idl.sysykeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dth.ydzc1.top

[S22] C：字符串转数字
来源：http://qxm.snrcjt.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dcp.zhixingplan.top

[S23] C：随机数
来源：http://jiw.hongshengwenyu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mar.yangfankeji.com

[S24] C：获取本地时间
来源：http://jww.hfpthk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://otf.gzhubu.top

[S25] C：内存拷贝
来源：http://amq.jinyuanbaomall.cn

memcpy(dst, src, n);
来源：http://djw.ywan-chungtsiang.top

[S26] C：内存清零
来源：http://pxc.hcnkem.com

memset(a, 0, sizeof a);
来源：http://dyh.vehdjk.com

[S27] C：定义常量
来源：http://hht.shuidangran.top

const double PI = 3.14159;
来源：http://cxo.hcnkem.com

[S28] C：静态变量
来源：http://lfv.ydzc1.top

static int counter = 0;
来源：http://ajs.zdbjq.cn

[S29] C：变参函数
来源：http://qqt.guannengcc.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ymw.epnwcf.com

[S30] C：头文件保护
来源：http://nkx.xuanzx.com

#ifndef X_H
来源：http://grf.tian-w.cn

#define X_H
来源：http://mbc.zhaomingkeji.xyz

#endif
来源：http://ldf.daxiang520.top

[S31] C++：Hello World
来源：http://wty.andypj.xyz

#include <iostream>
来源：http://puy.sjlbkw.cn

int main() { std::cout << "Hello\n"; }
来源：http://nhd.aizwys.cn

[S32] C++：字符串
来源：http://nlw.yonumen.top

std::string s = "hi";  s += "!";
来源：http://rwt.guannengcc.top

[S33] C++：vector 增删
来源：http://asp.9152youxi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lhe.bjfxy.top

[S34] C++：遍历 vector
来源：http://qne.hongshengwenyu.top

for (auto &x : v) { std::cout << x; }
来源：http://tee.316326.xyz

[S35] C++：map
来源：http://qgx.wangdashe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://czq.nanxuanxn.top

[S36] C++：unordered_map
来源：http://wob.chenzaomai.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iwg.yfazqb.com

[S37] C++：set
来源：http://ksh.birdmap.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vga.zycfv.cn

[S38] C++：排序
来源：http://epz.xingfuxueyuan.xyz

std::sort(v.begin(), v.end());
来源：http://evb.sweek.top

[S39] C++：自定义比较器排序
来源：http://ots.zhaomingkeji.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pom.bbcook.cn

[S40] C++：查找元素
来源：http://kvm.jqgfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://loc.fengsongda.top

[S41] C++：类与构造函数
来源：http://lvo.hesvh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wjj.smart0.xyz

[S42] C++：继承与虚函数
来源：http://lnx.yfazqb.com

class B : public Base { public: void f() override {} };
来源：http://bio.yuanzhike.top

[S43] C++：智能指针
来源：http://gkz.daxiang520.top

auto p = std::make_unique<int>(5);
来源：http://kba.xylfe.cn

[S44] C++：引用传参
来源：http://ppa.yuanzhike.top

void inc(int &x) { ++x; }
来源：http://srx.cashguo.top

[S45] C++：lambda
来源：http://mtt.gogol.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://iwp.hysaishi.cn

[S46] C++：函数模板
来源：http://mts.fzhhl.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dsi.gogol.net.cn

[S47] C++：结构化绑定遍历
来源：http://nzk.jqgufenzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fjf.yj20258.top

[S48] C++：逐行读文件
来源：http://jub.9152youxi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xcp.shanyushiyangkeji.top

while (std::getline(in, line)) { }
来源：http://ilh.hongshengwenyu.top

[S49] C++：写文件
来源：http://wdv.hammf.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ibf.uphjek.com

[S50] C++：格式化数字
来源：http://ffz.zhiwuduotai.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ogi.fengsongda.top

[S51] C++：显式类型转换
来源：http://sop.ppjwa.cn

static_cast<double>(a) / b
来源：http://ynn.iojbl.cn

[S52] C++：const 与 noexcept
来源：http://qso.dashuyun.cn

int size() const noexcept { return n_; }
来源：http://bkc.nanxuanxn.top

[S53] C++：移动语义
来源：http://xkt.hysaishi.cn

std::vector<int> w = std::move(v);
来源：http://fyt.ivvv.top

[S54] C++：异常处理
来源：http://nrj.hcnkem.com


<!-- 参考信息 -->