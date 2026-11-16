代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aew.jinqigfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mwi.tianlin.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wmg.yuanzhike.top

[P04] 求长度
来源：http://wjr.fengsongda.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rkj.bjfxy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ups.jinghuilouyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nks.fktsv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tod.jinqigufen.top

Java: list.size();  map.size();  s.length()
来源：http://ygm.ybcxt.top

Go:   len(arr);  len(m)
来源：http://sfu.ppjwa.cn

Ruby: x.length;  x.size
来源：http://fpq.daxiang520.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wwj.vehdjk.com

[P05] 判断两个对象内容是否相等
来源：http://eiq.gzhubu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://bxl.xylfe.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wml.ydjk.org.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ysd.fengsongda.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qgl.sxryk.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qka.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://hap.gaohongyu789.top

Ruby: a == b
来源：http://tol.zhoulong.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wca.gzhubu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://faf.cucudq.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ote.jinqigufen.top

PHP:  if (empty($x)) {}
来源：http://abs.jqgufenzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mdn.sjlbkw.cn

TS:   if (x == null) {}
来源：http://ocw.yj20258888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://bhr.zhoulong.xyz

Go:   if x == nil {}
来源：http://wzl.gogol.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cyw.nwbrower.top

C#:   if (x is null) {}
来源：http://qhl.tian-w.cn

[P07] 防抖与节流
来源：http://cpt.zdbjq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sst.yangfankeji.com

PHP:  // 手写时间戳比较
来源：http://sea.jiagoushi.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://elr.sufxvd.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lrt.daxiang520.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qou.dianchejie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pcm.xingfuxueyuan.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://gwb.yangfankeji.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fxh.daria6918.cn

[P08] 处理浮点精度问题
来源：http://wnb.dashuyun.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yqe.epnwcf.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hku.aibaodan.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lcq.xinyue.icu

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dob.kuanghao11.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ljb.c1oappe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bic.redwolf501.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://att.52xcode.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wtc.birdmap.top

================================================================================
来源：http://oje.redwolf501.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mui.vqdsnc.cn

================================================================================
来源：http://edy.0kj1m.cn

[Q01] 创建表
来源：http://naw.havefunace.top

CREATE TABLE users (
来源：http://mrd.chenzaomai.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yxk.fzhhl.top

name VARCHAR(50) NOT NULL,
来源：http://heo.hongshengwenyu.top

email VARCHAR(100) UNIQUE,
来源：http://zif.shanyushiyangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qjv.hcnkem.com

);
来源：http://upv.yj20258.top

[Q02] 创建带外键的表
来源：http://cac.yanxiufei.cn

CREATE TABLE orders (
来源：http://aco.xuanzx.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://urn.zhengqikj.top

user_id INT NOT NULL,
来源：http://atn.zhoulong.xyz

amount DECIMAL(10, 2),
来源：http://nly.dianchejie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ygt.cucudq.cn

);
来源：http://xzj.wangdashe.top

[Q03] 增加列
来源：http://tub.chenlongwang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ikv.c1oappe.top

[Q04] 修改列类型
来源：http://cqn.andypj.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kzq.ydjk.org.cn

[Q05] 重命名列
来源：http://cpu.sxryk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jad.xingfuxueyuan.xyz

[Q06] 删除列
来源：http://dnl.quarkkingdee.top

ALTER TABLE users DROP COLUMN age;
来源：http://aqe.yanxiufei.cn

[Q07] 删除表
来源：http://ewq.quarkkingdee.top

DROP TABLE IF EXISTS orders;
来源：http://yld.snrcjt.cn

[Q08] 创建普通索引
来源：http://cxr.uphjek.com

CREATE INDEX idx_users_email ON users(email);
来源：http://hhv.xuetiantiany.cn

[Q09] 创建唯一索引
来源：http://jqw.pycfn.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bub.xuetiantiany.cn

[Q10] 插入单行
来源：http://swq.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vln.fehbvm.com

[Q11] 一次插入多行
来源：http://wdd.316326.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iin.jinqigufen.top

[Q12] 插入后取自增 ID
来源：http://qyr.chenlongwang.top

INSERT INTO users (name) VALUES ('C');
来源：http://ovv.jqgfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jkc.shangyingyoupin.top

[Q13] 忽略重复插入
来源：http://wkw.yuanzhike.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oax.chenlongwang.top

[Q14] 存在则更新（upsert）
来源：http://fwi.haohaochexian.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xeu.shanyushiyangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cev.zhengqikj.top

[Q15] 查询全部
来源：http://hoj.smart0.xyz

SELECT * FROM users;
来源：http://nhy.zhongyouzk.top

[Q16] 查询指定列
来源：http://hru.shzxlz.cn

SELECT id, name FROM users;
来源：http://mpi.ybcxt.top

[Q17] 条件查询
来源：http://bfr.tanke756.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jmb.feifeiyinyue.top

[Q18] 模糊匹配
来源：http://vcw.xuanzx.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zwj.52xcode.cn

[Q19] 范围查询
来源：http://rhs.ywan-chungtsiang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xpo.dianchejie.cn

[Q20] IN 列表
来源：http://oty.yangfankeji.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nig.jlsjyb.cn

[Q21] 空值判断
来源：http://bjd.fehbvm.com

SELECT * FROM users WHERE email IS NULL;
来源：http://bwi.zhixingplan.top

[Q22] 排序
来源：http://imi.svipenyu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zba.jyoumei.cn

[Q23] 分页
来源：http://asu.meibo888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uwm.daria6918.cn

[Q24] 去重
来源：http://lpr.zycfv.cn

SELECT DISTINCT city FROM users;
来源：http://gxc.tian-w.cn

[Q25] 只取前 N 条
来源：http://mws.cdnleiting.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qbt.zhengqikj.top

[Q26] 计数
来源：http://yla.ybcxt.top

SELECT COUNT(*) FROM users;
来源：http://gsb.zhijiandao.cn

[Q27] 条件计数
来源：http://aro.xinyue.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gaz.jinqigufen.top

[Q28] 求和与平均
来源：http://won.dianchejie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xxk.havefunace.top

[Q29] 最大最小值
来源：http://xov.meibo888.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yqa.yj20258.top

[Q30] 分组统计
来源：http://bol.xziqi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zzb.birdmap.top

[Q31] 分组后过滤
来源：http://mzb.zhixingplan.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://got.nanxuanxn.top

[Q32] 分组拼接字符串
来源：http://mwj.smart0.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hhi.andypj.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ppd.sweek.top

[Q33] 多列分组
来源：http://ydb.yanxiufei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ygf.bbcook.cn

[Q34] 每组取第一条
来源：http://gvx.hesvh.cn

SELECT * FROM (
来源：http://qbh.xziqi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lme.xziqi.cn

) t WHERE rn = 1;
来源：http://zcd.yuanzhike.top

[Q35] 内连接
来源：http://efq.ppjwa.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mei.fehbvm.com

[Q36] 左连接
来源：http://kyr.cheryme.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kal.yj20258.top

[Q37] 右连接
来源：http://fee.mhx1999.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zbq.tianlin.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://wpn.bjfxy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qmm.birdmap.top

[Q39] 自连接（查上下级）
来源：http://ujj.xuanzx.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://xsr.aizwys.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fvc.redwolf501.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ujn.dianchejie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cdg.jinyuanbaomall.cn

[Q41] 多表连接
来源：http://dcp.jlsjyb.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://thx.snrcjt.cn

JOIN users u ON u.id = o.user_id
来源：http://uil.nwbrower.top

JOIN products p ON p.id = o.product_id;
来源：http://fmv.ctjpmb.com

[Q42] 连接条件附加过滤
来源：http://cdr.hnxiangtu.top

SELECT u.name, o.amount FROM users u
来源：http://pok.redwolf501.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://maf.zhixingplan.top

[Q43] 标量子查询
来源：http://edx.smart0.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ehk.zycfv.cn

[Q44] IN 子查询
来源：http://rio.dashuyun.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jdg.gaohongyu789.top

[Q45] EXISTS 判断存在
来源：http://pmy.ybcxt.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oqt.jinqigfzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://ccb.bjfxy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://stt.fktsv.cn

[Q47] 与平均值比较
来源：http://lox.guannengcc.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://djt.bbcook.cn

[Q48] CTE 公用表表达式
来源：http://avl.zycfv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cyi.guannengcc.top

SELECT * FROM t WHERE c > 5;
来源：http://xrj.shzxlz.cn

[Q49] 更新单行
来源：http://mel.yuxming.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://skn.shanyushiyangkeji.top

[Q50] 批量更新
来源：http://kpn.zhoulong.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cpz.yanxiufei.cn

[Q51] 用子查询更新
来源：http://bhd.fzhhl.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mqd.sjlbkw.cn

[Q52] 删除指定行
来源：http://gex.tanke756.top

DELETE FROM users WHERE id = 10;
来源：http://mwe.ctjpmb.com

[Q53] 按条件删除
来源：http://nls.fehbvm.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fer.hongshengwenyu.top

[Q54] 清空表
来源：http://npi.redwolf501.top

TRUNCATE TABLE logs;
来源：http://tng.jqgufenzy.top

[Q55] 排名（并列占位）
来源：http://fpa.hesvh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mye.gaohongyu789.top

[Q56] 密集排名（并列不占位）
来源：http://hau.birdmap.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://onr.chenzaomai.com

[Q57] 行号
来源：http://mta.yueranfly.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vxw.hcnkem.com

[Q58] 累计求和
来源：http://kwb.gotoacloud.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yry.xylfe.cn

[Q59] 分组内累计
来源：http://iib.zhoulong.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dix.jiagoushi.top

[Q60] 取上一行 / 下一行
来源：http://bwr.tian-w.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lvm.yj202588.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ayw.jinqigfzy.top

[Q61] 移动平均
来源：http://nzm.xuanzx.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ghf.jinqigfzy.top

[Q62] 分组占比
来源：http://dsw.shanyushiyangtech.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lgw.hnxiangtu.top

[Q63] 开启事务
来源：http://cys.sufxvd.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mox.ybcxt.top

[Q64] 提交事务
来源：http://gbu.cdnleiting.top

COMMIT;
来源：http://lnk.fehbvm.com

[Q65] 回滚事务
来源：http://ztp.hnqzz.top

ROLLBACK;
来源：http://uxk.nwbrower.top

[Q66] 行锁查询
来源：http://deg.gzhubu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://psf.birdmap.top

[Q67] 设置隔离级别
来源：http://xiq.xuetiantiany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://odd.jianghu66.top

[Q68] 保存点
来源：http://flx.hammf.cn

SAVEPOINT sp1;
来源：http://coa.shangyingyoupin.top

ROLLBACK TO sp1;
来源：http://sjy.aibaodan.cn

[Q69] 查看执行计划
来源：http://ruf.jqgfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lot.hammf.cn

[Q70] 更新统计信息
来源：http://ytu.hesvh.cn

ANALYZE TABLE users;
来源：http://pwf.jqgufenzy.top

[Q71] 查看建表语句
来源：http://epi.havefunace.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rsk.xuetiantiany.cn

[Q72] 查看索引
来源：http://ezs.fzhhl.top

SHOW INDEX FROM users;
来源：http://rwn.jiagoushi.top

[Q73] 查看表状态
来源：http://yvc.jinghuilouyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uod.dianchejie.cn

[Q74] 强制使用索引
来源：http://nhb.pengpengdd.cyou

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uje.cqqwz.cn

[Q75] 日期格式化
来源：http://rkh.jinqigfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ksf.nanxuanxn.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dpq.dianchejie.cn

[Q76] 按天统计
来源：http://ezq.aibaodan.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yhj.jqgufenzy.top

[Q77] 时间加减
来源：http://lgc.mhx1999.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://exg.aibaodan.cn

[Q78] 当前时间
来源：http://rnx.zdqjudy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jap.chenjidiqi.icu

[Q79] 字符串拼接
来源：http://ktk.jinyuanbaomall.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mtb.aibaodan.cn

[Q80] 字符串截取
来源：http://pqr.gogol.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cic.sweek.top

[Q81] 字符串替换
来源：http://bem.tian-w.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pvh.hywenlv.cn

[Q82] 字符长度与字节长度
来源：http://afm.hywenlv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://itm.sxryk.cn

[Q83] 大小写转换
来源：http://txc.jinqigfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://svr.epnwcf.com

[Q84] 去除首尾空格
来源：http://bwl.bjfxy.top

SELECT TRIM(name) FROM users;
来源：http://lku.xziqi.cn

[Q85] 数值取整
来源：http://csn.52xcode.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tsj.ydzc1.top

[Q86] 读取 JSON 字段
来源：http://thd.birdmap.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://umv.jinqigufen.top

[Q87] JSON 字段做条件
来源：http://czn.aibaodan.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mcy.9152youxi.cn

[Q88] 行转列（条件聚合）
来源：http://vst.feifeiyinyue.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://asv.epnwcf.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rgs.hesvh.cn

[Q89] 判断表是否存在
来源：http://hmz.daria6918.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pwb.yongpay.top

[Q90] 生成序号列
来源：http://iks.havefunace.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zxn.redwolf501.top

================================================================================
来源：http://zpd.0kj1m.cn

R. Bash 专题
来源：http://cgr.zhiwuduotai.top

================================================================================
来源：http://hwg.hesvh.cn

[R01] shebang 与严格模式
来源：http://tol.jinqigufen.top

#!/usr/bin/env bash
来源：http://umc.tianlin.xyz

set -euo pipefail
来源：http://ksb.xinyue.icu

[R02] 变量赋值与使用
来源：http://rch.cqqwz.cn

name="Tom"; echo "$name"
来源：http://hen.birdmap.top

[R03] 只读变量
来源：http://hwt.yvedp.cn

readonly PI=3.14
来源：http://drz.shangyingyoupin.top

[R04] 位置参数
来源：http://usi.xinyue.icu

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cwe.aizwys.cn

[R05] 参数默认值
来源：http://ezl.svipenyu.cn

name="${1:-default}"
来源：http://ssh.zdqjudy.top

[R06] 判断命令是否存在
来源：http://nlj.ybcxt.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vvd.smart0.xyz

[R07] if 判断文件
来源：http://sxn.mhx1999.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jsm.gaohongyu789.top

[R08] 数值比较
来源：http://dug.xziqi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uds.smart0.xyz

[R09] 字符串比较
来源：http://wdg.tianlin.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://omo.xuanzx.com

[R10] 正则匹配
来源：http://iqe.hnqzz.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uvb.zhixingplan.top

[R11] case 多分支
来源：http://ame.feifeiyinyue.top

case "$1" in
来源：http://txo.ppjwa.cn

start) echo "启动" ;;
来源：http://jyo.guowangkeji.top

stop)  echo "停止" ;;
来源：http://vwu.pycfn.com

*)     echo "未知命令" ;;
来源：http://tln.zhiwuduotai.top

esac
来源：http://tmb.xziqi.cn

[R12] for 遍历文件
来源：http://xnr.jinqigufen.top

for f in *.txt; do echo "$f"; done
来源：http://zkr.gaohongyu789.top

[R13] for 计数循环
来源：http://vmt.daria6918.cn

for i in {1..10}; do echo "$i"; done
来源：http://wgn.tanke756.top

[R14] C 风格 for
来源：http://lfw.yj20258.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cie.gogol.net.cn

[R15] while 逐行读文件
来源：http://eph.pycfn.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ujz.xingfuxueyuan.xyz

[R16] until 等待条件
来源：http://kld.andypj.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jtr.gaohongyu789.top

[R17] 数组定义与取值
来源：http://rbt.bjfxy.top

arr=(a b c); echo "${arr[0]}"
来源：http://llk.fktsv.cn

[R18] 遍历数组
来源：http://upb.hongshengwenyu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jro.shzxlz.cn

[R19] 数组长度
来源：http://mdi.smart0.xyz


<!-- 参考信息 -->