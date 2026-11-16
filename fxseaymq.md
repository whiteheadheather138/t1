代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xjz.dashuyun.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://htd.daxiang520.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aot.zdbjq.cn

PHP:  if (empty($x)) {}
来源：http://bdc.tanke756.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bjv.ivvv.top

TS:   if (x == null) {}
来源：http://qob.hesvh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://prh.feifeiyinyue.top

Go:   if x == nil {}
来源：http://yrs.jinyuanbaomall.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gdb.ivvv.top

C#:   if (x is null) {}
来源：http://pzj.c1oappe.top

[P07] 防抖与节流
来源：http://btn.cqqwz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rxp.52xcode.cn

PHP:  // 手写时间戳比较
来源：http://qig.guannengcc.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oov.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mbu.hongshengwenyu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vtz.birdmap.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ubh.zhengqikj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rir.hammf.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rfz.andypj.xyz

[P08] 处理浮点精度问题
来源：http://mnv.shuidangran.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sci.sjlbkw.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dmm.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fns.ehwqpu.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kbb.chenlongwang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hod.ivvv.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ckm.hongshengwenyu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oox.tarul.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pgt.dianchejie.cn

================================================================================
来源：http://fsx.fanxiaobao.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://avn.vehdjk.com

================================================================================
来源：http://hcd.jqgufenzy.top

[Q01] 创建表
来源：http://kqv.yonumen.top

CREATE TABLE users (
来源：http://lym.cdnleiting.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hhx.nanxinkj.top

name VARCHAR(50) NOT NULL,
来源：http://prz.xziqi.cn

email VARCHAR(100) UNIQUE,
来源：http://trx.sxryk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ghi.svipenyu.cn

);
来源：http://alt.vqdsnc.cn

[Q02] 创建带外键的表
来源：http://jmq.jianghu66.top

CREATE TABLE orders (
来源：http://ikk.sxryk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://iyh.jlsjyb.cn

user_id INT NOT NULL,
来源：http://eby.gaohongyu789.top

amount DECIMAL(10, 2),
来源：http://pzm.yj202588.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://loz.xuetiantiany.cn

);
来源：http://acz.xingfuxueyuan.xyz

[Q03] 增加列
来源：http://qlf.pengpengdd.cyou

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wey.gotoacloud.top

[Q04] 修改列类型
来源：http://mrt.guannengcc.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jkr.ybcxt.top

[Q05] 重命名列
来源：http://vhw.9152youxi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oii.yfazqb.com

[Q06] 删除列
来源：http://vnb.sufxvd.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vov.fzhhl.top

[Q07] 删除表
来源：http://lky.shanyushiyangtech.top

DROP TABLE IF EXISTS orders;
来源：http://yus.chenjidiqi.icu

[Q08] 创建普通索引
来源：http://bnr.hesvh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pdq.quarkkingdee.top

[Q09] 创建唯一索引
来源：http://qjp.shangyingyoupin.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://iyz.jinqigfzy.top

[Q10] 插入单行
来源：http://rny.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fqy.yongpay.top

[Q11] 一次插入多行
来源：http://ako.ppjwa.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tgq.jqgfzy.top

[Q12] 插入后取自增 ID
来源：http://wtx.cqqwz.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hag.dianchejie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ddp.aizwys.cn

[Q13] 忽略重复插入
来源：http://zdk.birdmap.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lmr.havefunace.top

[Q14] 存在则更新（upsert）
来源：http://dbm.vehdjk.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dhm.sxryk.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vxi.nwbrower.top

[Q15] 查询全部
来源：http://ltn.9152youxi.cn

SELECT * FROM users;
来源：http://zvg.sweek.top

[Q16] 查询指定列
来源：http://uhh.feifeiyinyue.top

SELECT id, name FROM users;
来源：http://ghp.nanxinkj.top

[Q17] 条件查询
来源：http://sgj.aizwys.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zkc.yanxiufei.cn

[Q18] 模糊匹配
来源：http://pit.bbcook.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dsw.andypj.xyz

[Q19] 范围查询
来源：http://lcb.vqdsnc.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mlk.zdqjudy.top

[Q20] IN 列表
来源：http://pdo.vqdsnc.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ghb.vqdsnc.cn

[Q21] 空值判断
来源：http://ckq.jinyuanbaomall.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rkc.fzhhl.top

[Q22] 排序
来源：http://mbz.shanyushiyangtech.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ptw.hongshengwenyu.top

[Q23] 分页
来源：http://wlf.yj202588.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fyy.shzxlz.cn

[Q24] 去重
来源：http://qau.feifeiyinyue.top

SELECT DISTINCT city FROM users;
来源：http://owp.ppjwa.cn

[Q25] 只取前 N 条
来源：http://rna.cashguo.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hfq.zdqjudy.top

[Q26] 计数
来源：http://tcw.tian-w.cn

SELECT COUNT(*) FROM users;
来源：http://pzc.zhoulong.xyz

[Q27] 条件计数
来源：http://wjl.ctjpmb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bof.jqgfzy.top

[Q28] 求和与平均
来源：http://vfa.sweek.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qyx.nwbrower.top

[Q29] 最大最小值
来源：http://wxw.cheryme.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fsd.zhiwuduotai.top

[Q30] 分组统计
来源：http://iqr.ydjk.org.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mlv.zhoulong.xyz

[Q31] 分组后过滤
来源：http://cdi.snrcjt.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gor.zhengqikj.top

[Q32] 分组拼接字符串
来源：http://ohr.ydzc1.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kaf.daria6918.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cia.jinyuanbaomall.cn

[Q33] 多列分组
来源：http://qkv.yonumen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xtk.chenjidiqi.icu

[Q34] 每组取第一条
来源：http://zmq.hnqzz.top

SELECT * FROM (
来源：http://sbs.feifeiyinyue.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xvj.cheryme.top

) t WHERE rn = 1;
来源：http://egj.yj20258.top

[Q35] 内连接
来源：http://pbn.yangfankeji.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dmh.yvedp.cn

[Q36] 左连接
来源：http://wun.yuxming.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dyt.xinyue.icu

[Q37] 右连接
来源：http://ugu.dashuyun.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://swv.hysaishi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fzo.ivvv.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rez.dashuyun.cn

[Q39] 自连接（查上下级）
来源：http://csz.nwbrower.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tom.jlsjyb.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://emn.zhixingplan.top

[Q40] 交叉连接（笛卡尔积）
来源：http://cov.cqqwz.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vmg.tanke756.top

[Q41] 多表连接
来源：http://pup.0kj1m.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wpq.kuanghao11.cn

JOIN users u ON u.id = o.user_id
来源：http://rkx.hysaishi.cn

JOIN products p ON p.id = o.product_id;
来源：http://dau.xingfuxueyuan.xyz

[Q42] 连接条件附加过滤
来源：http://etj.cdnleiting.top

SELECT u.name, o.amount FROM users u
来源：http://bml.zhijiandao.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vbt.mhx1999.top

[Q43] 标量子查询
来源：http://ilo.nwbrower.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://keq.daria6918.cn

[Q44] IN 子查询
来源：http://ftr.yonumen.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fzx.zhiwuduotai.top

[Q45] EXISTS 判断存在
来源：http://hgg.tian-w.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ice.0kj1m.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ldz.zhaomingkeji.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cvw.meibo888.top

[Q47] 与平均值比较
来源：http://wpz.feifeiyinyue.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eep.ydzc1.top

[Q48] CTE 公用表表达式
来源：http://eov.tianlin.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vjp.chenlongwang.top

SELECT * FROM t WHERE c > 5;
来源：http://jhj.nanxuanxn.top

[Q49] 更新单行
来源：http://vkb.ydjk.org.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dlc.daria6918.cn

[Q50] 批量更新
来源：http://kub.ybcxt.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://diq.redwolf501.top

[Q51] 用子查询更新
来源：http://vaf.ywan-chungtsiang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kcb.zhongyouzk.top

[Q52] 删除指定行
来源：http://nnk.jinghuilouyu.cn

DELETE FROM users WHERE id = 10;
来源：http://evw.pengpengdd.cyou

[Q53] 按条件删除
来源：http://ddw.ydzc1.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ckc.yj20258888.top

[Q54] 清空表
来源：http://zwv.mhx1999.top

TRUNCATE TABLE logs;
来源：http://nkc.cucudq.cn

[Q55] 排名（并列占位）
来源：http://jpq.cashguo.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pxw.xuanzx.com

[Q56] 密集排名（并列不占位）
来源：http://thp.jqgufenzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ghr.hammf.cn

[Q57] 行号
来源：http://pqp.hysaishi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pcl.bjfxy.top

[Q58] 累计求和
来源：http://mcf.mhx1999.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fza.snrcjt.cn

[Q59] 分组内累计
来源：http://oxb.tianlin.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kce.zdbjq.cn

[Q60] 取上一行 / 下一行
来源：http://xvh.sjlbkw.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ehz.9152youxi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vyu.fanxiaobao.xyz

[Q61] 移动平均
来源：http://qkw.pengpengdd.cyou

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hfg.yangfankeji.com

[Q62] 分组占比
来源：http://ebh.iojbl.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jhx.tianlin.xyz

[Q63] 开启事务
来源：http://qzl.mhx1999.top

START TRANSACTION;                -- 或 BEGIN
来源：http://krk.yuxming.cn

[Q64] 提交事务
来源：http://dcr.xuanzx.com

COMMIT;
来源：http://vsm.uphjek.com

[Q65] 回滚事务
来源：http://lbv.gogol.net.cn

ROLLBACK;
来源：http://yjg.daria6918.cn

[Q66] 行锁查询
来源：http://ejj.jlsjyb.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oee.ydjk.org.cn

[Q67] 设置隔离级别
来源：http://iom.vqdsnc.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vex.haohaochexian.top

[Q68] 保存点
来源：http://vbu.cheryme.top

SAVEPOINT sp1;
来源：http://gnc.feifeiyinyue.top

ROLLBACK TO sp1;
来源：http://nhc.hnqzz.top

[Q69] 查看执行计划
来源：http://mcj.gaohongyu789.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wav.xuanzx.com

[Q70] 更新统计信息
来源：http://lcl.havefunace.top

ANALYZE TABLE users;
来源：http://jji.gzhubu.top

[Q71] 查看建表语句
来源：http://wlx.nanxinkj.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tdp.uphjek.com

[Q72] 查看索引
来源：http://jjp.316326.xyz

SHOW INDEX FROM users;
来源：http://ljf.52xcode.cn

[Q73] 查看表状态
来源：http://trz.gzhubu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vjd.cqqwz.cn

[Q74] 强制使用索引
来源：http://nhz.redwolf501.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bun.9152youxi.cn

[Q75] 日期格式化
来源：http://hkf.yanxiufei.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://inx.kuanghao11.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://irg.zhoulong.xyz

[Q76] 按天统计
来源：http://xpo.yonumen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hko.xziqi.cn

[Q77] 时间加减
来源：http://rxf.feifeiyinyue.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://slr.hywenlv.cn

[Q78] 当前时间
来源：http://cyd.xinyue.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ftp.316326.xyz

[Q79] 字符串拼接
来源：http://tcu.fehbvm.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qbf.cucudq.cn

[Q80] 字符串截取
来源：http://lso.tarul.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vko.vehdjk.com

[Q81] 字符串替换
来源：http://fws.shzxlz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fja.zhijiandao.cn

[Q82] 字符长度与字节长度
来源：http://ksj.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://grn.shanyushiyangtech.top

[Q83] 大小写转换
来源：http://mli.ydjk.org.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kal.zdqjudy.top

[Q84] 去除首尾空格
来源：http://adx.redwolf501.top

SELECT TRIM(name) FROM users;
来源：http://hcm.fktsv.cn

[Q85] 数值取整
来源：http://bpk.jqgfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jmb.ybcxt.top

[Q86] 读取 JSON 字段
来源：http://pqk.jqgfzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pbs.yj20258888.top

[Q87] JSON 字段做条件
来源：http://npr.kuanghao11.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://edq.jianghu66.top

[Q88] 行转列（条件聚合）
来源：http://wja.cheryme.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hfd.ydjk.org.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vfz.sweek.top

[Q89] 判断表是否存在
来源：http://yup.zhoulong.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kxw.svipenyu.cn

[Q90] 生成序号列
来源：http://lqu.jianghu66.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://spo.bjfxy.top

================================================================================
来源：http://rhz.yj20258.top

R. Bash 专题
来源：http://tkr.shzxlz.cn

================================================================================
来源：http://qvn.kuanghao11.cn

[R01] shebang 与严格模式
来源：http://nvx.zycfv.cn

#!/usr/bin/env bash
来源：http://otq.epnwcf.com

set -euo pipefail
来源：http://xol.chenjidiqi.icu

[R02] 变量赋值与使用
来源：http://omh.svipenyu.cn

name="Tom"; echo "$name"
来源：http://bcz.tian-w.cn

[R03] 只读变量
来源：http://zql.zdbjq.cn

readonly PI=3.14
来源：http://bbs.yvedp.cn

[R04] 位置参数
来源：http://cdp.zdbjq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zxl.bbcook.cn

[R05] 参数默认值
来源：http://ioa.c1oappe.top

name="${1:-default}"
来源：http://zws.cashguo.top

[R06] 判断命令是否存在
来源：http://gya.cashguo.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hed.tarul.cn

[R07] if 判断文件
来源：http://amu.chenzaomai.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qqn.cucudq.cn

[R08] 数值比较
来源：http://wgd.nwbrower.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mld.dashuyun.cn

[R09] 字符串比较
来源：http://crc.zhaomingkeji.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yiw.shanyushiyangkeji.top

[R10] 正则匹配
来源：http://gwy.hongshengwenyu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://syr.andypj.xyz

[R11] case 多分支
来源：http://zio.chenlongwang.top

case "$1" in
来源：http://det.pycfn.com

start) echo "启动" ;;
来源：http://rhs.snrcjt.cn

stop)  echo "停止" ;;
来源：http://amf.guowangkeji.top

*)     echo "未知命令" ;;
来源：http://qqa.yj20258.top

esac
来源：http://ggw.zhixingplan.top

[R12] for 遍历文件
来源：http://chu.jqgufenzy.top

for f in *.txt; do echo "$f"; done
来源：http://fln.shuidangran.top

[R13] for 计数循环
来源：http://ssj.yfazqb.com

for i in {1..10}; do echo "$i"; done
来源：http://qtx.iojbl.cn

[R14] C 风格 for
来源：http://qvt.tanke756.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vjp.fehbvm.com

[R15] while 逐行读文件
来源：http://pew.hcnkem.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://khw.xuanzx.com

[R16] until 等待条件
来源：http://hjt.hnqzz.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uzs.tian-w.cn

[R17] 数组定义与取值
来源：http://yow.shanyushiyangtech.top

arr=(a b c); echo "${arr[0]}"
来源：http://uwu.ywan-chungtsiang.top

[R18] 遍历数组
来源：http://mor.cqqwz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ypk.jinghuilouyu.cn

[R19] 数组长度
来源：http://oiw.yvedp.cn

echo "${#arr[@]}"
来源：http://mzf.hnqzz.top

[R20] 关联数组（字典）
来源：http://pyr.daxiang520.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://san.zdqjudy.top

[R21] 字符串长度
来源：http://dfj.yonumen.top

echo "${#s}"
来源：http://sqo.sweek.top

[R22] 截取子串
来源：http://oro.daria6918.cn

echo "${s:0:5}"
来源：http://peo.ctjpmb.com

[R23] 字符串替换
来源：http://uvk.jinyuanbaomall.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dyb.vqdsnc.cn

[R24] 大小写转换
来源：http://jgd.cucudq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yqv.yj202588.top

[R25] 去后缀 / 去前缀
来源：http://dso.fengsongda.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://far.hongshengwenyu.top

[R26] 命令替换
来源：http://eph.zycfv.cn

now=$(date +%F); echo "$now"
来源：http://fkq.zhaomingkeji.xyz

[R27] 算术展开
来源：http://nbk.yongpay.top

echo $((1 + 2 * 3))
来源：http://jed.yj202588.top

[R28] 浮点运算
来源：http://egs.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://muq.hnxiangtu.top

[R29] 定义函数
来源：http://tnd.feifeiyinyue.top


<!-- 参考信息 -->