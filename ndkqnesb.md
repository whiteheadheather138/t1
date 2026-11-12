代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sto.yvedp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uvz.quarkkingdee.top

[P03] 生成短随机字符串
来源：http://pqz.yuxming.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ryg.quarkkingdee.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://utl.shanyushiyangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zth.yonumen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ehi.jqgufenzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qld.xuanzx.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ifw.ppjwa.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fvi.yueranfly.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ayl.pycfn.com

[P04] 求长度
来源：http://iie.ydjk.org.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yxp.ydzc1.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qkl.ywan-chungtsiang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://isu.zhaomingkeji.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jfz.zycfv.cn

Java: list.size();  map.size();  s.length()
来源：http://nxj.wangshuangyany.cn

Go:   len(arr);  len(m)
来源：http://swo.9152youxi.cn

Ruby: x.length;  x.size
来源：http://luu.c1oappe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://iub.gogol.net.cn

[P05] 判断两个对象内容是否相等
来源：http://vjq.ydjk.org.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rgc.svipenyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://izv.fehbvm.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vss.bbcook.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jjz.svipenyu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wgs.xziqi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qxu.hongshengwenyu.top

Ruby: a == b
来源：http://jxa.c1oappe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pbf.kuanghao11.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zea.yj20258888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sfc.jinqigfzy.top

PHP:  if (empty($x)) {}
来源：http://vtu.jyoumei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qnf.ydzc1.top

TS:   if (x == null) {}
来源：http://vmf.wangdashe.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jte.guannengcc.top

Go:   if x == nil {}
来源：http://izg.tarul.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zse.jinyuanbaomall.cn

C#:   if (x is null) {}
来源：http://fap.jqgfzy.top

[P07] 防抖与节流
来源：http://dyk.daria6918.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qoa.chenjidiqi.icu

PHP:  // 手写时间戳比较
来源：http://bcu.yongpay.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xml.hywenlv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hzw.fanxiaobao.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hsb.yangfankeji.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jif.xylfe.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://clj.zhongyouzk.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cyh.hnqzz.top

[P08] 处理浮点精度问题
来源：http://xpk.yj20258888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aav.xingfuxueyuan.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ruw.shanyushiyangkeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iiy.pycfn.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lur.meibo888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://chb.meibo888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zzf.shzxlz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kyq.zhiwuduotai.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rut.zhoulong.xyz

================================================================================
来源：http://bcq.smart0.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gwz.jyoumei.cn

================================================================================
来源：http://xfw.xylfe.cn

[Q01] 创建表
来源：http://dyy.tanke756.top

CREATE TABLE users (
来源：http://bzm.birdmap.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rpn.havefunace.top

name VARCHAR(50) NOT NULL,
来源：http://faw.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://ujb.yueranfly.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vzw.yuxming.cn

);
来源：http://fnw.yonumen.top

[Q02] 创建带外键的表
来源：http://cwr.smart0.xyz

CREATE TABLE orders (
来源：http://waz.zhengqikj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vae.smart0.xyz

user_id INT NOT NULL,
来源：http://fzl.zdbjq.cn

amount DECIMAL(10, 2),
来源：http://svl.guowangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xlz.zhoulong.xyz

);
来源：http://jbj.yanxiufei.cn

[Q03] 增加列
来源：http://vof.xinyue.icu

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kqf.shanyushiyangtech.top

[Q04] 修改列类型
来源：http://acl.yvedp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bpf.ctjpmb.com

[Q05] 重命名列
来源：http://ecb.ywan-chungtsiang.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pkx.yuanzhike.top

[Q06] 删除列
来源：http://qlp.birdmap.top

ALTER TABLE users DROP COLUMN age;
来源：http://cny.tarul.cn

[Q07] 删除表
来源：http://lwo.fanxiaobao.xyz

DROP TABLE IF EXISTS orders;
来源：http://vyj.yj20258.top

[Q08] 创建普通索引
来源：http://bss.yj202588.top

CREATE INDEX idx_users_email ON users(email);
来源：http://edd.fanxiaobao.xyz

[Q09] 创建唯一索引
来源：http://jys.hywenlv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lpx.ivvv.top

[Q10] 插入单行
来源：http://iib.c1oappe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wfy.dianchejie.cn

[Q11] 一次插入多行
来源：http://qwv.zdbjq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mpw.jianghu66.top

[Q12] 插入后取自增 ID
来源：http://icz.yj20258888.top

INSERT INTO users (name) VALUES ('C');
来源：http://moi.hysaishi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://twe.xinyue.icu

[Q13] 忽略重复插入
来源：http://hit.shanyushiyangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ufs.yvedp.cn

[Q14] 存在则更新（upsert）
来源：http://lnd.cqqwz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uuu.hongshengwenyu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://huz.quarkkingdee.top

[Q15] 查询全部
来源：http://hfq.feifeiyinyue.top

SELECT * FROM users;
来源：http://gyw.redwolf501.top

[Q16] 查询指定列
来源：http://kmq.yueranfly.top

SELECT id, name FROM users;
来源：http://kaa.zhixingplan.top

[Q17] 条件查询
来源：http://gli.aizwys.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ecu.shanyushiyangkeji.top

[Q18] 模糊匹配
来源：http://taa.ybcxt.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://orp.9152youxi.cn

[Q19] 范围查询
来源：http://wyo.zhongyouzk.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eds.jqgufenzy.top

[Q20] IN 列表
来源：http://pib.xylfe.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gsa.wangdashe.top

[Q21] 空值判断
来源：http://ytk.sufxvd.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wyy.jianghu66.top

[Q22] 排序
来源：http://gbj.shzxlz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wjp.xinyue.icu

[Q23] 分页
来源：http://geh.zhengqikj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pcb.sweek.top

[Q24] 去重
来源：http://xdf.jlsjyb.cn

SELECT DISTINCT city FROM users;
来源：http://gyh.fanxiaobao.xyz

[Q25] 只取前 N 条
来源：http://aov.52xcode.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cro.shuidangran.top

[Q26] 计数
来源：http://syl.zhaomingkeji.xyz

SELECT COUNT(*) FROM users;
来源：http://xqy.dianchejie.cn

[Q27] 条件计数
来源：http://dbf.daria6918.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vyi.tian-w.cn

[Q28] 求和与平均
来源：http://unp.zhixingplan.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qbl.mhx1999.top

[Q29] 最大最小值
来源：http://uyi.nanxinkj.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jkk.fzhhl.top

[Q30] 分组统计
来源：http://pmq.kuanghao11.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gww.tian-w.cn

[Q31] 分组后过滤
来源：http://avw.zycfv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://biu.pengpengdd.cyou

[Q32] 分组拼接字符串
来源：http://ogp.ydzc1.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gcf.yuxming.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jlg.cheryme.top

[Q33] 多列分组
来源：http://pyc.wangshuangyany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gle.aizwys.cn

[Q34] 每组取第一条
来源：http://dkb.jianghu66.top

SELECT * FROM (
来源：http://qmf.yfazqb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://naz.fanxiaobao.xyz

) t WHERE rn = 1;
来源：http://com.yj202588.top

[Q35] 内连接
来源：http://cag.epnwcf.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fwb.daria6918.cn

[Q36] 左连接
来源：http://een.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://itg.ehwqpu.com

[Q37] 右连接
来源：http://wte.yj20258888.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qvc.nwbrower.top

[Q38] 全外连接（PostgreSQL）
来源：http://qdt.xuanzx.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fzp.yonumen.top

[Q39] 自连接（查上下级）
来源：http://wno.birdmap.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://cyh.pengpengdd.cyou

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hkp.shanyushiyangtech.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jdy.shzxlz.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oil.sufxvd.cn

[Q41] 多表连接
来源：http://aue.shuidangran.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://eyc.cdnleiting.top

JOIN users u ON u.id = o.user_id
来源：http://cka.aizwys.cn

JOIN products p ON p.id = o.product_id;
来源：http://bxb.havefunace.top

[Q42] 连接条件附加过滤
来源：http://lml.jyoumei.cn

SELECT u.name, o.amount FROM users u
来源：http://zna.cucudq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ugy.zhixingplan.top

[Q43] 标量子查询
来源：http://okr.sweek.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nmx.mhx1999.top

[Q44] IN 子查询
来源：http://nsg.gzhubu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kcn.shzxlz.cn

[Q45] EXISTS 判断存在
来源：http://kou.cdnleiting.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vpc.zhiwuduotai.top

[Q46] NOT EXISTS 判断不存在
来源：http://yjw.ywan-chungtsiang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://irx.yfazqb.com

[Q47] 与平均值比较
来源：http://ehd.yanxiufei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ied.ehwqpu.com

[Q48] CTE 公用表表达式
来源：http://fny.fzhhl.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xzg.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://rqh.vqdsnc.cn

[Q49] 更新单行
来源：http://rex.ehwqpu.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ezm.chenlongwang.top

[Q50] 批量更新
来源：http://wpz.gotoacloud.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jic.0kj1m.cn

[Q51] 用子查询更新
来源：http://adj.zhiwuduotai.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qxl.cashguo.top

[Q52] 删除指定行
来源：http://qil.vqdsnc.cn

DELETE FROM users WHERE id = 10;
来源：http://poa.snrcjt.cn

[Q53] 按条件删除
来源：http://lta.sufxvd.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kzw.bbcook.cn

[Q54] 清空表
来源：http://zwn.fengsongda.top

TRUNCATE TABLE logs;
来源：http://yes.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://kla.yonumen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mku.haohaochexian.top

[Q56] 密集排名（并列不占位）
来源：http://wzl.yangfankeji.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pwe.jinqigfzy.top

[Q57] 行号
来源：http://nce.fehbvm.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mno.snrcjt.cn

[Q58] 累计求和
来源：http://wip.jinqigfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gdx.jqgfzy.top

[Q59] 分组内累计
来源：http://ysc.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rnd.quarkkingdee.top

[Q60] 取上一行 / 下一行
来源：http://nfq.xuetiantiany.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cyr.bjfxy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://awt.hywenlv.cn

[Q61] 移动平均
来源：http://gxw.shuidangran.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://srw.cucudq.cn

[Q62] 分组占比
来源：http://jzk.gotoacloud.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cni.birdmap.top

[Q63] 开启事务
来源：http://qhv.dianchejie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qwu.xylfe.cn

[Q64] 提交事务
来源：http://iui.vehdjk.com

COMMIT;
来源：http://qfd.hesvh.cn

[Q65] 回滚事务
来源：http://fli.xuetiantiany.cn

ROLLBACK;
来源：http://heb.yuanzhike.top

[Q66] 行锁查询
来源：http://thz.cqqwz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gzn.aibaodan.cn

[Q67] 设置隔离级别
来源：http://rca.cqqwz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uiu.daxiang520.top

[Q68] 保存点
来源：http://iic.jqgufenzy.top

SAVEPOINT sp1;
来源：http://pyj.ppjwa.cn

ROLLBACK TO sp1;
来源：http://oqf.tianlin.xyz

[Q69] 查看执行计划
来源：http://qnp.kuanghao11.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wwa.snrcjt.cn

[Q70] 更新统计信息
来源：http://bmf.sjlbkw.cn

ANALYZE TABLE users;
来源：http://dgm.aibaodan.cn

[Q71] 查看建表语句
来源：http://ohf.feifeiyinyue.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://woz.fengsongda.top

[Q72] 查看索引
来源：http://mnw.yj202588.top

SHOW INDEX FROM users;
来源：http://orb.fktsv.cn

[Q73] 查看表状态
来源：http://dib.shuidangran.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rpe.vqdsnc.cn

[Q74] 强制使用索引
来源：http://imc.yuxming.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ulw.zhengqikj.top

[Q75] 日期格式化
来源：http://bki.ydzc1.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kin.feifeiyinyue.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pcg.ctjpmb.com

[Q76] 按天统计
来源：http://rsg.zhoulong.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://unc.hongshengwenyu.top

[Q77] 时间加减
来源：http://vmt.zdqjudy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cdm.ydjk.org.cn

[Q78] 当前时间
来源：http://bnl.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://stl.shangyingyoupin.top

[Q79] 字符串拼接
来源：http://wqn.daria6918.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sth.andypj.xyz

[Q80] 字符串截取
来源：http://fjo.chenzaomai.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hci.316326.xyz

[Q81] 字符串替换
来源：http://jxe.hysaishi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qpk.guowangkeji.top

[Q82] 字符长度与字节长度
来源：http://xzn.zycfv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mgv.fehbvm.com

[Q83] 大小写转换
来源：http://qit.ivvv.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kut.dashuyun.cn

[Q84] 去除首尾空格
来源：http://frx.jinqigfzy.top

SELECT TRIM(name) FROM users;
来源：http://hjs.jinghuilouyu.cn

[Q85] 数值取整
来源：http://seg.nanxuanxn.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://brb.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://omj.jinqigfzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cwg.ywan-chungtsiang.top

[Q87] JSON 字段做条件
来源：http://yuz.yonumen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cwh.shanyushiyangtech.top

[Q88] 行转列（条件聚合）
来源：http://rrd.pycfn.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qyz.tanke756.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hjv.jinghuilouyu.cn

[Q89] 判断表是否存在
来源：http://nyv.vqdsnc.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yvr.fzhhl.top

[Q90] 生成序号列
来源：http://lej.nwbrower.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uvr.cashguo.top

================================================================================
来源：http://ged.c1oappe.top

R. Bash 专题
来源：http://uht.ehwqpu.com

================================================================================
来源：http://nnu.tarul.cn

[R01] shebang 与严格模式
来源：http://ryv.cheryme.top

#!/usr/bin/env bash
来源：http://phx.hnxiangtu.top

set -euo pipefail
来源：http://yym.aibaodan.cn

[R02] 变量赋值与使用
来源：http://baa.jinyuanbaomall.cn

name="Tom"; echo "$name"
来源：http://usu.smart0.xyz

[R03] 只读变量
来源：http://ykm.jiagoushi.top

readonly PI=3.14
来源：http://ein.nanxuanxn.top

[R04] 位置参数
来源：http://etu.gogol.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mgs.wangdashe.top

[R05] 参数默认值
来源：http://bjy.sjlbkw.cn

name="${1:-default}"
来源：http://tep.jianghu66.top

[R06] 判断命令是否存在
来源：http://doq.bjfxy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ntw.hongshengwenyu.top

[R07] if 判断文件
来源：http://qvp.tarul.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://loq.jiagoushi.top

[R08] 数值比较
来源：http://jli.vqdsnc.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cat.shanyushiyangtech.top

[R09] 字符串比较
来源：http://jsx.bjfxy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bor.52xcode.cn

[R10] 正则匹配
来源：http://iml.ydzc1.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gui.hywenlv.cn

[R11] case 多分支
来源：http://cxh.jinyuanbaomall.cn

case "$1" in
来源：http://jyy.mhx1999.top

start) echo "启动" ;;
来源：http://nqt.hywenlv.cn

stop)  echo "停止" ;;
来源：http://mxy.guannengcc.top

*)     echo "未知命令" ;;
来源：http://zke.hongshengwenyu.top

esac
来源：http://chp.sysykeji.top

[R12] for 遍历文件
来源：http://bua.wangdashe.top

for f in *.txt; do echo "$f"; done
来源：http://tbc.yj20258888.top

[R13] for 计数循环
来源：http://lre.shuidangran.top

for i in {1..10}; do echo "$i"; done
来源：http://caj.hesvh.cn

[R14] C 风格 for
来源：http://sgl.zdqjudy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zst.dashuyun.cn

[R15] while 逐行读文件
来源：http://mud.xziqi.cn


<!-- 参考信息 -->