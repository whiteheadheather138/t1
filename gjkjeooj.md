代发 wailian999

ANALYZE TABLE users;
来源：http://zpq.ctjpmb.com

[Q71] 查看建表语句
来源：http://uxf.yfazqb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ynz.hywenlv.cn

[Q72] 查看索引
来源：http://ufp.daxiang520.top

SHOW INDEX FROM users;
来源：http://ucd.wangdashe.top

[Q73] 查看表状态
来源：http://sbu.cheryme.top

SHOW TABLE STATUS LIKE 'users';
来源：http://oqu.yuxming.cn

[Q74] 强制使用索引
来源：http://bbn.smart0.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pcy.sweek.top

[Q75] 日期格式化
来源：http://noo.hywenlv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://noq.wangdashe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://owx.chenzaomai.com

[Q76] 按天统计
来源：http://fil.zhongyouzk.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://num.hfpthk.cn

[Q77] 时间加减
来源：http://xzr.ywan-chungtsiang.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qua.cqqwz.cn

[Q78] 当前时间
来源：http://nci.ehwqpu.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dgr.chenlongwang.top

[Q79] 字符串拼接
来源：http://cqy.vqdsnc.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zlt.zhaomingkeji.xyz

[Q80] 字符串截取
来源：http://itf.shuidangran.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fue.fengsongda.top

[Q81] 字符串替换
来源：http://pqn.zhixingplan.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ouw.xuetiantiany.cn

[Q82] 字符长度与字节长度
来源：http://nop.vehdjk.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rqt.tianlin.xyz

[Q83] 大小写转换
来源：http://oet.ydjk.org.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ecr.jinghuilouyu.cn

[Q84] 去除首尾空格
来源：http://ycs.cdnleiting.top

SELECT TRIM(name) FROM users;
来源：http://ljn.yuanzhike.top

[Q85] 数值取整
来源：http://uzy.vqdsnc.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://igj.ivvv.top

[Q86] 读取 JSON 字段
来源：http://rdf.tanke756.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bjl.tarul.cn

[Q87] JSON 字段做条件
来源：http://zmp.316326.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://igu.hywenlv.cn

[Q88] 行转列（条件聚合）
来源：http://ata.sxryk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vqz.snrcjt.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lxa.birdmap.top

[Q89] 判断表是否存在
来源：http://kni.hywenlv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://abf.tarul.cn

[Q90] 生成序号列
来源：http://giw.zhaomingkeji.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gah.sxryk.cn

================================================================================
来源：http://ard.epnwcf.com

R. Bash 专题
来源：http://iwp.sufxvd.cn

================================================================================
来源：http://aop.daxiang520.top

[R01] shebang 与严格模式
来源：http://ccp.xuanzx.com

#!/usr/bin/env bash
来源：http://ngw.c1oappe.top

set -euo pipefail
来源：http://pyp.daxiang520.top

[R02] 变量赋值与使用
来源：http://fqm.haohaochexian.top

name="Tom"; echo "$name"
来源：http://gpq.zycfv.cn

[R03] 只读变量
来源：http://ytx.hcnkem.com

readonly PI=3.14
来源：http://ynj.dianchejie.cn

[R04] 位置参数
来源：http://nfc.xylfe.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fsk.aizwys.cn

[R05] 参数默认值
来源：http://oep.chenzaomai.com

name="${1:-default}"
来源：http://fqv.zhijiandao.cn

[R06] 判断命令是否存在
来源：http://xpn.haohaochexian.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zik.hnxiangtu.top

[R07] if 判断文件
来源：http://fxv.tanke756.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qqu.vqdsnc.cn

[R08] 数值比较
来源：http://lej.zhongyouzk.top

if (( a > b )); then echo "a 更大"; fi
来源：http://liv.ywan-chungtsiang.top

[R09] 字符串比较
来源：http://ljh.gogol.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pip.snrcjt.cn

[R10] 正则匹配
来源：http://hyo.jinqigufen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ync.pengpengdd.cyou

[R11] case 多分支
来源：http://cgy.ctjpmb.com

case "$1" in
来源：http://buh.hysaishi.cn

start) echo "启动" ;;
来源：http://vja.ydjk.org.cn

stop)  echo "停止" ;;
来源：http://frm.yonumen.top

*)     echo "未知命令" ;;
来源：http://osj.haohaochexian.top

esac
来源：http://hee.hysaishi.cn

[R12] for 遍历文件
来源：http://nte.tian-w.cn

for f in *.txt; do echo "$f"; done
来源：http://geo.pycfn.com

[R13] for 计数循环
来源：http://qou.pengpengdd.cyou

for i in {1..10}; do echo "$i"; done
来源：http://gmp.jyoumei.cn

[R14] C 风格 for
来源：http://dfj.hysaishi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ejt.xylfe.cn

[R15] while 逐行读文件
来源：http://hwp.zhongyouzk.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xhw.hammf.cn

[R16] until 等待条件
来源：http://evi.zhaomingkeji.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gea.9152youxi.cn

[R17] 数组定义与取值
来源：http://dkr.yongpay.top

arr=(a b c); echo "${arr[0]}"
来源：http://tqb.jyoumei.cn

[R18] 遍历数组
来源：http://crw.gaohongyu789.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cst.zycfv.cn

[R19] 数组长度
来源：http://wtd.cdnleiting.top

echo "${#arr[@]}"
来源：http://xvv.zhijiandao.cn

[R20] 关联数组（字典）
来源：http://ool.jianghu66.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rjl.jlsjyb.cn

[R21] 字符串长度
来源：http://mhe.yueranfly.top

echo "${#s}"
来源：http://pdl.kuanghao11.cn

[R22] 截取子串
来源：http://ntt.snrcjt.cn

echo "${s:0:5}"
来源：http://sjn.yueranfly.top

[R23] 字符串替换
来源：http://qym.jqgfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oeu.quarkkingdee.top

[R24] 大小写转换
来源：http://xom.fanxiaobao.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://zqi.tianlin.xyz

[R25] 去后缀 / 去前缀
来源：http://ehm.52xcode.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gff.yueranfly.top

[R26] 命令替换
来源：http://baq.sufxvd.cn

now=$(date +%F); echo "$now"
来源：http://npz.dashuyun.cn

[R27] 算术展开
来源：http://zro.svipenyu.cn

echo $((1 + 2 * 3))
来源：http://umj.feifeiyinyue.top

[R28] 浮点运算
来源：http://qvu.tianlin.xyz

echo "scale=2; 10/3" | bc
来源：http://uww.haohaochexian.top

[R29] 定义函数
来源：http://ctp.52xcode.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hya.shanyushiyangtech.top

[R30] 函数返回状态码
来源：http://tmu.sufxvd.cn

f() { return 0; }; f || echo "失败了"
来源：http://thq.quarkkingdee.top

[R31] 局部变量
来源：http://gyl.nanxinkj.top

f() { local x=1; echo "$x"; }
来源：http://vha.yj202588.top

[R32] 参数个数校验
来源：http://voi.zhixingplan.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pfc.ppjwa.cn

[R33] 捕获错误并提示行号
来源：http://shm.gogol.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ihk.ydzc1.top

[R34] 退出时清理
来源：http://vww.jinyuanbaomall.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pnd.dianchejie.cn

[R35] 后台执行并等待
来源：http://dky.gogol.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nwh.aibaodan.cn

[R36] 并发执行多个任务
来源：http://ecm.snrcjt.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lie.dianchejie.cn

[R37] 把输出赋给变量
来源：http://dtv.cashguo.top

files=$(ls -1)
来源：http://dnn.zdbjq.cn

[R38] 管道串联
来源：http://osn.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://vqw.cheryme.top

[R39] 重定向标准输出与错误
来源：http://gbn.cucudq.cn

cmd > out.log 2>&1
来源：http://shu.jiagoushi.top

[R40] 追加写日志
来源：http://ksh.pycfn.com

echo "log" >> out.log
来源：http://udx.yanxiufei.cn

[R41] 丢弃输出
来源：http://oky.cucudq.cn

cmd >/dev/null 2>&1
来源：http://coa.xuetiantiany.cn

[R42] 输入重定向
来源：http://ele.haohaochexian.top

wc -l < a.txt
来源：http://ufg.dianchejie.cn

[R43] 按名字查找文件
来源：http://tyd.sweek.top

find . -name "*.log" -type f
来源：http://qtz.jyoumei.cn

[R44] 按修改时间查找
来源：http://rjx.nwbrower.top

find . -mtime -7 -type f
来源：http://nkx.zdqjudy.top

[R45] 批量删除
来源：http://itk.wangshuangyany.cn

find . -name "*.tmp" -delete
来源：http://sxs.xingfuxueyuan.xyz

[R46] 递归替换文件内容
来源：http://yan.c1oappe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zto.wangdashe.top

[R47] sed 单行替换
来源：http://nyn.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://sih.feifeiyinyue.top

[R48] awk 取指定列
来源：http://iiv.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://emi.cheryme.top

[R49] awk 带条件
来源：http://mex.xuanzx.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dqc.snrcjt.cn

[R50] awk 求和
来源：http://ysr.nanxuanxn.top

awk '{s += $2} END {print s}' a.txt
来源：http://ats.zhongyouzk.top

[R51] 排序去重取前几
来源：http://hxf.xuanzx.com

sort a.txt | uniq -c | sort -rn | head
来源：http://bkf.mhx1999.top

[R52] 统计行数
来源：http://kjp.pengpengdd.cyou

wc -l a.txt
来源：http://cij.sxryk.cn

[R53] 查看文件头与实时尾
来源：http://iza.ywan-chungtsiang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rwy.gzhubu.top

[R54] 比较两个文件
来源：http://oal.zhengqikj.top

diff a.txt b.txt
来源：http://shj.316326.xyz

[R55] 压缩与解压
来源：http://wvg.jqgfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://icr.vqdsnc.cn

[R56] 远程拷贝
来源：http://lru.shzxlz.cn

scp file user@host:/path/
来源：http://wvu.andypj.xyz

[R57] 远程执行命令
来源：http://klt.svipenyu.cn

ssh user@host 'uptime'
来源：http://hdx.zhixingplan.top

[R58] 下载文件
来源：http://ztq.sysykeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lub.jinqigufen.top

[R59] 发 POST JSON
来源：http://pgo.zhiwuduotai.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://laz.kuanghao11.cn

[R60] 只看 HTTP 状态码
来源：http://zox.yvedp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tkr.xuetiantiany.cn

[R61] 磁盘占用
来源：http://rut.fanxiaobao.xyz

df -h;  du -sh *
来源：http://abp.zdqjudy.top

[R62] 找最占空间的文件
来源：http://hog.fzhhl.top

du -ah . | sort -rh | head -10
来源：http://bqx.fzhhl.top

[R63] 内存与进程
来源：http://szh.birdmap.top

free -h;  ps aux | grep nginx
来源：http://xua.wangshuangyany.cn

[R64] 结束进程
来源：http://opl.yuxming.cn

kill -9 $(pgrep -f app.py)
来源：http://hnb.wangshuangyany.cn

[R65] 查看端口占用
来源：http://izo.dashuyun.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kwk.zhongyouzk.top

[R66] 定时任务
来源：http://dwd.hysaishi.cn

crontab -e;  crontab -l
来源：http://zec.nwbrower.top

[R67] 生成随机十六进制串
来源：http://pqe.xinyue.icu

openssl rand -hex 16
来源：http://hhi.hnxiangtu.top

[R68] 计算文件校验值
来源：http://iog.yonumen.top

sha256sum a.txt;  md5sum a.txt
来源：http://gyg.ydjk.org.cn

[R69] 生成随机密码
来源：http://ccn.ywan-chungtsiang.top

head -c 16 /dev/urandom | base64
来源：http://gch.shangyingyoupin.top

[R70] 时间戳与互转
来源：http://okp.jianghu66.top

date +%s;  date -d @1700000000
来源：http://txg.hongshengwenyu.top

[R71] 日期格式化
来源：http://mik.c1oappe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rqm.yonumen.top

[R72] 等待端口就绪
来源：http://xzr.ehwqpu.com

until nc -z localhost 3306; do sleep 1; done
来源：http://nar.kuanghao11.cn

[R73] 分割大日志
来源：http://hzu.zhoulong.xyz

split -l 1000 big.log part_
来源：http://unj.cheryme.top

[R74] 批量重命名
来源：http://bdi.dashuyun.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qhu.52xcode.cn

[R75] 导出环境变量
来源：http://tnm.zhongyouzk.top

export PATH="$HOME/bin:$PATH"
来源：http://wvo.zycfv.cn

[R76] 使用临时文件
来源：http://bku.haohaochexian.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://aic.cashguo.top

[R77] 读取用户输入
来源：http://dou.yuanzhike.top

read -rp "请输入: " ans
来源：http://jgs.cheryme.top

[R78] 交互式菜单
来源：http://tjf.yonumen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qqy.shuidangran.top

[R79] 解析命令行选项
来源：http://bwy.chenzaomai.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dzo.sjlbkw.cn

[R80] 查看脚本执行耗时
来源：http://ozm.hongshengwenyu.top

time ./run.sh
来源：http://iuo.birdmap.top

================================================================================
来源：http://kov.jinghuilouyu.cn

S. C / C++ 专题
来源：http://yxq.jinyuanbaomall.cn

================================================================================
来源：http://myy.shuidangran.top

[S01] C：Hello World
来源：http://set.xingfuxueyuan.xyz

#include <stdio.h>
来源：http://xtp.tian-w.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zkl.tian-w.cn

[S02] C：变量与格式化输出
来源：http://oij.c1oappe.top

int a = 10; printf("%d\n", a);
来源：http://tcx.cheryme.top

[S03] C：读入整数
来源：http://ycg.gaohongyu789.top

int x; scanf("%d", &x);
来源：http://pto.aibaodan.cn

[S04] C：字符串复制
来源：http://olf.0kj1m.cn

char dst[32]; strcpy(dst, "hi");
来源：http://avz.ehwqpu.com

[S05] C：字符串长度
来源：http://ckm.havefunace.top

strlen(s)
来源：http://nzg.svipenyu.cn

[S06] C：字符串比较
来源：http://ojn.haohaochexian.top

strcmp(a, b) == 0
来源：http://arb.yuxming.cn

[S07] C：数组遍历求和
来源：http://fpp.cheryme.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ygm.aibaodan.cn

[S08] C：动态内存分配与释放
来源：http://xiq.guowangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zcc.sysykeji.top

[S09] C：结构体定义与初始化
来源：http://vrv.shuidangran.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iya.hywenlv.cn

[S10] C：指针与解引用
来源：http://veo.andypj.xyz

int *p = &a;  *p = 5;
来源：http://dey.chenjidiqi.icu

[S11] C：逐行读文件
来源：http://woo.dashuyun.cn

FILE *f = fopen("a.txt", "r");
来源：http://ais.yangfankeji.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://jpp.jinyuanbaomall.cn

fclose(f);
来源：http://jjt.yj202588.top

[S12] C：写文件
来源：http://vxf.ybcxt.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xiy.daxiang520.top

[S13] C：宏定义
来源：http://cul.iojbl.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jie.zhixingplan.top

[S14] C：枚举
来源：http://ugw.hnqzz.top

enum Color { RED, GREEN, BLUE };
来源：http://kiq.xinyue.icu

[S15] C：类型转换
来源：http://wof.ivvv.top

(double) a / b
来源：http://mdm.mhx1999.top

[S16] C：位操作置位
来源：http://tae.haohaochexian.top

x |= (1 << 3);
来源：http://smz.kuanghao11.cn

[S17] C：安全拼接字符串
来源：http://ajd.hywenlv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://syy.havefunace.top

[S18] C：命令行参数
来源：http://sbx.hcnkem.com

int main(int argc, char **argv)
来源：http://kku.xuetiantiany.cn

[S19] C：快速排序
来源：http://eih.hnqzz.top

qsort(a, n, sizeof(int), cmp);
来源：http://qlv.ydzc1.top

[S20] C：二分查找
来源：http://ypk.bjfxy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://imc.vqdsnc.cn

[S21] C：字符类别判断
来源：http://adw.ybcxt.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ymm.yuxming.cn

[S22] C：字符串转数字
来源：http://awj.hnqzz.top

atoi("42");  strtod("3.14", NULL);
来源：http://okx.fengsongda.top

[S23] C：随机数
来源：http://epo.tarul.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bnq.ctjpmb.com

[S24] C：获取本地时间
来源：http://tjh.ehwqpu.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ull.havefunace.top

[S25] C：内存拷贝
来源：http://pte.shanyushiyangtech.top

memcpy(dst, src, n);
来源：http://pbg.guannengcc.top

[S26] C：内存清零
来源：http://utj.birdmap.top

memset(a, 0, sizeof a);
来源：http://izz.yongpay.top

[S27] C：定义常量
来源：http://sxy.yvedp.cn

const double PI = 3.14159;
来源：http://xnl.nanxuanxn.top

[S28] C：静态变量
来源：http://vgu.mhx1999.top

static int counter = 0;
来源：http://icu.0kj1m.cn

[S29] C：变参函数
来源：http://yds.0kj1m.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uoj.fanxiaobao.xyz

[S30] C：头文件保护
来源：http://rhk.meibo888.top

#ifndef X_H
来源：http://etx.fehbvm.com

#define X_H
来源：http://oye.cashguo.top

#endif
来源：http://ely.shzxlz.cn

[S31] C++：Hello World
来源：http://fwn.316326.xyz

#include <iostream>
来源：http://nhz.yj202588.top

int main() { std::cout << "Hello\n"; }
来源：http://tfg.fengsongda.top

[S32] C++：字符串
来源：http://puy.havefunace.top

std::string s = "hi";  s += "!";
来源：http://pul.sysykeji.top

[S33] C++：vector 增删
来源：http://gtd.hongshengwenyu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kdd.jinyuanbaomall.cn

[S34] C++：遍历 vector
来源：http://hfl.andypj.xyz

for (auto &x : v) { std::cout << x; }
来源：http://wjc.pycfn.com

[S35] C++：map
来源：http://xrm.jiagoushi.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ftk.haohaochexian.top

[S36] C++：unordered_map
来源：http://dgc.xuetiantiany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wmy.52xcode.cn

[S37] C++：set
来源：http://uuw.yj202588.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gin.zhengqikj.top

[S38] C++：排序
来源：http://jcm.ydzc1.top

std::sort(v.begin(), v.end());
来源：http://wrx.cqqwz.cn

[S39] C++：自定义比较器排序
来源：http://mjy.jinqigufen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lzs.hammf.cn

[S40] C++：查找元素
来源：http://dak.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ayk.shanyushiyangtech.top


<!-- 参考信息 -->