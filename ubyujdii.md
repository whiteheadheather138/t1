代发 wailian999

ANALYZE TABLE users;
来源：http://klk.jiagoushi.top

[Q71] 查看建表语句
来源：http://wgh.shangyingyoupin.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pan.sysykeji.top

[Q72] 查看索引
来源：http://fsz.epnwcf.com

SHOW INDEX FROM users;
来源：http://xgw.9152youxi.cn

[Q73] 查看表状态
来源：http://ijn.zhengqikj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bxo.havefunace.top

[Q74] 强制使用索引
来源：http://sic.snrcjt.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ims.ywan-chungtsiang.top

[Q75] 日期格式化
来源：http://grq.cqqwz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ddw.ydjk.org.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xhn.hongshengwenyu.top

[Q76] 按天统计
来源：http://aly.jiagoushi.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yoe.jinyuanbaomall.cn

[Q77] 时间加减
来源：http://tnh.xingfuxueyuan.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iuo.hfpthk.cn

[Q78] 当前时间
来源：http://wpc.9152youxi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dco.yj202588.top

[Q79] 字符串拼接
来源：http://dkd.shanyushiyangtech.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xkd.9152youxi.cn

[Q80] 字符串截取
来源：http://wyn.9152youxi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tql.9152youxi.cn

[Q81] 字符串替换
来源：http://jpc.sufxvd.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fop.yj202588.top

[Q82] 字符长度与字节长度
来源：http://xtp.yj202588.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kkb.316326.xyz

[Q83] 大小写转换
来源：http://dmk.jianghu66.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://riz.gogol.net.cn

[Q84] 去除首尾空格
来源：http://sgg.yuxming.cn

SELECT TRIM(name) FROM users;
来源：http://qqb.xuetiantiany.cn

[Q85] 数值取整
来源：http://xjo.xingfuxueyuan.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://etm.cheryme.top

[Q86] 读取 JSON 字段
来源：http://doi.xingfuxueyuan.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fct.zhongyouzk.top

[Q87] JSON 字段做条件
来源：http://rip.yonumen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zdu.bjfxy.top

[Q88] 行转列（条件聚合）
来源：http://eup.gaohongyu789.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tsy.jqgufenzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fil.zhixingplan.top

[Q89] 判断表是否存在
来源：http://ecs.gotoacloud.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rxw.quarkkingdee.top

[Q90] 生成序号列
来源：http://urt.quarkkingdee.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bka.smart0.xyz

================================================================================
来源：http://qzq.xylfe.cn

R. Bash 专题
来源：http://jcc.ywan-chungtsiang.top

================================================================================
来源：http://awn.yangfankeji.com

[R01] shebang 与严格模式
来源：http://pch.yueranfly.top

#!/usr/bin/env bash
来源：http://gte.jyoumei.cn

set -euo pipefail
来源：http://ihw.jianghu66.top

[R02] 变量赋值与使用
来源：http://nsb.svipenyu.cn

name="Tom"; echo "$name"
来源：http://zwo.xylfe.cn

[R03] 只读变量
来源：http://wyo.yj20258888.top

readonly PI=3.14
来源：http://qsm.zhoulong.xyz

[R04] 位置参数
来源：http://jpk.jinqigufen.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vde.shangyingyoupin.top

[R05] 参数默认值
来源：http://cff.fengsongda.top

name="${1:-default}"
来源：http://wzu.sjlbkw.cn

[R06] 判断命令是否存在
来源：http://mjr.zhiwuduotai.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jjt.shanyushiyangkeji.top

[R07] if 判断文件
来源：http://bgk.nanxinkj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bmb.chenjidiqi.icu

[R08] 数值比较
来源：http://tyq.316326.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://cyd.hammf.cn

[R09] 字符串比较
来源：http://qxa.sweek.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zuu.cdnleiting.top

[R10] 正则匹配
来源：http://elm.shuidangran.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://crj.xuetiantiany.cn

[R11] case 多分支
来源：http://qua.feifeiyinyue.top

case "$1" in
来源：http://zjw.shuidangran.top

start) echo "启动" ;;
来源：http://pko.hywenlv.cn

stop)  echo "停止" ;;
来源：http://ljx.sufxvd.cn

*)     echo "未知命令" ;;
来源：http://osi.zhijiandao.cn

esac
来源：http://dhc.redwolf501.top

[R12] for 遍历文件
来源：http://vmz.kuanghao11.cn

for f in *.txt; do echo "$f"; done
来源：http://qjd.guannengcc.top

[R13] for 计数循环
来源：http://iam.ydjk.org.cn

for i in {1..10}; do echo "$i"; done
来源：http://cew.cashguo.top

[R14] C 风格 for
来源：http://sdb.snrcjt.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vgm.chenlongwang.top

[R15] while 逐行读文件
来源：http://qpg.yuxming.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://apb.hnxiangtu.top

[R16] until 等待条件
来源：http://lao.hnqzz.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ris.daria6918.cn

[R17] 数组定义与取值
来源：http://gkq.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://lkm.jyoumei.cn

[R18] 遍历数组
来源：http://ouy.xuanzx.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://joe.sxryk.cn

[R19] 数组长度
来源：http://qew.zhiwuduotai.top

echo "${#arr[@]}"
来源：http://sfd.wangshuangyany.cn

[R20] 关联数组（字典）
来源：http://euc.xuanzx.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vqy.nanxuanxn.top

[R21] 字符串长度
来源：http://gzc.fzhhl.top

echo "${#s}"
来源：http://iwm.yanxiufei.cn

[R22] 截取子串
来源：http://nud.hongshengwenyu.top

echo "${s:0:5}"
来源：http://prc.xuanzx.com

[R23] 字符串替换
来源：http://win.andypj.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ckp.haohaochexian.top

[R24] 大小写转换
来源：http://clg.hesvh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mbp.pycfn.com

[R25] 去后缀 / 去前缀
来源：http://ivw.pengpengdd.cyou

echo "${f%.txt}"; echo "${f#./}"
来源：http://qcw.52xcode.cn

[R26] 命令替换
来源：http://jco.yj202588.top

now=$(date +%F); echo "$now"
来源：http://wii.c1oappe.top

[R27] 算术展开
来源：http://dxs.dashuyun.cn

echo $((1 + 2 * 3))
来源：http://khw.nwbrower.top

[R28] 浮点运算
来源：http://wzt.hnxiangtu.top

echo "scale=2; 10/3" | bc
来源：http://dqe.daria6918.cn

[R29] 定义函数
来源：http://ggt.ivvv.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uyv.zycfv.cn

[R30] 函数返回状态码
来源：http://amz.wangshuangyany.cn

f() { return 0; }; f || echo "失败了"
来源：http://jjz.uphjek.com

[R31] 局部变量
来源：http://qkn.fehbvm.com

f() { local x=1; echo "$x"; }
来源：http://ukv.ctjpmb.com

[R32] 参数个数校验
来源：http://sat.fktsv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bwf.bbcook.cn

[R33] 捕获错误并提示行号
来源：http://pxz.smart0.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://adm.gotoacloud.top

[R34] 退出时清理
来源：http://gug.zhijiandao.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ufv.hcnkem.com

[R35] 后台执行并等待
来源：http://edz.bbcook.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uut.shangyingyoupin.top

[R36] 并发执行多个任务
来源：http://coq.cashguo.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yfz.jinqigufen.top

[R37] 把输出赋给变量
来源：http://cjx.yj20258888.top

files=$(ls -1)
来源：http://wbt.chenjidiqi.icu

[R38] 管道串联
来源：http://qmy.xuanzx.com

cat a.txt | grep -i error | wc -l
来源：http://xzs.ivvv.top

[R39] 重定向标准输出与错误
来源：http://ody.zycfv.cn

cmd > out.log 2>&1
来源：http://fbz.fzhhl.top

[R40] 追加写日志
来源：http://mph.hywenlv.cn

echo "log" >> out.log
来源：http://ljz.gotoacloud.top

[R41] 丢弃输出
来源：http://jwm.guannengcc.top

cmd >/dev/null 2>&1
来源：http://eqp.quarkkingdee.top

[R42] 输入重定向
来源：http://zkv.chenjidiqi.icu

wc -l < a.txt
来源：http://dda.yanxiufei.cn

[R43] 按名字查找文件
来源：http://bll.c1oappe.top

find . -name "*.log" -type f
来源：http://ygy.316326.xyz

[R44] 按修改时间查找
来源：http://mta.yueranfly.top

find . -mtime -7 -type f
来源：http://rwe.fzhhl.top

[R45] 批量删除
来源：http://eyw.jinghuilouyu.cn

find . -name "*.tmp" -delete
来源：http://awx.birdmap.top

[R46] 递归替换文件内容
来源：http://qgy.zdqjudy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mks.cashguo.top

[R47] sed 单行替换
来源：http://mkr.ydjk.org.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fxn.9152youxi.cn

[R48] awk 取指定列
来源：http://frs.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://ooh.uphjek.com

[R49] awk 带条件
来源：http://icv.gotoacloud.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://icn.gotoacloud.top

[R50] awk 求和
来源：http://xob.yanxiufei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://znl.zhongyouzk.top

[R51] 排序去重取前几
来源：http://fjb.gogol.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ufk.nwbrower.top

[R52] 统计行数
来源：http://skk.ydjk.org.cn

wc -l a.txt
来源：http://aqr.cucudq.cn

[R53] 查看文件头与实时尾
来源：http://app.quarkkingdee.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ejp.jinyuanbaomall.cn

[R54] 比较两个文件
来源：http://uqf.meibo888.top

diff a.txt b.txt
来源：http://ufz.shanyushiyangtech.top

[R55] 压缩与解压
来源：http://wgr.ydzc1.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://glo.zdqjudy.top

[R56] 远程拷贝
来源：http://ncl.quarkkingdee.top

scp file user@host:/path/
来源：http://crl.smart0.xyz

[R57] 远程执行命令
来源：http://qxk.chenzaomai.com

ssh user@host 'uptime'
来源：http://jdp.jinghuilouyu.cn

[R58] 下载文件
来源：http://ndl.guannengcc.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sem.daria6918.cn

[R59] 发 POST JSON
来源：http://xhc.ppjwa.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wjd.jqgfzy.top

[R60] 只看 HTTP 状态码
来源：http://xsx.yuxming.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oca.hongshengwenyu.top

[R61] 磁盘占用
来源：http://bzm.shanyushiyangtech.top

df -h;  du -sh *
来源：http://osq.fehbvm.com

[R62] 找最占空间的文件
来源：http://yge.havefunace.top

du -ah . | sort -rh | head -10
来源：http://kos.cqqwz.cn

[R63] 内存与进程
来源：http://kzv.bbcook.cn

free -h;  ps aux | grep nginx
来源：http://hex.uphjek.com

[R64] 结束进程
来源：http://nqt.52xcode.cn

kill -9 $(pgrep -f app.py)
来源：http://jeo.guannengcc.top

[R65] 查看端口占用
来源：http://sbu.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kuu.guowangkeji.top

[R66] 定时任务
来源：http://mmc.iojbl.cn

crontab -e;  crontab -l
来源：http://qbp.pengpengdd.cyou

[R67] 生成随机十六进制串
来源：http://fgb.nanxinkj.top

openssl rand -hex 16
来源：http://eqa.dashuyun.cn

[R68] 计算文件校验值
来源：http://rbe.shanyushiyangtech.top

sha256sum a.txt;  md5sum a.txt
来源：http://ots.chenjidiqi.icu

[R69] 生成随机密码
来源：http://vsu.wangshuangyany.cn

head -c 16 /dev/urandom | base64
来源：http://xvt.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://bxz.quarkkingdee.top

date +%s;  date -d @1700000000
来源：http://fbt.zdqjudy.top

[R71] 日期格式化
来源：http://mle.jianghu66.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fec.jlsjyb.cn

[R72] 等待端口就绪
来源：http://myq.iojbl.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mmd.zycfv.cn

[R73] 分割大日志
来源：http://jrk.dashuyun.cn

split -l 1000 big.log part_
来源：http://iss.fengsongda.top

[R74] 批量重命名
来源：http://jhu.pycfn.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://veq.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://mid.ivvv.top

export PATH="$HOME/bin:$PATH"
来源：http://tqz.zhoulong.xyz

[R76] 使用临时文件
来源：http://rdd.tianlin.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jfc.jyoumei.cn

[R77] 读取用户输入
来源：http://vpb.yj202588.top

read -rp "请输入: " ans
来源：http://utx.tian-w.cn

[R78] 交互式菜单
来源：http://hii.yuxming.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://apv.yj20258.top

[R79] 解析命令行选项
来源：http://krg.ybcxt.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gbg.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://tgp.xylfe.cn

time ./run.sh
来源：http://izx.tianlin.xyz

================================================================================
来源：http://ast.shanyushiyangkeji.top

S. C / C++ 专题
来源：http://zti.pengpengdd.cyou

================================================================================
来源：http://sfh.yangfankeji.com

[S01] C：Hello World
来源：http://cga.yfazqb.com

#include <stdio.h>
来源：http://omy.zhaomingkeji.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://iid.jianghu66.top

[S02] C：变量与格式化输出
来源：http://vet.zhaomingkeji.xyz

int a = 10; printf("%d\n", a);
来源：http://aut.9152youxi.cn

[S03] C：读入整数
来源：http://rgr.iojbl.cn

int x; scanf("%d", &x);
来源：http://plx.ydzc1.top

[S04] C：字符串复制
来源：http://wpx.jinqigufen.top

char dst[32]; strcpy(dst, "hi");
来源：http://hfh.chenjidiqi.icu

[S05] C：字符串长度
来源：http://nlo.chenjidiqi.icu

strlen(s)
来源：http://agf.shanyushiyangkeji.top

[S06] C：字符串比较
来源：http://kxq.ybcxt.top

strcmp(a, b) == 0
来源：http://mtd.fehbvm.com

[S07] C：数组遍历求和
来源：http://vgc.jinqigufen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kyl.hesvh.cn

[S08] C：动态内存分配与释放
来源：http://gvs.yvedp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fqv.cheryme.top

[S09] C：结构体定义与初始化
来源：http://wxh.chenzaomai.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qgy.yfazqb.com

[S10] C：指针与解引用
来源：http://ymo.0kj1m.cn

int *p = &a;  *p = 5;
来源：http://ioz.birdmap.top

[S11] C：逐行读文件
来源：http://kpv.ehwqpu.com

FILE *f = fopen("a.txt", "r");
来源：http://ebc.daria6918.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cwy.yueranfly.top

fclose(f);
来源：http://dfd.fzhhl.top

[S12] C：写文件
来源：http://vzw.hnxiangtu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ilr.yj20258888.top

[S13] C：宏定义
来源：http://shm.ywan-chungtsiang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eap.ehwqpu.com

[S14] C：枚举
来源：http://aal.hongshengwenyu.top

enum Color { RED, GREEN, BLUE };
来源：http://buw.jinqigufen.top

[S15] C：类型转换
来源：http://sjp.havefunace.top

(double) a / b
来源：http://fkq.cucudq.cn

[S16] C：位操作置位
来源：http://mel.gogol.net.cn

x |= (1 << 3);
来源：http://vej.zhixingplan.top

[S17] C：安全拼接字符串
来源：http://ceb.quarkkingdee.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://onv.zhijiandao.cn

[S18] C：命令行参数
来源：http://iyx.jinqigufen.top

int main(int argc, char **argv)
来源：http://hpv.shangyingyoupin.top

[S19] C：快速排序
来源：http://cjp.daria6918.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dsf.ctjpmb.com

[S20] C：二分查找
来源：http://fxp.hnxiangtu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lwz.dianchejie.cn

[S21] C：字符类别判断
来源：http://bba.fzhhl.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mmh.epnwcf.com

[S22] C：字符串转数字
来源：http://bnm.sysykeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://uzl.ybcxt.top

[S23] C：随机数
来源：http://ybe.zdbjq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rht.xingfuxueyuan.xyz

[S24] C：获取本地时间
来源：http://fqz.sweek.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qdt.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://lyu.chenlongwang.top

memcpy(dst, src, n);
来源：http://fwz.ehwqpu.com

[S26] C：内存清零
来源：http://omc.hnxiangtu.top

memset(a, 0, sizeof a);
来源：http://dow.jinghuilouyu.cn

[S27] C：定义常量
来源：http://ixp.yangfankeji.com

const double PI = 3.14159;
来源：http://doa.iojbl.cn

[S28] C：静态变量
来源：http://pee.xuetiantiany.cn

static int counter = 0;
来源：http://rgz.jqgufenzy.top

[S29] C：变参函数
来源：http://xsc.aizwys.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vuf.ybcxt.top

[S30] C：头文件保护
来源：http://guq.quarkkingdee.top

#ifndef X_H
来源：http://enn.cdnleiting.top

#define X_H
来源：http://oya.nanxinkj.top

#endif
来源：http://skv.kuanghao11.cn

[S31] C++：Hello World
来源：http://rdv.0kj1m.cn

#include <iostream>
来源：http://fez.hammf.cn

int main() { std::cout << "Hello\n"; }
来源：http://dim.feifeiyinyue.top

[S32] C++：字符串
来源：http://zdi.aizwys.cn

std::string s = "hi";  s += "!";
来源：http://azu.yj20258888.top

[S33] C++：vector 增删
来源：http://pea.daria6918.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xuo.ctjpmb.com

[S34] C++：遍历 vector
来源：http://nsq.jinqigufen.top

for (auto &x : v) { std::cout << x; }
来源：http://tyu.cashguo.top

[S35] C++：map
来源：http://eir.hcnkem.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ohi.ehwqpu.com

[S36] C++：unordered_map
来源：http://hmu.tarul.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gcp.tanke756.top

[S37] C++：set
来源：http://ztu.pengpengdd.cyou

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mew.havefunace.top

[S38] C++：排序
来源：http://qet.bbcook.cn

std::sort(v.begin(), v.end());
来源：http://ulh.fktsv.cn

[S39] C++：自定义比较器排序
来源：http://sde.gogol.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jrj.bjfxy.top

[S40] C++：查找元素
来源：http://qxv.zhengqikj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://psk.tian-w.cn


<!-- 参考信息 -->