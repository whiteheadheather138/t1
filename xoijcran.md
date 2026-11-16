代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nyl.snrcjt.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hib.yj202588.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ktm.52xcode.cn

[P04] 求长度
来源：http://gmf.jlsjyb.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uyp.daria6918.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://moz.jinqigfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lkn.shanyushiyangtech.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wxf.tarul.cn

Java: list.size();  map.size();  s.length()
来源：http://wct.daria6918.cn

Go:   len(arr);  len(m)
来源：http://lnw.zhijiandao.cn

Ruby: x.length;  x.size
来源：http://btq.52xcode.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://axk.jqgufenzy.top

[P05] 判断两个对象内容是否相等
来源：http://qim.zhiwuduotai.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zxe.mhx1999.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://thu.vehdjk.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ztr.xylfe.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uhv.ydjk.org.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xde.aibaodan.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bcn.cqqwz.cn

Ruby: a == b
来源：http://hqj.jianghu66.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uee.shuidangran.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uyu.sxryk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yno.xuetiantiany.cn

PHP:  if (empty($x)) {}
来源：http://jtc.tanke756.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aby.meibo888.top

TS:   if (x == null) {}
来源：http://rru.yvedp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vks.dashuyun.cn

Go:   if x == nil {}
来源：http://ekk.jlsjyb.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ikn.wangshuangyany.cn

C#:   if (x is null) {}
来源：http://mkc.hysaishi.cn

[P07] 防抖与节流
来源：http://lfc.zycfv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://onx.cdnleiting.top

PHP:  // 手写时间戳比较
来源：http://pih.dianchejie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ogw.jinqigufen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://niu.hywenlv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jyk.yueranfly.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kgl.jqgufenzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ymb.tarul.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hay.9152youxi.cn

[P08] 处理浮点精度问题
来源：http://wvv.xziqi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wse.hfpthk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hvp.yuanzhike.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kpu.tarul.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yqn.chenjidiqi.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hza.ybcxt.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zxk.9152youxi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ilw.sysykeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gtx.yanxiufei.cn

================================================================================
来源：http://omo.jinghuilouyu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://twv.svipenyu.cn

================================================================================
来源：http://bhx.shanyushiyangkeji.top

[Q01] 创建表
来源：http://tcz.chenjidiqi.icu

CREATE TABLE users (
来源：http://lnq.cashguo.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vcx.c1oappe.top

name VARCHAR(50) NOT NULL,
来源：http://qxs.yuanzhike.top

email VARCHAR(100) UNIQUE,
来源：http://nuj.jinyuanbaomall.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lxb.hammf.cn

);
来源：http://mez.xingfuxueyuan.xyz

[Q02] 创建带外键的表
来源：http://rso.ctjpmb.com

CREATE TABLE orders (
来源：http://ndv.xziqi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://laj.ctjpmb.com

user_id INT NOT NULL,
来源：http://owp.chenzaomai.com

amount DECIMAL(10, 2),
来源：http://ecp.nanxinkj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://etm.jiagoushi.top

);
来源：http://twq.wangdashe.top

[Q03] 增加列
来源：http://omr.chenlongwang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://imf.yj20258888.top

[Q04] 修改列类型
来源：http://bso.jinqigufen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yyk.svipenyu.cn

[Q05] 重命名列
来源：http://gyp.aibaodan.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nhm.shanyushiyangkeji.top

[Q06] 删除列
来源：http://riu.yangfankeji.com

ALTER TABLE users DROP COLUMN age;
来源：http://ymo.fengsongda.top

[Q07] 删除表
来源：http://wns.jinqigfzy.top

DROP TABLE IF EXISTS orders;
来源：http://jsm.feifeiyinyue.top

[Q08] 创建普通索引
来源：http://sui.cashguo.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rsi.smart0.xyz

[Q09] 创建唯一索引
来源：http://slh.shzxlz.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mrg.fzhhl.top

[Q10] 插入单行
来源：http://vwt.hammf.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hjd.yuxming.cn

[Q11] 一次插入多行
来源：http://rbf.52xcode.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ffo.jlsjyb.cn

[Q12] 插入后取自增 ID
来源：http://yrf.hammf.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lqg.aibaodan.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jym.ehwqpu.com

[Q13] 忽略重复插入
来源：http://fsr.guowangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qlv.hongshengwenyu.top

[Q14] 存在则更新（upsert）
来源：http://qoz.52xcode.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://erq.316326.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vxj.cdnleiting.top

[Q15] 查询全部
来源：http://jgj.jiagoushi.top

SELECT * FROM users;
来源：http://wuh.jqgfzy.top

[Q16] 查询指定列
来源：http://mze.zhijiandao.cn

SELECT id, name FROM users;
来源：http://tvy.jyoumei.cn

[Q17] 条件查询
来源：http://wux.hcnkem.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kxl.yanxiufei.cn

[Q18] 模糊匹配
来源：http://zec.ywan-chungtsiang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ibp.sysykeji.top

[Q19] 范围查询
来源：http://byj.hnqzz.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pwn.nwbrower.top

[Q20] IN 列表
来源：http://hvd.hywenlv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ruy.wangshuangyany.cn

[Q21] 空值判断
来源：http://pyu.ctjpmb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://arg.ybcxt.top

[Q22] 排序
来源：http://onx.svipenyu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oam.havefunace.top

[Q23] 分页
来源：http://pae.yuxming.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://aun.ybcxt.top

[Q24] 去重
来源：http://gzp.zhixingplan.top

SELECT DISTINCT city FROM users;
来源：http://krr.jqgfzy.top

[Q25] 只取前 N 条
来源：http://zcp.vqdsnc.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qoq.jiagoushi.top

[Q26] 计数
来源：http://vnt.zhaomingkeji.xyz

SELECT COUNT(*) FROM users;
来源：http://wit.cheryme.top

[Q27] 条件计数
来源：http://oii.jqgufenzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hpi.fzhhl.top

[Q28] 求和与平均
来源：http://mgk.zhijiandao.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pyu.guowangkeji.top

[Q29] 最大最小值
来源：http://dhv.bjfxy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fhx.bjfxy.top

[Q30] 分组统计
来源：http://dfl.chenjidiqi.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ovg.haohaochexian.top

[Q31] 分组后过滤
来源：http://oei.yuanzhike.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eux.andypj.xyz

[Q32] 分组拼接字符串
来源：http://dvy.cucudq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xdj.chenzaomai.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ktg.vqdsnc.cn

[Q33] 多列分组
来源：http://aoi.ywan-chungtsiang.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ldk.gzhubu.top

[Q34] 每组取第一条
来源：http://gxt.hnqzz.top

SELECT * FROM (
来源：http://hsw.haohaochexian.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wpd.hesvh.cn

) t WHERE rn = 1;
来源：http://eag.epnwcf.com

[Q35] 内连接
来源：http://xla.hnxiangtu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kgr.jqgufenzy.top

[Q36] 左连接
来源：http://plj.hongshengwenyu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fie.cheryme.top

[Q37] 右连接
来源：http://flq.shanyushiyangtech.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://aks.snrcjt.cn

[Q38] 全外连接（PostgreSQL）
来源：http://her.yangfankeji.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ldi.jinqigfzy.top

[Q39] 自连接（查上下级）
来源：http://fqb.gotoacloud.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xvg.xinyue.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://moo.dashuyun.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vqc.hywenlv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cff.meibo888.top

[Q41] 多表连接
来源：http://ena.fzhhl.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bpr.wangdashe.top

JOIN users u ON u.id = o.user_id
来源：http://ycy.dianchejie.cn

JOIN products p ON p.id = o.product_id;
来源：http://zxt.gogol.net.cn

[Q42] 连接条件附加过滤
来源：http://gxj.yonumen.top

SELECT u.name, o.amount FROM users u
来源：http://qug.wangshuangyany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vsk.zhengqikj.top

[Q43] 标量子查询
来源：http://bes.zhaomingkeji.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jnx.andypj.xyz

[Q44] IN 子查询
来源：http://jhk.sufxvd.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dew.jinghuilouyu.cn

[Q45] EXISTS 判断存在
来源：http://ejd.fehbvm.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://utw.cdnleiting.top

[Q46] NOT EXISTS 判断不存在
来源：http://udp.chenjidiqi.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://myv.tianlin.xyz

[Q47] 与平均值比较
来源：http://pnj.redwolf501.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cvt.jqgfzy.top

[Q48] CTE 公用表表达式
来源：http://khl.dashuyun.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://htc.shanyushiyangkeji.top

SELECT * FROM t WHERE c > 5;
来源：http://cqa.pengpengdd.cyou

[Q49] 更新单行
来源：http://nke.yanxiufei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vaf.shanyushiyangtech.top

[Q50] 批量更新
来源：http://teu.gotoacloud.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hgq.zycfv.cn

[Q51] 用子查询更新
来源：http://egx.ppjwa.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://txz.xingfuxueyuan.xyz

[Q52] 删除指定行
来源：http://otv.xuetiantiany.cn

DELETE FROM users WHERE id = 10;
来源：http://kaa.cucudq.cn

[Q53] 按条件删除
来源：http://qmu.pengpengdd.cyou

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hlk.yj20258888.top

[Q54] 清空表
来源：http://krw.gogol.net.cn

TRUNCATE TABLE logs;
来源：http://rha.yongpay.top

[Q55] 排名（并列占位）
来源：http://fce.wangdashe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wbe.ydzc1.top

[Q56] 密集排名（并列不占位）
来源：http://gat.chenlongwang.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kpk.wangdashe.top

[Q57] 行号
来源：http://ojt.ehwqpu.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pen.fengsongda.top

[Q58] 累计求和
来源：http://yzp.quarkkingdee.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gkx.meibo888.top

[Q59] 分组内累计
来源：http://fse.sxryk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fgo.jinqigufen.top

[Q60] 取上一行 / 下一行
来源：http://hzl.hfpthk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wym.sysykeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://umt.dianchejie.cn

[Q61] 移动平均
来源：http://brj.c1oappe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lph.wangshuangyany.cn

[Q62] 分组占比
来源：http://ekb.yvedp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uzv.haohaochexian.top

[Q63] 开启事务
来源：http://ksk.tian-w.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rol.shuidangran.top

[Q64] 提交事务
来源：http://bnn.ydjk.org.cn

COMMIT;
来源：http://bln.kuanghao11.cn

[Q65] 回滚事务
来源：http://qtc.0kj1m.cn

ROLLBACK;
来源：http://ool.zycfv.cn

[Q66] 行锁查询
来源：http://akg.shanyushiyangtech.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rwg.sufxvd.cn

[Q67] 设置隔离级别
来源：http://hwz.dashuyun.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jgz.daxiang520.top

[Q68] 保存点
来源：http://yvc.aizwys.cn

SAVEPOINT sp1;
来源：http://lww.jqgfzy.top

ROLLBACK TO sp1;
来源：http://rwn.chenjidiqi.icu

[Q69] 查看执行计划
来源：http://smf.chenlongwang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ces.meibo888.top

[Q70] 更新统计信息
来源：http://sbx.xziqi.cn

ANALYZE TABLE users;
来源：http://kly.c1oappe.top

[Q71] 查看建表语句
来源：http://sbo.bbcook.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ulr.jinqigufen.top

[Q72] 查看索引
来源：http://lgq.jinqigfzy.top

SHOW INDEX FROM users;
来源：http://xfn.ehwqpu.com

[Q73] 查看表状态
来源：http://xhj.yonumen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nbr.meibo888.top

[Q74] 强制使用索引
来源：http://mhj.cdnleiting.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ovo.zhaomingkeji.xyz

[Q75] 日期格式化
来源：http://mqh.jianghu66.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dwj.chenzaomai.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rhu.cdnleiting.top

[Q76] 按天统计
来源：http://slj.zhiwuduotai.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://npx.zycfv.cn

[Q77] 时间加减
来源：http://fwp.jianghu66.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rgx.jinqigfzy.top

[Q78] 当前时间
来源：http://yrj.yvedp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ayj.chenjidiqi.icu

[Q79] 字符串拼接
来源：http://msh.chenjidiqi.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ehc.nanxinkj.top

[Q80] 字符串截取
来源：http://xio.cucudq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bwg.jinyuanbaomall.cn

[Q81] 字符串替换
来源：http://mgd.nanxinkj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hnq.xylfe.cn

[Q82] 字符长度与字节长度
来源：http://uya.ctjpmb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://add.pengpengdd.cyou

[Q83] 大小写转换
来源：http://jim.ctjpmb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uzu.52xcode.cn

[Q84] 去除首尾空格
来源：http://aba.andypj.xyz

SELECT TRIM(name) FROM users;
来源：http://hlo.yonumen.top

[Q85] 数值取整
来源：http://ysw.gaohongyu789.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zej.yonumen.top

[Q86] 读取 JSON 字段
来源：http://ctc.epnwcf.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uzm.shanyushiyangtech.top

[Q87] JSON 字段做条件
来源：http://rlx.nanxuanxn.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fxy.yvedp.cn

[Q88] 行转列（条件聚合）
来源：http://vpm.hesvh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qii.hammf.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fwb.yvedp.cn

[Q89] 判断表是否存在
来源：http://rik.jinqigufen.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://srf.pengpengdd.cyou

[Q90] 生成序号列
来源：http://poj.316326.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://amm.cashguo.top

================================================================================
来源：http://zni.yvedp.cn

R. Bash 专题
来源：http://nac.316326.xyz

================================================================================
来源：http://wwh.pycfn.com

[R01] shebang 与严格模式
来源：http://rns.jqgufenzy.top

#!/usr/bin/env bash
来源：http://ret.yj20258.top

set -euo pipefail
来源：http://zux.jinghuilouyu.cn

[R02] 变量赋值与使用
来源：http://cwe.hcnkem.com

name="Tom"; echo "$name"
来源：http://edb.ehwqpu.com

[R03] 只读变量
来源：http://zcs.aibaodan.cn

readonly PI=3.14
来源：http://rvp.shzxlz.cn

[R04] 位置参数
来源：http://zwt.haohaochexian.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bue.andypj.xyz

[R05] 参数默认值
来源：http://vsc.zhixingplan.top

name="${1:-default}"
来源：http://lpc.nanxinkj.top

[R06] 判断命令是否存在
来源：http://omz.hesvh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iri.hesvh.cn

[R07] if 判断文件
来源：http://vfv.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tbk.cucudq.cn

[R08] 数值比较
来源：http://prb.hfpthk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xwu.cashguo.top

[R09] 字符串比较
来源：http://oqe.yvedp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ant.zhongyouzk.top

[R10] 正则匹配
来源：http://kaa.sjlbkw.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://urd.fktsv.cn

[R11] case 多分支
来源：http://sbt.ybcxt.top

case "$1" in
来源：http://rrp.cucudq.cn

start) echo "启动" ;;
来源：http://hcy.cqqwz.cn

stop)  echo "停止" ;;
来源：http://auf.zycfv.cn

*)     echo "未知命令" ;;
来源：http://yjv.dianchejie.cn

esac
来源：http://jqt.gotoacloud.top

[R12] for 遍历文件
来源：http://zgs.cqqwz.cn

for f in *.txt; do echo "$f"; done
来源：http://iqs.jyoumei.cn

[R13] for 计数循环
来源：http://ebx.shuidangran.top

for i in {1..10}; do echo "$i"; done
来源：http://wvs.zycfv.cn

[R14] C 风格 for
来源：http://ohc.xylfe.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nvr.zhijiandao.cn

[R15] while 逐行读文件
来源：http://ymf.fzhhl.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://trx.gotoacloud.top

[R16] until 等待条件
来源：http://njf.jlsjyb.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rgr.cheryme.top

[R17] 数组定义与取值
来源：http://llp.pycfn.com

arr=(a b c); echo "${arr[0]}"
来源：http://xwa.hnxiangtu.top

[R18] 遍历数组
来源：http://fbu.cucudq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bdr.zhixingplan.top

[R19] 数组长度
来源：http://jtc.kuanghao11.cn


<!-- 参考信息 -->