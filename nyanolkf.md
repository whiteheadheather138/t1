代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wzz.ydzc1.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lnu.xingfuxueyuan.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uys.snrcjt.cn

[P04] 求长度
来源：http://maj.dianchejie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mzj.chenjidiqi.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://txg.fzhhl.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qxm.hnqzz.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xri.redwolf501.top

Java: list.size();  map.size();  s.length()
来源：http://ccb.zhengqikj.top

Go:   len(arr);  len(m)
来源：http://fxl.xuanzx.com

Ruby: x.length;  x.size
来源：http://rmj.yuanzhike.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rmy.sweek.top

[P05] 判断两个对象内容是否相等
来源：http://emw.meibo888.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://cre.ivvv.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qcm.zhaomingkeji.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hdm.hnxiangtu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tgc.uphjek.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pzc.jqgfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://qgq.bbcook.cn

Ruby: a == b
来源：http://jrs.fehbvm.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yjy.fanxiaobao.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hmo.fehbvm.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nql.nanxinkj.top

PHP:  if (empty($x)) {}
来源：http://lzk.fehbvm.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fwp.yj202588.top

TS:   if (x == null) {}
来源：http://qwx.ctjpmb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://cmp.jqgufenzy.top

Go:   if x == nil {}
来源：http://krm.fengsongda.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eyy.zhoulong.xyz

C#:   if (x is null) {}
来源：http://svt.zdbjq.cn

[P07] 防抖与节流
来源：http://fby.hnqzz.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jnw.fengsongda.top

PHP:  // 手写时间戳比较
来源：http://ugf.hongshengwenyu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fqn.yj20258888.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zlt.haohaochexian.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ypc.fktsv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bkx.sjlbkw.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://skx.chenzaomai.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ljw.guannengcc.top

[P08] 处理浮点精度问题
来源：http://ohw.xingfuxueyuan.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qgb.shuidangran.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xnm.shangyingyoupin.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ytl.zhoulong.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://omr.dianchejie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yhv.xuanzx.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yex.pengpengdd.cyou

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xeo.jinqigfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wnr.fanxiaobao.xyz

================================================================================
来源：http://qpm.yj202588.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bkm.ybcxt.top

================================================================================
来源：http://xdj.haohaochexian.top

[Q01] 创建表
来源：http://xnp.ehwqpu.com

CREATE TABLE users (
来源：http://vss.yuxming.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uio.xuanzx.com

name VARCHAR(50) NOT NULL,
来源：http://iax.uphjek.com

email VARCHAR(100) UNIQUE,
来源：http://qvb.quarkkingdee.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ymj.ppjwa.cn

);
来源：http://dhc.pycfn.com

[Q02] 创建带外键的表
来源：http://lck.sweek.top

CREATE TABLE orders (
来源：http://nam.fehbvm.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uny.uphjek.com

user_id INT NOT NULL,
来源：http://adw.hesvh.cn

amount DECIMAL(10, 2),
来源：http://hgk.c1oappe.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pqv.vqdsnc.cn

);
来源：http://thl.c1oappe.top

[Q03] 增加列
来源：http://uyi.cucudq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uzv.dianchejie.cn

[Q04] 修改列类型
来源：http://acz.ppjwa.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hjp.birdmap.top

[Q05] 重命名列
来源：http://opg.9152youxi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jck.aizwys.cn

[Q06] 删除列
来源：http://ieo.zhixingplan.top

ALTER TABLE users DROP COLUMN age;
来源：http://hza.fktsv.cn

[Q07] 删除表
来源：http://hux.havefunace.top

DROP TABLE IF EXISTS orders;
来源：http://ztm.epnwcf.com

[Q08] 创建普通索引
来源：http://zig.zhengqikj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fbf.haohaochexian.top

[Q09] 创建唯一索引
来源：http://edz.iojbl.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mvq.chenlongwang.top

[Q10] 插入单行
来源：http://nnz.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xvi.0kj1m.cn

[Q11] 一次插入多行
来源：http://pfa.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://spk.daria6918.cn

[Q12] 插入后取自增 ID
来源：http://pge.ppjwa.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xwt.chenjidiqi.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qia.gogol.net.cn

[Q13] 忽略重复插入
来源：http://qta.jinqigufen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iyg.guannengcc.top

[Q14] 存在则更新（upsert）
来源：http://dgt.jqgfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rtc.hywenlv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mwh.hysaishi.cn

[Q15] 查询全部
来源：http://iyh.cheryme.top

SELECT * FROM users;
来源：http://gwx.cheryme.top

[Q16] 查询指定列
来源：http://pov.cheryme.top

SELECT id, name FROM users;
来源：http://oxq.yongpay.top

[Q17] 条件查询
来源：http://wvj.yvedp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xtl.xingfuxueyuan.xyz

[Q18] 模糊匹配
来源：http://nzs.xinyue.icu

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xet.gzhubu.top

[Q19] 范围查询
来源：http://zha.pengpengdd.cyou

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dsh.jqgfzy.top

[Q20] IN 列表
来源：http://jff.cucudq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://evw.gotoacloud.top

[Q21] 空值判断
来源：http://ndl.9152youxi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jyt.tarul.cn

[Q22] 排序
来源：http://vxh.chenjidiqi.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yjc.nwbrower.top

[Q23] 分页
来源：http://biv.pengpengdd.cyou

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lmk.fanxiaobao.xyz

[Q24] 去重
来源：http://xxz.fengsongda.top

SELECT DISTINCT city FROM users;
来源：http://jdy.xinyue.icu

[Q25] 只取前 N 条
来源：http://cvm.shuidangran.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xhc.sxryk.cn

[Q26] 计数
来源：http://uss.zhixingplan.top

SELECT COUNT(*) FROM users;
来源：http://ckq.c1oappe.top

[Q27] 条件计数
来源：http://ioj.daria6918.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vby.guowangkeji.top

[Q28] 求和与平均
来源：http://nkt.tarul.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cil.zhengqikj.top

[Q29] 最大最小值
来源：http://unf.shuidangran.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://nej.pengpengdd.cyou

[Q30] 分组统计
来源：http://sfh.yj20258888.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zrs.aibaodan.cn

[Q31] 分组后过滤
来源：http://oih.shanyushiyangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zct.jqgufenzy.top

[Q32] 分组拼接字符串
来源：http://txi.zhoulong.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://otk.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nzt.svipenyu.cn

[Q33] 多列分组
来源：http://ebp.jlsjyb.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gtt.fengsongda.top

[Q34] 每组取第一条
来源：http://dnc.zhengqikj.top

SELECT * FROM (
来源：http://tzj.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://swt.zhengqikj.top

) t WHERE rn = 1;
来源：http://wlp.chenzaomai.com

[Q35] 内连接
来源：http://lkj.hcnkem.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mub.smart0.xyz

[Q36] 左连接
来源：http://izk.jianghu66.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://twt.zhiwuduotai.top

[Q37] 右连接
来源：http://qkf.vqdsnc.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ctg.cucudq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rbl.jiagoushi.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xhk.ivvv.top

[Q39] 自连接（查上下级）
来源：http://yph.zhoulong.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://iuw.ywan-chungtsiang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oyh.uphjek.com

[Q40] 交叉连接（笛卡尔积）
来源：http://ske.guowangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uey.nwbrower.top

[Q41] 多表连接
来源：http://ghe.smart0.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://yzy.nanxinkj.top

JOIN users u ON u.id = o.user_id
来源：http://haa.sweek.top

JOIN products p ON p.id = o.product_id;
来源：http://ldd.cheryme.top

[Q42] 连接条件附加过滤
来源：http://qxa.guowangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://odx.xuetiantiany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vuv.jqgufenzy.top

[Q43] 标量子查询
来源：http://euf.hywenlv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mng.hammf.cn

[Q44] IN 子查询
来源：http://xak.yuxming.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://aqn.shuidangran.top

[Q45] EXISTS 判断存在
来源：http://ugs.ivvv.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wne.gzhubu.top

[Q46] NOT EXISTS 判断不存在
来源：http://ygj.daxiang520.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eaw.birdmap.top

[Q47] 与平均值比较
来源：http://kde.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nmh.vqdsnc.cn

[Q48] CTE 公用表表达式
来源：http://ndx.zhoulong.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ajd.uphjek.com

SELECT * FROM t WHERE c > 5;
来源：http://vfi.xuetiantiany.cn

[Q49] 更新单行
来源：http://alf.zdqjudy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://epe.zdbjq.cn

[Q50] 批量更新
来源：http://mis.zhoulong.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jdy.yuxming.cn

[Q51] 用子查询更新
来源：http://mrq.birdmap.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kuk.zhiwuduotai.top

[Q52] 删除指定行
来源：http://epb.haohaochexian.top

DELETE FROM users WHERE id = 10;
来源：http://adp.yongpay.top

[Q53] 按条件删除
来源：http://pgj.chenjidiqi.icu

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zxb.sjlbkw.cn

[Q54] 清空表
来源：http://uyy.jinyuanbaomall.cn

TRUNCATE TABLE logs;
来源：http://udv.hammf.cn

[Q55] 排名（并列占位）
来源：http://iii.zhaomingkeji.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bat.nanxinkj.top

[Q56] 密集排名（并列不占位）
来源：http://ksi.sxryk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kgu.tian-w.cn

[Q57] 行号
来源：http://slh.ybcxt.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ffn.feifeiyinyue.top

[Q58] 累计求和
来源：http://aaf.0kj1m.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wqo.gogol.net.cn

[Q59] 分组内累计
来源：http://xdb.mhx1999.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xqm.nanxuanxn.top

[Q60] 取上一行 / 下一行
来源：http://rin.gogol.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jct.0kj1m.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qgg.xylfe.cn

[Q61] 移动平均
来源：http://kid.316326.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ats.nanxuanxn.top

[Q62] 分组占比
来源：http://vky.vehdjk.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bgw.chenzaomai.com

[Q63] 开启事务
来源：http://vfj.zhijiandao.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fwm.zhengqikj.top

[Q64] 提交事务
来源：http://urj.tian-w.cn

COMMIT;
来源：http://nyk.wangshuangyany.cn

[Q65] 回滚事务
来源：http://tgz.hesvh.cn

ROLLBACK;
来源：http://pls.xziqi.cn

[Q66] 行锁查询
来源：http://dwj.xinyue.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sgf.sweek.top

[Q67] 设置隔离级别
来源：http://unk.ybcxt.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cej.shzxlz.cn

[Q68] 保存点
来源：http://wdv.nanxinkj.top

SAVEPOINT sp1;
来源：http://ckm.sxryk.cn

ROLLBACK TO sp1;
来源：http://iap.zdqjudy.top

[Q69] 查看执行计划
来源：http://hmz.9152youxi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fmy.mhx1999.top

[Q70] 更新统计信息
来源：http://qlg.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://jln.smart0.xyz

[Q71] 查看建表语句
来源：http://udh.zhoulong.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://giu.hnqzz.top

[Q72] 查看索引
来源：http://ujv.yuxming.cn

SHOW INDEX FROM users;
来源：http://edr.xylfe.cn

[Q73] 查看表状态
来源：http://tpw.shanyushiyangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://upb.nanxinkj.top

[Q74] 强制使用索引
来源：http://nve.cdnleiting.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://srd.hfpthk.cn

[Q75] 日期格式化
来源：http://mtj.xylfe.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nwl.xziqi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ljm.hesvh.cn

[Q76] 按天统计
来源：http://ioq.dashuyun.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jwg.birdmap.top

[Q77] 时间加减
来源：http://cdn.zhixingplan.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nll.jiagoushi.top

[Q78] 当前时间
来源：http://vay.snrcjt.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wwi.fzhhl.top

[Q79] 字符串拼接
来源：http://hdl.aibaodan.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vdp.haohaochexian.top

[Q80] 字符串截取
来源：http://axn.jiagoushi.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uxz.ppjwa.cn

[Q81] 字符串替换
来源：http://zyb.tanke756.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mzq.kuanghao11.cn

[Q82] 字符长度与字节长度
来源：http://dnt.jinqigfzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jnd.hongshengwenyu.top

[Q83] 大小写转换
来源：http://wjc.shuidangran.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mfp.yj20258.top

[Q84] 去除首尾空格
来源：http://sis.svipenyu.cn

SELECT TRIM(name) FROM users;
来源：http://oyw.hcnkem.com

[Q85] 数值取整
来源：http://szk.cdnleiting.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ysi.yfazqb.com

[Q86] 读取 JSON 字段
来源：http://bln.hywenlv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rja.yvedp.cn

[Q87] JSON 字段做条件
来源：http://yik.smart0.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mbq.kuanghao11.cn

[Q88] 行转列（条件聚合）
来源：http://gni.c1oappe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lfd.ydjk.org.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zzg.ywan-chungtsiang.top

[Q89] 判断表是否存在
来源：http://uey.jinghuilouyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tcq.snrcjt.cn

[Q90] 生成序号列
来源：http://aft.bbcook.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ufg.svipenyu.cn

================================================================================
来源：http://crv.shanyushiyangkeji.top

R. Bash 专题
来源：http://kqp.hongshengwenyu.top

================================================================================
来源：http://aue.yangfankeji.com

[R01] shebang 与严格模式
来源：http://qoc.hesvh.cn

#!/usr/bin/env bash
来源：http://wva.tian-w.cn

set -euo pipefail
来源：http://qbn.hywenlv.cn

[R02] 变量赋值与使用
来源：http://tfv.hesvh.cn

name="Tom"; echo "$name"
来源：http://ugq.ywan-chungtsiang.top

[R03] 只读变量
来源：http://dyv.fehbvm.com

readonly PI=3.14
来源：http://cfu.chenzaomai.com

[R04] 位置参数
来源：http://sui.ybcxt.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yfj.fzhhl.top

[R05] 参数默认值
来源：http://nbp.smart0.xyz

name="${1:-default}"
来源：http://wkb.hnqzz.top

[R06] 判断命令是否存在
来源：http://ajg.zhoulong.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jfm.fanxiaobao.xyz

[R07] if 判断文件
来源：http://saz.chenjidiqi.icu

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yjs.guannengcc.top

[R08] 数值比较
来源：http://jch.c1oappe.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vdw.316326.xyz

[R09] 字符串比较
来源：http://kmh.kuanghao11.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jss.havefunace.top

[R10] 正则匹配
来源：http://pys.gaohongyu789.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lln.hnqzz.top

[R11] case 多分支
来源：http://qck.hysaishi.cn

case "$1" in
来源：http://rec.yfazqb.com

start) echo "启动" ;;
来源：http://emd.jiagoushi.top

stop)  echo "停止" ;;
来源：http://nte.jianghu66.top

*)     echo "未知命令" ;;
来源：http://jmn.meibo888.top

esac
来源：http://nfg.dianchejie.cn

[R12] for 遍历文件
来源：http://llf.zhaomingkeji.xyz

for f in *.txt; do echo "$f"; done
来源：http://ivq.birdmap.top

[R13] for 计数循环
来源：http://xad.dianchejie.cn

for i in {1..10}; do echo "$i"; done
来源：http://jks.wangshuangyany.cn

[R14] C 风格 for
来源：http://ylq.uphjek.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://svr.yvedp.cn

[R15] while 逐行读文件
来源：http://ydq.havefunace.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lcv.jiagoushi.top

[R16] until 等待条件
来源：http://jlg.ydjk.org.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://srt.yfazqb.com

[R17] 数组定义与取值
来源：http://gui.feifeiyinyue.top

arr=(a b c); echo "${arr[0]}"
来源：http://sjb.fehbvm.com

[R18] 遍历数组
来源：http://sqh.sufxvd.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jut.zhengqikj.top

[R19] 数组长度
来源：http://gkz.52xcode.cn


<!-- 参考信息 -->