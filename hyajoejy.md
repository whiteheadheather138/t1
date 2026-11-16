代发 wailian999

SELECT * FROM users;
来源：http://juj.meibo888.top

[Q16] 查询指定列
来源：http://dwh.316326.xyz

SELECT id, name FROM users;
来源：http://jma.cucudq.cn

[Q17] 条件查询
来源：http://ojk.hywenlv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lhi.feifeiyinyue.top

[Q18] 模糊匹配
来源：http://zyy.fzhhl.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://azl.fehbvm.com

[Q19] 范围查询
来源：http://bmc.yangfankeji.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eru.ehwqpu.com

[Q20] IN 列表
来源：http://scl.dashuyun.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gye.aibaodan.cn

[Q21] 空值判断
来源：http://adj.dashuyun.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jqb.nanxuanxn.top

[Q22] 排序
来源：http://ehx.andypj.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nvd.xinyue.icu

[Q23] 分页
来源：http://pct.cdnleiting.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rux.zdbjq.cn

[Q24] 去重
来源：http://wxq.andypj.xyz

SELECT DISTINCT city FROM users;
来源：http://zgy.cashguo.top

[Q25] 只取前 N 条
来源：http://nrk.vehdjk.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wze.epnwcf.com

[Q26] 计数
来源：http://kqz.cqqwz.cn

SELECT COUNT(*) FROM users;
来源：http://tbf.zdqjudy.top

[Q27] 条件计数
来源：http://eht.cdnleiting.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jny.aizwys.cn

[Q28] 求和与平均
来源：http://vfr.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tnb.jinqigfzy.top

[Q29] 最大最小值
来源：http://hpe.sxryk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://oay.hesvh.cn

[Q30] 分组统计
来源：http://nio.bjfxy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kti.sjlbkw.cn

[Q31] 分组后过滤
来源：http://atq.zdbjq.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fgw.hysaishi.cn

[Q32] 分组拼接字符串
来源：http://jql.fanxiaobao.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ufn.hesvh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xgc.nanxinkj.top

[Q33] 多列分组
来源：http://nsu.quarkkingdee.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wsi.jyoumei.cn

[Q34] 每组取第一条
来源：http://fmv.snrcjt.cn

SELECT * FROM (
来源：http://vxe.sysykeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wof.jinqigufen.top

) t WHERE rn = 1;
来源：http://oso.xziqi.cn

[Q35] 内连接
来源：http://ldp.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ucf.hammf.cn

[Q36] 左连接
来源：http://opp.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ggf.tanke756.top

[Q37] 右连接
来源：http://qhc.hnxiangtu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cxv.zhiwuduotai.top

[Q38] 全外连接（PostgreSQL）
来源：http://dqh.hesvh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cez.bjfxy.top

[Q39] 自连接（查上下级）
来源：http://jcj.sjlbkw.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://het.zdqjudy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ijh.zhixingplan.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wkt.uphjek.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://owp.quarkkingdee.top

[Q41] 多表连接
来源：http://lrj.hnxiangtu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://sam.guowangkeji.top

JOIN users u ON u.id = o.user_id
来源：http://pkz.yvedp.cn

JOIN products p ON p.id = o.product_id;
来源：http://qlx.aibaodan.cn

[Q42] 连接条件附加过滤
来源：http://uvt.zdbjq.cn

SELECT u.name, o.amount FROM users u
来源：http://kar.xingfuxueyuan.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://egt.sxryk.cn

[Q43] 标量子查询
来源：http://fpp.cashguo.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://esz.jinqigufen.top

[Q44] IN 子查询
来源：http://wrc.jqgufenzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qfa.tarul.cn

[Q45] EXISTS 判断存在
来源：http://qwa.hesvh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jbr.yonumen.top

[Q46] NOT EXISTS 判断不存在
来源：http://hfx.jinqigfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://prw.quarkkingdee.top

[Q47] 与平均值比较
来源：http://zng.jinghuilouyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ipq.yueranfly.top

[Q48] CTE 公用表表达式
来源：http://tmj.hfpthk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wsn.ehwqpu.com

SELECT * FROM t WHERE c > 5;
来源：http://cry.ydjk.org.cn

[Q49] 更新单行
来源：http://een.ctjpmb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://toi.yj20258.top

[Q50] 批量更新
来源：http://efp.xingfuxueyuan.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ipu.xuanzx.com

[Q51] 用子查询更新
来源：http://ogw.zhengqikj.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://skg.andypj.xyz

[Q52] 删除指定行
来源：http://sck.hnqzz.top

DELETE FROM users WHERE id = 10;
来源：http://qug.hcnkem.com

[Q53] 按条件删除
来源：http://usd.ehwqpu.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://doq.hesvh.cn

[Q54] 清空表
来源：http://tke.wangdashe.top

TRUNCATE TABLE logs;
来源：http://gkb.daria6918.cn

[Q55] 排名（并列占位）
来源：http://ojb.guowangkeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hna.yuxming.cn

[Q56] 密集排名（并列不占位）
来源：http://tze.shuidangran.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lso.sufxvd.cn

[Q57] 行号
来源：http://dbc.hywenlv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baw.jinqigufen.top

[Q58] 累计求和
来源：http://iyf.0kj1m.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oqc.cashguo.top

[Q59] 分组内累计
来源：http://vov.aibaodan.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rbd.yongpay.top

[Q60] 取上一行 / 下一行
来源：http://slg.aizwys.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jvu.fzhhl.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ffn.shanyushiyangkeji.top

[Q61] 移动平均
来源：http://kam.andypj.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yuo.316326.xyz

[Q62] 分组占比
来源：http://oud.nwbrower.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kgv.cashguo.top

[Q63] 开启事务
来源：http://esl.tarul.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ldy.xziqi.cn

[Q64] 提交事务
来源：http://nwc.cucudq.cn

COMMIT;
来源：http://xfx.yvedp.cn

[Q65] 回滚事务
来源：http://gzz.gzhubu.top

ROLLBACK;
来源：http://qwd.shangyingyoupin.top

[Q66] 行锁查询
来源：http://cog.xuanzx.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ind.yanxiufei.cn

[Q67] 设置隔离级别
来源：http://sjt.zhongyouzk.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rid.cucudq.cn

[Q68] 保存点
来源：http://ldf.tian-w.cn

SAVEPOINT sp1;
来源：http://ggu.uphjek.com

ROLLBACK TO sp1;
来源：http://lak.aibaodan.cn

[Q69] 查看执行计划
来源：http://pdf.zhoulong.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://juq.nanxinkj.top

[Q70] 更新统计信息
来源：http://cwq.nanxinkj.top

ANALYZE TABLE users;
来源：http://glc.ctjpmb.com

[Q71] 查看建表语句
来源：http://wbk.wangdashe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kme.xinyue.icu

[Q72] 查看索引
来源：http://kws.zdbjq.cn

SHOW INDEX FROM users;
来源：http://okg.hammf.cn

[Q73] 查看表状态
来源：http://bhg.ydzc1.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ukn.epnwcf.com

[Q74] 强制使用索引
来源：http://rjc.uphjek.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mkm.cqqwz.cn

[Q75] 日期格式化
来源：http://mfc.jinghuilouyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://alb.shzxlz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dlh.uphjek.com

[Q76] 按天统计
来源：http://rxp.nwbrower.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://osl.redwolf501.top

[Q77] 时间加减
来源：http://skv.sxryk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pls.bjfxy.top

[Q78] 当前时间
来源：http://wxv.sysykeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vhr.jiagoushi.top

[Q79] 字符串拼接
来源：http://tqq.xingfuxueyuan.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ikz.tarul.cn

[Q80] 字符串截取
来源：http://dqg.yanxiufei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dey.daxiang520.top

[Q81] 字符串替换
来源：http://weh.chenjidiqi.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mje.shuidangran.top

[Q82] 字符长度与字节长度
来源：http://jer.cdnleiting.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rmb.jqgufenzy.top

[Q83] 大小写转换
来源：http://ijf.haohaochexian.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dje.shanyushiyangtech.top

[Q84] 去除首尾空格
来源：http://gnv.tarul.cn

SELECT TRIM(name) FROM users;
来源：http://gvt.hnqzz.top

[Q85] 数值取整
来源：http://rmx.jlsjyb.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mca.yj20258.top

[Q86] 读取 JSON 字段
来源：http://wxk.zdbjq.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vro.zhongyouzk.top

[Q87] JSON 字段做条件
来源：http://igq.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pqt.redwolf501.top

[Q88] 行转列（条件聚合）
来源：http://ekg.vqdsnc.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://isi.xuanzx.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tsq.0kj1m.cn

[Q89] 判断表是否存在
来源：http://fay.cheryme.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rmg.hnqzz.top

[Q90] 生成序号列
来源：http://jon.bjfxy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pqe.hywenlv.cn

================================================================================
来源：http://xor.cqqwz.cn

R. Bash 专题
来源：http://ohi.xingfuxueyuan.xyz

================================================================================
来源：http://bav.bbcook.cn

[R01] shebang 与严格模式
来源：http://wsu.cheryme.top

#!/usr/bin/env bash
来源：http://yxi.svipenyu.cn

set -euo pipefail
来源：http://afm.birdmap.top

[R02] 变量赋值与使用
来源：http://ecw.jinqigufen.top

name="Tom"; echo "$name"
来源：http://upt.316326.xyz

[R03] 只读变量
来源：http://elw.tian-w.cn

readonly PI=3.14
来源：http://xpx.andypj.xyz

[R04] 位置参数
来源：http://ewc.nwbrower.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://emd.xziqi.cn

[R05] 参数默认值
来源：http://vrc.jinghuilouyu.cn

name="${1:-default}"
来源：http://uek.vqdsnc.cn

[R06] 判断命令是否存在
来源：http://esq.fanxiaobao.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yxt.ivvv.top

[R07] if 判断文件
来源：http://xuj.kuanghao11.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://unn.tianlin.xyz

[R08] 数值比较
来源：http://nrn.0kj1m.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://svs.wangshuangyany.cn

[R09] 字符串比较
来源：http://ddt.chenlongwang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://anu.zhijiandao.cn

[R10] 正则匹配
来源：http://upy.zhengqikj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uqi.zdqjudy.top

[R11] case 多分支
来源：http://uac.andypj.xyz

case "$1" in
来源：http://nxd.316326.xyz

start) echo "启动" ;;
来源：http://edg.sjlbkw.cn

stop)  echo "停止" ;;
来源：http://svh.hnqzz.top

*)     echo "未知命令" ;;
来源：http://hlw.bbcook.cn

esac
来源：http://kru.haohaochexian.top

[R12] for 遍历文件
来源：http://abd.gzhubu.top

for f in *.txt; do echo "$f"; done
来源：http://nqs.gzhubu.top

[R13] for 计数循环
来源：http://wjg.nanxuanxn.top

for i in {1..10}; do echo "$i"; done
来源：http://utg.ehwqpu.com

[R14] C 风格 for
来源：http://ywd.cheryme.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wie.cashguo.top

[R15] while 逐行读文件
来源：http://twt.chenzaomai.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dwn.zhengqikj.top

[R16] until 等待条件
来源：http://fyy.yueranfly.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cuz.haohaochexian.top

[R17] 数组定义与取值
来源：http://qfb.ywan-chungtsiang.top

arr=(a b c); echo "${arr[0]}"
来源：http://mdj.chenzaomai.com

[R18] 遍历数组
来源：http://nwp.yj20258888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pip.ywan-chungtsiang.top

[R19] 数组长度
来源：http://eex.jinqigufen.top

echo "${#arr[@]}"
来源：http://dte.shanyushiyangkeji.top

[R20] 关联数组（字典）
来源：http://nqs.gogol.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wyu.uphjek.com

[R21] 字符串长度
来源：http://ihs.hfpthk.cn

echo "${#s}"
来源：http://xyc.zhixingplan.top

[R22] 截取子串
来源：http://ckg.aibaodan.cn

echo "${s:0:5}"
来源：http://fms.ppjwa.cn

[R23] 字符串替换
来源：http://ily.sxryk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ynv.smart0.xyz

[R24] 大小写转换
来源：http://bkb.yj20258888.top

echo "${s^^}"; echo "${s,,}"
来源：http://mls.fktsv.cn

[R25] 去后缀 / 去前缀
来源：http://pux.ydjk.org.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ibk.tarul.cn

[R26] 命令替换
来源：http://cnn.yangfankeji.com

now=$(date +%F); echo "$now"
来源：http://srw.xuanzx.com

[R27] 算术展开
来源：http://spz.shuidangran.top

echo $((1 + 2 * 3))
来源：http://cfj.zhiwuduotai.top

[R28] 浮点运算
来源：http://xkz.yj20258888.top

echo "scale=2; 10/3" | bc
来源：http://oip.ctjpmb.com

[R29] 定义函数
来源：http://mgd.sysykeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xjc.gzhubu.top

[R30] 函数返回状态码
来源：http://rfh.fengsongda.top

f() { return 0; }; f || echo "失败了"
来源：http://jpq.bjfxy.top

[R31] 局部变量
来源：http://sfd.yuanzhike.top

f() { local x=1; echo "$x"; }
来源：http://kaj.jinqigufen.top

[R32] 参数个数校验
来源：http://asi.ppjwa.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://plk.shuidangran.top

[R33] 捕获错误并提示行号
来源：http://msf.hesvh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nwn.yueranfly.top

[R34] 退出时清理
来源：http://wwg.tianlin.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://vsa.iojbl.cn

[R35] 后台执行并等待
来源：http://cbz.jqgufenzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mqi.hfpthk.cn

[R36] 并发执行多个任务
来源：http://une.iojbl.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ish.wangshuangyany.cn

[R37] 把输出赋给变量
来源：http://uad.shangyingyoupin.top

files=$(ls -1)
来源：http://unk.jianghu66.top

[R38] 管道串联
来源：http://any.hysaishi.cn

cat a.txt | grep -i error | wc -l
来源：http://jjx.fengsongda.top

[R39] 重定向标准输出与错误
来源：http://ten.gaohongyu789.top

cmd > out.log 2>&1
来源：http://kfl.shzxlz.cn

[R40] 追加写日志
来源：http://emj.haohaochexian.top

echo "log" >> out.log
来源：http://esv.sjlbkw.cn

[R41] 丢弃输出
来源：http://bhq.redwolf501.top

cmd >/dev/null 2>&1
来源：http://yfd.zhiwuduotai.top

[R42] 输入重定向
来源：http://enw.xingfuxueyuan.xyz

wc -l < a.txt
来源：http://ava.chenlongwang.top

[R43] 按名字查找文件
来源：http://efr.vehdjk.com

find . -name "*.log" -type f
来源：http://bep.zhengqikj.top

[R44] 按修改时间查找
来源：http://lwm.shuidangran.top

find . -mtime -7 -type f
来源：http://ggr.pycfn.com

[R45] 批量删除
来源：http://rnv.yj20258.top

find . -name "*.tmp" -delete
来源：http://gbi.aibaodan.cn

[R46] 递归替换文件内容
来源：http://fzg.epnwcf.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bkh.chenlongwang.top

[R47] sed 单行替换
来源：http://vxg.chenjidiqi.icu

sed -i 's/foo/bar/g' a.txt
来源：http://orm.c1oappe.top

[R48] awk 取指定列
来源：http://lfo.hywenlv.cn

awk '{print $1, $3}' a.txt
来源：http://wsm.sxryk.cn

[R49] awk 带条件
来源：http://lnx.yangfankeji.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fql.hesvh.cn

[R50] awk 求和
来源：http://awe.redwolf501.top

awk '{s += $2} END {print s}' a.txt
来源：http://axm.daxiang520.top

[R51] 排序去重取前几
来源：http://mdm.xinyue.icu

sort a.txt | uniq -c | sort -rn | head
来源：http://wfx.sjlbkw.cn

[R52] 统计行数
来源：http://puw.hesvh.cn

wc -l a.txt
来源：http://lpt.ivvv.top

[R53] 查看文件头与实时尾
来源：http://mxc.xylfe.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kwn.tarul.cn

[R54] 比较两个文件
来源：http://zrd.daxiang520.top

diff a.txt b.txt
来源：http://kex.guowangkeji.top

[R55] 压缩与解压
来源：http://nle.mhx1999.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dco.sufxvd.cn

[R56] 远程拷贝
来源：http://hoj.meibo888.top

scp file user@host:/path/
来源：http://aoo.quarkkingdee.top

[R57] 远程执行命令
来源：http://zbq.52xcode.cn

ssh user@host 'uptime'
来源：http://qua.sufxvd.cn

[R58] 下载文件
来源：http://ore.chenzaomai.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nhj.fehbvm.com

[R59] 发 POST JSON
来源：http://rqo.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ocx.shangyingyoupin.top

[R60] 只看 HTTP 状态码
来源：http://zzy.guannengcc.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ztq.ydjk.org.cn

[R61] 磁盘占用
来源：http://lim.shanyushiyangtech.top

df -h;  du -sh *
来源：http://nnl.yvedp.cn

[R62] 找最占空间的文件
来源：http://mzk.meibo888.top

du -ah . | sort -rh | head -10
来源：http://aiu.ppjwa.cn

[R63] 内存与进程
来源：http://oye.zhixingplan.top

free -h;  ps aux | grep nginx
来源：http://fyy.yfazqb.com

[R64] 结束进程
来源：http://rdl.aibaodan.cn

kill -9 $(pgrep -f app.py)
来源：http://tha.cdnleiting.top

[R65] 查看端口占用
来源：http://ptj.tanke756.top


<!-- 参考信息 -->