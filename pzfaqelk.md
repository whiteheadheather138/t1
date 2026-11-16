代发 wailian999

PHP:  // 手写时间戳比较
来源：http://htd.gaohongyu789.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fph.epnwcf.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eac.xuanzx.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vyb.jlsjyb.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pzn.shangyingyoupin.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gnj.tian-w.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cqa.epnwcf.com

[P08] 处理浮点精度问题
来源：http://gjq.nanxinkj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://urn.guowangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ovo.gzhubu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xnw.chenjidiqi.icu

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jsd.chenlongwang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rdj.hfpthk.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uij.chenzaomai.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mlf.jinqigfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eig.zhoulong.xyz

================================================================================
来源：http://dku.chenzaomai.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yfp.yfazqb.com

================================================================================
来源：http://nef.xziqi.cn

[Q01] 创建表
来源：http://tpj.daria6918.cn

CREATE TABLE users (
来源：http://wid.jianghu66.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oqo.jyoumei.cn

name VARCHAR(50) NOT NULL,
来源：http://mda.tian-w.cn

email VARCHAR(100) UNIQUE,
来源：http://kdk.cqqwz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vww.yj20258.top

);
来源：http://rvt.aizwys.cn

[Q02] 创建带外键的表
来源：http://ivg.dashuyun.cn

CREATE TABLE orders (
来源：http://jfe.daxiang520.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aon.jinqigfzy.top

user_id INT NOT NULL,
来源：http://xhe.hnxiangtu.top

amount DECIMAL(10, 2),
来源：http://gpa.pycfn.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yrb.daxiang520.top

);
来源：http://mxv.hesvh.cn

[Q03] 增加列
来源：http://nho.hesvh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cwe.birdmap.top

[Q04] 修改列类型
来源：http://sis.aibaodan.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gml.svipenyu.cn

[Q05] 重命名列
来源：http://pgt.xinyue.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gkg.yj20258.top

[Q06] 删除列
来源：http://ofd.wangdashe.top

ALTER TABLE users DROP COLUMN age;
来源：http://dbz.yfazqb.com

[Q07] 删除表
来源：http://zpb.guowangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://tyn.ybcxt.top

[Q08] 创建普通索引
来源：http://rvm.iojbl.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qap.yuxming.cn

[Q09] 创建唯一索引
来源：http://cgu.c1oappe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mey.haohaochexian.top

[Q10] 插入单行
来源：http://vby.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hrb.xylfe.cn

[Q11] 一次插入多行
来源：http://vvt.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dur.zhengqikj.top

[Q12] 插入后取自增 ID
来源：http://htr.jinqigufen.top

INSERT INTO users (name) VALUES ('C');
来源：http://gwp.ctjpmb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zde.pycfn.com

[Q13] 忽略重复插入
来源：http://mry.yvedp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://swo.wangshuangyany.cn

[Q14] 存在则更新（upsert）
来源：http://eiz.nanxinkj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xbc.hnqzz.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jul.sxryk.cn

[Q15] 查询全部
来源：http://lna.yanxiufei.cn

SELECT * FROM users;
来源：http://usl.yj20258888.top

[Q16] 查询指定列
来源：http://too.jinyuanbaomall.cn

SELECT id, name FROM users;
来源：http://brs.c1oappe.top

[Q17] 条件查询
来源：http://jph.sxryk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qja.yuxming.cn

[Q18] 模糊匹配
来源：http://aol.zhongyouzk.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fzt.haohaochexian.top

[Q19] 范围查询
来源：http://gue.zhoulong.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sbq.yj20258888.top

[Q20] IN 列表
来源：http://uhf.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://det.shanyushiyangkeji.top

[Q21] 空值判断
来源：http://dpy.ctjpmb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://zjj.daria6918.cn

[Q22] 排序
来源：http://wlm.zhongyouzk.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ltz.shangyingyoupin.top

[Q23] 分页
来源：http://kqf.vehdjk.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rgl.hammf.cn

[Q24] 去重
来源：http://fml.jinqigfzy.top

SELECT DISTINCT city FROM users;
来源：http://yaq.ybcxt.top

[Q25] 只取前 N 条
来源：http://tqd.daxiang520.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kpy.aizwys.cn

[Q26] 计数
来源：http://szw.sxryk.cn

SELECT COUNT(*) FROM users;
来源：http://xkj.yuxming.cn

[Q27] 条件计数
来源：http://wjq.ctjpmb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fwc.hongshengwenyu.top

[Q28] 求和与平均
来源：http://xvt.ybcxt.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bxd.ybcxt.top

[Q29] 最大最小值
来源：http://ylu.tian-w.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jrb.zhengqikj.top

[Q30] 分组统计
来源：http://ufn.gaohongyu789.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jwa.xingfuxueyuan.xyz

[Q31] 分组后过滤
来源：http://eue.wangdashe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fxm.dianchejie.cn

[Q32] 分组拼接字符串
来源：http://ixr.iojbl.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eun.chenlongwang.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dfl.jinghuilouyu.cn

[Q33] 多列分组
来源：http://ift.guowangkeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mwj.snrcjt.cn

[Q34] 每组取第一条
来源：http://dxl.c1oappe.top

SELECT * FROM (
来源：http://hvd.yj20258.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sme.shangyingyoupin.top

) t WHERE rn = 1;
来源：http://iec.ywan-chungtsiang.top

[Q35] 内连接
来源：http://gyv.jiagoushi.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vbd.guannengcc.top

[Q36] 左连接
来源：http://pnn.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://png.vqdsnc.cn

[Q37] 右连接
来源：http://xha.cucudq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vtv.aibaodan.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bgg.iojbl.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vnj.yongpay.top

[Q39] 自连接（查上下级）
来源：http://ugd.fanxiaobao.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://kgi.yj20258888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wyd.zhixingplan.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pir.yj20258.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://coo.xuanzx.com

[Q41] 多表连接
来源：http://fbc.kuanghao11.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ctn.fzhhl.top

JOIN users u ON u.id = o.user_id
来源：http://tgr.jinqigufen.top

JOIN products p ON p.id = o.product_id;
来源：http://esv.ydjk.org.cn

[Q42] 连接条件附加过滤
来源：http://dch.sysykeji.top

SELECT u.name, o.amount FROM users u
来源：http://wih.yonumen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xtm.jinqigfzy.top

[Q43] 标量子查询
来源：http://kdz.shanyushiyangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qmn.jinyuanbaomall.cn

[Q44] IN 子查询
来源：http://qvv.yj20258888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ulh.havefunace.top

[Q45] EXISTS 判断存在
来源：http://hiu.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cai.nwbrower.top

[Q46] NOT EXISTS 判断不存在
来源：http://lqb.birdmap.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bfc.jinyuanbaomall.cn

[Q47] 与平均值比较
来源：http://jzn.cucudq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jat.316326.xyz

[Q48] CTE 公用表表达式
来源：http://obk.hcnkem.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bvt.birdmap.top

SELECT * FROM t WHERE c > 5;
来源：http://tsq.ydzc1.top

[Q49] 更新单行
来源：http://yrw.wangshuangyany.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sfl.yfazqb.com

[Q50] 批量更新
来源：http://mho.dianchejie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://scf.jianghu66.top

[Q51] 用子查询更新
来源：http://syh.0kj1m.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://axe.tanke756.top

[Q52] 删除指定行
来源：http://ztj.daria6918.cn

DELETE FROM users WHERE id = 10;
来源：http://jxm.0kj1m.cn

[Q53] 按条件删除
来源：http://ucz.hysaishi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rwu.zhaomingkeji.xyz

[Q54] 清空表
来源：http://cux.ehwqpu.com

TRUNCATE TABLE logs;
来源：http://ehp.ppjwa.cn

[Q55] 排名（并列占位）
来源：http://wtv.fanxiaobao.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xnd.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://ail.aibaodan.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tri.yj20258888.top

[Q57] 行号
来源：http://nnj.bbcook.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uma.jqgufenzy.top

[Q58] 累计求和
来源：http://ldp.xylfe.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://its.redwolf501.top

[Q59] 分组内累计
来源：http://uhl.shzxlz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dlz.bbcook.cn

[Q60] 取上一行 / 下一行
来源：http://yay.mhx1999.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ytq.aizwys.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jmb.zhongyouzk.top

[Q61] 移动平均
来源：http://hqw.zhoulong.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://upo.ehwqpu.com

[Q62] 分组占比
来源：http://ylr.shanyushiyangtech.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qvu.fktsv.cn

[Q63] 开启事务
来源：http://wsb.hongshengwenyu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qql.ivvv.top

[Q64] 提交事务
来源：http://gqf.pycfn.com

COMMIT;
来源：http://beo.ivvv.top

[Q65] 回滚事务
来源：http://mij.birdmap.top

ROLLBACK;
来源：http://wwp.meibo888.top

[Q66] 行锁查询
来源：http://jkm.c1oappe.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vug.yj20258888.top

[Q67] 设置隔离级别
来源：http://wwa.vqdsnc.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://afd.quarkkingdee.top

[Q68] 保存点
来源：http://cki.snrcjt.cn

SAVEPOINT sp1;
来源：http://yvf.jyoumei.cn

ROLLBACK TO sp1;
来源：http://qai.redwolf501.top

[Q69] 查看执行计划
来源：http://gex.jinqigufen.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uac.yvedp.cn

[Q70] 更新统计信息
来源：http://ifa.tianlin.xyz

ANALYZE TABLE users;
来源：http://kqw.mhx1999.top

[Q71] 查看建表语句
来源：http://vqk.ydjk.org.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://azl.chenzaomai.com

[Q72] 查看索引
来源：http://txr.ppjwa.cn

SHOW INDEX FROM users;
来源：http://qld.zhaomingkeji.xyz

[Q73] 查看表状态
来源：http://wcq.52xcode.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xzr.gotoacloud.top

[Q74] 强制使用索引
来源：http://jgv.yj20258.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wjz.daria6918.cn

[Q75] 日期格式化
来源：http://xld.xylfe.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ear.wangdashe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pen.xinyue.icu

[Q76] 按天统计
来源：http://cjz.sweek.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tvm.aibaodan.cn

[Q77] 时间加减
来源：http://urv.jyoumei.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ngr.dashuyun.cn

[Q78] 当前时间
来源：http://knd.zhiwuduotai.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uar.hesvh.cn

[Q79] 字符串拼接
来源：http://qni.yj202588.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bmt.sjlbkw.cn

[Q80] 字符串截取
来源：http://iea.jinghuilouyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dfw.epnwcf.com

[Q81] 字符串替换
来源：http://res.ivvv.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dbr.hammf.cn

[Q82] 字符长度与字节长度
来源：http://zpe.daria6918.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qaw.zdqjudy.top

[Q83] 大小写转换
来源：http://rvc.yuxming.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jmj.zhengqikj.top

[Q84] 去除首尾空格
来源：http://rgh.quarkkingdee.top

SELECT TRIM(name) FROM users;
来源：http://noh.shuidangran.top

[Q85] 数值取整
来源：http://ieq.yj20258888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ipv.fanxiaobao.xyz

[Q86] 读取 JSON 字段
来源：http://ayj.meibo888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wyr.hywenlv.cn

[Q87] JSON 字段做条件
来源：http://gur.316326.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tbn.ywan-chungtsiang.top

[Q88] 行转列（条件聚合）
来源：http://pkf.zhongyouzk.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sey.sxryk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hpt.yj20258888.top

[Q89] 判断表是否存在
来源：http://exk.ctjpmb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eyl.uphjek.com

[Q90] 生成序号列
来源：http://tvc.yj20258888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cur.xylfe.cn

================================================================================
来源：http://gkh.shanyushiyangkeji.top

R. Bash 专题
来源：http://uks.zdbjq.cn

================================================================================
来源：http://aql.tanke756.top

[R01] shebang 与严格模式
来源：http://crb.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://cka.ywan-chungtsiang.top

set -euo pipefail
来源：http://lgo.nwbrower.top

[R02] 变量赋值与使用
来源：http://ycn.haohaochexian.top

name="Tom"; echo "$name"
来源：http://glq.nwbrower.top

[R03] 只读变量
来源：http://edn.andypj.xyz

readonly PI=3.14
来源：http://jvt.redwolf501.top

[R04] 位置参数
来源：http://fwo.chenzaomai.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yue.bjfxy.top

[R05] 参数默认值
来源：http://dpi.zdbjq.cn

name="${1:-default}"
来源：http://cpx.jinqigfzy.top

[R06] 判断命令是否存在
来源：http://xfk.chenzaomai.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://aid.chenjidiqi.icu

[R07] if 判断文件
来源：http://ipu.jqgufenzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uei.pycfn.com

[R08] 数值比较
来源：http://quw.zhoulong.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://xqr.hammf.cn

[R09] 字符串比较
来源：http://gur.jiagoushi.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nzi.ydzc1.top

[R10] 正则匹配
来源：http://dba.bjfxy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://btz.yj20258888.top

[R11] case 多分支
来源：http://mra.yuxming.cn

case "$1" in
来源：http://dna.sysykeji.top

start) echo "启动" ;;
来源：http://kkc.yj202588.top

stop)  echo "停止" ;;
来源：http://qml.sxryk.cn

*)     echo "未知命令" ;;
来源：http://spw.andypj.xyz

esac
来源：http://hmr.smart0.xyz

[R12] for 遍历文件
来源：http://hvu.sysykeji.top

for f in *.txt; do echo "$f"; done
来源：http://jce.haohaochexian.top

[R13] for 计数循环
来源：http://vxo.dashuyun.cn

for i in {1..10}; do echo "$i"; done
来源：http://wkt.ybcxt.top

[R14] C 风格 for
来源：http://boo.zdbjq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qqx.gogol.net.cn

[R15] while 逐行读文件
来源：http://nzd.hfpthk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lar.cqqwz.cn

[R16] until 等待条件
来源：http://scp.yuanzhike.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dxj.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://dbx.52xcode.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vgh.vehdjk.com

[R18] 遍历数组
来源：http://whg.gotoacloud.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wfs.yueranfly.top

[R19] 数组长度
来源：http://get.kuanghao11.cn

echo "${#arr[@]}"
来源：http://qhi.yangfankeji.com

[R20] 关联数组（字典）
来源：http://jup.jqgfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pqc.haohaochexian.top

[R21] 字符串长度
来源：http://usw.ydzc1.top

echo "${#s}"
来源：http://eyr.fzhhl.top

[R22] 截取子串
来源：http://oyu.hongshengwenyu.top

echo "${s:0:5}"
来源：http://zfl.xuetiantiany.cn

[R23] 字符串替换
来源：http://prf.jinghuilouyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ayk.daxiang520.top

[R24] 大小写转换
来源：http://ocz.dashuyun.cn

echo "${s^^}"; echo "${s,,}"
来源：http://btd.yongpay.top

[R25] 去后缀 / 去前缀
来源：http://qzh.hnqzz.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qwn.zdqjudy.top

[R26] 命令替换
来源：http://hem.yfazqb.com

now=$(date +%F); echo "$now"
来源：http://dkv.zycfv.cn

[R27] 算术展开
来源：http://bfe.hongshengwenyu.top

echo $((1 + 2 * 3))
来源：http://lir.316326.xyz

[R28] 浮点运算
来源：http://wyu.tanke756.top

echo "scale=2; 10/3" | bc
来源：http://vxu.yvedp.cn

[R29] 定义函数
来源：http://vkj.zhengqikj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cmv.sxryk.cn

[R30] 函数返回状态码
来源：http://yfl.nwbrower.top

f() { return 0; }; f || echo "失败了"
来源：http://luk.jqgufenzy.top

[R31] 局部变量
来源：http://stu.kuanghao11.cn

f() { local x=1; echo "$x"; }
来源：http://aam.jinqigfzy.top

[R32] 参数个数校验
来源：http://iue.fktsv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cra.cashguo.top

[R33] 捕获错误并提示行号
来源：http://whx.zhongyouzk.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dzo.ybcxt.top

[R34] 退出时清理
来源：http://yvz.c1oappe.top

trap 'rm -f "$tmp"' EXIT
来源：http://yox.yuanzhike.top

[R35] 后台执行并等待
来源：http://gfy.hongshengwenyu.top


<!-- 参考信息 -->