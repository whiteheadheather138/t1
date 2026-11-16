代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kmi.hammf.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://avw.ivvv.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kxt.shanyushiyangtech.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://piq.chenlongwang.top

================================================================================
来源：http://pkn.hesvh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vck.zhoulong.xyz

================================================================================
来源：http://ekm.pycfn.com

[Q01] 创建表
来源：http://ada.nanxuanxn.top

CREATE TABLE users (
来源：http://ytr.guannengcc.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nkr.hcnkem.com

name VARCHAR(50) NOT NULL,
来源：http://xxj.pycfn.com

email VARCHAR(100) UNIQUE,
来源：http://aee.gogol.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rfl.iojbl.cn

);
来源：http://pry.yj20258888.top

[Q02] 创建带外键的表
来源：http://rlo.nwbrower.top

CREATE TABLE orders (
来源：http://ebm.aizwys.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wel.cashguo.top

user_id INT NOT NULL,
来源：http://aot.gogol.net.cn

amount DECIMAL(10, 2),
来源：http://wvs.yj20258888.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qqd.hammf.cn

);
来源：http://ycj.haohaochexian.top

[Q03] 增加列
来源：http://pcw.zhongyouzk.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://doq.chenjidiqi.icu

[Q04] 修改列类型
来源：http://twn.meibo888.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kfl.ehwqpu.com

[Q05] 重命名列
来源：http://zkv.hcnkem.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fxq.zhijiandao.cn

[Q06] 删除列
来源：http://eaj.yongpay.top

ALTER TABLE users DROP COLUMN age;
来源：http://vtt.zdbjq.cn

[Q07] 删除表
来源：http://ylz.zhengqikj.top

DROP TABLE IF EXISTS orders;
来源：http://dlo.hfpthk.cn

[Q08] 创建普通索引
来源：http://yos.ydzc1.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hej.guannengcc.top

[Q09] 创建唯一索引
来源：http://fab.kuanghao11.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://elq.sysykeji.top

[Q10] 插入单行
来源：http://qap.yvedp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mgs.0kj1m.cn

[Q11] 一次插入多行
来源：http://zzf.zdqjudy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://izo.pycfn.com

[Q12] 插入后取自增 ID
来源：http://tuc.9152youxi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://had.smart0.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zcd.daxiang520.top

[Q13] 忽略重复插入
来源：http://sch.gzhubu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yud.xuanzx.com

[Q14] 存在则更新（upsert）
来源：http://zpn.c1oappe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jnq.yvedp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cos.fzhhl.top

[Q15] 查询全部
来源：http://hcd.chenzaomai.com

SELECT * FROM users;
来源：http://xzc.nanxinkj.top

[Q16] 查询指定列
来源：http://gpl.fzhhl.top

SELECT id, name FROM users;
来源：http://hey.mhx1999.top

[Q17] 条件查询
来源：http://wzd.yueranfly.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gqe.guannengcc.top

[Q18] 模糊匹配
来源：http://iwb.jqgfzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hqy.shuidangran.top

[Q19] 范围查询
来源：http://mhf.xylfe.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kwr.hammf.cn

[Q20] IN 列表
来源：http://quz.sufxvd.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eya.cucudq.cn

[Q21] 空值判断
来源：http://dgv.0kj1m.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dme.pengpengdd.cyou

[Q22] 排序
来源：http://wra.smart0.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eyj.mhx1999.top

[Q23] 分页
来源：http://omn.smart0.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fdi.nanxinkj.top

[Q24] 去重
来源：http://bts.jinghuilouyu.cn

SELECT DISTINCT city FROM users;
来源：http://dod.ehwqpu.com

[Q25] 只取前 N 条
来源：http://tck.zdbjq.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qbu.fanxiaobao.xyz

[Q26] 计数
来源：http://byb.fktsv.cn

SELECT COUNT(*) FROM users;
来源：http://lsq.hfpthk.cn

[Q27] 条件计数
来源：http://edr.bjfxy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wtz.jqgfzy.top

[Q28] 求和与平均
来源：http://cnt.hongshengwenyu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://klz.yangfankeji.com

[Q29] 最大最小值
来源：http://unr.ydzc1.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vuo.cucudq.cn

[Q30] 分组统计
来源：http://iqv.jqgfzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lwa.jinqigfzy.top

[Q31] 分组后过滤
来源：http://ish.smart0.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bnd.0kj1m.cn

[Q32] 分组拼接字符串
来源：http://toz.redwolf501.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tgl.xingfuxueyuan.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ljb.sufxvd.cn

[Q33] 多列分组
来源：http://vks.yonumen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ren.aizwys.cn

[Q34] 每组取第一条
来源：http://ifx.tian-w.cn

SELECT * FROM (
来源：http://uiu.cashguo.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qza.zhoulong.xyz

) t WHERE rn = 1;
来源：http://zah.yj20258.top

[Q35] 内连接
来源：http://hvb.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gac.fehbvm.com

[Q36] 左连接
来源：http://cus.yj20258.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://opq.dashuyun.cn

[Q37] 右连接
来源：http://bvx.jinqigfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nvq.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nbw.feifeiyinyue.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bzu.dianchejie.cn

[Q39] 自连接（查上下级）
来源：http://vwl.guowangkeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://owy.hnqzz.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://can.ivvv.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ohy.dashuyun.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uaa.birdmap.top

[Q41] 多表连接
来源：http://psw.jianghu66.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://xoz.zhiwuduotai.top

JOIN users u ON u.id = o.user_id
来源：http://rbl.zycfv.cn

JOIN products p ON p.id = o.product_id;
来源：http://oit.svipenyu.cn

[Q42] 连接条件附加过滤
来源：http://xef.chenlongwang.top

SELECT u.name, o.amount FROM users u
来源：http://wpq.nanxinkj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dek.fktsv.cn

[Q43] 标量子查询
来源：http://czc.nanxinkj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pwo.xinyue.icu

[Q44] IN 子查询
来源：http://zuk.hnxiangtu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hei.yanxiufei.cn

[Q45] EXISTS 判断存在
来源：http://ztl.zhaomingkeji.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iny.yj20258.top

[Q46] NOT EXISTS 判断不存在
来源：http://wii.vqdsnc.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://clt.hammf.cn

[Q47] 与平均值比较
来源：http://ekd.aizwys.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bae.sysykeji.top

[Q48] CTE 公用表表达式
来源：http://kts.nwbrower.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ucl.zhijiandao.cn

SELECT * FROM t WHERE c > 5;
来源：http://vvj.fengsongda.top

[Q49] 更新单行
来源：http://dch.dianchejie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://okz.cucudq.cn

[Q50] 批量更新
来源：http://qwu.hywenlv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://llv.shangyingyoupin.top

[Q51] 用子查询更新
来源：http://jho.yj20258.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lth.zhengqikj.top

[Q52] 删除指定行
来源：http://ggh.sweek.top

DELETE FROM users WHERE id = 10;
来源：http://djv.nanxinkj.top

[Q53] 按条件删除
来源：http://dck.yj20258.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qmp.sjlbkw.cn

[Q54] 清空表
来源：http://lkv.gzhubu.top

TRUNCATE TABLE logs;
来源：http://mbd.sysykeji.top

[Q55] 排名（并列占位）
来源：http://ort.dashuyun.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kxu.jyoumei.cn

[Q56] 密集排名（并列不占位）
来源：http://pkr.wangshuangyany.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rjj.yuanzhike.top

[Q57] 行号
来源：http://zgf.smart0.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ewm.shzxlz.cn

[Q58] 累计求和
来源：http://bee.ctjpmb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xqx.iojbl.cn

[Q59] 分组内累计
来源：http://gdj.snrcjt.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xxr.zhengqikj.top

[Q60] 取上一行 / 下一行
来源：http://cxf.zhaomingkeji.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gph.xuetiantiany.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://brm.shangyingyoupin.top

[Q61] 移动平均
来源：http://uqz.ydzc1.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aoo.cdnleiting.top

[Q62] 分组占比
来源：http://qmw.vqdsnc.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vka.svipenyu.cn

[Q63] 开启事务
来源：http://ich.aizwys.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oqf.snrcjt.cn

[Q64] 提交事务
来源：http://pbi.tanke756.top

COMMIT;
来源：http://bpp.cucudq.cn

[Q65] 回滚事务
来源：http://zck.ctjpmb.com

ROLLBACK;
来源：http://wxg.xylfe.cn

[Q66] 行锁查询
来源：http://zva.hywenlv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yug.bjfxy.top

[Q67] 设置隔离级别
来源：http://ncz.jqgfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nta.yanxiufei.cn

[Q68] 保存点
来源：http://vnd.0kj1m.cn

SAVEPOINT sp1;
来源：http://tjn.sweek.top

ROLLBACK TO sp1;
来源：http://cit.yfazqb.com

[Q69] 查看执行计划
来源：http://jxq.cdnleiting.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://okn.tianlin.xyz

[Q70] 更新统计信息
来源：http://vio.sufxvd.cn

ANALYZE TABLE users;
来源：http://erl.xziqi.cn

[Q71] 查看建表语句
来源：http://lic.ctjpmb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eth.zhixingplan.top

[Q72] 查看索引
来源：http://hgp.chenlongwang.top

SHOW INDEX FROM users;
来源：http://tnm.guannengcc.top

[Q73] 查看表状态
来源：http://qqa.yj20258888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://owv.wangdashe.top

[Q74] 强制使用索引
来源：http://fze.tarul.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cof.nanxinkj.top

[Q75] 日期格式化
来源：http://umx.yonumen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qda.quarkkingdee.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vkc.yangfankeji.com

[Q76] 按天统计
来源：http://yfw.zhongyouzk.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dtt.chenzaomai.com

[Q77] 时间加减
来源：http://cmv.yuanzhike.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xpb.iojbl.cn

[Q78] 当前时间
来源：http://bzq.meibo888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bpc.andypj.xyz

[Q79] 字符串拼接
来源：http://ynv.xingfuxueyuan.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pgb.gzhubu.top

[Q80] 字符串截取
来源：http://xlv.yueranfly.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fnr.zdbjq.cn

[Q81] 字符串替换
来源：http://lyz.xylfe.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tjj.jinghuilouyu.cn

[Q82] 字符长度与字节长度
来源：http://wxf.cashguo.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sqc.tian-w.cn

[Q83] 大小写转换
来源：http://mtb.yangfankeji.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://djg.xylfe.cn

[Q84] 去除首尾空格
来源：http://emu.hesvh.cn

SELECT TRIM(name) FROM users;
来源：http://xzk.shanyushiyangtech.top

[Q85] 数值取整
来源：http://soy.ppjwa.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vdm.fzhhl.top

[Q86] 读取 JSON 字段
来源：http://ydf.yfazqb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://stj.hcnkem.com

[Q87] JSON 字段做条件
来源：http://tpn.meibo888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gqv.daria6918.cn

[Q88] 行转列（条件聚合）
来源：http://wsm.guowangkeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ukz.chenjidiqi.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ezp.hnxiangtu.top

[Q89] 判断表是否存在
来源：http://iao.52xcode.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ptf.gotoacloud.top

[Q90] 生成序号列
来源：http://red.xinyue.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hld.zhongyouzk.top

================================================================================
来源：http://ppy.yvedp.cn

R. Bash 专题
来源：http://hcq.sweek.top

================================================================================
来源：http://zbz.haohaochexian.top

[R01] shebang 与严格模式
来源：http://erl.aibaodan.cn

#!/usr/bin/env bash
来源：http://kwc.jinyuanbaomall.cn

set -euo pipefail
来源：http://sew.xinyue.icu

[R02] 变量赋值与使用
来源：http://feb.ydjk.org.cn

name="Tom"; echo "$name"
来源：http://gfv.bbcook.cn

[R03] 只读变量
来源：http://rcs.tian-w.cn

readonly PI=3.14
来源：http://kec.epnwcf.com

[R04] 位置参数
来源：http://qom.ehwqpu.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ffn.bjfxy.top

[R05] 参数默认值
来源：http://mzy.dashuyun.cn

name="${1:-default}"
来源：http://jll.hnxiangtu.top

[R06] 判断命令是否存在
来源：http://enc.aibaodan.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://toa.gaohongyu789.top

[R07] if 判断文件
来源：http://ztx.zycfv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vcp.zhixingplan.top

[R08] 数值比较
来源：http://sco.chenjidiqi.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://tct.chenjidiqi.icu

[R09] 字符串比较
来源：http://pka.dianchejie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ess.gaohongyu789.top

[R10] 正则匹配
来源：http://bvf.zhoulong.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lhl.shanyushiyangkeji.top

[R11] case 多分支
来源：http://puj.snrcjt.cn

case "$1" in
来源：http://ttf.jianghu66.top

start) echo "启动" ;;
来源：http://sky.zhixingplan.top

stop)  echo "停止" ;;
来源：http://kwl.xylfe.cn

*)     echo "未知命令" ;;
来源：http://hbj.chenlongwang.top

esac
来源：http://awx.daria6918.cn

[R12] for 遍历文件
来源：http://tzq.iojbl.cn

for f in *.txt; do echo "$f"; done
来源：http://bqs.yangfankeji.com

[R13] for 计数循环
来源：http://ynq.zdbjq.cn

for i in {1..10}; do echo "$i"; done
来源：http://xrm.dashuyun.cn

[R14] C 风格 for
来源：http://yig.gotoacloud.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tss.shanyushiyangtech.top

[R15] while 逐行读文件
来源：http://xbj.jinghuilouyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ory.wangshuangyany.cn

[R16] until 等待条件
来源：http://dgt.hongshengwenyu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pgw.yuanzhike.top

[R17] 数组定义与取值
来源：http://urk.zycfv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://drg.ywan-chungtsiang.top

[R18] 遍历数组
来源：http://ddw.hysaishi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://muw.cqqwz.cn

[R19] 数组长度
来源：http://nyu.daxiang520.top

echo "${#arr[@]}"
来源：http://jdr.xuetiantiany.cn

[R20] 关联数组（字典）
来源：http://bzj.gaohongyu789.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hnh.xylfe.cn

[R21] 字符串长度
来源：http://jxn.zhoulong.xyz

echo "${#s}"
来源：http://vbr.sxryk.cn

[R22] 截取子串
来源：http://slq.shanyushiyangkeji.top

echo "${s:0:5}"
来源：http://xcm.feifeiyinyue.top

[R23] 字符串替换
来源：http://zgg.sysykeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://duo.ivvv.top

[R24] 大小写转换
来源：http://bsz.hammf.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gia.shangyingyoupin.top

[R25] 去后缀 / 去前缀
来源：http://bux.kuanghao11.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gxd.zhengqikj.top

[R26] 命令替换
来源：http://vsb.zhoulong.xyz

now=$(date +%F); echo "$now"
来源：http://lcr.aibaodan.cn

[R27] 算术展开
来源：http://voc.cucudq.cn

echo $((1 + 2 * 3))
来源：http://epg.bbcook.cn

[R28] 浮点运算
来源：http://lug.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://mpj.sufxvd.cn

[R29] 定义函数
来源：http://zrv.ydjk.org.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vqd.shanyushiyangtech.top

[R30] 函数返回状态码
来源：http://mns.yonumen.top

f() { return 0; }; f || echo "失败了"
来源：http://bvd.xuetiantiany.cn

[R31] 局部变量
来源：http://gwj.fehbvm.com

f() { local x=1; echo "$x"; }
来源：http://fpt.zhijiandao.cn

[R32] 参数个数校验
来源：http://qes.yuanzhike.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cpb.9152youxi.cn

[R33] 捕获错误并提示行号
来源：http://yem.zhoulong.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eyg.yueranfly.top

[R34] 退出时清理
来源：http://lzf.zdqjudy.top

trap 'rm -f "$tmp"' EXIT
来源：http://zwg.zhijiandao.cn

[R35] 后台执行并等待
来源：http://kmg.zhoulong.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://jav.jianghu66.top

[R36] 并发执行多个任务
来源：http://fcq.hnqzz.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nvb.feifeiyinyue.top

[R37] 把输出赋给变量
来源：http://mee.xingfuxueyuan.xyz

files=$(ls -1)
来源：http://nfj.yj20258888.top

[R38] 管道串联
来源：http://wmc.hesvh.cn

cat a.txt | grep -i error | wc -l
来源：http://lsi.meibo888.top

[R39] 重定向标准输出与错误
来源：http://ood.yueranfly.top

cmd > out.log 2>&1
来源：http://pbk.sufxvd.cn

[R40] 追加写日志
来源：http://npv.yangfankeji.com

echo "log" >> out.log
来源：http://job.yangfankeji.com

[R41] 丢弃输出
来源：http://jut.hnqzz.top


<!-- 参考信息 -->