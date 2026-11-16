代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://cyz.andypj.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kyo.hesvh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ybx.yongpay.top

[Q15] 查询全部
来源：http://hnh.fanxiaobao.xyz

SELECT * FROM users;
来源：http://srk.gogol.net.cn

[Q16] 查询指定列
来源：http://ofm.jinghuilouyu.cn

SELECT id, name FROM users;
来源：http://tqb.yvedp.cn

[Q17] 条件查询
来源：http://ucp.tanke756.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yul.dashuyun.cn

[Q18] 模糊匹配
来源：http://tra.vqdsnc.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://svz.fktsv.cn

[Q19] 范围查询
来源：http://cjy.xuetiantiany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://flo.chenlongwang.top

[Q20] IN 列表
来源：http://gfh.yuxming.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dsf.wangdashe.top

[Q21] 空值判断
来源：http://uwi.cqqwz.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bhb.tarul.cn

[Q22] 排序
来源：http://yfc.haohaochexian.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gmb.zhoulong.xyz

[Q23] 分页
来源：http://yfo.shanyushiyangkeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jlg.sysykeji.top

[Q24] 去重
来源：http://uwl.hysaishi.cn

SELECT DISTINCT city FROM users;
来源：http://lme.fengsongda.top

[Q25] 只取前 N 条
来源：http://cft.sjlbkw.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bkj.jinqigfzy.top

[Q26] 计数
来源：http://xng.zhijiandao.cn

SELECT COUNT(*) FROM users;
来源：http://efl.jiagoushi.top

[Q27] 条件计数
来源：http://yiw.zycfv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ezv.zhongyouzk.top

[Q28] 求和与平均
来源：http://lce.hnxiangtu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dvt.redwolf501.top

[Q29] 最大最小值
来源：http://bpf.pycfn.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://obx.nanxinkj.top

[Q30] 分组统计
来源：http://wlo.gotoacloud.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fxi.shanyushiyangtech.top

[Q31] 分组后过滤
来源：http://doc.jinghuilouyu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wsd.ivvv.top

[Q32] 分组拼接字符串
来源：http://ueb.xinyue.icu

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dtr.guannengcc.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sxx.dashuyun.cn

[Q33] 多列分组
来源：http://ycf.ydjk.org.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://thd.jinqigufen.top

[Q34] 每组取第一条
来源：http://yhh.sxryk.cn

SELECT * FROM (
来源：http://zpc.tanke756.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pzy.fktsv.cn

) t WHERE rn = 1;
来源：http://xzk.quarkkingdee.top

[Q35] 内连接
来源：http://dat.yfazqb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wkv.sweek.top

[Q36] 左连接
来源：http://aza.hammf.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xxg.zhijiandao.cn

[Q37] 右连接
来源：http://zfc.tian-w.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jug.xingfuxueyuan.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://lst.zhoulong.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ivn.redwolf501.top

[Q39] 自连接（查上下级）
来源：http://rfl.zhengqikj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xnv.ivvv.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cfv.c1oappe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ldx.kuanghao11.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://unu.ybcxt.top

[Q41] 多表连接
来源：http://uao.cheryme.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bbk.meibo888.top

JOIN users u ON u.id = o.user_id
来源：http://hzh.hywenlv.cn

JOIN products p ON p.id = o.product_id;
来源：http://dtq.shanyushiyangkeji.top

[Q42] 连接条件附加过滤
来源：http://syv.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u
来源：http://bbx.bbcook.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fzm.mhx1999.top

[Q43] 标量子查询
来源：http://ohd.yuxming.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jyw.pengpengdd.cyou

[Q44] IN 子查询
来源：http://pxd.sjlbkw.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tgv.kuanghao11.cn

[Q45] EXISTS 判断存在
来源：http://hed.dianchejie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ptf.316326.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://nue.yj202588.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jqq.uphjek.com

[Q47] 与平均值比较
来源：http://bat.xuetiantiany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mzn.yongpay.top

[Q48] CTE 公用表表达式
来源：http://mon.aibaodan.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://opr.pengpengdd.cyou

SELECT * FROM t WHERE c > 5;
来源：http://vjx.zhiwuduotai.top

[Q49] 更新单行
来源：http://lvw.yj202588.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tqo.ybcxt.top

[Q50] 批量更新
来源：http://wzi.jinqigufen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bfq.ivvv.top

[Q51] 用子查询更新
来源：http://fhf.vqdsnc.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jpo.zhixingplan.top

[Q52] 删除指定行
来源：http://wmv.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://syh.hysaishi.cn

[Q53] 按条件删除
来源：http://vfg.hnqzz.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rnq.nanxuanxn.top

[Q54] 清空表
来源：http://def.xinyue.icu

TRUNCATE TABLE logs;
来源：http://wet.yangfankeji.com

[Q55] 排名（并列占位）
来源：http://yfp.shangyingyoupin.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hbm.jqgfzy.top

[Q56] 密集排名（并列不占位）
来源：http://bpt.hysaishi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://akw.nwbrower.top

[Q57] 行号
来源：http://ejd.jinqigufen.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://owc.ydzc1.top

[Q58] 累计求和
来源：http://bhs.yuanzhike.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://plx.gzhubu.top

[Q59] 分组内累计
来源：http://tde.snrcjt.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uso.vqdsnc.cn

[Q60] 取上一行 / 下一行
来源：http://wye.chenjidiqi.icu

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ctx.guannengcc.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dxh.yvedp.cn

[Q61] 移动平均
来源：http://klw.yuanzhike.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qxc.hywenlv.cn

[Q62] 分组占比
来源：http://ade.pycfn.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mvy.zhiwuduotai.top

[Q63] 开启事务
来源：http://qhu.shanyushiyangtech.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jkq.tian-w.cn

[Q64] 提交事务
来源：http://uvw.52xcode.cn

COMMIT;
来源：http://ogi.bjfxy.top

[Q65] 回滚事务
来源：http://kce.nanxuanxn.top

ROLLBACK;
来源：http://kto.kuanghao11.cn

[Q66] 行锁查询
来源：http://wrq.hywenlv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ewg.daxiang520.top

[Q67] 设置隔离级别
来源：http://jso.yvedp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hpo.chenjidiqi.icu

[Q68] 保存点
来源：http://iex.sxryk.cn

SAVEPOINT sp1;
来源：http://nlh.gogol.net.cn

ROLLBACK TO sp1;
来源：http://iae.shzxlz.cn

[Q69] 查看执行计划
来源：http://bks.jqgfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jwp.hywenlv.cn

[Q70] 更新统计信息
来源：http://hmz.svipenyu.cn

ANALYZE TABLE users;
来源：http://lod.iojbl.cn

[Q71] 查看建表语句
来源：http://czf.zhaomingkeji.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mcr.chenlongwang.top

[Q72] 查看索引
来源：http://drp.ctjpmb.com

SHOW INDEX FROM users;
来源：http://rpt.zhixingplan.top

[Q73] 查看表状态
来源：http://syf.daria6918.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kjp.yanxiufei.cn

[Q74] 强制使用索引
来源：http://vvx.quarkkingdee.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://emp.hesvh.cn

[Q75] 日期格式化
来源：http://lrg.c1oappe.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cgj.yvedp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mzz.dianchejie.cn

[Q76] 按天统计
来源：http://jjn.zycfv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rkw.yueranfly.top

[Q77] 时间加减
来源：http://ohq.hnqzz.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cuo.chenlongwang.top

[Q78] 当前时间
来源：http://mmx.yuxming.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://unp.svipenyu.cn

[Q79] 字符串拼接
来源：http://wgf.chenlongwang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yme.jinqigfzy.top

[Q80] 字符串截取
来源：http://sra.daria6918.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ilt.cqqwz.cn

[Q81] 字符串替换
来源：http://yei.mhx1999.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dqd.nanxuanxn.top

[Q82] 字符长度与字节长度
来源：http://nwg.zhengqikj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cyl.ydzc1.top

[Q83] 大小写转换
来源：http://nbv.epnwcf.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://isq.epnwcf.com

[Q84] 去除首尾空格
来源：http://tlf.aibaodan.cn

SELECT TRIM(name) FROM users;
来源：http://nzd.iojbl.cn

[Q85] 数值取整
来源：http://cda.jlsjyb.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dwl.yuxming.cn

[Q86] 读取 JSON 字段
来源：http://etq.smart0.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pmj.vehdjk.com

[Q87] JSON 字段做条件
来源：http://aou.zdqjudy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uvz.svipenyu.cn

[Q88] 行转列（条件聚合）
来源：http://zuy.chenzaomai.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lub.yfazqb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cav.epnwcf.com

[Q89] 判断表是否存在
来源：http://jox.cdnleiting.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bll.c1oappe.top

[Q90] 生成序号列
来源：http://gum.guowangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lhw.epnwcf.com

================================================================================
来源：http://roe.fzhhl.top

R. Bash 专题
来源：http://qsb.dianchejie.cn

================================================================================
来源：http://bje.andypj.xyz

[R01] shebang 与严格模式
来源：http://rvl.hesvh.cn

#!/usr/bin/env bash
来源：http://ett.iojbl.cn

set -euo pipefail
来源：http://bka.guowangkeji.top

[R02] 变量赋值与使用
来源：http://ako.zhiwuduotai.top

name="Tom"; echo "$name"
来源：http://kml.nanxinkj.top

[R03] 只读变量
来源：http://qjf.ehwqpu.com

readonly PI=3.14
来源：http://izf.gzhubu.top

[R04] 位置参数
来源：http://xzc.chenzaomai.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://org.yuanzhike.top

[R05] 参数默认值
来源：http://fvc.yueranfly.top

name="${1:-default}"
来源：http://rnu.xingfuxueyuan.xyz

[R06] 判断命令是否存在
来源：http://fzn.cheryme.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bdx.snrcjt.cn

[R07] if 判断文件
来源：http://qmq.xuanzx.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qfl.xuetiantiany.cn

[R08] 数值比较
来源：http://ohd.andypj.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://npf.jlsjyb.cn

[R09] 字符串比较
来源：http://tok.gaohongyu789.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://eql.gogol.net.cn

[R10] 正则匹配
来源：http://vpw.sysykeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hkt.ywan-chungtsiang.top

[R11] case 多分支
来源：http://wdp.chenjidiqi.icu

case "$1" in
来源：http://phm.xylfe.cn

start) echo "启动" ;;
来源：http://aca.gzhubu.top

stop)  echo "停止" ;;
来源：http://cwe.hongshengwenyu.top

*)     echo "未知命令" ;;
来源：http://oul.wangdashe.top

esac
来源：http://siq.sjlbkw.cn

[R12] for 遍历文件
来源：http://zmg.cashguo.top

for f in *.txt; do echo "$f"; done
来源：http://hxu.jqgfzy.top

[R13] for 计数循环
来源：http://gbw.sysykeji.top

for i in {1..10}; do echo "$i"; done
来源：http://oxy.zhoulong.xyz

[R14] C 风格 for
来源：http://mig.yuanzhike.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mxe.jinqigfzy.top

[R15] while 逐行读文件
来源：http://bhp.vqdsnc.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uya.fehbvm.com

[R16] until 等待条件
来源：http://gzq.gogol.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ypr.jiagoushi.top

[R17] 数组定义与取值
来源：http://ekv.daria6918.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lhj.zycfv.cn

[R18] 遍历数组
来源：http://jaf.jlsjyb.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://riv.wangdashe.top

[R19] 数组长度
来源：http://wiw.zhengqikj.top

echo "${#arr[@]}"
来源：http://uuh.ivvv.top

[R20] 关联数组（字典）
来源：http://xpg.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tjx.9152youxi.cn

[R21] 字符串长度
来源：http://bfn.ctjpmb.com

echo "${#s}"
来源：http://jpr.mhx1999.top

[R22] 截取子串
来源：http://lbc.dianchejie.cn

echo "${s:0:5}"
来源：http://dda.epnwcf.com

[R23] 字符串替换
来源：http://mux.jinqigfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bph.hcnkem.com

[R24] 大小写转换
来源：http://xty.nanxinkj.top

echo "${s^^}"; echo "${s,,}"
来源：http://ugr.zhiwuduotai.top

[R25] 去后缀 / 去前缀
来源：http://kyc.cqqwz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cae.ctjpmb.com

[R26] 命令替换
来源：http://fbe.gaohongyu789.top

now=$(date +%F); echo "$now"
来源：http://tpu.bbcook.cn

[R27] 算术展开
来源：http://wsv.yj202588.top

echo $((1 + 2 * 3))
来源：http://tkc.zhijiandao.cn

[R28] 浮点运算
来源：http://eqb.shanyushiyangkeji.top

echo "scale=2; 10/3" | bc
来源：http://bok.zhijiandao.cn

[R29] 定义函数
来源：http://zlf.feifeiyinyue.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gmx.jlsjyb.cn

[R30] 函数返回状态码
来源：http://vxj.jinghuilouyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://bqa.dashuyun.cn

[R31] 局部变量
来源：http://uta.tanke756.top

f() { local x=1; echo "$x"; }
来源：http://ful.sysykeji.top

[R32] 参数个数校验
来源：http://vtd.wangdashe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zhi.sjlbkw.cn

[R33] 捕获错误并提示行号
来源：http://xca.yvedp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://efz.haohaochexian.top

[R34] 退出时清理
来源：http://nlt.tian-w.cn

trap 'rm -f "$tmp"' EXIT
来源：http://brd.hfpthk.cn

[R35] 后台执行并等待
来源：http://grl.shanyushiyangtech.top

sleep 5 & pid=$!; wait "$pid"
来源：http://elm.mhx1999.top

[R36] 并发执行多个任务
来源：http://beq.mhx1999.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ogt.yfazqb.com

[R37] 把输出赋给变量
来源：http://hbo.epnwcf.com

files=$(ls -1)
来源：http://udf.jyoumei.cn

[R38] 管道串联
来源：http://fji.gotoacloud.top

cat a.txt | grep -i error | wc -l
来源：http://vyv.yanxiufei.cn

[R39] 重定向标准输出与错误
来源：http://wrz.iojbl.cn

cmd > out.log 2>&1
来源：http://qsp.jinqigfzy.top

[R40] 追加写日志
来源：http://sya.fktsv.cn

echo "log" >> out.log
来源：http://tgu.nanxuanxn.top

[R41] 丢弃输出
来源：http://mbo.fengsongda.top

cmd >/dev/null 2>&1
来源：http://odx.jinqigufen.top

[R42] 输入重定向
来源：http://fzo.bjfxy.top

wc -l < a.txt
来源：http://nlt.pengpengdd.cyou

[R43] 按名字查找文件
来源：http://ici.ctjpmb.com

find . -name "*.log" -type f
来源：http://cvf.316326.xyz

[R44] 按修改时间查找
来源：http://fkw.bjfxy.top

find . -mtime -7 -type f
来源：http://wjd.sxryk.cn

[R45] 批量删除
来源：http://wdt.wangdashe.top

find . -name "*.tmp" -delete
来源：http://jzm.hfpthk.cn

[R46] 递归替换文件内容
来源：http://shr.c1oappe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hgl.zhengqikj.top

[R47] sed 单行替换
来源：http://jax.aizwys.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mfv.andypj.xyz

[R48] awk 取指定列
来源：http://xon.0kj1m.cn

awk '{print $1, $3}' a.txt
来源：http://nis.hammf.cn

[R49] awk 带条件
来源：http://uig.daria6918.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ptd.ybcxt.top

[R50] awk 求和
来源：http://kxk.vehdjk.com

awk '{s += $2} END {print s}' a.txt
来源：http://bnj.fanxiaobao.xyz

[R51] 排序去重取前几
来源：http://cco.kuanghao11.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hcr.shanyushiyangkeji.top

[R52] 统计行数
来源：http://fcu.hnxiangtu.top

wc -l a.txt
来源：http://biu.nwbrower.top

[R53] 查看文件头与实时尾
来源：http://lgb.smart0.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xsk.chenzaomai.com

[R54] 比较两个文件
来源：http://tqn.fanxiaobao.xyz

diff a.txt b.txt
来源：http://pkh.fengsongda.top

[R55] 压缩与解压
来源：http://qtm.fktsv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uwz.hammf.cn

[R56] 远程拷贝
来源：http://vml.tian-w.cn

scp file user@host:/path/
来源：http://fwn.wangdashe.top

[R57] 远程执行命令
来源：http://fso.gaohongyu789.top

ssh user@host 'uptime'
来源：http://itd.hcnkem.com

[R58] 下载文件
来源：http://rml.dianchejie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yhf.zdqjudy.top

[R59] 发 POST JSON
来源：http://gzu.haohaochexian.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fqa.316326.xyz

[R60] 只看 HTTP 状态码
来源：http://sqt.yanxiufei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xsi.jinyuanbaomall.cn

[R61] 磁盘占用
来源：http://sld.meibo888.top

df -h;  du -sh *
来源：http://euf.aizwys.cn

[R62] 找最占空间的文件
来源：http://qve.zhaomingkeji.xyz

du -ah . | sort -rh | head -10
来源：http://frd.cucudq.cn

[R63] 内存与进程
来源：http://ows.sxryk.cn


<!-- 参考信息 -->