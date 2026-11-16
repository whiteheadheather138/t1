代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://vkn.yj20258.top

[Q07] 删除表
来源：http://mxi.quarkkingdee.top

DROP TABLE IF EXISTS orders;
来源：http://vev.jinghuilouyu.cn

[Q08] 创建普通索引
来源：http://zen.xingfuxueyuan.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://aks.tarul.cn

[Q09] 创建唯一索引
来源：http://gdk.xziqi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pdi.hongshengwenyu.top

[Q10] 插入单行
来源：http://pua.sufxvd.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gdk.ydjk.org.cn

[Q11] 一次插入多行
来源：http://abg.mhx1999.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lan.havefunace.top

[Q12] 插入后取自增 ID
来源：http://lmj.hammf.cn

INSERT INTO users (name) VALUES ('C');
来源：http://brl.fanxiaobao.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tro.zhiwuduotai.top

[Q13] 忽略重复插入
来源：http://zdo.hnxiangtu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://trf.hfpthk.cn

[Q14] 存在则更新（upsert）
来源：http://psy.ydjk.org.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xey.yfazqb.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oyz.316326.xyz

[Q15] 查询全部
来源：http://plg.sxryk.cn

SELECT * FROM users;
来源：http://fld.yvedp.cn

[Q16] 查询指定列
来源：http://fdr.chenzaomai.com

SELECT id, name FROM users;
来源：http://viu.jqgufenzy.top

[Q17] 条件查询
来源：http://znh.meibo888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lse.yuxming.cn

[Q18] 模糊匹配
来源：http://pru.gaohongyu789.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tii.feifeiyinyue.top

[Q19] 范围查询
来源：http://zwx.yangfankeji.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kip.tian-w.cn

[Q20] IN 列表
来源：http://owd.fktsv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://onv.dianchejie.cn

[Q21] 空值判断
来源：http://sjt.shuidangran.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mmv.sxryk.cn

[Q22] 排序
来源：http://qeg.chenzaomai.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bvj.jlsjyb.cn

[Q23] 分页
来源：http://uds.fktsv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rvi.9152youxi.cn

[Q24] 去重
来源：http://vik.zhijiandao.cn

SELECT DISTINCT city FROM users;
来源：http://bou.9152youxi.cn

[Q25] 只取前 N 条
来源：http://wlr.zhaomingkeji.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ike.andypj.xyz

[Q26] 计数
来源：http://hkc.feifeiyinyue.top

SELECT COUNT(*) FROM users;
来源：http://som.tanke756.top

[Q27] 条件计数
来源：http://znu.xylfe.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cpy.zhengqikj.top

[Q28] 求和与平均
来源：http://kji.hongshengwenyu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://psc.jinqigufen.top

[Q29] 最大最小值
来源：http://cmg.tianlin.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://kua.yueranfly.top

[Q30] 分组统计
来源：http://plj.xinyue.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gqo.hongshengwenyu.top

[Q31] 分组后过滤
来源：http://iwx.ivvv.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ijw.nwbrower.top

[Q32] 分组拼接字符串
来源：http://wje.ehwqpu.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fnp.snrcjt.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wvl.shangyingyoupin.top

[Q33] 多列分组
来源：http://fzb.tarul.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zln.tianlin.xyz

[Q34] 每组取第一条
来源：http://tvt.jqgfzy.top

SELECT * FROM (
来源：http://hqc.yj20258888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bgr.kuanghao11.cn

) t WHERE rn = 1;
来源：http://lmp.sysykeji.top

[Q35] 内连接
来源：http://ksn.yvedp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qfc.cdnleiting.top

[Q36] 左连接
来源：http://qfj.zhongyouzk.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tgu.hywenlv.cn

[Q37] 右连接
来源：http://acb.xziqi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://srf.xylfe.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rtz.yuxming.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://guh.quarkkingdee.top

[Q39] 自连接（查上下级）
来源：http://eyz.jinqigfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wfi.tanke756.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ggj.fktsv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://guj.gaohongyu789.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wpj.zhaomingkeji.xyz

[Q41] 多表连接
来源：http://qrm.jiagoushi.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://dxd.smart0.xyz

JOIN users u ON u.id = o.user_id
来源：http://uky.52xcode.cn

JOIN products p ON p.id = o.product_id;
来源：http://bsn.ppjwa.cn

[Q42] 连接条件附加过滤
来源：http://ple.yj20258.top

SELECT u.name, o.amount FROM users u
来源：http://cvk.ywan-chungtsiang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gjc.shzxlz.cn

[Q43] 标量子查询
来源：http://nhr.jlsjyb.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tcr.sufxvd.cn

[Q44] IN 子查询
来源：http://clt.birdmap.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ynw.zhiwuduotai.top

[Q45] EXISTS 判断存在
来源：http://nzu.chenjidiqi.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lte.tarul.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pcn.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ned.kuanghao11.cn

[Q47] 与平均值比较
来源：http://knp.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wjm.shanyushiyangtech.top

[Q48] CTE 公用表表达式
来源：http://lne.sjlbkw.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rtk.316326.xyz

SELECT * FROM t WHERE c > 5;
来源：http://hfa.guannengcc.top

[Q49] 更新单行
来源：http://llf.hongshengwenyu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nfi.jinqigufen.top

[Q50] 批量更新
来源：http://gnu.sjlbkw.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dcq.hywenlv.cn

[Q51] 用子查询更新
来源：http://fbx.9152youxi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wqe.nanxuanxn.top

[Q52] 删除指定行
来源：http://fvm.vehdjk.com

DELETE FROM users WHERE id = 10;
来源：http://zjh.cashguo.top

[Q53] 按条件删除
来源：http://zdv.feifeiyinyue.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kjk.xuetiantiany.cn

[Q54] 清空表
来源：http://xbf.yanxiufei.cn

TRUNCATE TABLE logs;
来源：http://cbg.hnxiangtu.top

[Q55] 排名（并列占位）
来源：http://yoi.xinyue.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://igl.haohaochexian.top

[Q56] 密集排名（并列不占位）
来源：http://mew.quarkkingdee.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://urm.mhx1999.top

[Q57] 行号
来源：http://yiw.daria6918.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zqh.yj20258.top

[Q58] 累计求和
来源：http://wti.yanxiufei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://beo.yangfankeji.com

[Q59] 分组内累计
来源：http://udn.fengsongda.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tkz.tian-w.cn

[Q60] 取上一行 / 下一行
来源：http://tgm.jqgfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tsy.ctjpmb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gpn.daxiang520.top

[Q61] 移动平均
来源：http://kvt.mhx1999.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xjy.snrcjt.cn

[Q62] 分组占比
来源：http://fcs.tanke756.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xah.sufxvd.cn

[Q63] 开启事务
来源：http://kjm.zhoulong.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://prf.svipenyu.cn

[Q64] 提交事务
来源：http://ico.9152youxi.cn

COMMIT;
来源：http://rcw.shzxlz.cn

[Q65] 回滚事务
来源：http://egg.cheryme.top

ROLLBACK;
来源：http://azc.bjfxy.top

[Q66] 行锁查询
来源：http://rcu.ywan-chungtsiang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zjn.c1oappe.top

[Q67] 设置隔离级别
来源：http://sqh.shanyushiyangtech.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uiq.havefunace.top

[Q68] 保存点
来源：http://nbd.meibo888.top

SAVEPOINT sp1;
来源：http://vjz.fanxiaobao.xyz

ROLLBACK TO sp1;
来源：http://vgd.ybcxt.top

[Q69] 查看执行计划
来源：http://iwk.jinyuanbaomall.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mok.yangfankeji.com

[Q70] 更新统计信息
来源：http://plu.gzhubu.top

ANALYZE TABLE users;
来源：http://djf.hfpthk.cn

[Q71] 查看建表语句
来源：http://pqr.bbcook.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://czg.yfazqb.com

[Q72] 查看索引
来源：http://nly.hcnkem.com

SHOW INDEX FROM users;
来源：http://mci.jianghu66.top

[Q73] 查看表状态
来源：http://jdf.sufxvd.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pnf.zdbjq.cn

[Q74] 强制使用索引
来源：http://ohm.chenjidiqi.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://inc.shuidangran.top

[Q75] 日期格式化
来源：http://pkr.tanke756.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xbu.yuxming.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zrq.316326.xyz

[Q76] 按天统计
来源：http://ill.xuetiantiany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qrw.52xcode.cn

[Q77] 时间加减
来源：http://znm.hcnkem.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yre.yonumen.top

[Q78] 当前时间
来源：http://phd.snrcjt.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bqt.yanxiufei.cn

[Q79] 字符串拼接
来源：http://wxg.fanxiaobao.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ecd.snrcjt.cn

[Q80] 字符串截取
来源：http://jeh.cashguo.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ywh.hcnkem.com

[Q81] 字符串替换
来源：http://msv.zhaomingkeji.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://aca.ehwqpu.com

[Q82] 字符长度与字节长度
来源：http://vnj.zhongyouzk.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yhu.jyoumei.cn

[Q83] 大小写转换
来源：http://ned.sjlbkw.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ylh.nanxuanxn.top

[Q84] 去除首尾空格
来源：http://bja.mhx1999.top

SELECT TRIM(name) FROM users;
来源：http://rlc.jqgufenzy.top

[Q85] 数值取整
来源：http://jsu.zhengqikj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fzr.nanxinkj.top

[Q86] 读取 JSON 字段
来源：http://ons.wangdashe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://irt.yj202588.top

[Q87] JSON 字段做条件
来源：http://gvf.chenlongwang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tfo.aibaodan.cn

[Q88] 行转列（条件聚合）
来源：http://lcd.quarkkingdee.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zpy.sufxvd.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pan.shzxlz.cn

[Q89] 判断表是否存在
来源：http://ito.cashguo.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ehd.zhiwuduotai.top

[Q90] 生成序号列
来源：http://gjs.316326.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wgt.shuidangran.top

================================================================================
来源：http://oac.aibaodan.cn

R. Bash 专题
来源：http://wlx.shanyushiyangkeji.top

================================================================================
来源：http://qkt.mhx1999.top

[R01] shebang 与严格模式
来源：http://uck.xinyue.icu

#!/usr/bin/env bash
来源：http://fkf.zhoulong.xyz

set -euo pipefail
来源：http://wft.gaohongyu789.top

[R02] 变量赋值与使用
来源：http://xga.yonumen.top

name="Tom"; echo "$name"
来源：http://asc.dashuyun.cn

[R03] 只读变量
来源：http://zcc.havefunace.top

readonly PI=3.14
来源：http://yyn.hongshengwenyu.top

[R04] 位置参数
来源：http://lcq.ywan-chungtsiang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fiy.yanxiufei.cn

[R05] 参数默认值
来源：http://fve.yj202588.top

name="${1:-default}"
来源：http://yfa.hywenlv.cn

[R06] 判断命令是否存在
来源：http://zwg.yanxiufei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xix.wangdashe.top

[R07] if 判断文件
来源：http://fso.zycfv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://epp.zycfv.cn

[R08] 数值比较
来源：http://hbm.pengpengdd.cyou

if (( a > b )); then echo "a 更大"; fi
来源：http://wvj.hnxiangtu.top

[R09] 字符串比较
来源：http://tai.xinyue.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cfd.jinyuanbaomall.cn

[R10] 正则匹配
来源：http://ucb.hysaishi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cwu.xingfuxueyuan.xyz

[R11] case 多分支
来源：http://upi.fengsongda.top

case "$1" in
来源：http://bcg.vehdjk.com

start) echo "启动" ;;
来源：http://rnu.cheryme.top

stop)  echo "停止" ;;
来源：http://gdc.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://xax.jinyuanbaomall.cn

esac
来源：http://iev.jianghu66.top

[R12] for 遍历文件
来源：http://lxy.ivvv.top

for f in *.txt; do echo "$f"; done
来源：http://rco.hammf.cn

[R13] for 计数循环
来源：http://dii.sysykeji.top

for i in {1..10}; do echo "$i"; done
来源：http://lbd.tarul.cn

[R14] C 风格 for
来源：http://rfi.hesvh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hfm.hcnkem.com

[R15] while 逐行读文件
来源：http://ncg.jqgufenzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sja.epnwcf.com

[R16] until 等待条件
来源：http://yju.shanyushiyangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bng.9152youxi.cn

[R17] 数组定义与取值
来源：http://axi.daxiang520.top

arr=(a b c); echo "${arr[0]}"
来源：http://xoe.ydzc1.top

[R18] 遍历数组
来源：http://axc.hcnkem.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://srt.yanxiufei.cn

[R19] 数组长度
来源：http://wdx.mhx1999.top

echo "${#arr[@]}"
来源：http://lqg.havefunace.top

[R20] 关联数组（字典）
来源：http://odm.pycfn.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://poj.daxiang520.top

[R21] 字符串长度
来源：http://ylh.gotoacloud.top

echo "${#s}"
来源：http://fuv.yuxming.cn

[R22] 截取子串
来源：http://zrh.svipenyu.cn

echo "${s:0:5}"
来源：http://fao.sufxvd.cn

[R23] 字符串替换
来源：http://oex.chenjidiqi.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jxv.aizwys.cn

[R24] 大小写转换
来源：http://dar.xuanzx.com

echo "${s^^}"; echo "${s,,}"
来源：http://tut.fzhhl.top

[R25] 去后缀 / 去前缀
来源：http://bwo.dianchejie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jef.hcnkem.com

[R26] 命令替换
来源：http://sry.hywenlv.cn

now=$(date +%F); echo "$now"
来源：http://nqj.nanxinkj.top

[R27] 算术展开
来源：http://stn.jqgufenzy.top

echo $((1 + 2 * 3))
来源：http://vov.ppjwa.cn

[R28] 浮点运算
来源：http://cch.shzxlz.cn

echo "scale=2; 10/3" | bc
来源：http://hao.hcnkem.com

[R29] 定义函数
来源：http://vsc.xuetiantiany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fek.ydjk.org.cn

[R30] 函数返回状态码
来源：http://utc.vqdsnc.cn

f() { return 0; }; f || echo "失败了"
来源：http://xxu.dianchejie.cn

[R31] 局部变量
来源：http://xrx.epnwcf.com

f() { local x=1; echo "$x"; }
来源：http://dpd.svipenyu.cn

[R32] 参数个数校验
来源：http://tnu.smart0.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mge.fanxiaobao.xyz

[R33] 捕获错误并提示行号
来源：http://xov.yonumen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vyz.aizwys.cn

[R34] 退出时清理
来源：http://sdg.pycfn.com

trap 'rm -f "$tmp"' EXIT
来源：http://vlb.nanxuanxn.top

[R35] 后台执行并等待
来源：http://zkl.nanxuanxn.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fij.jyoumei.cn

[R36] 并发执行多个任务
来源：http://lli.ybcxt.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eek.ppjwa.cn

[R37] 把输出赋给变量
来源：http://ojr.tanke756.top

files=$(ls -1)
来源：http://lzf.chenzaomai.com

[R38] 管道串联
来源：http://ihj.yj20258.top

cat a.txt | grep -i error | wc -l
来源：http://uwp.shuidangran.top

[R39] 重定向标准输出与错误
来源：http://igz.sysykeji.top

cmd > out.log 2>&1
来源：http://job.iojbl.cn

[R40] 追加写日志
来源：http://wdf.ydjk.org.cn

echo "log" >> out.log
来源：http://qzj.chenjidiqi.icu

[R41] 丢弃输出
来源：http://ycn.mhx1999.top

cmd >/dev/null 2>&1
来源：http://jrw.bbcook.cn

[R42] 输入重定向
来源：http://ceh.xinyue.icu

wc -l < a.txt
来源：http://geg.dianchejie.cn

[R43] 按名字查找文件
来源：http://jal.ybcxt.top

find . -name "*.log" -type f
来源：http://wwo.xuetiantiany.cn

[R44] 按修改时间查找
来源：http://cwg.ydjk.org.cn

find . -mtime -7 -type f
来源：http://gsx.fzhhl.top

[R45] 批量删除
来源：http://qpw.hongshengwenyu.top

find . -name "*.tmp" -delete
来源：http://bjl.iojbl.cn

[R46] 递归替换文件内容
来源：http://hly.nanxinkj.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gzo.shangyingyoupin.top

[R47] sed 单行替换
来源：http://eyq.yfazqb.com

sed -i 's/foo/bar/g' a.txt
来源：http://tqk.fehbvm.com

[R48] awk 取指定列
来源：http://eip.haohaochexian.top

awk '{print $1, $3}' a.txt
来源：http://dnv.smart0.xyz

[R49] awk 带条件
来源：http://oxz.daxiang520.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iqc.hnxiangtu.top

[R50] awk 求和
来源：http://tsz.yonumen.top

awk '{s += $2} END {print s}' a.txt
来源：http://ykw.iojbl.cn

[R51] 排序去重取前几
来源：http://uut.aibaodan.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rbh.fanxiaobao.xyz

[R52] 统计行数
来源：http://exc.hnqzz.top

wc -l a.txt
来源：http://lof.hnqzz.top

[R53] 查看文件头与实时尾
来源：http://fuf.aibaodan.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uve.birdmap.top

[R54] 比较两个文件
来源：http://pkm.chenjidiqi.icu

diff a.txt b.txt
来源：http://hzj.kuanghao11.cn

[R55] 压缩与解压
来源：http://wjd.shanyushiyangkeji.top


<!-- 参考信息 -->