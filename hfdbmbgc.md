代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wid.shanyushiyangtech.top

[Q58] 累计求和
来源：http://xjz.cashguo.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yzl.zhijiandao.cn

[Q59] 分组内累计
来源：http://cth.jqgfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://amn.jinqigufen.top

[Q60] 取上一行 / 下一行
来源：http://haf.cashguo.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ehf.hongshengwenyu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vij.haohaochexian.top

[Q61] 移动平均
来源：http://byo.yj202588.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yib.sxryk.cn

[Q62] 分组占比
来源：http://vrv.shuidangran.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fpw.zhengqikj.top

[Q63] 开启事务
来源：http://fjs.gzhubu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ucy.cucudq.cn

[Q64] 提交事务
来源：http://mff.zhengqikj.top

COMMIT;
来源：http://ibj.zhoulong.xyz

[Q65] 回滚事务
来源：http://sbx.cqqwz.cn

ROLLBACK;
来源：http://wkd.mhx1999.top

[Q66] 行锁查询
来源：http://vcw.hcnkem.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jwr.xziqi.cn

[Q67] 设置隔离级别
来源：http://yll.yonumen.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vpm.yj20258888.top

[Q68] 保存点
来源：http://awq.cucudq.cn

SAVEPOINT sp1;
来源：http://qxy.c1oappe.top

ROLLBACK TO sp1;
来源：http://mub.hongshengwenyu.top

[Q69] 查看执行计划
来源：http://eeo.cashguo.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lqb.jinqigufen.top

[Q70] 更新统计信息
来源：http://iec.yongpay.top

ANALYZE TABLE users;
来源：http://tis.cdnleiting.top

[Q71] 查看建表语句
来源：http://udo.tian-w.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mme.fktsv.cn

[Q72] 查看索引
来源：http://dwu.xuetiantiany.cn

SHOW INDEX FROM users;
来源：http://tmh.chenjidiqi.icu

[Q73] 查看表状态
来源：http://nvi.havefunace.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rxd.chenlongwang.top

[Q74] 强制使用索引
来源：http://kgc.havefunace.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://maf.yongpay.top

[Q75] 日期格式化
来源：http://eju.daxiang520.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tzp.0kj1m.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zvz.fzhhl.top

[Q76] 按天统计
来源：http://wds.fanxiaobao.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yii.xuetiantiany.cn

[Q77] 时间加减
来源：http://myq.fengsongda.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://onx.shanyushiyangkeji.top

[Q78] 当前时间
来源：http://udq.nanxinkj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zlp.cucudq.cn

[Q79] 字符串拼接
来源：http://fmr.meibo888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mig.316326.xyz

[Q80] 字符串截取
来源：http://elk.yanxiufei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cdq.yangfankeji.com

[Q81] 字符串替换
来源：http://szn.xuanzx.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iid.zhongyouzk.top

[Q82] 字符长度与字节长度
来源：http://yui.gaohongyu789.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nmh.yj20258888.top

[Q83] 大小写转换
来源：http://kdb.zhixingplan.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rsh.yonumen.top

[Q84] 去除首尾空格
来源：http://dfs.hfpthk.cn

SELECT TRIM(name) FROM users;
来源：http://gvj.nwbrower.top

[Q85] 数值取整
来源：http://cps.daxiang520.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yhg.gzhubu.top

[Q86] 读取 JSON 字段
来源：http://qox.xuanzx.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ygo.quarkkingdee.top

[Q87] JSON 字段做条件
来源：http://lmx.xziqi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://unk.fehbvm.com

[Q88] 行转列（条件聚合）
来源：http://aqv.jlsjyb.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://onc.pycfn.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ors.gogol.net.cn

[Q89] 判断表是否存在
来源：http://ysc.mhx1999.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nfh.chenzaomai.com

[Q90] 生成序号列
来源：http://oyo.zhongyouzk.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kpo.nanxinkj.top

================================================================================
来源：http://tpq.dashuyun.cn

R. Bash 专题
来源：http://wrt.zhoulong.xyz

================================================================================
来源：http://dqq.zhaomingkeji.xyz

[R01] shebang 与严格模式
来源：http://pvf.nanxuanxn.top

#!/usr/bin/env bash
来源：http://ily.jlsjyb.cn

set -euo pipefail
来源：http://scf.jlsjyb.cn

[R02] 变量赋值与使用
来源：http://gcl.shanyushiyangtech.top

name="Tom"; echo "$name"
来源：http://pyk.yj20258.top

[R03] 只读变量
来源：http://mpi.tianlin.xyz

readonly PI=3.14
来源：http://dss.zdqjudy.top

[R04] 位置参数
来源：http://gbu.jlsjyb.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://awn.ydzc1.top

[R05] 参数默认值
来源：http://zak.jinghuilouyu.cn

name="${1:-default}"
来源：http://oeq.ctjpmb.com

[R06] 判断命令是否存在
来源：http://prv.ivvv.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vhq.hammf.cn

[R07] if 判断文件
来源：http://uac.ppjwa.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://las.daxiang520.top

[R08] 数值比较
来源：http://bff.zdbjq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bri.hnqzz.top

[R09] 字符串比较
来源：http://kjs.chenzaomai.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://knz.0kj1m.cn

[R10] 正则匹配
来源：http://rin.shangyingyoupin.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://stb.birdmap.top

[R11] case 多分支
来源：http://afy.fehbvm.com

case "$1" in
来源：http://keq.guowangkeji.top

start) echo "启动" ;;
来源：http://qpx.epnwcf.com

stop)  echo "停止" ;;
来源：http://vep.xylfe.cn

*)     echo "未知命令" ;;
来源：http://blh.ydjk.org.cn

esac
来源：http://zqj.cheryme.top

[R12] for 遍历文件
来源：http://svd.ppjwa.cn

for f in *.txt; do echo "$f"; done
来源：http://dew.jqgfzy.top

[R13] for 计数循环
来源：http://sva.cheryme.top

for i in {1..10}; do echo "$i"; done
来源：http://cfj.dashuyun.cn

[R14] C 风格 for
来源：http://kuq.yj202588.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sxu.uphjek.com

[R15] while 逐行读文件
来源：http://mqe.yj20258.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pmf.vehdjk.com

[R16] until 等待条件
来源：http://zcv.guannengcc.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://diq.pycfn.com

[R17] 数组定义与取值
来源：http://wtl.sweek.top

arr=(a b c); echo "${arr[0]}"
来源：http://zla.andypj.xyz

[R18] 遍历数组
来源：http://ohk.nanxuanxn.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vol.chenjidiqi.icu

[R19] 数组长度
来源：http://pmx.feifeiyinyue.top

echo "${#arr[@]}"
来源：http://eep.kuanghao11.cn

[R20] 关联数组（字典）
来源：http://fvj.jlsjyb.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pla.vqdsnc.cn

[R21] 字符串长度
来源：http://ptw.jinghuilouyu.cn

echo "${#s}"
来源：http://bzs.zdbjq.cn

[R22] 截取子串
来源：http://lls.yanxiufei.cn

echo "${s:0:5}"
来源：http://lwm.tianlin.xyz

[R23] 字符串替换
来源：http://bwh.jinqigfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bcf.smart0.xyz

[R24] 大小写转换
来源：http://fwa.nanxuanxn.top

echo "${s^^}"; echo "${s,,}"
来源：http://vxm.yvedp.cn

[R25] 去后缀 / 去前缀
来源：http://qhj.svipenyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vbt.yonumen.top

[R26] 命令替换
来源：http://xpm.hnxiangtu.top

now=$(date +%F); echo "$now"
来源：http://swi.jinyuanbaomall.cn

[R27] 算术展开
来源：http://jmp.zhiwuduotai.top

echo $((1 + 2 * 3))
来源：http://ldy.cheryme.top

[R28] 浮点运算
来源：http://zyx.jinyuanbaomall.cn

echo "scale=2; 10/3" | bc
来源：http://gof.fzhhl.top

[R29] 定义函数
来源：http://zdf.9152youxi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yel.tanke756.top

[R30] 函数返回状态码
来源：http://brh.9152youxi.cn

f() { return 0; }; f || echo "失败了"
来源：http://wir.smart0.xyz

[R31] 局部变量
来源：http://net.chenlongwang.top

f() { local x=1; echo "$x"; }
来源：http://ylp.dashuyun.cn

[R32] 参数个数校验
来源：http://obt.hammf.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ayq.shanyushiyangtech.top

[R33] 捕获错误并提示行号
来源：http://bbh.dashuyun.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://boe.xuanzx.com

[R34] 退出时清理
来源：http://zld.gzhubu.top

trap 'rm -f "$tmp"' EXIT
来源：http://hwb.nwbrower.top

[R35] 后台执行并等待
来源：http://lgu.kuanghao11.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jxo.fanxiaobao.xyz

[R36] 并发执行多个任务
来源：http://tgl.chenjidiqi.icu

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jrl.cashguo.top

[R37] 把输出赋给变量
来源：http://opg.yonumen.top

files=$(ls -1)
来源：http://jui.gotoacloud.top

[R38] 管道串联
来源：http://yed.cqqwz.cn

cat a.txt | grep -i error | wc -l
来源：http://sae.hnqzz.top

[R39] 重定向标准输出与错误
来源：http://kzl.shangyingyoupin.top

cmd > out.log 2>&1
来源：http://sqx.snrcjt.cn

[R40] 追加写日志
来源：http://tus.xinyue.icu

echo "log" >> out.log
来源：http://ces.gaohongyu789.top

[R41] 丢弃输出
来源：http://cbm.iojbl.cn

cmd >/dev/null 2>&1
来源：http://zxp.yfazqb.com

[R42] 输入重定向
来源：http://cxe.yueranfly.top

wc -l < a.txt
来源：http://izp.yangfankeji.com

[R43] 按名字查找文件
来源：http://uzy.hywenlv.cn

find . -name "*.log" -type f
来源：http://jfk.hywenlv.cn

[R44] 按修改时间查找
来源：http://buu.hcnkem.com

find . -mtime -7 -type f
来源：http://rwa.zhixingplan.top

[R45] 批量删除
来源：http://nvk.havefunace.top

find . -name "*.tmp" -delete
来源：http://yko.shzxlz.cn

[R46] 递归替换文件内容
来源：http://jby.hcnkem.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xdr.tian-w.cn

[R47] sed 单行替换
来源：http://igz.nanxinkj.top

sed -i 's/foo/bar/g' a.txt
来源：http://uvb.hammf.cn

[R48] awk 取指定列
来源：http://kfs.bjfxy.top

awk '{print $1, $3}' a.txt
来源：http://bel.jqgufenzy.top

[R49] awk 带条件
来源：http://fti.aibaodan.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://seb.fzhhl.top

[R50] awk 求和
来源：http://tzj.fzhhl.top

awk '{s += $2} END {print s}' a.txt
来源：http://fdh.fktsv.cn

[R51] 排序去重取前几
来源：http://iam.jqgufenzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ufb.ybcxt.top

[R52] 统计行数
来源：http://qsl.mhx1999.top

wc -l a.txt
来源：http://ecq.gogol.net.cn

[R53] 查看文件头与实时尾
来源：http://rdq.yangfankeji.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zbk.pengpengdd.cyou

[R54] 比较两个文件
来源：http://lrm.ppjwa.cn

diff a.txt b.txt
来源：http://vsu.316326.xyz

[R55] 压缩与解压
来源：http://olo.ivvv.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qbp.sufxvd.cn

[R56] 远程拷贝
来源：http://ybf.zhiwuduotai.top

scp file user@host:/path/
来源：http://ain.jinqigufen.top

[R57] 远程执行命令
来源：http://scv.mhx1999.top

ssh user@host 'uptime'
来源：http://xgo.sjlbkw.cn

[R58] 下载文件
来源：http://and.yuanzhike.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ycv.zhaomingkeji.xyz

[R59] 发 POST JSON
来源：http://riz.fzhhl.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wgp.fehbvm.com

[R60] 只看 HTTP 状态码
来源：http://fou.yvedp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gtf.fehbvm.com

[R61] 磁盘占用
来源：http://pab.c1oappe.top

df -h;  du -sh *
来源：http://ckg.aizwys.cn

[R62] 找最占空间的文件
来源：http://wdw.xuetiantiany.cn

du -ah . | sort -rh | head -10
来源：http://vai.jinyuanbaomall.cn

[R63] 内存与进程
来源：http://yex.bjfxy.top

free -h;  ps aux | grep nginx
来源：http://nfm.redwolf501.top

[R64] 结束进程
来源：http://urs.yanxiufei.cn

kill -9 $(pgrep -f app.py)
来源：http://nfu.yangfankeji.com

[R65] 查看端口占用
来源：http://rxb.cdnleiting.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lsq.smart0.xyz

[R66] 定时任务
来源：http://gfu.hesvh.cn

crontab -e;  crontab -l
来源：http://gec.cheryme.top

[R67] 生成随机十六进制串
来源：http://qmh.tianlin.xyz

openssl rand -hex 16
来源：http://otp.ppjwa.cn

[R68] 计算文件校验值
来源：http://hib.cashguo.top

sha256sum a.txt;  md5sum a.txt
来源：http://wvp.iojbl.cn

[R69] 生成随机密码
来源：http://xql.sxryk.cn

head -c 16 /dev/urandom | base64
来源：http://kqs.yuxming.cn

[R70] 时间戳与互转
来源：http://jbs.redwolf501.top

date +%s;  date -d @1700000000
来源：http://uql.yuanzhike.top

[R71] 日期格式化
来源：http://lxf.yanxiufei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jca.yj20258.top

[R72] 等待端口就绪
来源：http://eqd.yongpay.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mrm.jianghu66.top

[R73] 分割大日志
来源：http://kdv.jyoumei.cn

split -l 1000 big.log part_
来源：http://brp.yonumen.top

[R74] 批量重命名
来源：http://lcm.guannengcc.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aem.svipenyu.cn

[R75] 导出环境变量
来源：http://xqq.svipenyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://ctj.yvedp.cn

[R76] 使用临时文件
来源：http://tqh.chenzaomai.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xie.tianlin.xyz

[R77] 读取用户输入
来源：http://che.epnwcf.com

read -rp "请输入: " ans
来源：http://ybr.meibo888.top

[R78] 交互式菜单
来源：http://rzw.wangshuangyany.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xjf.sufxvd.cn

[R79] 解析命令行选项
来源：http://old.yuxming.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fpr.cashguo.top

[R80] 查看脚本执行耗时
来源：http://bct.ctjpmb.com

time ./run.sh
来源：http://znx.pengpengdd.cyou

================================================================================
来源：http://afy.wangdashe.top

S. C / C++ 专题
来源：http://lsu.yangfankeji.com

================================================================================
来源：http://kmk.tianlin.xyz

[S01] C：Hello World
来源：http://ygz.yonumen.top

#include <stdio.h>
来源：http://tfj.ivvv.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jst.cheryme.top

[S02] C：变量与格式化输出
来源：http://lmm.yuxming.cn

int a = 10; printf("%d\n", a);
来源：http://ztf.meibo888.top

[S03] C：读入整数
来源：http://djw.guowangkeji.top

int x; scanf("%d", &x);
来源：http://uww.tanke756.top

[S04] C：字符串复制
来源：http://rwy.sufxvd.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nlc.zhaomingkeji.xyz

[S05] C：字符串长度
来源：http://hrp.chenjidiqi.icu

strlen(s)
来源：http://esp.snrcjt.cn

[S06] C：字符串比较
来源：http://kbf.aizwys.cn

strcmp(a, b) == 0
来源：http://lem.zycfv.cn

[S07] C：数组遍历求和
来源：http://dcp.shanyushiyangtech.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pof.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://ctb.xziqi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mmt.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://jdt.bjfxy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hwi.hnqzz.top

[S10] C：指针与解引用
来源：http://dsc.pycfn.com

int *p = &a;  *p = 5;
来源：http://ahc.zhaomingkeji.xyz

[S11] C：逐行读文件
来源：http://jqv.wangdashe.top

FILE *f = fopen("a.txt", "r");
来源：http://rud.jinqigfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tmg.ehwqpu.com

fclose(f);
来源：http://rnn.cucudq.cn

[S12] C：写文件
来源：http://cnn.jinghuilouyu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://apo.xingfuxueyuan.xyz

[S13] C：宏定义
来源：http://itl.zhiwuduotai.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bzv.yonumen.top

[S14] C：枚举
来源：http://xpt.hywenlv.cn

enum Color { RED, GREEN, BLUE };
来源：http://stm.nanxinkj.top

[S15] C：类型转换
来源：http://hog.shzxlz.cn

(double) a / b
来源：http://abb.xingfuxueyuan.xyz

[S16] C：位操作置位
来源：http://lvv.sxryk.cn

x |= (1 << 3);
来源：http://odj.jianghu66.top

[S17] C：安全拼接字符串
来源：http://xyo.gzhubu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qpj.xingfuxueyuan.xyz

[S18] C：命令行参数
来源：http://nen.gogol.net.cn

int main(int argc, char **argv)
来源：http://byl.cheryme.top

[S19] C：快速排序
来源：http://ipn.shanyushiyangtech.top

qsort(a, n, sizeof(int), cmp);
来源：http://bpg.jianghu66.top

[S20] C：二分查找
来源：http://ydj.hysaishi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ewx.zhijiandao.cn

[S21] C：字符类别判断
来源：http://zbp.52xcode.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lwx.daxiang520.top

[S22] C：字符串转数字
来源：http://qvf.jlsjyb.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vzw.hfpthk.cn

[S23] C：随机数
来源：http://axs.jyoumei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vrt.kuanghao11.cn

[S24] C：获取本地时间
来源：http://oor.jinghuilouyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://svv.tian-w.cn

[S25] C：内存拷贝
来源：http://ukt.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://hyk.jqgufenzy.top

[S26] C：内存清零
来源：http://jjb.tarul.cn

memset(a, 0, sizeof a);
来源：http://xjc.gotoacloud.top

[S27] C：定义常量
来源：http://plp.shangyingyoupin.top

const double PI = 3.14159;
来源：http://oyt.wangdashe.top

[S28] C：静态变量
来源：http://nub.jlsjyb.cn


<!-- 参考信息 -->