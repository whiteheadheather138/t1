代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uey.sysykeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gtm.shanyushiyangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lvi.jlsjyb.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ezi.shanyushiyangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://ahc.tian-w.cn

Go:   len(arr);  len(m)
来源：http://qbm.ybcxt.top

Ruby: x.length;  x.size
来源：http://tgc.pycfn.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://wch.mhx1999.top

[P05] 判断两个对象内容是否相等
来源：http://qwk.jlsjyb.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ysc.epnwcf.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ovu.zhaomingkeji.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nyh.yj20258.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://onm.haohaochexian.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://osa.zhiwuduotai.top

Go:   reflect.DeepEqual(a, b)
来源：http://doh.c1oappe.top

Ruby: a == b
来源：http://oxm.xylfe.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pqc.tian-w.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ooj.gzhubu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hzh.cdnleiting.top

PHP:  if (empty($x)) {}
来源：http://xgd.fengsongda.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ztx.jqgufenzy.top

TS:   if (x == null) {}
来源：http://bxf.316326.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://tyx.jinyuanbaomall.cn

Go:   if x == nil {}
来源：http://ahz.bbcook.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kiu.yonumen.top

C#:   if (x is null) {}
来源：http://ine.aizwys.cn

[P07] 防抖与节流
来源：http://nms.bbcook.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fpj.xziqi.cn

PHP:  // 手写时间戳比较
来源：http://uuf.sxryk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gai.guowangkeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zkg.ywan-chungtsiang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cvb.ivvv.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rmt.hcnkem.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://rmo.birdmap.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cui.hfpthk.cn

[P08] 处理浮点精度问题
来源：http://wbq.jqgfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jay.yfazqb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ejb.fanxiaobao.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rpp.chenlongwang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qvp.yj20258.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://utq.tarul.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iqw.zdqjudy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cpn.gotoacloud.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pvs.hesvh.cn

================================================================================
来源：http://tbw.cucudq.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lup.chenjidiqi.icu

================================================================================
来源：http://vnm.fengsongda.top

[Q01] 创建表
来源：http://lns.iojbl.cn

CREATE TABLE users (
来源：http://hfd.zhiwuduotai.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qim.zhixingplan.top

name VARCHAR(50) NOT NULL,
来源：http://mig.mhx1999.top

email VARCHAR(100) UNIQUE,
来源：http://nmi.cucudq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://plh.yj20258.top

);
来源：http://ixs.birdmap.top

[Q02] 创建带外键的表
来源：http://cfi.hongshengwenyu.top

CREATE TABLE orders (
来源：http://awh.yfazqb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uir.cucudq.cn

user_id INT NOT NULL,
来源：http://lkd.ydzc1.top

amount DECIMAL(10, 2),
来源：http://fcb.jinghuilouyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bed.sxryk.cn

);
来源：http://ttt.tianlin.xyz

[Q03] 增加列
来源：http://uer.yj202588.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://flj.52xcode.cn

[Q04] 修改列类型
来源：http://qoi.haohaochexian.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oyc.yvedp.cn

[Q05] 重命名列
来源：http://wyz.cucudq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qgd.ydzc1.top

[Q06] 删除列
来源：http://ovd.daria6918.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wva.gaohongyu789.top

[Q07] 删除表
来源：http://oxo.daxiang520.top

DROP TABLE IF EXISTS orders;
来源：http://ctk.cqqwz.cn

[Q08] 创建普通索引
来源：http://lne.hcnkem.com

CREATE INDEX idx_users_email ON users(email);
来源：http://tui.xuanzx.com

[Q09] 创建唯一索引
来源：http://tei.zdbjq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hre.ehwqpu.com

[Q10] 插入单行
来源：http://jgx.bjfxy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mth.aibaodan.cn

[Q11] 一次插入多行
来源：http://rrh.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kqj.yanxiufei.cn

[Q12] 插入后取自增 ID
来源：http://jug.vqdsnc.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lwb.c1oappe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xuh.yuanzhike.top

[Q13] 忽略重复插入
来源：http://wsp.zhoulong.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pkc.cashguo.top

[Q14] 存在则更新（upsert）
来源：http://krq.ehwqpu.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wal.cqqwz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://suv.havefunace.top

[Q15] 查询全部
来源：http://edq.zhengqikj.top

SELECT * FROM users;
来源：http://lux.meibo888.top

[Q16] 查询指定列
来源：http://brw.gogol.net.cn

SELECT id, name FROM users;
来源：http://dgd.zycfv.cn

[Q17] 条件查询
来源：http://elg.chenjidiqi.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vqj.jlsjyb.cn

[Q18] 模糊匹配
来源：http://sfv.aibaodan.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gtq.hfpthk.cn

[Q19] 范围查询
来源：http://ckw.zhiwuduotai.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jag.yj20258.top

[Q20] IN 列表
来源：http://wfh.cdnleiting.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jip.jqgufenzy.top

[Q21] 空值判断
来源：http://xnj.gotoacloud.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vla.birdmap.top

[Q22] 排序
来源：http://nkz.meibo888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xmi.yvedp.cn

[Q23] 分页
来源：http://jut.jinyuanbaomall.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://egc.vqdsnc.cn

[Q24] 去重
来源：http://ecs.zdbjq.cn

SELECT DISTINCT city FROM users;
来源：http://frt.svipenyu.cn

[Q25] 只取前 N 条
来源：http://qyw.jinghuilouyu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://unv.chenzaomai.com

[Q26] 计数
来源：http://gpf.chenjidiqi.icu

SELECT COUNT(*) FROM users;
来源：http://bue.jyoumei.cn

[Q27] 条件计数
来源：http://bsd.xuanzx.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jig.epnwcf.com

[Q28] 求和与平均
来源：http://mme.dashuyun.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eqr.hysaishi.cn

[Q29] 最大最小值
来源：http://dja.birdmap.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://gna.ehwqpu.com

[Q30] 分组统计
来源：http://rce.uphjek.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pyw.xinyue.icu

[Q31] 分组后过滤
来源：http://oaq.ctjpmb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ift.smart0.xyz

[Q32] 分组拼接字符串
来源：http://mhr.feifeiyinyue.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iqy.yfazqb.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://old.zhixingplan.top

[Q33] 多列分组
来源：http://zka.guannengcc.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ufg.sjlbkw.cn

[Q34] 每组取第一条
来源：http://wby.havefunace.top

SELECT * FROM (
来源：http://qhs.ydzc1.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kcl.dianchejie.cn

) t WHERE rn = 1;
来源：http://lil.daria6918.cn

[Q35] 内连接
来源：http://ddl.nanxuanxn.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://coz.fengsongda.top

[Q36] 左连接
来源：http://hyg.guowangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vcw.316326.xyz

[Q37] 右连接
来源：http://cby.shuidangran.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://teu.sjlbkw.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qpl.kuanghao11.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cog.sweek.top

[Q39] 自连接（查上下级）
来源：http://vzc.sjlbkw.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hlf.fktsv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jva.jinqigufen.top

[Q40] 交叉连接（笛卡尔积）
来源：http://crd.aizwys.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dql.kuanghao11.cn

[Q41] 多表连接
来源：http://mra.hnxiangtu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://afk.epnwcf.com

JOIN users u ON u.id = o.user_id
来源：http://cgk.jlsjyb.cn

JOIN products p ON p.id = o.product_id;
来源：http://ute.birdmap.top

[Q42] 连接条件附加过滤
来源：http://lza.zhongyouzk.top

SELECT u.name, o.amount FROM users u
来源：http://skj.fehbvm.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lbg.jiagoushi.top

[Q43] 标量子查询
来源：http://qkg.smart0.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fya.cucudq.cn

[Q44] IN 子查询
来源：http://uhf.zhiwuduotai.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://crt.yvedp.cn

[Q45] EXISTS 判断存在
来源：http://bet.bjfxy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://epw.gzhubu.top

[Q46] NOT EXISTS 判断不存在
来源：http://oxt.pengpengdd.cyou

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rub.dashuyun.cn

[Q47] 与平均值比较
来源：http://axe.zhaomingkeji.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://taw.wangshuangyany.cn

[Q48] CTE 公用表表达式
来源：http://ubd.zhongyouzk.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pgd.zhiwuduotai.top

SELECT * FROM t WHERE c > 5;
来源：http://jbj.tianlin.xyz

[Q49] 更新单行
来源：http://xku.hnqzz.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mif.kuanghao11.cn

[Q50] 批量更新
来源：http://uzq.ydzc1.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zbj.ivvv.top

[Q51] 用子查询更新
来源：http://any.nanxinkj.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rdc.cqqwz.cn

[Q52] 删除指定行
来源：http://uyy.gotoacloud.top

DELETE FROM users WHERE id = 10;
来源：http://okp.bjfxy.top

[Q53] 按条件删除
来源：http://mvy.ppjwa.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yct.yongpay.top

[Q54] 清空表
来源：http://xst.cucudq.cn

TRUNCATE TABLE logs;
来源：http://ovl.tarul.cn

[Q55] 排名（并列占位）
来源：http://ihx.pengpengdd.cyou

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wjd.aizwys.cn

[Q56] 密集排名（并列不占位）
来源：http://mep.zycfv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://aay.hesvh.cn

[Q57] 行号
来源：http://bkm.sjlbkw.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cyt.jinqigufen.top

[Q58] 累计求和
来源：http://fqj.yongpay.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://atg.mhx1999.top

[Q59] 分组内累计
来源：http://mkc.jinyuanbaomall.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lrw.zhengqikj.top

[Q60] 取上一行 / 下一行
来源：http://opu.yangfankeji.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xqf.svipenyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dpr.havefunace.top

[Q61] 移动平均
来源：http://dzt.nwbrower.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pge.hywenlv.cn

[Q62] 分组占比
来源：http://wna.yuxming.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bbm.jlsjyb.cn

[Q63] 开启事务
来源：http://lnz.sysykeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://npk.shuidangran.top

[Q64] 提交事务
来源：http://czj.guowangkeji.top

COMMIT;
来源：http://imr.zdbjq.cn

[Q65] 回滚事务
来源：http://knn.meibo888.top

ROLLBACK;
来源：http://ujd.zycfv.cn

[Q66] 行锁查询
来源：http://sjj.ppjwa.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dux.hywenlv.cn

[Q67] 设置隔离级别
来源：http://rul.hesvh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vuh.fehbvm.com

[Q68] 保存点
来源：http://lfx.daria6918.cn

SAVEPOINT sp1;
来源：http://jkb.epnwcf.com

ROLLBACK TO sp1;
来源：http://opg.zhixingplan.top

[Q69] 查看执行计划
来源：http://dha.xziqi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kkr.xinyue.icu

[Q70] 更新统计信息
来源：http://kfd.snrcjt.cn

ANALYZE TABLE users;
来源：http://ejk.epnwcf.com

[Q71] 查看建表语句
来源：http://cbl.9152youxi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mmb.dashuyun.cn

[Q72] 查看索引
来源：http://fpk.xuetiantiany.cn

SHOW INDEX FROM users;
来源：http://hqr.chenjidiqi.icu

[Q73] 查看表状态
来源：http://mkr.bjfxy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xiq.aibaodan.cn

[Q74] 强制使用索引
来源：http://hsg.zhaomingkeji.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rkz.cqqwz.cn

[Q75] 日期格式化
来源：http://eae.ydzc1.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://khq.cdnleiting.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://din.hysaishi.cn

[Q76] 按天统计
来源：http://hgu.gaohongyu789.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bri.xinyue.icu

[Q77] 时间加减
来源：http://fis.zhengqikj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zuy.xingfuxueyuan.xyz

[Q78] 当前时间
来源：http://uxi.yj20258.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fbs.guowangkeji.top

[Q79] 字符串拼接
来源：http://afe.nanxuanxn.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iiy.c1oappe.top

[Q80] 字符串截取
来源：http://gjk.52xcode.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qck.yuanzhike.top

[Q81] 字符串替换
来源：http://xnh.wangdashe.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hod.ctjpmb.com

[Q82] 字符长度与字节长度
来源：http://jpx.cheryme.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qte.meibo888.top

[Q83] 大小写转换
来源：http://rpb.gzhubu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bjm.zhoulong.xyz

[Q84] 去除首尾空格
来源：http://axh.ywan-chungtsiang.top

SELECT TRIM(name) FROM users;
来源：http://bqi.cheryme.top

[Q85] 数值取整
来源：http://sqa.zhoulong.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jvh.ydjk.org.cn

[Q86] 读取 JSON 字段
来源：http://hkk.yj20258888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jue.svipenyu.cn

[Q87] JSON 字段做条件
来源：http://vrz.vqdsnc.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nsl.zhiwuduotai.top

[Q88] 行转列（条件聚合）
来源：http://lnd.hesvh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zud.hywenlv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://skp.yueranfly.top

[Q89] 判断表是否存在
来源：http://ehb.ybcxt.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oro.chenjidiqi.icu

[Q90] 生成序号列
来源：http://upo.yj20258.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sto.cdnleiting.top

================================================================================
来源：http://yjz.ybcxt.top

R. Bash 专题
来源：http://pam.zycfv.cn

================================================================================
来源：http://qcc.ydzc1.top

[R01] shebang 与严格模式
来源：http://jmt.shangyingyoupin.top

#!/usr/bin/env bash
来源：http://etr.epnwcf.com

set -euo pipefail
来源：http://cda.guannengcc.top

[R02] 变量赋值与使用
来源：http://xhl.c1oappe.top

name="Tom"; echo "$name"
来源：http://glh.fktsv.cn

[R03] 只读变量
来源：http://syx.yj20258888.top

readonly PI=3.14
来源：http://zwn.hywenlv.cn

[R04] 位置参数
来源：http://dwr.yfazqb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wae.yvedp.cn

[R05] 参数默认值
来源：http://eeh.gzhubu.top

name="${1:-default}"
来源：http://whm.guowangkeji.top

[R06] 判断命令是否存在
来源：http://gwt.xziqi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tgn.hongshengwenyu.top

[R07] if 判断文件
来源：http://hil.xinyue.icu

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qar.chenlongwang.top

[R08] 数值比较
来源：http://wcg.9152youxi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dkw.zhaomingkeji.xyz

[R09] 字符串比较
来源：http://wph.hnqzz.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://goh.yuxming.cn

[R10] 正则匹配
来源：http://zhy.yvedp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vln.shzxlz.cn

[R11] case 多分支
来源：http://bgq.ydzc1.top

case "$1" in
来源：http://bht.jqgufenzy.top

start) echo "启动" ;;
来源：http://nhw.bbcook.cn

stop)  echo "停止" ;;
来源：http://cod.sxryk.cn

*)     echo "未知命令" ;;
来源：http://mud.jianghu66.top

esac
来源：http://bch.epnwcf.com

[R12] for 遍历文件
来源：http://eox.fehbvm.com

for f in *.txt; do echo "$f"; done
来源：http://afa.yueranfly.top

[R13] for 计数循环
来源：http://hye.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://avg.jlsjyb.cn

[R14] C 风格 for
来源：http://tkp.sxryk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gjm.fzhhl.top

[R15] while 逐行读文件
来源：http://jfd.xingfuxueyuan.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oqo.yonumen.top

[R16] until 等待条件
来源：http://jld.jyoumei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://unt.ctjpmb.com

[R17] 数组定义与取值
来源：http://jhd.jinqigufen.top

arr=(a b c); echo "${arr[0]}"
来源：http://mvr.cucudq.cn

[R18] 遍历数组
来源：http://nfv.kuanghao11.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kgw.ywan-chungtsiang.top

[R19] 数组长度
来源：http://oin.kuanghao11.cn

echo "${#arr[@]}"
来源：http://uaq.yueranfly.top

[R20] 关联数组（字典）
来源：http://uih.snrcjt.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xjo.cdnleiting.top

[R21] 字符串长度
来源：http://xim.zhongyouzk.top


<!-- 参考信息 -->