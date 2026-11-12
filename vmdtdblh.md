代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tts.shuidangran.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lou.ywan-chungtsiang.top

[P03] 生成短随机字符串
来源：http://rdu.smart0.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lxs.ivvv.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lqc.shanyushiyangtech.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jew.daria6918.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fzo.yanxiufei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://olo.nwbrower.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rul.sjlbkw.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fgj.yuxming.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rib.yanxiufei.cn

[P04] 求长度
来源：http://ywv.shzxlz.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://axq.xylfe.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pvb.zhaomingkeji.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tjr.c1oappe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ltu.xylfe.cn

Java: list.size();  map.size();  s.length()
来源：http://uhu.cdnleiting.top

Go:   len(arr);  len(m)
来源：http://jsh.nanxinkj.top

Ruby: x.length;  x.size
来源：http://tcl.haohaochexian.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rme.havefunace.top

[P05] 判断两个对象内容是否相等
来源：http://drj.ehwqpu.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://eez.cashguo.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jiv.yangfankeji.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dag.tanke756.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ict.dashuyun.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ivq.hysaishi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://orl.haohaochexian.top

Ruby: a == b
来源：http://net.yangfankeji.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ilv.guowangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://aad.gotoacloud.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nvb.gotoacloud.top

PHP:  if (empty($x)) {}
来源：http://bnx.0kj1m.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jwh.smart0.xyz

TS:   if (x == null) {}
来源：http://sap.svipenyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wnb.dashuyun.cn

Go:   if x == nil {}
来源：http://poq.fzhhl.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cts.zhoulong.xyz

C#:   if (x is null) {}
来源：http://iza.xingfuxueyuan.xyz

[P07] 防抖与节流
来源：http://rnl.zhixingplan.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fys.xylfe.cn

PHP:  // 手写时间戳比较
来源：http://ytq.cucudq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vmx.shuidangran.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cjq.yonumen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bsi.ybcxt.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kyo.gaohongyu789.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hfn.xylfe.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fkt.pycfn.com

[P08] 处理浮点精度问题
来源：http://nzd.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dvc.xylfe.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sbz.feifeiyinyue.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ofc.nwbrower.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tuh.aizwys.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fmv.yangfankeji.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xws.guannengcc.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jwu.zhiwuduotai.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://esf.meibo888.top

================================================================================
来源：http://dqd.zhaomingkeji.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xnh.fktsv.cn

================================================================================
来源：http://dbz.zhoulong.xyz

[Q01] 创建表
来源：http://tka.pycfn.com

CREATE TABLE users (
来源：http://iei.epnwcf.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mgq.shangyingyoupin.top

name VARCHAR(50) NOT NULL,
来源：http://nnq.hesvh.cn

email VARCHAR(100) UNIQUE,
来源：http://xww.sxryk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lng.fanxiaobao.xyz

);
来源：http://ddd.xinyue.icu

[Q02] 创建带外键的表
来源：http://jju.zdbjq.cn

CREATE TABLE orders (
来源：http://gup.cheryme.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kzy.shzxlz.cn

user_id INT NOT NULL,
来源：http://bzy.chenjidiqi.icu

amount DECIMAL(10, 2),
来源：http://ypy.yfazqb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://alh.xziqi.cn

);
来源：http://elo.epnwcf.com

[Q03] 增加列
来源：http://xma.shanyushiyangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dhz.jianghu66.top

[Q04] 修改列类型
来源：http://ipa.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hhf.sjlbkw.cn

[Q05] 重命名列
来源：http://evw.tian-w.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://phb.yj202588.top

[Q06] 删除列
来源：http://akx.svipenyu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dkw.cucudq.cn

[Q07] 删除表
来源：http://fdp.haohaochexian.top

DROP TABLE IF EXISTS orders;
来源：http://gto.nanxuanxn.top

[Q08] 创建普通索引
来源：http://arf.quarkkingdee.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jrc.jyoumei.cn

[Q09] 创建唯一索引
来源：http://orn.yvedp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kje.gotoacloud.top

[Q10] 插入单行
来源：http://hoq.vehdjk.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://szc.daria6918.cn

[Q11] 一次插入多行
来源：http://gac.ctjpmb.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xyx.c1oappe.top

[Q12] 插入后取自增 ID
来源：http://pqn.mhx1999.top

INSERT INTO users (name) VALUES ('C');
来源：http://grr.nanxuanxn.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mob.nanxinkj.top

[Q13] 忽略重复插入
来源：http://tyy.guowangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://owe.bbcook.cn

[Q14] 存在则更新（upsert）
来源：http://pcl.ivvv.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ezx.yanxiufei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lkm.yangfankeji.com

[Q15] 查询全部
来源：http://jzc.hongshengwenyu.top

SELECT * FROM users;
来源：http://bqs.ywan-chungtsiang.top

[Q16] 查询指定列
来源：http://vwa.bjfxy.top

SELECT id, name FROM users;
来源：http://zdt.bjfxy.top

[Q17] 条件查询
来源：http://ymk.zdqjudy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zxw.yj202588.top

[Q18] 模糊匹配
来源：http://dvh.gzhubu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://clk.dashuyun.cn

[Q19] 范围查询
来源：http://bsp.zhiwuduotai.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wlm.zhongyouzk.top

[Q20] IN 列表
来源：http://tsr.wangdashe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xea.jinqigfzy.top

[Q21] 空值判断
来源：http://vzd.hfpthk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rbz.hnxiangtu.top

[Q22] 排序
来源：http://xew.jlsjyb.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ezy.yonumen.top

[Q23] 分页
来源：http://jlc.c1oappe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uoq.tianlin.xyz

[Q24] 去重
来源：http://iuq.bbcook.cn

SELECT DISTINCT city FROM users;
来源：http://wxn.cdnleiting.top

[Q25] 只取前 N 条
来源：http://nrv.sufxvd.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ojg.xingfuxueyuan.xyz

[Q26] 计数
来源：http://dfy.nanxuanxn.top

SELECT COUNT(*) FROM users;
来源：http://lwt.quarkkingdee.top

[Q27] 条件计数
来源：http://jyw.nanxinkj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ivv.pengpengdd.cyou

[Q28] 求和与平均
来源：http://tpa.haohaochexian.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dqw.cheryme.top

[Q29] 最大最小值
来源：http://bur.dianchejie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pjw.fengsongda.top

[Q30] 分组统计
来源：http://trf.yonumen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xju.wangshuangyany.cn

[Q31] 分组后过滤
来源：http://yes.c1oappe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yha.gotoacloud.top

[Q32] 分组拼接字符串
来源：http://ama.sjlbkw.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cey.ppjwa.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://msa.guowangkeji.top

[Q33] 多列分组
来源：http://hgl.smart0.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nhl.ydjk.org.cn

[Q34] 每组取第一条
来源：http://uem.tianlin.xyz

SELECT * FROM (
来源：http://ace.epnwcf.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dvu.jinqigfzy.top

) t WHERE rn = 1;
来源：http://zqe.meibo888.top

[Q35] 内连接
来源：http://bmk.guannengcc.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gyf.ydjk.org.cn

[Q36] 左连接
来源：http://jhu.yueranfly.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lxs.daxiang520.top

[Q37] 右连接
来源：http://rzw.andypj.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kta.cashguo.top

[Q38] 全外连接（PostgreSQL）
来源：http://pzs.andypj.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nqm.gogol.net.cn

[Q39] 自连接（查上下级）
来源：http://qmg.sweek.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qgq.zycfv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dau.chenzaomai.com

[Q40] 交叉连接（笛卡尔积）
来源：http://szl.0kj1m.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ngi.bjfxy.top

[Q41] 多表连接
来源：http://wns.wangdashe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nnu.cdnleiting.top

JOIN users u ON u.id = o.user_id
来源：http://jmy.gzhubu.top

JOIN products p ON p.id = o.product_id;
来源：http://gul.nanxinkj.top

[Q42] 连接条件附加过滤
来源：http://ctc.0kj1m.cn

SELECT u.name, o.amount FROM users u
来源：http://nsk.ivvv.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mvx.haohaochexian.top

[Q43] 标量子查询
来源：http://oiy.yj20258888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fnq.yonumen.top

[Q44] IN 子查询
来源：http://dai.yvedp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jsp.pycfn.com

[Q45] EXISTS 判断存在
来源：http://qkh.yuanzhike.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://awq.hongshengwenyu.top

[Q46] NOT EXISTS 判断不存在
来源：http://bwv.smart0.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cpo.bbcook.cn

[Q47] 与平均值比较
来源：http://mtm.hysaishi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ers.tarul.cn

[Q48] CTE 公用表表达式
来源：http://ifg.sweek.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pff.aibaodan.cn

SELECT * FROM t WHERE c > 5;
来源：http://smm.pycfn.com

[Q49] 更新单行
来源：http://bey.fengsongda.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bde.shangyingyoupin.top

[Q50] 批量更新
来源：http://rnu.chenlongwang.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://awv.hywenlv.cn

[Q51] 用子查询更新
来源：http://blo.jyoumei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://knw.jqgfzy.top

[Q52] 删除指定行
来源：http://exq.chenlongwang.top

DELETE FROM users WHERE id = 10;
来源：http://xpo.hywenlv.cn

[Q53] 按条件删除
来源：http://xjg.yuxming.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sxr.cucudq.cn

[Q54] 清空表
来源：http://xgm.sweek.top

TRUNCATE TABLE logs;
来源：http://yll.ehwqpu.com

[Q55] 排名（并列占位）
来源：http://gbk.hongshengwenyu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tno.ydjk.org.cn

[Q56] 密集排名（并列不占位）
来源：http://bwm.aibaodan.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hxb.zhongyouzk.top

[Q57] 行号
来源：http://icj.zycfv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ojw.sxryk.cn

[Q58] 累计求和
来源：http://cad.shanyushiyangtech.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://omy.ydjk.org.cn

[Q59] 分组内累计
来源：http://soh.epnwcf.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tsj.hongshengwenyu.top

[Q60] 取上一行 / 下一行
来源：http://cxj.chenjidiqi.icu

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zaf.zhengqikj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ulh.zhiwuduotai.top

[Q61] 移动平均
来源：http://lna.sweek.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aqz.yueranfly.top

[Q62] 分组占比
来源：http://gbt.jqgufenzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ebr.nwbrower.top

[Q63] 开启事务
来源：http://qit.hysaishi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hxb.nanxinkj.top

[Q64] 提交事务
来源：http://azz.xziqi.cn

COMMIT;
来源：http://bsh.ivvv.top

[Q65] 回滚事务
来源：http://ziq.epnwcf.com

ROLLBACK;
来源：http://ehb.hnqzz.top

[Q66] 行锁查询
来源：http://hkl.xuanzx.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bcn.jqgfzy.top

[Q67] 设置隔离级别
来源：http://kwh.tian-w.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jrm.cdnleiting.top

[Q68] 保存点
来源：http://kjv.fktsv.cn

SAVEPOINT sp1;
来源：http://xxb.jinghuilouyu.cn

ROLLBACK TO sp1;
来源：http://huu.hammf.cn

[Q69] 查看执行计划
来源：http://gng.tanke756.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nhu.yj202588.top

[Q70] 更新统计信息
来源：http://yim.pycfn.com

ANALYZE TABLE users;
来源：http://ecj.9152youxi.cn

[Q71] 查看建表语句
来源：http://mkc.vqdsnc.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pap.9152youxi.cn

[Q72] 查看索引
来源：http://iss.hongshengwenyu.top

SHOW INDEX FROM users;
来源：http://lle.pycfn.com

[Q73] 查看表状态
来源：http://xqu.hfpthk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pns.hywenlv.cn

[Q74] 强制使用索引
来源：http://rkf.316326.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mdg.yj20258888.top

[Q75] 日期格式化
来源：http://twx.xziqi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fgw.sysykeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qpz.wangdashe.top

[Q76] 按天统计
来源：http://uob.zhixingplan.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gfu.yangfankeji.com

[Q77] 时间加减
来源：http://wdo.jyoumei.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://agm.snrcjt.cn

[Q78] 当前时间
来源：http://qlu.meibo888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fjb.yueranfly.top

[Q79] 字符串拼接
来源：http://jog.xingfuxueyuan.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nxt.jinyuanbaomall.cn

[Q80] 字符串截取
来源：http://pbs.ywan-chungtsiang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://anh.guannengcc.top

[Q81] 字符串替换
来源：http://opt.cdnleiting.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tal.yanxiufei.cn

[Q82] 字符长度与字节长度
来源：http://ygw.aizwys.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kyu.hfpthk.cn

[Q83] 大小写转换
来源：http://oje.zhengqikj.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vfx.yongpay.top

[Q84] 去除首尾空格
来源：http://okn.feifeiyinyue.top

SELECT TRIM(name) FROM users;
来源：http://bdn.fengsongda.top

[Q85] 数值取整
来源：http://rov.wangshuangyany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bea.bjfxy.top

[Q86] 读取 JSON 字段
来源：http://rgs.jiagoushi.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cqv.jqgfzy.top

[Q87] JSON 字段做条件
来源：http://axq.havefunace.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qvx.zhoulong.xyz

[Q88] 行转列（条件聚合）
来源：http://vfz.xylfe.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dmb.hesvh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kwh.yangfankeji.com

[Q89] 判断表是否存在
来源：http://zsv.zhaomingkeji.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://upv.zhixingplan.top

[Q90] 生成序号列
来源：http://hdu.9152youxi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vjs.yongpay.top

================================================================================
来源：http://hoa.zhoulong.xyz

R. Bash 专题
来源：http://oah.0kj1m.cn

================================================================================
来源：http://alv.ctjpmb.com

[R01] shebang 与严格模式
来源：http://ddk.hesvh.cn

#!/usr/bin/env bash
来源：http://sdi.gaohongyu789.top

set -euo pipefail
来源：http://ffa.sweek.top

[R02] 变量赋值与使用
来源：http://egg.jinghuilouyu.cn

name="Tom"; echo "$name"
来源：http://lap.hnqzz.top

[R03] 只读变量
来源：http://lum.pycfn.com

readonly PI=3.14
来源：http://rvq.hcnkem.com

[R04] 位置参数
来源：http://zus.hcnkem.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yla.shuidangran.top

[R05] 参数默认值
来源：http://air.chenjidiqi.icu

name="${1:-default}"
来源：http://svc.zdqjudy.top

[R06] 判断命令是否存在
来源：http://iue.316326.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ttr.hnqzz.top

[R07] if 判断文件
来源：http://mrk.ybcxt.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zwj.vehdjk.com

[R08] 数值比较
来源：http://wvw.gzhubu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mlq.daria6918.cn

[R09] 字符串比较
来源：http://nlx.fzhhl.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qje.bbcook.cn

[R10] 正则匹配
来源：http://srv.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://che.hcnkem.com

[R11] case 多分支
来源：http://htc.fktsv.cn

case "$1" in
来源：http://ndi.vehdjk.com

start) echo "启动" ;;
来源：http://ill.meibo888.top

stop)  echo "停止" ;;
来源：http://rih.zhengqikj.top

*)     echo "未知命令" ;;
来源：http://fov.gotoacloud.top

esac
来源：http://eov.316326.xyz

[R12] for 遍历文件
来源：http://wqp.jiagoushi.top

for f in *.txt; do echo "$f"; done
来源：http://lzn.zhaomingkeji.xyz

[R13] for 计数循环
来源：http://euz.iojbl.cn

for i in {1..10}; do echo "$i"; done
来源：http://slc.shuidangran.top

[R14] C 风格 for
来源：http://bfo.sxryk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ilo.fehbvm.com

[R15] while 逐行读文件
来源：http://dnn.hesvh.cn


<!-- 参考信息 -->