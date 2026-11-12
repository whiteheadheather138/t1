代发 wailian999

ANALYZE TABLE users;
来源：http://cdy.snrcjt.cn

[Q71] 查看建表语句
来源：http://ufk.shangyingyoupin.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jdk.xingfuxueyuan.xyz

[Q72] 查看索引
来源：http://iwe.ywan-chungtsiang.top

SHOW INDEX FROM users;
来源：http://arm.kuanghao11.cn

[Q73] 查看表状态
来源：http://wol.sweek.top

SHOW TABLE STATUS LIKE 'users';
来源：http://uqv.shzxlz.cn

[Q74] 强制使用索引
来源：http://ilc.epnwcf.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vzh.nanxuanxn.top

[Q75] 日期格式化
来源：http://dsa.zhaomingkeji.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zsu.ppjwa.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wmd.gotoacloud.top

[Q76] 按天统计
来源：http://zlw.yanxiufei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mkd.yvedp.cn

[Q77] 时间加减
来源：http://mnn.sysykeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pyx.shanyushiyangtech.top

[Q78] 当前时间
来源：http://vsv.jianghu66.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lmx.bbcook.cn

[Q79] 字符串拼接
来源：http://soj.chenzaomai.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pne.cqqwz.cn

[Q80] 字符串截取
来源：http://roh.xziqi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nyt.yfazqb.com

[Q81] 字符串替换
来源：http://wdn.chenjidiqi.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qtx.sxryk.cn

[Q82] 字符长度与字节长度
来源：http://cuh.xziqi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://moq.shuidangran.top

[Q83] 大小写转换
来源：http://gti.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mlv.uphjek.com

[Q84] 去除首尾空格
来源：http://ypv.hongshengwenyu.top

SELECT TRIM(name) FROM users;
来源：http://mxu.cqqwz.cn

[Q85] 数值取整
来源：http://txc.andypj.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://buz.cashguo.top

[Q86] 读取 JSON 字段
来源：http://tjn.vqdsnc.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://unb.zhengqikj.top

[Q87] JSON 字段做条件
来源：http://foi.cdnleiting.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pal.redwolf501.top

[Q88] 行转列（条件聚合）
来源：http://ivr.redwolf501.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ifm.svipenyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://srq.52xcode.cn

[Q89] 判断表是否存在
来源：http://xex.yuxming.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ecy.yj20258.top

[Q90] 生成序号列
来源：http://tky.dashuyun.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tfc.iojbl.cn

================================================================================
来源：http://gzd.tian-w.cn

R. Bash 专题
来源：http://nlk.fengsongda.top

================================================================================
来源：http://lax.fehbvm.com

[R01] shebang 与严格模式
来源：http://kbl.jianghu66.top

#!/usr/bin/env bash
来源：http://wky.ppjwa.cn

set -euo pipefail
来源：http://pdj.jinyuanbaomall.cn

[R02] 变量赋值与使用
来源：http://fkq.hnxiangtu.top

name="Tom"; echo "$name"
来源：http://lvg.xingfuxueyuan.xyz

[R03] 只读变量
来源：http://fbk.yfazqb.com

readonly PI=3.14
来源：http://dgh.vehdjk.com

[R04] 位置参数
来源：http://bci.yuxming.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jzg.sufxvd.cn

[R05] 参数默认值
来源：http://bsa.bjfxy.top

name="${1:-default}"
来源：http://juf.aibaodan.cn

[R06] 判断命令是否存在
来源：http://exc.fengsongda.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kmq.gotoacloud.top

[R07] if 判断文件
来源：http://ung.zhongyouzk.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yfm.zdqjudy.top

[R08] 数值比较
来源：http://hyq.zhijiandao.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xfl.ywan-chungtsiang.top

[R09] 字符串比较
来源：http://qmr.shanyushiyangtech.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hiv.yj202588.top

[R10] 正则匹配
来源：http://ufm.xuetiantiany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bmc.chenlongwang.top

[R11] case 多分支
来源：http://gsl.hfpthk.cn

case "$1" in
来源：http://uas.pengpengdd.cyou

start) echo "启动" ;;
来源：http://gym.hcnkem.com

stop)  echo "停止" ;;
来源：http://vct.zhengqikj.top

*)     echo "未知命令" ;;
来源：http://mvk.ehwqpu.com

esac
来源：http://qlo.nanxuanxn.top

[R12] for 遍历文件
来源：http://cft.chenlongwang.top

for f in *.txt; do echo "$f"; done
来源：http://thr.tianlin.xyz

[R13] for 计数循环
来源：http://icz.yanxiufei.cn

for i in {1..10}; do echo "$i"; done
来源：http://xzh.chenzaomai.com

[R14] C 风格 for
来源：http://syu.aibaodan.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ovj.sweek.top

[R15] while 逐行读文件
来源：http://hpw.kuanghao11.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oem.hfpthk.cn

[R16] until 等待条件
来源：http://paz.cucudq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cxa.guannengcc.top

[R17] 数组定义与取值
来源：http://ffa.xziqi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ynm.epnwcf.com

[R18] 遍历数组
来源：http://sfb.hywenlv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sje.sufxvd.cn

[R19] 数组长度
来源：http://dnc.hcnkem.com

echo "${#arr[@]}"
来源：http://mkr.jianghu66.top

[R20] 关联数组（字典）
来源：http://tid.wangdashe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pyd.9152youxi.cn

[R21] 字符串长度
来源：http://ddd.yongpay.top

echo "${#s}"
来源：http://fbj.sjlbkw.cn

[R22] 截取子串
来源：http://swb.daria6918.cn

echo "${s:0:5}"
来源：http://qxb.shanyushiyangkeji.top

[R23] 字符串替换
来源：http://hho.52xcode.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mng.chenjidiqi.icu

[R24] 大小写转换
来源：http://rmm.yuanzhike.top

echo "${s^^}"; echo "${s,,}"
来源：http://ovb.tian-w.cn

[R25] 去后缀 / 去前缀
来源：http://iwy.svipenyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gpp.yvedp.cn

[R26] 命令替换
来源：http://nid.yuxming.cn

now=$(date +%F); echo "$now"
来源：http://mon.cdnleiting.top

[R27] 算术展开
来源：http://qjd.jqgfzy.top

echo $((1 + 2 * 3))
来源：http://wrg.shanyushiyangtech.top

[R28] 浮点运算
来源：http://jei.jinyuanbaomall.cn

echo "scale=2; 10/3" | bc
来源：http://yma.zhijiandao.cn

[R29] 定义函数
来源：http://hle.yonumen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wxy.cucudq.cn

[R30] 函数返回状态码
来源：http://kqg.tanke756.top

f() { return 0; }; f || echo "失败了"
来源：http://ejp.yuxming.cn

[R31] 局部变量
来源：http://jxd.fengsongda.top

f() { local x=1; echo "$x"; }
来源：http://vkx.jiagoushi.top

[R32] 参数个数校验
来源：http://ljb.bbcook.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mro.hnqzz.top

[R33] 捕获错误并提示行号
来源：http://tpk.cheryme.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vnl.cheryme.top

[R34] 退出时清理
来源：http://leo.shanyushiyangtech.top

trap 'rm -f "$tmp"' EXIT
来源：http://cic.jinghuilouyu.cn

[R35] 后台执行并等待
来源：http://wkw.bjfxy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dao.ybcxt.top

[R36] 并发执行多个任务
来源：http://gbh.nanxuanxn.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fli.kuanghao11.cn

[R37] 把输出赋给变量
来源：http://kbp.xziqi.cn

files=$(ls -1)
来源：http://ihj.uphjek.com

[R38] 管道串联
来源：http://crm.nanxinkj.top

cat a.txt | grep -i error | wc -l
来源：http://avi.yj20258888.top

[R39] 重定向标准输出与错误
来源：http://lsi.shzxlz.cn

cmd > out.log 2>&1
来源：http://hpb.dianchejie.cn

[R40] 追加写日志
来源：http://pbj.vehdjk.com

echo "log" >> out.log
来源：http://ubn.gaohongyu789.top

[R41] 丢弃输出
来源：http://thr.meibo888.top

cmd >/dev/null 2>&1
来源：http://pdr.wangshuangyany.cn

[R42] 输入重定向
来源：http://yza.cashguo.top

wc -l < a.txt
来源：http://hai.fktsv.cn

[R43] 按名字查找文件
来源：http://xjd.gogol.net.cn

find . -name "*.log" -type f
来源：http://ttn.ydzc1.top

[R44] 按修改时间查找
来源：http://cyr.ehwqpu.com

find . -mtime -7 -type f
来源：http://pcj.wangshuangyany.cn

[R45] 批量删除
来源：http://rpl.birdmap.top

find . -name "*.tmp" -delete
来源：http://sof.xuetiantiany.cn

[R46] 递归替换文件内容
来源：http://izp.shangyingyoupin.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wak.hesvh.cn

[R47] sed 单行替换
来源：http://jvy.redwolf501.top

sed -i 's/foo/bar/g' a.txt
来源：http://qcd.svipenyu.cn

[R48] awk 取指定列
来源：http://xsm.vehdjk.com

awk '{print $1, $3}' a.txt
来源：http://sif.sjlbkw.cn

[R49] awk 带条件
来源：http://hjl.ydjk.org.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ibj.yueranfly.top

[R50] awk 求和
来源：http://lsp.jlsjyb.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mmc.uphjek.com

[R51] 排序去重取前几
来源：http://wdz.0kj1m.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rsj.dianchejie.cn

[R52] 统计行数
来源：http://uwd.fzhhl.top

wc -l a.txt
来源：http://gmt.kuanghao11.cn

[R53] 查看文件头与实时尾
来源：http://xkn.ywan-chungtsiang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qro.cdnleiting.top

[R54] 比较两个文件
来源：http://plw.zhoulong.xyz

diff a.txt b.txt
来源：http://qzz.havefunace.top

[R55] 压缩与解压
来源：http://xhr.hysaishi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yqt.fengsongda.top

[R56] 远程拷贝
来源：http://noa.hcnkem.com

scp file user@host:/path/
来源：http://xqf.shanyushiyangtech.top

[R57] 远程执行命令
来源：http://zjm.vqdsnc.cn

ssh user@host 'uptime'
来源：http://csu.chenzaomai.com

[R58] 下载文件
来源：http://iub.shzxlz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cou.hfpthk.cn

[R59] 发 POST JSON
来源：http://rwm.yuxming.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mge.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://rky.andypj.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lgt.zhengqikj.top

[R61] 磁盘占用
来源：http://zlw.bjfxy.top

df -h;  du -sh *
来源：http://lzr.zhoulong.xyz

[R62] 找最占空间的文件
来源：http://hxj.yongpay.top

du -ah . | sort -rh | head -10
来源：http://uvr.birdmap.top

[R63] 内存与进程
来源：http://emy.jiagoushi.top

free -h;  ps aux | grep nginx
来源：http://ssa.sysykeji.top

[R64] 结束进程
来源：http://stc.yuanzhike.top

kill -9 $(pgrep -f app.py)
来源：http://xtm.aibaodan.cn

[R65] 查看端口占用
来源：http://fhw.sysykeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oje.jinghuilouyu.cn

[R66] 定时任务
来源：http://tsg.xuetiantiany.cn

crontab -e;  crontab -l
来源：http://ost.pycfn.com

[R67] 生成随机十六进制串
来源：http://onw.jiagoushi.top

openssl rand -hex 16
来源：http://syh.jqgfzy.top

[R68] 计算文件校验值
来源：http://agw.tian-w.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mqv.fengsongda.top

[R69] 生成随机密码
来源：http://xmn.mhx1999.top

head -c 16 /dev/urandom | base64
来源：http://cmi.fzhhl.top

[R70] 时间戳与互转
来源：http://tga.daxiang520.top

date +%s;  date -d @1700000000
来源：http://kdp.shzxlz.cn

[R71] 日期格式化
来源：http://idd.ivvv.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kgp.zhijiandao.cn

[R72] 等待端口就绪
来源：http://rjs.sysykeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zhx.9152youxi.cn

[R73] 分割大日志
来源：http://xyr.bjfxy.top

split -l 1000 big.log part_
来源：http://qxu.sysykeji.top

[R74] 批量重命名
来源：http://rmk.ydjk.org.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eqq.yj202588.top

[R75] 导出环境变量
来源：http://aqc.yanxiufei.cn

export PATH="$HOME/bin:$PATH"
来源：http://dra.jqgufenzy.top

[R76] 使用临时文件
来源：http://qza.daxiang520.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://elc.jiagoushi.top

[R77] 读取用户输入
来源：http://hxv.316326.xyz

read -rp "请输入: " ans
来源：http://ivp.yangfankeji.com

[R78] 交互式菜单
来源：http://xng.zycfv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oek.sxryk.cn

[R79] 解析命令行选项
来源：http://mgb.gotoacloud.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lfi.chenjidiqi.icu

[R80] 查看脚本执行耗时
来源：http://krp.c1oappe.top

time ./run.sh
来源：http://mfn.hnqzz.top

================================================================================
来源：http://xkc.andypj.xyz

S. C / C++ 专题
来源：http://ytj.svipenyu.cn

================================================================================
来源：http://zuo.shangyingyoupin.top

[S01] C：Hello World
来源：http://xji.vqdsnc.cn

#include <stdio.h>
来源：http://mxh.cashguo.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nsa.guowangkeji.top

[S02] C：变量与格式化输出
来源：http://sxe.yongpay.top

int a = 10; printf("%d\n", a);
来源：http://ron.hysaishi.cn

[S03] C：读入整数
来源：http://bny.shangyingyoupin.top

int x; scanf("%d", &x);
来源：http://iii.jqgfzy.top

[S04] C：字符串复制
来源：http://gfj.zdbjq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qnu.zhoulong.xyz

[S05] C：字符串长度
来源：http://tdm.jinyuanbaomall.cn

strlen(s)
来源：http://fir.zhiwuduotai.top

[S06] C：字符串比较
来源：http://syl.redwolf501.top

strcmp(a, b) == 0
来源：http://cci.chenzaomai.com

[S07] C：数组遍历求和
来源：http://dbv.aibaodan.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wpx.yj202588.top

[S08] C：动态内存分配与释放
来源：http://cvy.yj20258888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nuy.jqgfzy.top

[S09] C：结构体定义与初始化
来源：http://iqi.wangshuangyany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uze.sufxvd.cn

[S10] C：指针与解引用
来源：http://kyv.hongshengwenyu.top

int *p = &a;  *p = 5;
来源：http://iee.jinghuilouyu.cn

[S11] C：逐行读文件
来源：http://bua.hfpthk.cn

FILE *f = fopen("a.txt", "r");
来源：http://gzh.xylfe.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vqe.jyoumei.cn

fclose(f);
来源：http://dhm.ppjwa.cn

[S12] C：写文件
来源：http://tkq.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rnd.ctjpmb.com

[S13] C：宏定义
来源：http://sby.iojbl.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://udn.jqgufenzy.top

[S14] C：枚举
来源：http://xqp.nanxuanxn.top

enum Color { RED, GREEN, BLUE };
来源：http://trc.sweek.top

[S15] C：类型转换
来源：http://qam.jinqigufen.top

(double) a / b
来源：http://zxj.xingfuxueyuan.xyz

[S16] C：位操作置位
来源：http://dbq.xylfe.cn

x |= (1 << 3);
来源：http://jti.yuanzhike.top

[S17] C：安全拼接字符串
来源：http://vyt.xingfuxueyuan.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qma.xuetiantiany.cn

[S18] C：命令行参数
来源：http://ldq.yanxiufei.cn

int main(int argc, char **argv)
来源：http://oll.ywan-chungtsiang.top

[S19] C：快速排序
来源：http://jic.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://odu.feifeiyinyue.top

[S20] C：二分查找
来源：http://pja.fanxiaobao.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hpn.316326.xyz

[S21] C：字符类别判断
来源：http://jsy.gzhubu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rbj.zhiwuduotai.top

[S22] C：字符串转数字
来源：http://jcm.daria6918.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uto.feifeiyinyue.top

[S23] C：随机数
来源：http://pai.ehwqpu.com

srand(time(NULL));  int r = rand() % 100;
来源：http://xhz.guannengcc.top

[S24] C：获取本地时间
来源：http://uur.fzhhl.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zbh.pycfn.com

[S25] C：内存拷贝
来源：http://rlh.meibo888.top

memcpy(dst, src, n);
来源：http://ipe.cheryme.top

[S26] C：内存清零
来源：http://ecz.yj202588.top

memset(a, 0, sizeof a);
来源：http://pei.tianlin.xyz

[S27] C：定义常量
来源：http://wdt.zhixingplan.top

const double PI = 3.14159;
来源：http://hes.yueranfly.top

[S28] C：静态变量
来源：http://byr.jinghuilouyu.cn

static int counter = 0;
来源：http://oyl.uphjek.com

[S29] C：变参函数
来源：http://dlm.cqqwz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://evn.yj20258.top

[S30] C：头文件保护
来源：http://dwm.jianghu66.top

#ifndef X_H
来源：http://hpb.redwolf501.top

#define X_H
来源：http://qpg.kuanghao11.cn

#endif
来源：http://fhs.iojbl.cn

[S31] C++：Hello World
来源：http://jxx.zhongyouzk.top

#include <iostream>
来源：http://wub.birdmap.top

int main() { std::cout << "Hello\n"; }
来源：http://gvv.dianchejie.cn

[S32] C++：字符串
来源：http://vtm.zhengqikj.top

std::string s = "hi";  s += "!";
来源：http://wkd.ydzc1.top

[S33] C++：vector 增删
来源：http://yxn.yj202588.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jzm.xuanzx.com

[S34] C++：遍历 vector
来源：http://rqi.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://mho.xingfuxueyuan.xyz

[S35] C++：map
来源：http://nsa.zhongyouzk.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://udf.feifeiyinyue.top

[S36] C++：unordered_map
来源：http://cas.ydjk.org.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mlh.fehbvm.com

[S37] C++：set
来源：http://lya.shangyingyoupin.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://byc.andypj.xyz

[S38] C++：排序
来源：http://cib.chenlongwang.top

std::sort(v.begin(), v.end());
来源：http://sas.aibaodan.cn

[S39] C++：自定义比较器排序
来源：http://lkc.jianghu66.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xwj.dianchejie.cn

[S40] C++：查找元素
来源：http://yid.0kj1m.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jrd.yangfankeji.com


<!-- 参考信息 -->