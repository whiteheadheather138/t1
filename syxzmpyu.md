代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://dpx.zhijiandao.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ozn.ctjpmb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hct.dianchejie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mea.fanxiaobao.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gnh.fzhhl.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uck.xingfuxueyuan.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://nnm.aibaodan.cn

Ruby: a == b
来源：http://eei.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iov.chenjidiqi.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ibc.guowangkeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qrr.zhiwuduotai.top

PHP:  if (empty($x)) {}
来源：http://pqi.daria6918.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ywp.jinqigufen.top

TS:   if (x == null) {}
来源：http://ltu.zycfv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lio.ybcxt.top

Go:   if x == nil {}
来源：http://zqi.andypj.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eyq.ivvv.top

C#:   if (x is null) {}
来源：http://pbj.zycfv.cn

[P07] 防抖与节流
来源：http://nxs.daria6918.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ham.haohaochexian.top

PHP:  // 手写时间戳比较
来源：http://bcx.fanxiaobao.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mnw.jqgfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tjz.mhx1999.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dfz.xuanzx.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xup.hywenlv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xqf.nwbrower.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hsf.uphjek.com

[P08] 处理浮点精度问题
来源：http://ixm.vqdsnc.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gxe.gzhubu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://chy.cdnleiting.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uii.yueranfly.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hub.jinqigfzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ddz.yongpay.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rgg.wangshuangyany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cvl.shanyushiyangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://boj.zdbjq.cn

================================================================================
来源：http://tlj.shzxlz.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://emt.shangyingyoupin.top

================================================================================
来源：http://gvq.vehdjk.com

[Q01] 创建表
来源：http://nzp.yj202588.top

CREATE TABLE users (
来源：http://elj.smart0.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://peo.shanyushiyangtech.top

name VARCHAR(50) NOT NULL,
来源：http://jmj.tarul.cn

email VARCHAR(100) UNIQUE,
来源：http://pjf.jqgufenzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nof.shuidangran.top

);
来源：http://rkn.shanyushiyangkeji.top

[Q02] 创建带外键的表
来源：http://ylb.jiagoushi.top

CREATE TABLE orders (
来源：http://tkq.chenlongwang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://frb.snrcjt.cn

user_id INT NOT NULL,
来源：http://erg.havefunace.top

amount DECIMAL(10, 2),
来源：http://pzc.c1oappe.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lfa.snrcjt.cn

);
来源：http://scp.yj20258888.top

[Q03] 增加列
来源：http://rxy.c1oappe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kcp.guowangkeji.top

[Q04] 修改列类型
来源：http://wil.sxryk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qzw.tanke756.top

[Q05] 重命名列
来源：http://ocu.0kj1m.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://huj.jianghu66.top

[Q06] 删除列
来源：http://wfv.fehbvm.com

ALTER TABLE users DROP COLUMN age;
来源：http://djp.jinghuilouyu.cn

[Q07] 删除表
来源：http://pvc.jinghuilouyu.cn

DROP TABLE IF EXISTS orders;
来源：http://too.52xcode.cn

[Q08] 创建普通索引
来源：http://pps.cashguo.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pnk.yonumen.top

[Q09] 创建唯一索引
来源：http://fwk.yvedp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lvj.pengpengdd.cyou

[Q10] 插入单行
来源：http://boh.sxryk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vbj.sxryk.cn

[Q11] 一次插入多行
来源：http://evy.mhx1999.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qps.jqgfzy.top

[Q12] 插入后取自增 ID
来源：http://ftq.sweek.top

INSERT INTO users (name) VALUES ('C');
来源：http://szl.hnxiangtu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vgg.fengsongda.top

[Q13] 忽略重复插入
来源：http://rht.vehdjk.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sqb.guannengcc.top

[Q14] 存在则更新（upsert）
来源：http://wec.guannengcc.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qpm.nanxuanxn.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xpb.52xcode.cn

[Q15] 查询全部
来源：http://jog.yangfankeji.com

SELECT * FROM users;
来源：http://qvl.bbcook.cn

[Q16] 查询指定列
来源：http://pha.gotoacloud.top

SELECT id, name FROM users;
来源：http://gqn.zhixingplan.top

[Q17] 条件查询
来源：http://lsn.dianchejie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kxz.9152youxi.cn

[Q18] 模糊匹配
来源：http://yba.yuanzhike.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jzw.jlsjyb.cn

[Q19] 范围查询
来源：http://nmu.redwolf501.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rcx.sxryk.cn

[Q20] IN 列表
来源：http://kvh.xingfuxueyuan.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xwx.sufxvd.cn

[Q21] 空值判断
来源：http://ksb.zhijiandao.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jkn.hammf.cn

[Q22] 排序
来源：http://tor.daxiang520.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://odo.zhoulong.xyz

[Q23] 分页
来源：http://bla.ybcxt.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pzw.zhaomingkeji.xyz

[Q24] 去重
来源：http://ksu.hcnkem.com

SELECT DISTINCT city FROM users;
来源：http://htz.jiagoushi.top

[Q25] 只取前 N 条
来源：http://lkl.xziqi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hfj.yongpay.top

[Q26] 计数
来源：http://srm.shuidangran.top

SELECT COUNT(*) FROM users;
来源：http://zib.pycfn.com

[Q27] 条件计数
来源：http://xwk.xuetiantiany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gkc.sysykeji.top

[Q28] 求和与平均
来源：http://llv.kuanghao11.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qge.shzxlz.cn

[Q29] 最大最小值
来源：http://oqx.yonumen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://cmm.ppjwa.cn

[Q30] 分组统计
来源：http://aun.hcnkem.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cql.tanke756.top

[Q31] 分组后过滤
来源：http://pip.tanke756.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gca.kuanghao11.cn

[Q32] 分组拼接字符串
来源：http://ynb.dianchejie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qpq.jinyuanbaomall.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bol.jinqigfzy.top

[Q33] 多列分组
来源：http://tml.aibaodan.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wdj.9152youxi.cn

[Q34] 每组取第一条
来源：http://epd.tian-w.cn

SELECT * FROM (
来源：http://khr.yj20258.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dby.yvedp.cn

) t WHERE rn = 1;
来源：http://vki.ehwqpu.com

[Q35] 内连接
来源：http://whs.jiagoushi.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mnf.jinghuilouyu.cn

[Q36] 左连接
来源：http://enj.yuanzhike.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xpr.mhx1999.top

[Q37] 右连接
来源：http://lys.yj20258888.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hot.jiagoushi.top

[Q38] 全外连接（PostgreSQL）
来源：http://iot.cdnleiting.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zng.zycfv.cn

[Q39] 自连接（查上下级）
来源：http://qce.dianchejie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ohb.tarul.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nus.hywenlv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://agc.tanke756.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rcn.zhiwuduotai.top

[Q41] 多表连接
来源：http://uef.svipenyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://duf.iojbl.cn

JOIN users u ON u.id = o.user_id
来源：http://ozz.redwolf501.top

JOIN products p ON p.id = o.product_id;
来源：http://oqv.jyoumei.cn

[Q42] 连接条件附加过滤
来源：http://eae.haohaochexian.top

SELECT u.name, o.amount FROM users u
来源：http://ebf.ehwqpu.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xdk.hnxiangtu.top

[Q43] 标量子查询
来源：http://uaf.pengpengdd.cyou

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fyf.jiagoushi.top

[Q44] IN 子查询
来源：http://vcq.xuanzx.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sia.svipenyu.cn

[Q45] EXISTS 判断存在
来源：http://xvp.fehbvm.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mhl.yj202588.top

[Q46] NOT EXISTS 判断不存在
来源：http://ldl.feifeiyinyue.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fkt.fzhhl.top

[Q47] 与平均值比较
来源：http://peo.c1oappe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bjz.guowangkeji.top

[Q48] CTE 公用表表达式
来源：http://zqt.52xcode.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xmc.guannengcc.top

SELECT * FROM t WHERE c > 5;
来源：http://wxn.mhx1999.top

[Q49] 更新单行
来源：http://eyy.ydzc1.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fsb.fzhhl.top

[Q50] 批量更新
来源：http://orq.jinyuanbaomall.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dfa.aibaodan.cn

[Q51] 用子查询更新
来源：http://mpf.nanxuanxn.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ttm.zhaomingkeji.xyz

[Q52] 删除指定行
来源：http://hki.hcnkem.com

DELETE FROM users WHERE id = 10;
来源：http://vao.ivvv.top

[Q53] 按条件删除
来源：http://fve.jqgufenzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sbo.jinyuanbaomall.cn

[Q54] 清空表
来源：http://wzx.redwolf501.top

TRUNCATE TABLE logs;
来源：http://zny.xylfe.cn

[Q55] 排名（并列占位）
来源：http://cgj.wangshuangyany.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ovr.jlsjyb.cn

[Q56] 密集排名（并列不占位）
来源：http://nbe.ctjpmb.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iqa.gaohongyu789.top

[Q57] 行号
来源：http://sgh.feifeiyinyue.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://adf.yfazqb.com

[Q58] 累计求和
来源：http://lpm.zhoulong.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://spj.nanxuanxn.top

[Q59] 分组内累计
来源：http://qtx.ydzc1.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jqg.pengpengdd.cyou

[Q60] 取上一行 / 下一行
来源：http://eok.xziqi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hab.ivvv.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hzw.ehwqpu.com

[Q61] 移动平均
来源：http://aol.hnxiangtu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xsz.hongshengwenyu.top

[Q62] 分组占比
来源：http://pni.zhijiandao.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rwh.sysykeji.top

[Q63] 开启事务
来源：http://szg.fzhhl.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ymx.jinqigfzy.top

[Q64] 提交事务
来源：http://ivv.xingfuxueyuan.xyz

COMMIT;
来源：http://uzy.hammf.cn

[Q65] 回滚事务
来源：http://wst.cucudq.cn

ROLLBACK;
来源：http://iek.ivvv.top

[Q66] 行锁查询
来源：http://ljb.tanke756.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hax.dashuyun.cn

[Q67] 设置隔离级别
来源：http://jie.xuanzx.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ggp.uphjek.com

[Q68] 保存点
来源：http://ufl.sweek.top

SAVEPOINT sp1;
来源：http://oxs.52xcode.cn

ROLLBACK TO sp1;
来源：http://cuj.haohaochexian.top

[Q69] 查看执行计划
来源：http://toe.guannengcc.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://epq.jinqigufen.top

[Q70] 更新统计信息
来源：http://xci.fzhhl.top

ANALYZE TABLE users;
来源：http://crs.guowangkeji.top

[Q71] 查看建表语句
来源：http://cor.pengpengdd.cyou

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://esm.feifeiyinyue.top

[Q72] 查看索引
来源：http://tlq.nanxuanxn.top

SHOW INDEX FROM users;
来源：http://zgt.wangshuangyany.cn

[Q73] 查看表状态
来源：http://bne.guowangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ysb.yueranfly.top

[Q74] 强制使用索引
来源：http://ttn.chenlongwang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://phw.bjfxy.top

[Q75] 日期格式化
来源：http://bvk.jinqigufen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hon.sufxvd.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kvx.zdqjudy.top

[Q76] 按天统计
来源：http://jsz.zycfv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pre.jiagoushi.top

[Q77] 时间加减
来源：http://xbp.tian-w.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kbb.zdbjq.cn

[Q78] 当前时间
来源：http://fys.nwbrower.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rij.fanxiaobao.xyz

[Q79] 字符串拼接
来源：http://npv.chenjidiqi.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ixo.bbcook.cn

[Q80] 字符串截取
来源：http://byz.jqgfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kqn.jinyuanbaomall.cn

[Q81] 字符串替换
来源：http://wep.sweek.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jex.fzhhl.top

[Q82] 字符长度与字节长度
来源：http://qxz.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://frj.gzhubu.top

[Q83] 大小写转换
来源：http://vjf.birdmap.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dye.pycfn.com

[Q84] 去除首尾空格
来源：http://mst.shuidangran.top

SELECT TRIM(name) FROM users;
来源：http://ajv.ybcxt.top

[Q85] 数值取整
来源：http://xcq.sysykeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://afa.yanxiufei.cn

[Q86] 读取 JSON 字段
来源：http://det.vqdsnc.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lxs.yueranfly.top

[Q87] JSON 字段做条件
来源：http://jww.kuanghao11.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mth.andypj.xyz

[Q88] 行转列（条件聚合）
来源：http://wih.0kj1m.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lle.hammf.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qlv.hammf.cn

[Q89] 判断表是否存在
来源：http://oxx.zhaomingkeji.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gbl.yvedp.cn

[Q90] 生成序号列
来源：http://faw.zhijiandao.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xiz.xylfe.cn

================================================================================
来源：http://tgg.xingfuxueyuan.xyz

R. Bash 专题
来源：http://xug.zhengqikj.top

================================================================================
来源：http://gdd.chenjidiqi.icu

[R01] shebang 与严格模式
来源：http://rns.redwolf501.top

#!/usr/bin/env bash
来源：http://jqi.iojbl.cn

set -euo pipefail
来源：http://ryl.quarkkingdee.top

[R02] 变量赋值与使用
来源：http://pkn.hesvh.cn

name="Tom"; echo "$name"
来源：http://ivk.yj20258888.top

[R03] 只读变量
来源：http://tgp.zhoulong.xyz

readonly PI=3.14
来源：http://koi.hywenlv.cn

[R04] 位置参数
来源：http://wwn.shangyingyoupin.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eox.sysykeji.top

[R05] 参数默认值
来源：http://leo.shuidangran.top

name="${1:-default}"
来源：http://bau.guannengcc.top

[R06] 判断命令是否存在
来源：http://tud.tarul.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ckk.tanke756.top

[R07] if 判断文件
来源：http://fsj.shuidangran.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sbh.hcnkem.com

[R08] 数值比较
来源：http://del.jinqigfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://yno.jianghu66.top

[R09] 字符串比较
来源：http://qtd.zdqjudy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vfe.fanxiaobao.xyz

[R10] 正则匹配
来源：http://zrb.shanyushiyangtech.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yav.hcnkem.com

[R11] case 多分支
来源：http://bkn.jlsjyb.cn

case "$1" in
来源：http://szn.jinqigufen.top

start) echo "启动" ;;
来源：http://kha.wangdashe.top

stop)  echo "停止" ;;
来源：http://ige.ydzc1.top

*)     echo "未知命令" ;;
来源：http://ewp.yj20258.top

esac
来源：http://lic.zhongyouzk.top

[R12] for 遍历文件
来源：http://nrk.meibo888.top

for f in *.txt; do echo "$f"; done
来源：http://zex.xingfuxueyuan.xyz

[R13] for 计数循环
来源：http://giu.sxryk.cn

for i in {1..10}; do echo "$i"; done
来源：http://bcs.haohaochexian.top

[R14] C 风格 for
来源：http://pfz.pengpengdd.cyou

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cjy.fktsv.cn

[R15] while 逐行读文件
来源：http://rnk.zhongyouzk.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bqh.cashguo.top

[R16] until 等待条件
来源：http://vvo.dashuyun.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yce.haohaochexian.top

[R17] 数组定义与取值
来源：http://hxk.havefunace.top

arr=(a b c); echo "${arr[0]}"
来源：http://ybs.smart0.xyz

[R18] 遍历数组
来源：http://qru.hesvh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jgc.shangyingyoupin.top

[R19] 数组长度
来源：http://fyt.shzxlz.cn

echo "${#arr[@]}"
来源：http://zta.xuetiantiany.cn

[R20] 关联数组（字典）
来源：http://euk.yongpay.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gvt.sysykeji.top

[R21] 字符串长度
来源：http://bnu.dashuyun.cn

echo "${#s}"
来源：http://rhi.tanke756.top

[R22] 截取子串
来源：http://edw.zdbjq.cn

echo "${s:0:5}"
来源：http://upx.ehwqpu.com

[R23] 字符串替换
来源：http://vac.kuanghao11.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ucf.chenjidiqi.icu

[R24] 大小写转换
来源：http://zwp.meibo888.top

echo "${s^^}"; echo "${s,,}"
来源：http://tfw.yueranfly.top

[R25] 去后缀 / 去前缀
来源：http://zwx.xylfe.cn


<!-- 参考信息 -->