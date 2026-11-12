代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tfv.ywan-chungtsiang.top

[Q75] 日期格式化
来源：http://who.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hbj.birdmap.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vwx.hnxiangtu.top

[Q76] 按天统计
来源：http://iot.cucudq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lwv.cheryme.top

[Q77] 时间加减
来源：http://wlj.shanyushiyangtech.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jsm.nanxinkj.top

[Q78] 当前时间
来源：http://rsi.tarul.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lmr.tianlin.xyz

[Q79] 字符串拼接
来源：http://feg.hfpthk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vnh.shzxlz.cn

[Q80] 字符串截取
来源：http://eab.bjfxy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qhe.jlsjyb.cn

[Q81] 字符串替换
来源：http://zld.sxryk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qfu.hammf.cn

[Q82] 字符长度与字节长度
来源：http://twa.fzhhl.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nem.yangfankeji.com

[Q83] 大小写转换
来源：http://kvs.fehbvm.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zqr.shzxlz.cn

[Q84] 去除首尾空格
来源：http://seu.tian-w.cn

SELECT TRIM(name) FROM users;
来源：http://mzs.jlsjyb.cn

[Q85] 数值取整
来源：http://ndq.gaohongyu789.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ium.ctjpmb.com

[Q86] 读取 JSON 字段
来源：http://xuw.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bus.kuanghao11.cn

[Q87] JSON 字段做条件
来源：http://hks.nanxuanxn.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mtg.ywan-chungtsiang.top

[Q88] 行转列（条件聚合）
来源：http://myq.shangyingyoupin.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zkg.zdbjq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jzv.zhixingplan.top

[Q89] 判断表是否存在
来源：http://hfy.snrcjt.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ilc.uphjek.com

[Q90] 生成序号列
来源：http://tgs.wangdashe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qnn.birdmap.top

================================================================================
来源：http://yap.cqqwz.cn

R. Bash 专题
来源：http://nsi.shanyushiyangtech.top

================================================================================
来源：http://woq.ppjwa.cn

[R01] shebang 与严格模式
来源：http://nga.yj20258888.top

#!/usr/bin/env bash
来源：http://zdo.yanxiufei.cn

set -euo pipefail
来源：http://dvy.zhongyouzk.top

[R02] 变量赋值与使用
来源：http://gvt.yonumen.top

name="Tom"; echo "$name"
来源：http://jvy.0kj1m.cn

[R03] 只读变量
来源：http://ojc.chenjidiqi.icu

readonly PI=3.14
来源：http://awz.shanyushiyangtech.top

[R04] 位置参数
来源：http://qyq.xuetiantiany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ufo.zhixingplan.top

[R05] 参数默认值
来源：http://opg.zhengqikj.top

name="${1:-default}"
来源：http://lcl.daria6918.cn

[R06] 判断命令是否存在
来源：http://aao.feifeiyinyue.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rtc.zhengqikj.top

[R07] if 判断文件
来源：http://nwb.jiagoushi.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yoj.9152youxi.cn

[R08] 数值比较
来源：http://yvv.gogol.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://avr.smart0.xyz

[R09] 字符串比较
来源：http://pwa.sufxvd.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vie.xylfe.cn

[R10] 正则匹配
来源：http://vzi.wangshuangyany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pfl.uphjek.com

[R11] case 多分支
来源：http://nyz.zycfv.cn

case "$1" in
来源：http://ben.svipenyu.cn

start) echo "启动" ;;
来源：http://esa.ehwqpu.com

stop)  echo "停止" ;;
来源：http://rog.guowangkeji.top

*)     echo "未知命令" ;;
来源：http://svr.jyoumei.cn

esac
来源：http://lyw.pengpengdd.cyou

[R12] for 遍历文件
来源：http://qpr.hysaishi.cn

for f in *.txt; do echo "$f"; done
来源：http://hqi.hnxiangtu.top

[R13] for 计数循环
来源：http://sbp.fktsv.cn

for i in {1..10}; do echo "$i"; done
来源：http://azr.hfpthk.cn

[R14] C 风格 for
来源：http://igo.shanyushiyangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dsx.yvedp.cn

[R15] while 逐行读文件
来源：http://ahu.yanxiufei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yro.bjfxy.top

[R16] until 等待条件
来源：http://jre.shangyingyoupin.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uwy.yonumen.top

[R17] 数组定义与取值
来源：http://kir.nanxinkj.top

arr=(a b c); echo "${arr[0]}"
来源：http://ald.hesvh.cn

[R18] 遍历数组
来源：http://xal.hnxiangtu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aol.xingfuxueyuan.xyz

[R19] 数组长度
来源：http://fzp.zhaomingkeji.xyz

echo "${#arr[@]}"
来源：http://wup.dashuyun.cn

[R20] 关联数组（字典）
来源：http://cpa.sufxvd.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://abt.vqdsnc.cn

[R21] 字符串长度
来源：http://ekh.sweek.top

echo "${#s}"
来源：http://sig.hammf.cn

[R22] 截取子串
来源：http://nwr.ybcxt.top

echo "${s:0:5}"
来源：http://ehe.sysykeji.top

[R23] 字符串替换
来源：http://jvx.shanyushiyangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iur.tanke756.top

[R24] 大小写转换
来源：http://lgf.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://aoy.fktsv.cn

[R25] 去后缀 / 去前缀
来源：http://jet.kuanghao11.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://utd.yj20258888.top

[R26] 命令替换
来源：http://iuk.hnqzz.top

now=$(date +%F); echo "$now"
来源：http://epw.yonumen.top

[R27] 算术展开
来源：http://mtr.yanxiufei.cn

echo $((1 + 2 * 3))
来源：http://khm.shanyushiyangkeji.top

[R28] 浮点运算
来源：http://aol.yongpay.top

echo "scale=2; 10/3" | bc
来源：http://zpp.tianlin.xyz

[R29] 定义函数
来源：http://hoj.sjlbkw.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ovg.sjlbkw.cn

[R30] 函数返回状态码
来源：http://dlk.0kj1m.cn

f() { return 0; }; f || echo "失败了"
来源：http://qti.zdqjudy.top

[R31] 局部变量
来源：http://oys.pycfn.com

f() { local x=1; echo "$x"; }
来源：http://mwg.xinyue.icu

[R32] 参数个数校验
来源：http://kia.fzhhl.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://olx.yj20258888.top

[R33] 捕获错误并提示行号
来源：http://pec.fanxiaobao.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wnx.hfpthk.cn

[R34] 退出时清理
来源：http://iib.sjlbkw.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nvh.gogol.net.cn

[R35] 后台执行并等待
来源：http://ftw.smart0.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://ecn.ydzc1.top

[R36] 并发执行多个任务
来源：http://xjs.dianchejie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ovz.birdmap.top

[R37] 把输出赋给变量
来源：http://qtu.nanxuanxn.top

files=$(ls -1)
来源：http://lch.hcnkem.com

[R38] 管道串联
来源：http://jjf.9152youxi.cn

cat a.txt | grep -i error | wc -l
来源：http://frd.zhongyouzk.top

[R39] 重定向标准输出与错误
来源：http://toz.nanxuanxn.top

cmd > out.log 2>&1
来源：http://vzq.shuidangran.top

[R40] 追加写日志
来源：http://lqz.hcnkem.com

echo "log" >> out.log
来源：http://czn.zycfv.cn

[R41] 丢弃输出
来源：http://iup.sweek.top

cmd >/dev/null 2>&1
来源：http://mvr.zhengqikj.top

[R42] 输入重定向
来源：http://kon.shanyushiyangkeji.top

wc -l < a.txt
来源：http://zkr.xingfuxueyuan.xyz

[R43] 按名字查找文件
来源：http://aju.jinqigufen.top

find . -name "*.log" -type f
来源：http://weq.epnwcf.com

[R44] 按修改时间查找
来源：http://qez.ehwqpu.com

find . -mtime -7 -type f
来源：http://igj.ppjwa.cn

[R45] 批量删除
来源：http://hrk.zhoulong.xyz

find . -name "*.tmp" -delete
来源：http://wxu.jlsjyb.cn

[R46] 递归替换文件内容
来源：http://ycd.sjlbkw.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bbh.chenlongwang.top

[R47] sed 单行替换
来源：http://esm.cashguo.top

sed -i 's/foo/bar/g' a.txt
来源：http://hfl.hnxiangtu.top

[R48] awk 取指定列
来源：http://rlf.jiagoushi.top

awk '{print $1, $3}' a.txt
来源：http://uif.xylfe.cn

[R49] awk 带条件
来源：http://xrr.tian-w.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://med.andypj.xyz

[R50] awk 求和
来源：http://ucw.nwbrower.top

awk '{s += $2} END {print s}' a.txt
来源：http://xps.epnwcf.com

[R51] 排序去重取前几
来源：http://pvi.sjlbkw.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jzq.havefunace.top

[R52] 统计行数
来源：http://zvq.hfpthk.cn

wc -l a.txt
来源：http://gjm.sxryk.cn

[R53] 查看文件头与实时尾
来源：http://ciu.hesvh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://woj.vqdsnc.cn

[R54] 比较两个文件
来源：http://bbw.zhiwuduotai.top

diff a.txt b.txt
来源：http://kde.shzxlz.cn

[R55] 压缩与解压
来源：http://qfi.redwolf501.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zjf.shanyushiyangtech.top

[R56] 远程拷贝
来源：http://lah.jianghu66.top

scp file user@host:/path/
来源：http://idu.ehwqpu.com

[R57] 远程执行命令
来源：http://ndc.sysykeji.top

ssh user@host 'uptime'
来源：http://wfh.sjlbkw.cn

[R58] 下载文件
来源：http://qjx.shzxlz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jwb.zdqjudy.top

[R59] 发 POST JSON
来源：http://qxq.wangshuangyany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ksv.316326.xyz

[R60] 只看 HTTP 状态码
来源：http://akr.cashguo.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aku.yanxiufei.cn

[R61] 磁盘占用
来源：http://itt.jiagoushi.top

df -h;  du -sh *
来源：http://nhz.jinqigufen.top

[R62] 找最占空间的文件
来源：http://xzv.xinyue.icu

du -ah . | sort -rh | head -10
来源：http://mto.jlsjyb.cn

[R63] 内存与进程
来源：http://idn.tianlin.xyz

free -h;  ps aux | grep nginx
来源：http://bph.fktsv.cn

[R64] 结束进程
来源：http://vpv.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://zzn.zhaomingkeji.xyz

[R65] 查看端口占用
来源：http://siq.epnwcf.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nge.zhijiandao.cn

[R66] 定时任务
来源：http://bxp.jinqigfzy.top

crontab -e;  crontab -l
来源：http://dng.pycfn.com

[R67] 生成随机十六进制串
来源：http://zbr.mhx1999.top

openssl rand -hex 16
来源：http://izp.andypj.xyz

[R68] 计算文件校验值
来源：http://owv.feifeiyinyue.top

sha256sum a.txt;  md5sum a.txt
来源：http://fty.shangyingyoupin.top

[R69] 生成随机密码
来源：http://sjw.yueranfly.top

head -c 16 /dev/urandom | base64
来源：http://ifc.fktsv.cn

[R70] 时间戳与互转
来源：http://zsm.jiagoushi.top

date +%s;  date -d @1700000000
来源：http://xpx.shanyushiyangtech.top

[R71] 日期格式化
来源：http://gnv.zhengqikj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zsl.yangfankeji.com

[R72] 等待端口就绪
来源：http://mja.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fhq.fzhhl.top

[R73] 分割大日志
来源：http://dpp.jinqigfzy.top

split -l 1000 big.log part_
来源：http://zqo.jinqigfzy.top

[R74] 批量重命名
来源：http://omk.c1oappe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ajy.daxiang520.top

[R75] 导出环境变量
来源：http://spy.yongpay.top

export PATH="$HOME/bin:$PATH"
来源：http://mot.9152youxi.cn

[R76] 使用临时文件
来源：http://rfb.zycfv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kxp.epnwcf.com

[R77] 读取用户输入
来源：http://gyo.cucudq.cn

read -rp "请输入: " ans
来源：http://vdt.gogol.net.cn

[R78] 交互式菜单
来源：http://mzb.wangshuangyany.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hui.xuetiantiany.cn

[R79] 解析命令行选项
来源：http://xwv.wangdashe.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vlj.yonumen.top

[R80] 查看脚本执行耗时
来源：http://ivc.yanxiufei.cn

time ./run.sh
来源：http://pmw.vehdjk.com

================================================================================
来源：http://rro.316326.xyz

S. C / C++ 专题
来源：http://exd.cucudq.cn

================================================================================
来源：http://vge.yuxming.cn

[S01] C：Hello World
来源：http://imc.hysaishi.cn

#include <stdio.h>
来源：http://xeq.zhongyouzk.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://clu.jqgfzy.top

[S02] C：变量与格式化输出
来源：http://wwt.52xcode.cn

int a = 10; printf("%d\n", a);
来源：http://oec.0kj1m.cn

[S03] C：读入整数
来源：http://ztq.wangdashe.top

int x; scanf("%d", &x);
来源：http://uvr.cashguo.top

[S04] C：字符串复制
来源：http://jhf.xziqi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kyh.zdbjq.cn

[S05] C：字符串长度
来源：http://wxj.uphjek.com

strlen(s)
来源：http://itf.gogol.net.cn

[S06] C：字符串比较
来源：http://zph.kuanghao11.cn

strcmp(a, b) == 0
来源：http://qam.pengpengdd.cyou

[S07] C：数组遍历求和
来源：http://dag.fzhhl.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kqe.sweek.top

[S08] C：动态内存分配与释放
来源：http://hxd.dashuyun.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vyi.smart0.xyz

[S09] C：结构体定义与初始化
来源：http://gbf.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nab.hammf.cn

[S10] C：指针与解引用
来源：http://zsm.meibo888.top

int *p = &a;  *p = 5;
来源：http://dat.shanyushiyangkeji.top

[S11] C：逐行读文件
来源：http://ztd.zdbjq.cn

FILE *f = fopen("a.txt", "r");
来源：http://mmi.tarul.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bcq.uphjek.com

fclose(f);
来源：http://rpl.0kj1m.cn

[S12] C：写文件
来源：http://vyj.aibaodan.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nlh.havefunace.top

[S13] C：宏定义
来源：http://esv.xziqi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ars.jianghu66.top

[S14] C：枚举
来源：http://exn.sufxvd.cn

enum Color { RED, GREEN, BLUE };
来源：http://lev.yongpay.top

[S15] C：类型转换
来源：http://uvz.hysaishi.cn

(double) a / b
来源：http://ntz.fehbvm.com

[S16] C：位操作置位
来源：http://zlc.hysaishi.cn

x |= (1 << 3);
来源：http://lrd.bjfxy.top

[S17] C：安全拼接字符串
来源：http://mak.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://znv.zhoulong.xyz

[S18] C：命令行参数
来源：http://fvr.ydzc1.top

int main(int argc, char **argv)
来源：http://gof.fktsv.cn

[S19] C：快速排序
来源：http://aag.jlsjyb.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bie.sjlbkw.cn

[S20] C：二分查找
来源：http://kiq.yangfankeji.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vre.pengpengdd.cyou

[S21] C：字符类别判断
来源：http://aqp.zycfv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vif.nanxuanxn.top

[S22] C：字符串转数字
来源：http://mxl.vehdjk.com

atoi("42");  strtod("3.14", NULL);
来源：http://god.ybcxt.top

[S23] C：随机数
来源：http://nyp.bjfxy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rtj.ydzc1.top

[S24] C：获取本地时间
来源：http://dyp.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cqw.xuetiantiany.cn

[S25] C：内存拷贝
来源：http://ihn.jqgufenzy.top

memcpy(dst, src, n);
来源：http://djs.52xcode.cn

[S26] C：内存清零
来源：http://bol.uphjek.com

memset(a, 0, sizeof a);
来源：http://iae.uphjek.com

[S27] C：定义常量
来源：http://psi.nwbrower.top

const double PI = 3.14159;
来源：http://bwf.ywan-chungtsiang.top

[S28] C：静态变量
来源：http://mya.wangdashe.top

static int counter = 0;
来源：http://oum.tanke756.top

[S29] C：变参函数
来源：http://jae.ppjwa.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pqj.chenjidiqi.icu

[S30] C：头文件保护
来源：http://kvn.yuxming.cn

#ifndef X_H
来源：http://pww.yuxming.cn

#define X_H
来源：http://dpt.xuetiantiany.cn

#endif
来源：http://rps.vehdjk.com

[S31] C++：Hello World
来源：http://kmy.fehbvm.com

#include <iostream>
来源：http://zik.jlsjyb.cn

int main() { std::cout << "Hello\n"; }
来源：http://wlv.zhaomingkeji.xyz

[S32] C++：字符串
来源：http://cfx.dianchejie.cn

std::string s = "hi";  s += "!";
来源：http://vhu.gogol.net.cn

[S33] C++：vector 增删
来源：http://bgf.yuanzhike.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zup.kuanghao11.cn

[S34] C++：遍历 vector
来源：http://ngc.cucudq.cn

for (auto &x : v) { std::cout << x; }
来源：http://jay.shzxlz.cn

[S35] C++：map
来源：http://lmv.c1oappe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kfh.cqqwz.cn

[S36] C++：unordered_map
来源：http://tou.nanxuanxn.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hri.ppjwa.cn

[S37] C++：set
来源：http://qbs.gotoacloud.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nig.sxryk.cn

[S38] C++：排序
来源：http://zcc.zhongyouzk.top

std::sort(v.begin(), v.end());
来源：http://cae.chenjidiqi.icu

[S39] C++：自定义比较器排序
来源：http://njj.xziqi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qsm.hysaishi.cn

[S40] C++：查找元素
来源：http://elp.uphjek.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xqu.hammf.cn

[S41] C++：类与构造函数
来源：http://uyp.wangdashe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fhy.chenjidiqi.icu

[S42] C++：继承与虚函数
来源：http://aht.havefunace.top

class B : public Base { public: void f() override {} };
来源：http://ova.cashguo.top

[S43] C++：智能指针
来源：http://ltw.daxiang520.top

auto p = std::make_unique<int>(5);
来源：http://shb.ydzc1.top

[S44] C++：引用传参
来源：http://zkl.yfazqb.com

void inc(int &x) { ++x; }
来源：http://lcr.daxiang520.top


<!-- 参考信息 -->