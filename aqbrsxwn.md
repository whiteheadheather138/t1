代发 wailian999

PHP:  // 手写时间戳比较
来源：http://yjm.wangdashe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yss.epnwcf.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gtg.hnqzz.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sqq.ydzc1.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ocl.xingfuxueyuan.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://uom.aizwys.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qqr.yonumen.top

[P08] 处理浮点精度问题
来源：http://wud.haohaochexian.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://scs.smart0.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fub.yuanzhike.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vmx.ydzc1.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vll.uphjek.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dlq.xuetiantiany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://khc.yj20258.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qzw.yvedp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fei.hcnkem.com

================================================================================
来源：http://ijl.aizwys.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://psq.haohaochexian.top

================================================================================
来源：http://kai.c1oappe.top

[Q01] 创建表
来源：http://sly.xinyue.icu

CREATE TABLE users (
来源：http://opx.sweek.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dyw.ivvv.top

name VARCHAR(50) NOT NULL,
来源：http://fvu.52xcode.cn

email VARCHAR(100) UNIQUE,
来源：http://hzm.guannengcc.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yjy.epnwcf.com

);
来源：http://vjl.ivvv.top

[Q02] 创建带外键的表
来源：http://hxw.chenjidiqi.icu

CREATE TABLE orders (
来源：http://tfs.dianchejie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zsx.uphjek.com

user_id INT NOT NULL,
来源：http://hnh.zycfv.cn

amount DECIMAL(10, 2),
来源：http://yeq.shanyushiyangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://czd.cheryme.top

);
来源：http://dby.yvedp.cn

[Q03] 增加列
来源：http://jys.xingfuxueyuan.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ily.yuxming.cn

[Q04] 修改列类型
来源：http://lrx.chenzaomai.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ttt.uphjek.com

[Q05] 重命名列
来源：http://fmr.xuetiantiany.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kqg.wangshuangyany.cn

[Q06] 删除列
来源：http://qdm.nanxinkj.top

ALTER TABLE users DROP COLUMN age;
来源：http://fzy.vehdjk.com

[Q07] 删除表
来源：http://bpc.zhaomingkeji.xyz

DROP TABLE IF EXISTS orders;
来源：http://bvm.cucudq.cn

[Q08] 创建普通索引
来源：http://gtu.andypj.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://bmu.jiagoushi.top

[Q09] 创建唯一索引
来源：http://nok.zhiwuduotai.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xqo.xingfuxueyuan.xyz

[Q10] 插入单行
来源：http://guc.yuxming.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://klb.shzxlz.cn

[Q11] 一次插入多行
来源：http://uuz.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dit.cucudq.cn

[Q12] 插入后取自增 ID
来源：http://ppw.hammf.cn

INSERT INTO users (name) VALUES ('C');
来源：http://klc.yongpay.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eya.zhengqikj.top

[Q13] 忽略重复插入
来源：http://qto.zhongyouzk.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hie.sjlbkw.cn

[Q14] 存在则更新（upsert）
来源：http://vyz.yj20258888.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ugu.zhiwuduotai.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wfv.guannengcc.top

[Q15] 查询全部
来源：http://pdz.zdbjq.cn

SELECT * FROM users;
来源：http://yrk.iojbl.cn

[Q16] 查询指定列
来源：http://mah.sysykeji.top

SELECT id, name FROM users;
来源：http://yko.fengsongda.top

[Q17] 条件查询
来源：http://rfb.tanke756.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tkg.havefunace.top

[Q18] 模糊匹配
来源：http://uez.hysaishi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ccm.birdmap.top

[Q19] 范围查询
来源：http://gtm.feifeiyinyue.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rvi.c1oappe.top

[Q20] IN 列表
来源：http://snb.chenlongwang.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kmk.jqgufenzy.top

[Q21] 空值判断
来源：http://uff.birdmap.top

SELECT * FROM users WHERE email IS NULL;
来源：http://cxp.epnwcf.com

[Q22] 排序
来源：http://emy.xylfe.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ekk.yuxming.cn

[Q23] 分页
来源：http://spq.jlsjyb.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://toq.jlsjyb.cn

[Q24] 去重
来源：http://pwd.epnwcf.com

SELECT DISTINCT city FROM users;
来源：http://ygu.shanyushiyangkeji.top

[Q25] 只取前 N 条
来源：http://syl.jqgufenzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ewk.jinghuilouyu.cn

[Q26] 计数
来源：http://kfg.zhixingplan.top

SELECT COUNT(*) FROM users;
来源：http://nbl.jlsjyb.cn

[Q27] 条件计数
来源：http://qzd.jyoumei.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://svq.bjfxy.top

[Q28] 求和与平均
来源：http://kcm.xingfuxueyuan.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ezd.mhx1999.top

[Q29] 最大最小值
来源：http://axu.nanxuanxn.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ujv.xziqi.cn

[Q30] 分组统计
来源：http://qyj.zhongyouzk.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rxx.tanke756.top

[Q31] 分组后过滤
来源：http://uea.xziqi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ofe.uphjek.com

[Q32] 分组拼接字符串
来源：http://nok.hesvh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rda.jyoumei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gxy.redwolf501.top

[Q33] 多列分组
来源：http://ghq.fengsongda.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wmf.bbcook.cn

[Q34] 每组取第一条
来源：http://vdb.ivvv.top

SELECT * FROM (
来源：http://boi.zdbjq.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uod.shzxlz.cn

) t WHERE rn = 1;
来源：http://ujs.sufxvd.cn

[Q35] 内连接
来源：http://gfj.gzhubu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fac.gotoacloud.top

[Q36] 左连接
来源：http://shz.hammf.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lhs.hammf.cn

[Q37] 右连接
来源：http://few.zhoulong.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://avm.yfazqb.com

[Q38] 全外连接（PostgreSQL）
来源：http://cii.kuanghao11.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iks.jqgfzy.top

[Q39] 自连接（查上下级）
来源：http://oyz.ydjk.org.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fow.yj20258.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xdk.tianlin.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://sma.nwbrower.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dwa.hywenlv.cn

[Q41] 多表连接
来源：http://eyx.chenjidiqi.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://tau.nanxuanxn.top

JOIN users u ON u.id = o.user_id
来源：http://jbu.c1oappe.top

JOIN products p ON p.id = o.product_id;
来源：http://esv.yueranfly.top

[Q42] 连接条件附加过滤
来源：http://rux.guowangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://pxc.daria6918.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nbd.ydjk.org.cn

[Q43] 标量子查询
来源：http://wwz.havefunace.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kiu.ybcxt.top

[Q44] IN 子查询
来源：http://hgg.cqqwz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://drw.dashuyun.cn

[Q45] EXISTS 判断存在
来源：http://uob.yj20258888.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ush.fanxiaobao.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://fdi.hnxiangtu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mgn.jianghu66.top

[Q47] 与平均值比较
来源：http://kaq.jqgufenzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fpe.daria6918.cn

[Q48] CTE 公用表表达式
来源：http://hhr.ywan-chungtsiang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gul.hesvh.cn

SELECT * FROM t WHERE c > 5;
来源：http://asa.jianghu66.top

[Q49] 更新单行
来源：http://sru.ehwqpu.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ohs.jinghuilouyu.cn

[Q50] 批量更新
来源：http://jct.c1oappe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://umi.hfpthk.cn

[Q51] 用子查询更新
来源：http://awe.tarul.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kib.wangdashe.top

[Q52] 删除指定行
来源：http://wfb.yvedp.cn

DELETE FROM users WHERE id = 10;
来源：http://mjq.vehdjk.com

[Q53] 按条件删除
来源：http://pkr.wangshuangyany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tsv.chenjidiqi.icu

[Q54] 清空表
来源：http://qyb.hywenlv.cn

TRUNCATE TABLE logs;
来源：http://chm.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://hgw.gotoacloud.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ywg.pycfn.com

[Q56] 密集排名（并列不占位）
来源：http://xwq.yuanzhike.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hxa.wangshuangyany.cn

[Q57] 行号
来源：http://qnp.zhoulong.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xpd.gogol.net.cn

[Q58] 累计求和
来源：http://vxk.quarkkingdee.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nrx.sxryk.cn

[Q59] 分组内累计
来源：http://psj.gaohongyu789.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tjg.chenlongwang.top

[Q60] 取上一行 / 下一行
来源：http://feb.gzhubu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fla.vqdsnc.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wrr.ehwqpu.com

[Q61] 移动平均
来源：http://jua.jlsjyb.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uba.xziqi.cn

[Q62] 分组占比
来源：http://pih.aibaodan.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://crv.hnxiangtu.top

[Q63] 开启事务
来源：http://vax.dianchejie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mlt.xuetiantiany.cn

[Q64] 提交事务
来源：http://sle.andypj.xyz

COMMIT;
来源：http://cni.ywan-chungtsiang.top

[Q65] 回滚事务
来源：http://ynh.pycfn.com

ROLLBACK;
来源：http://rqg.cheryme.top

[Q66] 行锁查询
来源：http://wtx.shzxlz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://siq.snrcjt.cn

[Q67] 设置隔离级别
来源：http://rjb.ivvv.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xnt.zdbjq.cn

[Q68] 保存点
来源：http://tzr.tanke756.top

SAVEPOINT sp1;
来源：http://bgh.52xcode.cn

ROLLBACK TO sp1;
来源：http://fpb.wangdashe.top

[Q69] 查看执行计划
来源：http://frj.hysaishi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://prg.cucudq.cn

[Q70] 更新统计信息
来源：http://jwh.dianchejie.cn

ANALYZE TABLE users;
来源：http://nbp.tarul.cn

[Q71] 查看建表语句
来源：http://rlt.fengsongda.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wzr.zhixingplan.top

[Q72] 查看索引
来源：http://cis.chenlongwang.top

SHOW INDEX FROM users;
来源：http://xup.meibo888.top

[Q73] 查看表状态
来源：http://maz.hammf.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://eja.jyoumei.cn

[Q74] 强制使用索引
来源：http://ybb.havefunace.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://avz.hywenlv.cn

[Q75] 日期格式化
来源：http://nbg.epnwcf.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pyg.ybcxt.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bfk.vehdjk.com

[Q76] 按天统计
来源：http://ktd.shanyushiyangtech.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bea.birdmap.top

[Q77] 时间加减
来源：http://dbb.pengpengdd.cyou

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fwg.shuidangran.top

[Q78] 当前时间
来源：http://eiw.guannengcc.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rrj.hesvh.cn

[Q79] 字符串拼接
来源：http://kxg.hesvh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dzz.zhiwuduotai.top

[Q80] 字符串截取
来源：http://gey.quarkkingdee.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pka.shuidangran.top

[Q81] 字符串替换
来源：http://ohe.ctjpmb.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jgc.zhoulong.xyz

[Q82] 字符长度与字节长度
来源：http://uty.fktsv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rln.fanxiaobao.xyz

[Q83] 大小写转换
来源：http://ovv.zycfv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cry.jinqigfzy.top

[Q84] 去除首尾空格
来源：http://dtx.fktsv.cn

SELECT TRIM(name) FROM users;
来源：http://rmr.hammf.cn

[Q85] 数值取整
来源：http://buz.fzhhl.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://owx.jyoumei.cn

[Q86] 读取 JSON 字段
来源：http://vba.quarkkingdee.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gqc.uphjek.com

[Q87] JSON 字段做条件
来源：http://tnl.cdnleiting.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oqp.xinyue.icu

[Q88] 行转列（条件聚合）
来源：http://mit.jianghu66.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xte.hnxiangtu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yrz.zycfv.cn

[Q89] 判断表是否存在
来源：http://hcv.chenzaomai.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gqm.aizwys.cn

[Q90] 生成序号列
来源：http://odz.ctjpmb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gvj.yj202588.top

================================================================================
来源：http://wrf.pycfn.com

R. Bash 专题
来源：http://efa.daxiang520.top

================================================================================
来源：http://wad.svipenyu.cn

[R01] shebang 与严格模式
来源：http://mhy.nanxinkj.top

#!/usr/bin/env bash
来源：http://prb.chenlongwang.top

set -euo pipefail
来源：http://mci.xinyue.icu

[R02] 变量赋值与使用
来源：http://qos.yj20258.top

name="Tom"; echo "$name"
来源：http://nbb.fktsv.cn

[R03] 只读变量
来源：http://pwi.xingfuxueyuan.xyz

readonly PI=3.14
来源：http://pdf.wangshuangyany.cn

[R04] 位置参数
来源：http://pch.shanyushiyangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wvw.quarkkingdee.top

[R05] 参数默认值
来源：http://ueo.xylfe.cn

name="${1:-default}"
来源：http://dtw.shuidangran.top

[R06] 判断命令是否存在
来源：http://olu.ybcxt.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ufy.xziqi.cn

[R07] if 判断文件
来源：http://eow.zdbjq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uxu.yangfankeji.com

[R08] 数值比较
来源：http://jhf.ywan-chungtsiang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://byq.snrcjt.cn

[R09] 字符串比较
来源：http://nnc.ehwqpu.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nwo.ydjk.org.cn

[R10] 正则匹配
来源：http://npq.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fnn.xinyue.icu

[R11] case 多分支
来源：http://ktj.redwolf501.top

case "$1" in
来源：http://nyy.c1oappe.top

start) echo "启动" ;;
来源：http://pbg.gotoacloud.top

stop)  echo "停止" ;;
来源：http://cqr.yj202588.top

*)     echo "未知命令" ;;
来源：http://rfg.gzhubu.top

esac
来源：http://hfp.havefunace.top

[R12] for 遍历文件
来源：http://tpm.yongpay.top

for f in *.txt; do echo "$f"; done
来源：http://mbj.jqgfzy.top

[R13] for 计数循环
来源：http://flz.chenjidiqi.icu

for i in {1..10}; do echo "$i"; done
来源：http://abr.ivvv.top

[R14] C 风格 for
来源：http://nfo.gaohongyu789.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wfa.yanxiufei.cn

[R15] while 逐行读文件
来源：http://bly.nanxinkj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pqu.9152youxi.cn

[R16] until 等待条件
来源：http://gga.bjfxy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qdv.c1oappe.top

[R17] 数组定义与取值
来源：http://hpa.aizwys.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qax.tian-w.cn

[R18] 遍历数组
来源：http://fhj.daria6918.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sil.cucudq.cn

[R19] 数组长度
来源：http://hyg.c1oappe.top

echo "${#arr[@]}"
来源：http://ujd.dianchejie.cn

[R20] 关联数组（字典）
来源：http://git.ppjwa.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tjq.tanke756.top

[R21] 字符串长度
来源：http://gso.xuanzx.com

echo "${#s}"
来源：http://edv.tianlin.xyz

[R22] 截取子串
来源：http://oue.52xcode.cn

echo "${s:0:5}"
来源：http://fdg.yfazqb.com

[R23] 字符串替换
来源：http://qwy.hongshengwenyu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rvh.tanke756.top

[R24] 大小写转换
来源：http://tut.ywan-chungtsiang.top

echo "${s^^}"; echo "${s,,}"
来源：http://ctu.jyoumei.cn

[R25] 去后缀 / 去前缀
来源：http://awf.tian-w.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lay.daxiang520.top

[R26] 命令替换
来源：http://tpy.daria6918.cn

now=$(date +%F); echo "$now"
来源：http://nyv.0kj1m.cn

[R27] 算术展开
来源：http://csz.mhx1999.top

echo $((1 + 2 * 3))
来源：http://isk.pycfn.com

[R28] 浮点运算
来源：http://til.cheryme.top

echo "scale=2; 10/3" | bc
来源：http://kpb.cqqwz.cn

[R29] 定义函数
来源：http://fff.jinqigfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lzy.hongshengwenyu.top

[R30] 函数返回状态码
来源：http://bwq.fktsv.cn

f() { return 0; }; f || echo "失败了"
来源：http://nby.yanxiufei.cn

[R31] 局部变量
来源：http://fae.yuanzhike.top

f() { local x=1; echo "$x"; }
来源：http://uwz.shanyushiyangkeji.top

[R32] 参数个数校验
来源：http://lkt.jqgufenzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tow.dashuyun.cn

[R33] 捕获错误并提示行号
来源：http://bbm.smart0.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wyi.vehdjk.com

[R34] 退出时清理
来源：http://vfg.jlsjyb.cn

trap 'rm -f "$tmp"' EXIT
来源：http://svf.fzhhl.top

[R35] 后台执行并等待
来源：http://vhk.hammf.cn


<!-- 参考信息 -->