代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gqh.nwbrower.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vez.cdnleiting.top

[P03] 生成短随机字符串
来源：http://pfu.shzxlz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zbt.hysaishi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qxe.jyoumei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jmn.ehwqpu.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dpp.xylfe.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nyz.zhiwuduotai.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://doa.bbcook.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bma.shanyushiyangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vtr.cucudq.cn

[P04] 求长度
来源：http://qpx.jlsjyb.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://clw.zhaomingkeji.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qzb.xingfuxueyuan.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bfa.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vio.zhiwuduotai.top

Java: list.size();  map.size();  s.length()
来源：http://osv.bjfxy.top

Go:   len(arr);  len(m)
来源：http://hoo.pengpengdd.cyou

Ruby: x.length;  x.size
来源：http://pdw.hnxiangtu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://itq.zycfv.cn

[P05] 判断两个对象内容是否相等
来源：http://vfz.kuanghao11.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://our.ybcxt.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ytg.yj20258.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jsi.hywenlv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mzu.ctjpmb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://byq.gogol.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xtz.jqgufenzy.top

Ruby: a == b
来源：http://sht.hammf.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rzr.tarul.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://elu.shuidangran.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ttq.gzhubu.top

PHP:  if (empty($x)) {}
来源：http://fap.yongpay.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ziu.jinghuilouyu.cn

TS:   if (x == null) {}
来源：http://nhc.hesvh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ial.zhijiandao.cn

Go:   if x == nil {}
来源：http://sbq.nwbrower.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zcl.nwbrower.top

C#:   if (x is null) {}
来源：http://fax.zhongyouzk.top

[P07] 防抖与节流
来源：http://gnc.smart0.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lzl.tarul.cn

PHP:  // 手写时间戳比较
来源：http://yog.tianlin.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tpd.smart0.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://crh.shangyingyoupin.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jrc.smart0.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xpu.sufxvd.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://iko.haohaochexian.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hon.cashguo.top

[P08] 处理浮点精度问题
来源：http://nfg.tarul.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://peo.316326.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cmf.vqdsnc.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gum.jianghu66.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rbb.yongpay.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ydz.gogol.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cvp.fehbvm.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zsy.zhiwuduotai.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wfj.xinyue.icu

================================================================================
来源：http://czr.yanxiufei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wbu.jyoumei.cn

================================================================================
来源：http://pld.redwolf501.top

[Q01] 创建表
来源：http://dwr.epnwcf.com

CREATE TABLE users (
来源：http://mea.yj20258.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sdu.hfpthk.cn

name VARCHAR(50) NOT NULL,
来源：http://cgn.pycfn.com

email VARCHAR(100) UNIQUE,
来源：http://lbc.cucudq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pcb.hnqzz.top

);
来源：http://peu.fzhhl.top

[Q02] 创建带外键的表
来源：http://bja.hfpthk.cn

CREATE TABLE orders (
来源：http://med.jqgfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pvt.wangdashe.top

user_id INT NOT NULL,
来源：http://wqm.feifeiyinyue.top

amount DECIMAL(10, 2),
来源：http://has.ivvv.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://eva.cucudq.cn

);
来源：http://mdy.0kj1m.cn

[Q03] 增加列
来源：http://btn.chenjidiqi.icu

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zdv.xuetiantiany.cn

[Q04] 修改列类型
来源：http://tun.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lpf.shanyushiyangkeji.top

[Q05] 重命名列
来源：http://dkc.pycfn.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gyv.wangdashe.top

[Q06] 删除列
来源：http://nit.zhijiandao.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gnz.haohaochexian.top

[Q07] 删除表
来源：http://rgv.hnxiangtu.top

DROP TABLE IF EXISTS orders;
来源：http://wnh.sweek.top

[Q08] 创建普通索引
来源：http://zht.meibo888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gia.quarkkingdee.top

[Q09] 创建唯一索引
来源：http://uiy.yongpay.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zee.9152youxi.cn

[Q10] 插入单行
来源：http://xns.fanxiaobao.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mvi.fehbvm.com

[Q11] 一次插入多行
来源：http://yuz.cdnleiting.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://szf.c1oappe.top

[Q12] 插入后取自增 ID
来源：http://riw.epnwcf.com

INSERT INTO users (name) VALUES ('C');
来源：http://hiq.yfazqb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wkc.sweek.top

[Q13] 忽略重复插入
来源：http://tev.daxiang520.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mro.jinghuilouyu.cn

[Q14] 存在则更新（upsert）
来源：http://lco.ctjpmb.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zmc.c1oappe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ned.c1oappe.top

[Q15] 查询全部
来源：http://vid.hesvh.cn

SELECT * FROM users;
来源：http://huy.shanyushiyangkeji.top

[Q16] 查询指定列
来源：http://hmt.xuetiantiany.cn

SELECT id, name FROM users;
来源：http://xjd.wangshuangyany.cn

[Q17] 条件查询
来源：http://fxj.meibo888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wvp.ehwqpu.com

[Q18] 模糊匹配
来源：http://ybf.fzhhl.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fbl.cdnleiting.top

[Q19] 范围查询
来源：http://hzb.tian-w.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cgq.yj202588.top

[Q20] IN 列表
来源：http://ptq.zhijiandao.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dro.vehdjk.com

[Q21] 空值判断
来源：http://aji.zhiwuduotai.top

SELECT * FROM users WHERE email IS NULL;
来源：http://sfj.haohaochexian.top

[Q22] 排序
来源：http://cwt.tianlin.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lay.zhixingplan.top

[Q23] 分页
来源：http://qlt.zhengqikj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://doc.sxryk.cn

[Q24] 去重
来源：http://yre.tanke756.top

SELECT DISTINCT city FROM users;
来源：http://odb.jiagoushi.top

[Q25] 只取前 N 条
来源：http://ssz.gaohongyu789.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vue.jinqigufen.top

[Q26] 计数
来源：http://iye.zhaomingkeji.xyz

SELECT COUNT(*) FROM users;
来源：http://kou.ppjwa.cn

[Q27] 条件计数
来源：http://ebf.cheryme.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uwv.zdbjq.cn

[Q28] 求和与平均
来源：http://acl.zhoulong.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kam.pycfn.com

[Q29] 最大最小值
来源：http://lud.yj202588.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jxp.xylfe.cn

[Q30] 分组统计
来源：http://mzu.guannengcc.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jxs.daria6918.cn

[Q31] 分组后过滤
来源：http://nqf.xuanzx.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nct.xylfe.cn

[Q32] 分组拼接字符串
来源：http://eps.yangfankeji.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mxa.aizwys.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ajc.zhoulong.xyz

[Q33] 多列分组
来源：http://gpw.cashguo.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jii.shangyingyoupin.top

[Q34] 每组取第一条
来源：http://hgz.jqgufenzy.top

SELECT * FROM (
来源：http://rdx.redwolf501.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zii.yongpay.top

) t WHERE rn = 1;
来源：http://lfc.haohaochexian.top

[Q35] 内连接
来源：http://ffe.wangshuangyany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mwr.yonumen.top

[Q36] 左连接
来源：http://vcs.hnxiangtu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qaw.birdmap.top

[Q37] 右连接
来源：http://reo.jqgfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ndi.feifeiyinyue.top

[Q38] 全外连接（PostgreSQL）
来源：http://ttp.zhengqikj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hhl.hnxiangtu.top

[Q39] 自连接（查上下级）
来源：http://rag.jianghu66.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wpb.sweek.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iaz.daxiang520.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ybg.birdmap.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vlu.nwbrower.top

[Q41] 多表连接
来源：http://uvm.vehdjk.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://sln.shanyushiyangtech.top

JOIN users u ON u.id = o.user_id
来源：http://zhe.yj202588.top

JOIN products p ON p.id = o.product_id;
来源：http://mcz.svipenyu.cn

[Q42] 连接条件附加过滤
来源：http://vnj.gogol.net.cn

SELECT u.name, o.amount FROM users u
来源：http://mhb.epnwcf.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://boi.tanke756.top

[Q43] 标量子查询
来源：http://bsq.fktsv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cba.meibo888.top

[Q44] IN 子查询
来源：http://lzo.andypj.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ahl.sysykeji.top

[Q45] EXISTS 判断存在
来源：http://uxd.uphjek.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zrm.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://ylg.fengsongda.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nny.hnqzz.top

[Q47] 与平均值比较
来源：http://htj.gzhubu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gej.shanyushiyangkeji.top

[Q48] CTE 公用表表达式
来源：http://ayg.yfazqb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xsv.nanxuanxn.top

SELECT * FROM t WHERE c > 5;
来源：http://mfb.aizwys.cn

[Q49] 更新单行
来源：http://mmr.tarul.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dig.hongshengwenyu.top

[Q50] 批量更新
来源：http://gob.nanxuanxn.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zft.dianchejie.cn

[Q51] 用子查询更新
来源：http://plg.dashuyun.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wyp.hnqzz.top

[Q52] 删除指定行
来源：http://fro.vehdjk.com

DELETE FROM users WHERE id = 10;
来源：http://adi.redwolf501.top

[Q53] 按条件删除
来源：http://hrn.xuetiantiany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dqh.yongpay.top

[Q54] 清空表
来源：http://ndn.cheryme.top

TRUNCATE TABLE logs;
来源：http://ihx.yj202588.top

[Q55] 排名（并列占位）
来源：http://uod.zycfv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bgq.hnxiangtu.top

[Q56] 密集排名（并列不占位）
来源：http://tii.nanxinkj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://inl.cashguo.top

[Q57] 行号
来源：http://ztj.yfazqb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jck.jlsjyb.cn

[Q58] 累计求和
来源：http://vaj.xziqi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kfx.fehbvm.com

[Q59] 分组内累计
来源：http://atv.chenjidiqi.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nvw.chenzaomai.com

[Q60] 取上一行 / 下一行
来源：http://tjw.shangyingyoupin.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aay.haohaochexian.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://glr.shuidangran.top

[Q61] 移动平均
来源：http://yph.jlsjyb.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sbf.zdqjudy.top

[Q62] 分组占比
来源：http://hpy.kuanghao11.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://btn.vehdjk.com

[Q63] 开启事务
来源：http://zwp.ivvv.top

START TRANSACTION;                -- 或 BEGIN
来源：http://aqy.yongpay.top

[Q64] 提交事务
来源：http://txj.fehbvm.com

COMMIT;
来源：http://apy.tanke756.top

[Q65] 回滚事务
来源：http://rlm.uphjek.com

ROLLBACK;
来源：http://tkc.9152youxi.cn

[Q66] 行锁查询
来源：http://ghq.fanxiaobao.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ujo.chenlongwang.top

[Q67] 设置隔离级别
来源：http://suy.zhaomingkeji.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fro.tianlin.xyz

[Q68] 保存点
来源：http://jnt.yongpay.top

SAVEPOINT sp1;
来源：http://smm.zdqjudy.top

ROLLBACK TO sp1;
来源：http://nwt.nwbrower.top

[Q69] 查看执行计划
来源：http://iyi.yueranfly.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ymk.hongshengwenyu.top

[Q70] 更新统计信息
来源：http://fcn.birdmap.top

ANALYZE TABLE users;
来源：http://ytj.jiagoushi.top

[Q71] 查看建表语句
来源：http://ltp.fengsongda.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://omr.zdbjq.cn

[Q72] 查看索引
来源：http://mpz.sjlbkw.cn

SHOW INDEX FROM users;
来源：http://jtj.chenlongwang.top

[Q73] 查看表状态
来源：http://pmx.xinyue.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://aku.shanyushiyangkeji.top

[Q74] 强制使用索引
来源：http://bjh.hesvh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ito.tarul.cn

[Q75] 日期格式化
来源：http://pwo.jinghuilouyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://thd.fktsv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fxm.mhx1999.top

[Q76] 按天统计
来源：http://jie.yj20258888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rzk.shangyingyoupin.top

[Q77] 时间加减
来源：http://law.yuanzhike.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ebt.daxiang520.top

[Q78] 当前时间
来源：http://hls.hesvh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cwv.tarul.cn

[Q79] 字符串拼接
来源：http://tse.tanke756.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qgc.shuidangran.top

[Q80] 字符串截取
来源：http://qfw.cqqwz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jcp.wangdashe.top

[Q81] 字符串替换
来源：http://ujh.0kj1m.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wpr.yj20258.top

[Q82] 字符长度与字节长度
来源：http://rtq.feifeiyinyue.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ykb.hongshengwenyu.top

[Q83] 大小写转换
来源：http://lln.meibo888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tbe.hesvh.cn

[Q84] 去除首尾空格
来源：http://wff.pengpengdd.cyou

SELECT TRIM(name) FROM users;
来源：http://cgq.yj202588.top

[Q85] 数值取整
来源：http://hyu.birdmap.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ehi.jiagoushi.top

[Q86] 读取 JSON 字段
来源：http://hfi.ivvv.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ent.c1oappe.top

[Q87] JSON 字段做条件
来源：http://zii.shanyushiyangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iqz.aibaodan.cn

[Q88] 行转列（条件聚合）
来源：http://grw.guannengcc.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ncb.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://buq.sweek.top

[Q89] 判断表是否存在
来源：http://vby.yonumen.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://poz.guowangkeji.top

[Q90] 生成序号列
来源：http://pjo.jianghu66.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://eha.nanxuanxn.top

================================================================================
来源：http://aom.hesvh.cn

R. Bash 专题
来源：http://ssq.shanyushiyangkeji.top

================================================================================
来源：http://ibx.aizwys.cn

[R01] shebang 与严格模式
来源：http://puw.fktsv.cn

#!/usr/bin/env bash
来源：http://urr.jinqigfzy.top

set -euo pipefail
来源：http://bcq.chenlongwang.top

[R02] 变量赋值与使用
来源：http://tay.hnxiangtu.top

name="Tom"; echo "$name"
来源：http://aox.xylfe.cn

[R03] 只读变量
来源：http://hrs.vqdsnc.cn

readonly PI=3.14
来源：http://vjn.jiagoushi.top

[R04] 位置参数
来源：http://hhq.aizwys.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lde.epnwcf.com

[R05] 参数默认值
来源：http://rui.aibaodan.cn

name="${1:-default}"
来源：http://myg.fengsongda.top

[R06] 判断命令是否存在
来源：http://gbp.xziqi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ivg.nwbrower.top

[R07] if 判断文件
来源：http://sqr.yfazqb.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://peu.hammf.cn

[R08] 数值比较
来源：http://clq.daxiang520.top

if (( a > b )); then echo "a 更大"; fi
来源：http://yvc.zhixingplan.top

[R09] 字符串比较
来源：http://pde.shanyushiyangtech.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xez.shzxlz.cn

[R10] 正则匹配
来源：http://kgz.nanxinkj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xpw.zhaomingkeji.xyz

[R11] case 多分支
来源：http://pnj.fzhhl.top

case "$1" in
来源：http://yau.yongpay.top

start) echo "启动" ;;
来源：http://thy.sxryk.cn

stop)  echo "停止" ;;
来源：http://rfp.ppjwa.cn

*)     echo "未知命令" ;;
来源：http://gld.zhiwuduotai.top

esac
来源：http://ynt.fktsv.cn

[R12] for 遍历文件
来源：http://wmn.hnqzz.top

for f in *.txt; do echo "$f"; done
来源：http://uhx.shuidangran.top

[R13] for 计数循环
来源：http://fva.9152youxi.cn

for i in {1..10}; do echo "$i"; done
来源：http://snv.shzxlz.cn

[R14] C 风格 for
来源：http://hmb.chenjidiqi.icu

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fhr.haohaochexian.top

[R15] while 逐行读文件
来源：http://kpt.nanxinkj.top


<!-- 参考信息 -->