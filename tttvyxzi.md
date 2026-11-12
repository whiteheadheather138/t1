代发 wailian999

[Q61] 移动平均
来源：http://unx.aibaodan.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uou.chenlongwang.top

[Q62] 分组占比
来源：http://tvs.sjlbkw.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lma.sxryk.cn

[Q63] 开启事务
来源：http://ufa.daria6918.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sct.wangshuangyany.cn

[Q64] 提交事务
来源：http://nag.pengpengdd.cyou

COMMIT;
来源：http://pjd.hesvh.cn

[Q65] 回滚事务
来源：http://mxy.chenjidiqi.icu

ROLLBACK;
来源：http://paz.iojbl.cn

[Q66] 行锁查询
来源：http://rie.tian-w.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qaw.aizwys.cn

[Q67] 设置隔离级别
来源：http://kui.tian-w.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fpc.xylfe.cn

[Q68] 保存点
来源：http://edy.sufxvd.cn

SAVEPOINT sp1;
来源：http://kbz.xziqi.cn

ROLLBACK TO sp1;
来源：http://fcr.jinghuilouyu.cn

[Q69] 查看执行计划
来源：http://ptx.wangdashe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://djg.yonumen.top

[Q70] 更新统计信息
来源：http://int.kuanghao11.cn

ANALYZE TABLE users;
来源：http://tac.gzhubu.top

[Q71] 查看建表语句
来源：http://axz.52xcode.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ona.redwolf501.top

[Q72] 查看索引
来源：http://vqj.tarul.cn

SHOW INDEX FROM users;
来源：http://ytq.jinqigfzy.top

[Q73] 查看表状态
来源：http://vbk.hongshengwenyu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bql.wangshuangyany.cn

[Q74] 强制使用索引
来源：http://ywj.birdmap.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jce.jiagoushi.top

[Q75] 日期格式化
来源：http://dfd.hesvh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nlu.aibaodan.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://axi.yangfankeji.com

[Q76] 按天统计
来源：http://sbr.vqdsnc.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uls.pengpengdd.cyou

[Q77] 时间加减
来源：http://khb.fktsv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xrn.tianlin.xyz

[Q78] 当前时间
来源：http://rry.fengsongda.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wws.fktsv.cn

[Q79] 字符串拼接
来源：http://abe.jinghuilouyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ifn.yuxming.cn

[Q80] 字符串截取
来源：http://miy.yvedp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qxt.yangfankeji.com

[Q81] 字符串替换
来源：http://fzf.shangyingyoupin.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tos.pengpengdd.cyou

[Q82] 字符长度与字节长度
来源：http://fvq.shzxlz.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ebq.snrcjt.cn

[Q83] 大小写转换
来源：http://urv.hesvh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mkl.yongpay.top

[Q84] 去除首尾空格
来源：http://gwj.xziqi.cn

SELECT TRIM(name) FROM users;
来源：http://nud.mhx1999.top

[Q85] 数值取整
来源：http://jnf.redwolf501.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bqx.hnqzz.top

[Q86] 读取 JSON 字段
来源：http://emv.haohaochexian.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bnf.tian-w.cn

[Q87] JSON 字段做条件
来源：http://ssa.yj20258888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://etn.hammf.cn

[Q88] 行转列（条件聚合）
来源：http://fcp.cheryme.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://exo.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qyt.vqdsnc.cn

[Q89] 判断表是否存在
来源：http://dlw.ppjwa.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tcn.snrcjt.cn

[Q90] 生成序号列
来源：http://gne.hongshengwenyu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jna.ydzc1.top

================================================================================
来源：http://onk.yuxming.cn

R. Bash 专题
来源：http://pxi.cashguo.top

================================================================================
来源：http://inm.nwbrower.top

[R01] shebang 与严格模式
来源：http://xhg.havefunace.top

#!/usr/bin/env bash
来源：http://cyk.zdqjudy.top

set -euo pipefail
来源：http://zpa.cqqwz.cn

[R02] 变量赋值与使用
来源：http://cxy.jyoumei.cn

name="Tom"; echo "$name"
来源：http://abe.smart0.xyz

[R03] 只读变量
来源：http://ils.fehbvm.com

readonly PI=3.14
来源：http://qso.xylfe.cn

[R04] 位置参数
来源：http://xqf.gogol.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://miv.smart0.xyz

[R05] 参数默认值
来源：http://qfy.haohaochexian.top

name="${1:-default}"
来源：http://tmn.wangdashe.top

[R06] 判断命令是否存在
来源：http://ize.ydjk.org.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dtm.xuanzx.com

[R07] if 判断文件
来源：http://dmf.hcnkem.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tvf.wangdashe.top

[R08] 数值比较
来源：http://hke.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lqf.ppjwa.cn

[R09] 字符串比较
来源：http://vwb.sufxvd.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hzi.xingfuxueyuan.xyz

[R10] 正则匹配
来源：http://kbx.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://roe.nwbrower.top

[R11] case 多分支
来源：http://ggn.jqgufenzy.top

case "$1" in
来源：http://cuu.316326.xyz

start) echo "启动" ;;
来源：http://nez.ehwqpu.com

stop)  echo "停止" ;;
来源：http://xbl.xuanzx.com

*)     echo "未知命令" ;;
来源：http://uqd.zhixingplan.top

esac
来源：http://kqh.hnqzz.top

[R12] for 遍历文件
来源：http://jtt.sjlbkw.cn

for f in *.txt; do echo "$f"; done
来源：http://ggm.smart0.xyz

[R13] for 计数循环
来源：http://fwd.havefunace.top

for i in {1..10}; do echo "$i"; done
来源：http://wai.chenzaomai.com

[R14] C 风格 for
来源：http://jsv.fktsv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ciq.yanxiufei.cn

[R15] while 逐行读文件
来源：http://xlj.jqgufenzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yxz.tarul.cn

[R16] until 等待条件
来源：http://fzf.hnxiangtu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dct.fzhhl.top

[R17] 数组定义与取值
来源：http://zyk.hnxiangtu.top

arr=(a b c); echo "${arr[0]}"
来源：http://ghv.quarkkingdee.top

[R18] 遍历数组
来源：http://isn.jinyuanbaomall.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gjk.zhengqikj.top

[R19] 数组长度
来源：http://eyc.jyoumei.cn

echo "${#arr[@]}"
来源：http://ltn.sysykeji.top

[R20] 关联数组（字典）
来源：http://eug.yonumen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gyk.316326.xyz

[R21] 字符串长度
来源：http://dta.xingfuxueyuan.xyz

echo "${#s}"
来源：http://nty.cqqwz.cn

[R22] 截取子串
来源：http://out.sxryk.cn

echo "${s:0:5}"
来源：http://vgf.yj20258888.top

[R23] 字符串替换
来源：http://num.xziqi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://six.yongpay.top

[R24] 大小写转换
来源：http://lbe.yanxiufei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://aou.ydjk.org.cn

[R25] 去后缀 / 去前缀
来源：http://bst.yvedp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xeb.birdmap.top

[R26] 命令替换
来源：http://vcp.guowangkeji.top

now=$(date +%F); echo "$now"
来源：http://hig.sxryk.cn

[R27] 算术展开
来源：http://pgk.ivvv.top

echo $((1 + 2 * 3))
来源：http://bqz.fzhhl.top

[R28] 浮点运算
来源：http://xbp.bbcook.cn

echo "scale=2; 10/3" | bc
来源：http://esi.gzhubu.top

[R29] 定义函数
来源：http://mtx.zhengqikj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mpu.shuidangran.top

[R30] 函数返回状态码
来源：http://okp.pengpengdd.cyou

f() { return 0; }; f || echo "失败了"
来源：http://qft.epnwcf.com

[R31] 局部变量
来源：http://thj.nanxuanxn.top

f() { local x=1; echo "$x"; }
来源：http://yws.jinqigufen.top

[R32] 参数个数校验
来源：http://rmc.hnxiangtu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zzv.chenjidiqi.icu

[R33] 捕获错误并提示行号
来源：http://qjj.jinqigufen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ljt.chenzaomai.com

[R34] 退出时清理
来源：http://uyw.hcnkem.com

trap 'rm -f "$tmp"' EXIT
来源：http://euk.xuetiantiany.cn

[R35] 后台执行并等待
来源：http://kys.fanxiaobao.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://wwl.ydjk.org.cn

[R36] 并发执行多个任务
来源：http://xcc.pycfn.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jwa.ydjk.org.cn

[R37] 把输出赋给变量
来源：http://frp.cqqwz.cn

files=$(ls -1)
来源：http://mkm.guannengcc.top

[R38] 管道串联
来源：http://vvj.jinqigfzy.top

cat a.txt | grep -i error | wc -l
来源：http://dtx.quarkkingdee.top

[R39] 重定向标准输出与错误
来源：http://adh.ydzc1.top

cmd > out.log 2>&1
来源：http://hto.tianlin.xyz

[R40] 追加写日志
来源：http://oem.jyoumei.cn

echo "log" >> out.log
来源：http://ogx.redwolf501.top

[R41] 丢弃输出
来源：http://sdk.fengsongda.top

cmd >/dev/null 2>&1
来源：http://cxt.zycfv.cn

[R42] 输入重定向
来源：http://rgx.fktsv.cn

wc -l < a.txt
来源：http://cvz.hfpthk.cn

[R43] 按名字查找文件
来源：http://cjp.cheryme.top

find . -name "*.log" -type f
来源：http://hku.tarul.cn

[R44] 按修改时间查找
来源：http://alv.mhx1999.top

find . -mtime -7 -type f
来源：http://whr.fzhhl.top

[R45] 批量删除
来源：http://wik.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://wco.ywan-chungtsiang.top

[R46] 递归替换文件内容
来源：http://sry.yvedp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://idd.xuanzx.com

[R47] sed 单行替换
来源：http://ajr.uphjek.com

sed -i 's/foo/bar/g' a.txt
来源：http://gyu.pengpengdd.cyou

[R48] awk 取指定列
来源：http://xdu.uphjek.com

awk '{print $1, $3}' a.txt
来源：http://ybc.sufxvd.cn

[R49] awk 带条件
来源：http://ktj.yj20258888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kei.uphjek.com

[R50] awk 求和
来源：http://akm.yongpay.top

awk '{s += $2} END {print s}' a.txt
来源：http://saw.316326.xyz

[R51] 排序去重取前几
来源：http://web.jqgfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://heu.birdmap.top

[R52] 统计行数
来源：http://uur.iojbl.cn

wc -l a.txt
来源：http://xlu.daxiang520.top

[R53] 查看文件头与实时尾
来源：http://ftr.yfazqb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jno.ywan-chungtsiang.top

[R54] 比较两个文件
来源：http://wip.jlsjyb.cn

diff a.txt b.txt
来源：http://nvj.jinghuilouyu.cn

[R55] 压缩与解压
来源：http://whz.hywenlv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ydz.yueranfly.top

[R56] 远程拷贝
来源：http://nrq.yj20258.top

scp file user@host:/path/
来源：http://urg.chenlongwang.top

[R57] 远程执行命令
来源：http://zuq.snrcjt.cn

ssh user@host 'uptime'
来源：http://kki.yanxiufei.cn

[R58] 下载文件
来源：http://via.shangyingyoupin.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qmq.gaohongyu789.top

[R59] 发 POST JSON
来源：http://kmn.xuetiantiany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xik.xinyue.icu

[R60] 只看 HTTP 状态码
来源：http://hvj.havefunace.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ccd.iojbl.cn

[R61] 磁盘占用
来源：http://uid.sufxvd.cn

df -h;  du -sh *
来源：http://ygp.fehbvm.com

[R62] 找最占空间的文件
来源：http://aoz.shuidangran.top

du -ah . | sort -rh | head -10
来源：http://qwa.zhiwuduotai.top

[R63] 内存与进程
来源：http://jnp.jinqigufen.top

free -h;  ps aux | grep nginx
来源：http://avb.yuanzhike.top

[R64] 结束进程
来源：http://wvw.hnqzz.top

kill -9 $(pgrep -f app.py)
来源：http://lam.yvedp.cn

[R65] 查看端口占用
来源：http://shv.yanxiufei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://chx.shangyingyoupin.top

[R66] 定时任务
来源：http://gsb.yuxming.cn

crontab -e;  crontab -l
来源：http://ryz.epnwcf.com

[R67] 生成随机十六进制串
来源：http://elk.yangfankeji.com

openssl rand -hex 16
来源：http://agz.hesvh.cn

[R68] 计算文件校验值
来源：http://diy.gotoacloud.top

sha256sum a.txt;  md5sum a.txt
来源：http://ake.aizwys.cn

[R69] 生成随机密码
来源：http://wif.sjlbkw.cn

head -c 16 /dev/urandom | base64
来源：http://cnv.xuetiantiany.cn

[R70] 时间戳与互转
来源：http://ucn.shanyushiyangkeji.top

date +%s;  date -d @1700000000
来源：http://zex.hesvh.cn

[R71] 日期格式化
来源：http://mbe.cucudq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ipm.zhaomingkeji.xyz

[R72] 等待端口就绪
来源：http://qrk.ywan-chungtsiang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kpu.jqgfzy.top

[R73] 分割大日志
来源：http://fqq.gzhubu.top

split -l 1000 big.log part_
来源：http://yeu.kuanghao11.cn

[R74] 批量重命名
来源：http://mpd.zycfv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://joh.yanxiufei.cn

[R75] 导出环境变量
来源：http://wwf.haohaochexian.top

export PATH="$HOME/bin:$PATH"
来源：http://any.gaohongyu789.top

[R76] 使用临时文件
来源：http://nqf.ctjpmb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://huo.nanxinkj.top

[R77] 读取用户输入
来源：http://whz.fktsv.cn

read -rp "请输入: " ans
来源：http://bgi.jinqigufen.top

[R78] 交互式菜单
来源：http://ubc.daria6918.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ztn.mhx1999.top

[R79] 解析命令行选项
来源：http://rxe.chenjidiqi.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tgy.uphjek.com

[R80] 查看脚本执行耗时
来源：http://lgn.yangfankeji.com

time ./run.sh
来源：http://byd.chenlongwang.top

================================================================================
来源：http://mbn.yanxiufei.cn

S. C / C++ 专题
来源：http://xkx.sjlbkw.cn

================================================================================
来源：http://diq.chenlongwang.top

[S01] C：Hello World
来源：http://riu.52xcode.cn

#include <stdio.h>
来源：http://krc.ehwqpu.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://mih.316326.xyz

[S02] C：变量与格式化输出
来源：http://seq.dashuyun.cn

int a = 10; printf("%d\n", a);
来源：http://laz.hywenlv.cn

[S03] C：读入整数
来源：http://zne.wangshuangyany.cn

int x; scanf("%d", &x);
来源：http://obz.ydzc1.top

[S04] C：字符串复制
来源：http://cyt.chenlongwang.top

char dst[32]; strcpy(dst, "hi");
来源：http://cet.feifeiyinyue.top

[S05] C：字符串长度
来源：http://cxv.cashguo.top

strlen(s)
来源：http://vcg.tanke756.top

[S06] C：字符串比较
来源：http://uqr.zhaomingkeji.xyz

strcmp(a, b) == 0
来源：http://dyv.jyoumei.cn

[S07] C：数组遍历求和
来源：http://fuo.cucudq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://syb.yj20258.top

[S08] C：动态内存分配与释放
来源：http://mra.gzhubu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bgs.kuanghao11.cn

[S09] C：结构体定义与初始化
来源：http://rjd.vqdsnc.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lpp.smart0.xyz

[S10] C：指针与解引用
来源：http://npz.jyoumei.cn

int *p = &a;  *p = 5;
来源：http://btj.havefunace.top

[S11] C：逐行读文件
来源：http://khz.shanyushiyangtech.top

FILE *f = fopen("a.txt", "r");
来源：http://wcy.hammf.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cwj.zhaomingkeji.xyz

fclose(f);
来源：http://wsr.vehdjk.com

[S12] C：写文件
来源：http://jgp.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fqy.mhx1999.top

[S13] C：宏定义
来源：http://ajm.hnqzz.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yzz.bjfxy.top

[S14] C：枚举
来源：http://ang.zhengqikj.top

enum Color { RED, GREEN, BLUE };
来源：http://sap.316326.xyz

[S15] C：类型转换
来源：http://asd.yj202588.top

(double) a / b
来源：http://rjg.hammf.cn

[S16] C：位操作置位
来源：http://ztq.uphjek.com

x |= (1 << 3);
来源：http://cal.daria6918.cn

[S17] C：安全拼接字符串
来源：http://oua.daria6918.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fhz.yanxiufei.cn

[S18] C：命令行参数
来源：http://msq.daria6918.cn

int main(int argc, char **argv)
来源：http://nyr.bjfxy.top

[S19] C：快速排序
来源：http://zlf.redwolf501.top

qsort(a, n, sizeof(int), cmp);
来源：http://atr.jyoumei.cn

[S20] C：二分查找
来源：http://ghe.gogol.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iyj.yanxiufei.cn

[S21] C：字符类别判断
来源：http://ukf.cheryme.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eaw.jinqigfzy.top

[S22] C：字符串转数字
来源：http://oym.zhoulong.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://vdd.c1oappe.top

[S23] C：随机数
来源：http://ghb.tianlin.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://zsj.vqdsnc.cn

[S24] C：获取本地时间
来源：http://lzc.ppjwa.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lia.ehwqpu.com

[S25] C：内存拷贝
来源：http://ong.xziqi.cn

memcpy(dst, src, n);
来源：http://qal.nwbrower.top

[S26] C：内存清零
来源：http://lqz.bbcook.cn

memset(a, 0, sizeof a);
来源：http://fie.cheryme.top

[S27] C：定义常量
来源：http://cuc.epnwcf.com

const double PI = 3.14159;
来源：http://owk.cdnleiting.top

[S28] C：静态变量
来源：http://cpu.daxiang520.top

static int counter = 0;
来源：http://ghl.zhijiandao.cn

[S29] C：变参函数
来源：http://grp.yongpay.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zyv.snrcjt.cn

[S30] C：头文件保护
来源：http://sqe.sysykeji.top

#ifndef X_H
来源：http://qby.zhengqikj.top

#define X_H
来源：http://jrs.hysaishi.cn

#endif
来源：http://zdz.gzhubu.top

[S31] C++：Hello World
来源：http://ulr.hammf.cn


<!-- 参考信息 -->