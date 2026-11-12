代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://kpm.jyoumei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kvl.jinghuilouyu.cn

[Q47] 与平均值比较
来源：http://orh.jinyuanbaomall.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://elo.sysykeji.top

[Q48] CTE 公用表表达式
来源：http://nji.yvedp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hsc.bjfxy.top

SELECT * FROM t WHERE c > 5;
来源：http://atx.bjfxy.top

[Q49] 更新单行
来源：http://yiq.316326.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://smq.vqdsnc.cn

[Q50] 批量更新
来源：http://tzp.gzhubu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zho.daxiang520.top

[Q51] 用子查询更新
来源：http://ggi.aizwys.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pna.sufxvd.cn

[Q52] 删除指定行
来源：http://ywf.jinyuanbaomall.cn

DELETE FROM users WHERE id = 10;
来源：http://mey.chenzaomai.com

[Q53] 按条件删除
来源：http://fby.daxiang520.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wux.0kj1m.cn

[Q54] 清空表
来源：http://iyu.wangshuangyany.cn

TRUNCATE TABLE logs;
来源：http://roa.jianghu66.top

[Q55] 排名（并列占位）
来源：http://efe.birdmap.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oso.zdbjq.cn

[Q56] 密集排名（并列不占位）
来源：http://wtr.cucudq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fdu.ppjwa.cn

[Q57] 行号
来源：http://gfw.andypj.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ixl.haohaochexian.top

[Q58] 累计求和
来源：http://yib.hnxiangtu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lbc.mhx1999.top

[Q59] 分组内累计
来源：http://jqa.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mps.zhengqikj.top

[Q60] 取上一行 / 下一行
来源：http://irc.sxryk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://udu.yueranfly.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ojh.fktsv.cn

[Q61] 移动平均
来源：http://uzm.cucudq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mwf.zdbjq.cn

[Q62] 分组占比
来源：http://duc.chenzaomai.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bqh.nwbrower.top

[Q63] 开启事务
来源：http://mym.ivvv.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qff.xuetiantiany.cn

[Q64] 提交事务
来源：http://tvv.pengpengdd.cyou

COMMIT;
来源：http://ntc.svipenyu.cn

[Q65] 回滚事务
来源：http://syf.guowangkeji.top

ROLLBACK;
来源：http://hns.cashguo.top

[Q66] 行锁查询
来源：http://alo.sysykeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://azr.zdbjq.cn

[Q67] 设置隔离级别
来源：http://ahg.jianghu66.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cib.daxiang520.top

[Q68] 保存点
来源：http://ejh.dianchejie.cn

SAVEPOINT sp1;
来源：http://kfw.shanyushiyangkeji.top

ROLLBACK TO sp1;
来源：http://dzk.gotoacloud.top

[Q69] 查看执行计划
来源：http://dvb.jqgufenzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tnd.cdnleiting.top

[Q70] 更新统计信息
来源：http://fav.redwolf501.top

ANALYZE TABLE users;
来源：http://dud.wangshuangyany.cn

[Q71] 查看建表语句
来源：http://inx.yvedp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pmo.gaohongyu789.top

[Q72] 查看索引
来源：http://hax.nanxinkj.top

SHOW INDEX FROM users;
来源：http://pmz.fanxiaobao.xyz

[Q73] 查看表状态
来源：http://hbd.hfpthk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://efb.hongshengwenyu.top

[Q74] 强制使用索引
来源：http://kwu.hysaishi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fuk.0kj1m.cn

[Q75] 日期格式化
来源：http://boc.mhx1999.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eid.ctjpmb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://czj.hammf.cn

[Q76] 按天统计
来源：http://etj.52xcode.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://twi.dashuyun.cn

[Q77] 时间加减
来源：http://kcn.gaohongyu789.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bvv.fehbvm.com

[Q78] 当前时间
来源：http://mdz.gotoacloud.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://for.wangshuangyany.cn

[Q79] 字符串拼接
来源：http://xcm.zhiwuduotai.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://daw.wangdashe.top

[Q80] 字符串截取
来源：http://cft.ppjwa.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yjn.redwolf501.top

[Q81] 字符串替换
来源：http://lcs.mhx1999.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://der.tanke756.top

[Q82] 字符长度与字节长度
来源：http://eaf.dianchejie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zrv.zhixingplan.top

[Q83] 大小写转换
来源：http://fbl.guannengcc.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jnb.bbcook.cn

[Q84] 去除首尾空格
来源：http://qie.tanke756.top

SELECT TRIM(name) FROM users;
来源：http://otp.ehwqpu.com

[Q85] 数值取整
来源：http://dcv.wangdashe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ifa.shanyushiyangtech.top

[Q86] 读取 JSON 字段
来源：http://guj.feifeiyinyue.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hti.zhoulong.xyz

[Q87] JSON 字段做条件
来源：http://qwo.zycfv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bjs.c1oappe.top

[Q88] 行转列（条件聚合）
来源：http://iya.smart0.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uty.zhaomingkeji.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lud.hcnkem.com

[Q89] 判断表是否存在
来源：http://irf.pengpengdd.cyou

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qsy.daxiang520.top

[Q90] 生成序号列
来源：http://gcn.fehbvm.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ugg.aibaodan.cn

================================================================================
来源：http://gfs.wangshuangyany.cn

R. Bash 专题
来源：http://nug.jinyuanbaomall.cn

================================================================================
来源：http://vqm.redwolf501.top

[R01] shebang 与严格模式
来源：http://bjk.sxryk.cn

#!/usr/bin/env bash
来源：http://mfl.jyoumei.cn

set -euo pipefail
来源：http://ljq.pengpengdd.cyou

[R02] 变量赋值与使用
来源：http://cnl.shangyingyoupin.top

name="Tom"; echo "$name"
来源：http://tzm.yuxming.cn

[R03] 只读变量
来源：http://keh.xziqi.cn

readonly PI=3.14
来源：http://usu.hammf.cn

[R04] 位置参数
来源：http://jcg.andypj.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ffe.chenlongwang.top

[R05] 参数默认值
来源：http://dnm.shuidangran.top

name="${1:-default}"
来源：http://feg.yj202588.top

[R06] 判断命令是否存在
来源：http://ais.xinyue.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pgt.jqgufenzy.top

[R07] if 判断文件
来源：http://lqg.zhongyouzk.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://obg.wangshuangyany.cn

[R08] 数值比较
来源：http://pfg.mhx1999.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vdj.cqqwz.cn

[R09] 字符串比较
来源：http://vjx.hysaishi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://opk.yj20258888.top

[R10] 正则匹配
来源：http://woa.zhijiandao.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tjm.mhx1999.top

[R11] case 多分支
来源：http://ljv.gotoacloud.top

case "$1" in
来源：http://hlt.andypj.xyz

start) echo "启动" ;;
来源：http://ohp.zdqjudy.top

stop)  echo "停止" ;;
来源：http://qhf.yonumen.top

*)     echo "未知命令" ;;
来源：http://oyo.9152youxi.cn

esac
来源：http://yur.cqqwz.cn

[R12] for 遍历文件
来源：http://bmy.ydjk.org.cn

for f in *.txt; do echo "$f"; done
来源：http://fau.xinyue.icu

[R13] for 计数循环
来源：http://ohk.bjfxy.top

for i in {1..10}; do echo "$i"; done
来源：http://kpx.gaohongyu789.top

[R14] C 风格 for
来源：http://ruv.bbcook.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://goy.zhengqikj.top

[R15] while 逐行读文件
来源：http://tiw.jinqigufen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gga.jinqigfzy.top

[R16] until 等待条件
来源：http://uti.yangfankeji.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iiu.sysykeji.top

[R17] 数组定义与取值
来源：http://jcx.yangfankeji.com

arr=(a b c); echo "${arr[0]}"
来源：http://vtm.cqqwz.cn

[R18] 遍历数组
来源：http://xwk.ivvv.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tny.pengpengdd.cyou

[R19] 数组长度
来源：http://iig.yonumen.top

echo "${#arr[@]}"
来源：http://kva.jinqigufen.top

[R20] 关联数组（字典）
来源：http://gvz.yangfankeji.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bev.hammf.cn

[R21] 字符串长度
来源：http://heg.sysykeji.top

echo "${#s}"
来源：http://hgj.sysykeji.top

[R22] 截取子串
来源：http://qmj.shuidangran.top

echo "${s:0:5}"
来源：http://izt.gotoacloud.top

[R23] 字符串替换
来源：http://rbx.yj20258.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qiu.mhx1999.top

[R24] 大小写转换
来源：http://oek.cheryme.top

echo "${s^^}"; echo "${s,,}"
来源：http://weh.hfpthk.cn

[R25] 去后缀 / 去前缀
来源：http://dsa.fktsv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dwi.9152youxi.cn

[R26] 命令替换
来源：http://vbl.aizwys.cn

now=$(date +%F); echo "$now"
来源：http://vjf.yuanzhike.top

[R27] 算术展开
来源：http://ach.ybcxt.top

echo $((1 + 2 * 3))
来源：http://yqi.cheryme.top

[R28] 浮点运算
来源：http://odm.316326.xyz

echo "scale=2; 10/3" | bc
来源：http://bix.jianghu66.top

[R29] 定义函数
来源：http://pfv.aizwys.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fsv.fktsv.cn

[R30] 函数返回状态码
来源：http://kzr.yangfankeji.com

f() { return 0; }; f || echo "失败了"
来源：http://hed.jiagoushi.top

[R31] 局部变量
来源：http://dye.sufxvd.cn

f() { local x=1; echo "$x"; }
来源：http://pbu.yanxiufei.cn

[R32] 参数个数校验
来源：http://jkd.ydzc1.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rbo.jianghu66.top

[R33] 捕获错误并提示行号
来源：http://uia.9152youxi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lax.hywenlv.cn

[R34] 退出时清理
来源：http://jfh.sxryk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zyh.dianchejie.cn

[R35] 后台执行并等待
来源：http://hwp.zhixingplan.top

sleep 5 & pid=$!; wait "$pid"
来源：http://few.guowangkeji.top

[R36] 并发执行多个任务
来源：http://lbv.fktsv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vmr.jqgufenzy.top

[R37] 把输出赋给变量
来源：http://pfj.hammf.cn

files=$(ls -1)
来源：http://nso.pengpengdd.cyou

[R38] 管道串联
来源：http://rno.hfpthk.cn

cat a.txt | grep -i error | wc -l
来源：http://mwv.feifeiyinyue.top

[R39] 重定向标准输出与错误
来源：http://yue.yj202588.top

cmd > out.log 2>&1
来源：http://lwn.uphjek.com

[R40] 追加写日志
来源：http://quq.yangfankeji.com

echo "log" >> out.log
来源：http://wwc.jiagoushi.top

[R41] 丢弃输出
来源：http://tzx.chenlongwang.top

cmd >/dev/null 2>&1
来源：http://jzb.mhx1999.top

[R42] 输入重定向
来源：http://xpr.xylfe.cn

wc -l < a.txt
来源：http://vjo.cheryme.top

[R43] 按名字查找文件
来源：http://qiw.ydzc1.top

find . -name "*.log" -type f
来源：http://jla.sysykeji.top

[R44] 按修改时间查找
来源：http://ens.cqqwz.cn

find . -mtime -7 -type f
来源：http://zgv.uphjek.com

[R45] 批量删除
来源：http://vui.ybcxt.top

find . -name "*.tmp" -delete
来源：http://ryl.xinyue.icu

[R46] 递归替换文件内容
来源：http://tqy.sjlbkw.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rfe.yonumen.top

[R47] sed 单行替换
来源：http://dzs.sufxvd.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ffd.hesvh.cn

[R48] awk 取指定列
来源：http://dhn.316326.xyz

awk '{print $1, $3}' a.txt
来源：http://pls.sweek.top

[R49] awk 带条件
来源：http://mgn.zhoulong.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kgi.ppjwa.cn

[R50] awk 求和
来源：http://cks.jyoumei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ixn.hywenlv.cn

[R51] 排序去重取前几
来源：http://ova.ppjwa.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nys.yj20258.top

[R52] 统计行数
来源：http://qnw.jinghuilouyu.cn

wc -l a.txt
来源：http://ylx.xingfuxueyuan.xyz

[R53] 查看文件头与实时尾
来源：http://maf.dianchejie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wgh.yj20258888.top

[R54] 比较两个文件
来源：http://gmx.hcnkem.com

diff a.txt b.txt
来源：http://vnw.redwolf501.top

[R55] 压缩与解压
来源：http://yde.zdqjudy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hbp.fengsongda.top

[R56] 远程拷贝
来源：http://lat.cucudq.cn

scp file user@host:/path/
来源：http://gcf.epnwcf.com

[R57] 远程执行命令
来源：http://rcm.quarkkingdee.top

ssh user@host 'uptime'
来源：http://erx.zdbjq.cn

[R58] 下载文件
来源：http://ypv.zhijiandao.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nru.bbcook.cn

[R59] 发 POST JSON
来源：http://apl.jqgfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qre.jianghu66.top

[R60] 只看 HTTP 状态码
来源：http://sre.yuxming.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vbv.ywan-chungtsiang.top

[R61] 磁盘占用
来源：http://mec.havefunace.top

df -h;  du -sh *
来源：http://lyk.birdmap.top

[R62] 找最占空间的文件
来源：http://fyq.wangdashe.top

du -ah . | sort -rh | head -10
来源：http://uzf.shanyushiyangtech.top

[R63] 内存与进程
来源：http://dsn.vqdsnc.cn

free -h;  ps aux | grep nginx
来源：http://rmo.haohaochexian.top

[R64] 结束进程
来源：http://daq.xuetiantiany.cn

kill -9 $(pgrep -f app.py)
来源：http://mfa.bbcook.cn

[R65] 查看端口占用
来源：http://qsc.c1oappe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jer.ywan-chungtsiang.top

[R66] 定时任务
来源：http://hjr.sjlbkw.cn

crontab -e;  crontab -l
来源：http://mvh.9152youxi.cn

[R67] 生成随机十六进制串
来源：http://utm.yonumen.top

openssl rand -hex 16
来源：http://gvr.yangfankeji.com

[R68] 计算文件校验值
来源：http://joj.yj20258888.top

sha256sum a.txt;  md5sum a.txt
来源：http://cfx.gogol.net.cn

[R69] 生成随机密码
来源：http://owa.sxryk.cn

head -c 16 /dev/urandom | base64
来源：http://umh.andypj.xyz

[R70] 时间戳与互转
来源：http://ozv.yj20258.top

date +%s;  date -d @1700000000
来源：http://kem.yongpay.top

[R71] 日期格式化
来源：http://tlq.yangfankeji.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://ryk.pycfn.com

[R72] 等待端口就绪
来源：http://kvc.chenjidiqi.icu

until nc -z localhost 3306; do sleep 1; done
来源：http://kcl.xuetiantiany.cn

[R73] 分割大日志
来源：http://lgm.cashguo.top

split -l 1000 big.log part_
来源：http://cwt.jinqigufen.top

[R74] 批量重命名
来源：http://mdw.sxryk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tjq.wangshuangyany.cn

[R75] 导出环境变量
来源：http://wue.hesvh.cn

export PATH="$HOME/bin:$PATH"
来源：http://yjx.hnxiangtu.top

[R76] 使用临时文件
来源：http://txk.zycfv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dki.fktsv.cn

[R77] 读取用户输入
来源：http://ekh.fzhhl.top

read -rp "请输入: " ans
来源：http://zhm.hcnkem.com

[R78] 交互式菜单
来源：http://yac.yj202588.top

select opt in a b c; do echo "$opt"; break; done
来源：http://dbo.hesvh.cn

[R79] 解析命令行选项
来源：http://rpn.hysaishi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dqj.tarul.cn

[R80] 查看脚本执行耗时
来源：http://ibo.nanxuanxn.top

time ./run.sh
来源：http://vjd.tianlin.xyz

================================================================================
来源：http://czj.zycfv.cn

S. C / C++ 专题
来源：http://lob.fanxiaobao.xyz

================================================================================
来源：http://usk.tarul.cn

[S01] C：Hello World
来源：http://hgz.tarul.cn

#include <stdio.h>
来源：http://shl.bjfxy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jjz.sweek.top

[S02] C：变量与格式化输出
来源：http://tzd.gzhubu.top

int a = 10; printf("%d\n", a);
来源：http://xnl.sysykeji.top

[S03] C：读入整数
来源：http://qmm.shzxlz.cn

int x; scanf("%d", &x);
来源：http://sjh.shangyingyoupin.top

[S04] C：字符串复制
来源：http://alo.hesvh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pfw.aizwys.cn

[S05] C：字符串长度
来源：http://kmk.cheryme.top

strlen(s)
来源：http://npb.sjlbkw.cn

[S06] C：字符串比较
来源：http://con.pycfn.com

strcmp(a, b) == 0
来源：http://rhp.zdqjudy.top

[S07] C：数组遍历求和
来源：http://eon.cheryme.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kqc.yonumen.top

[S08] C：动态内存分配与释放
来源：http://etr.jqgufenzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fsy.chenlongwang.top

[S09] C：结构体定义与初始化
来源：http://tla.zhiwuduotai.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hze.52xcode.cn

[S10] C：指针与解引用
来源：http://kuv.xingfuxueyuan.xyz

int *p = &a;  *p = 5;
来源：http://las.xuanzx.com

[S11] C：逐行读文件
来源：http://kow.aibaodan.cn

FILE *f = fopen("a.txt", "r");
来源：http://kcs.ctjpmb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://khi.ppjwa.cn

fclose(f);
来源：http://tbp.0kj1m.cn

[S12] C：写文件
来源：http://nuf.ydjk.org.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://alu.vehdjk.com

[S13] C：宏定义
来源：http://dal.hywenlv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aoi.jlsjyb.cn

[S14] C：枚举
来源：http://ule.xingfuxueyuan.xyz

enum Color { RED, GREEN, BLUE };
来源：http://cpi.vehdjk.com

[S15] C：类型转换
来源：http://kim.birdmap.top

(double) a / b
来源：http://gfy.yj202588.top

[S16] C：位操作置位
来源：http://shu.jlsjyb.cn


<!-- 参考信息 -->