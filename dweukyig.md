代发 wailian999

[P01] 生成 UUID
来源：http://xmr.xylfe.cn

Py:   str(uuid.uuid4())
来源：http://hse.chenzaomai.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fnh.jinqigufen.top

JS:   crypto.randomUUID()
来源：http://rnw.jqgufenzy.top

TS:   crypto.randomUUID()
来源：http://vsd.sweek.top

Java: UUID.randomUUID().toString()
来源：http://gny.mhx1999.top

Go:   // 用 github.com/google/uuid
来源：http://qru.cdnleiting.top

Ruby: SecureRandom.uuid
来源：http://gne.yueranfly.top

C#:   Guid.NewGuid().ToString()
来源：http://iuf.hysaishi.cn

[P02] MD5 / SHA256 摘要
来源：http://rmj.xingfuxueyuan.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://adv.hammf.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mjy.ctjpmb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tkv.hnxiangtu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vje.ywan-chungtsiang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ywi.andypj.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cdu.wangshuangyany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cjq.hfpthk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://chk.316326.xyz

[P03] 生成短随机字符串
来源：http://lxg.cdnleiting.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://imw.havefunace.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zcf.iojbl.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vfx.meibo888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pha.jinqigufen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nsj.dianchejie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vpu.fengsongda.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://iwx.cdnleiting.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qnr.jinghuilouyu.cn

[P04] 求长度
来源：http://agm.svipenyu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rhz.guowangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ylx.yueranfly.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lhv.iojbl.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aag.ppjwa.cn

Java: list.size();  map.size();  s.length()
来源：http://pde.wangdashe.top

Go:   len(arr);  len(m)
来源：http://qmd.dianchejie.cn

Ruby: x.length;  x.size
来源：http://hmu.nanxuanxn.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pey.sjlbkw.cn

[P05] 判断两个对象内容是否相等
来源：http://tuw.yueranfly.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://cuj.jinghuilouyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rwg.yvedp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ysf.snrcjt.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fij.cdnleiting.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vva.pycfn.com

Go:   reflect.DeepEqual(a, b)
来源：http://dak.xuetiantiany.cn

Ruby: a == b
来源：http://fyz.yj20258888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ivn.yj202588.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zne.zycfv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ies.smart0.xyz

PHP:  if (empty($x)) {}
来源：http://sqc.aibaodan.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dta.havefunace.top

TS:   if (x == null) {}
来源：http://xee.jinghuilouyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fbt.yuanzhike.top

Go:   if x == nil {}
来源：http://enz.jiagoushi.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ujb.gaohongyu789.top

C#:   if (x is null) {}
来源：http://ibk.yfazqb.com

[P07] 防抖与节流
来源：http://yml.jinqigfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mug.epnwcf.com

PHP:  // 手写时间戳比较
来源：http://qvj.yj20258.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pkt.ctjpmb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wnp.guowangkeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bez.jiagoushi.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oiz.dianchejie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ohl.hywenlv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://swx.yj20258.top

[P08] 处理浮点精度问题
来源：http://cnb.jqgufenzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hgc.shangyingyoupin.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dvd.ybcxt.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ptq.chenzaomai.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://omm.dianchejie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://khr.yuxming.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sww.sufxvd.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ctc.c1oappe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ngp.guowangkeji.top

================================================================================
来源：http://piw.xziqi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mvo.0kj1m.cn

================================================================================
来源：http://edk.xziqi.cn

[Q01] 创建表
来源：http://gej.pycfn.com

CREATE TABLE users (
来源：http://cbm.jlsjyb.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nao.birdmap.top

name VARCHAR(50) NOT NULL,
来源：http://ilf.hysaishi.cn

email VARCHAR(100) UNIQUE,
来源：http://cps.yanxiufei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qbx.jinghuilouyu.cn

);
来源：http://yir.xziqi.cn

[Q02] 创建带外键的表
来源：http://kjb.yj202588.top

CREATE TABLE orders (
来源：http://fvr.xingfuxueyuan.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ocb.kuanghao11.cn

user_id INT NOT NULL,
来源：http://qvu.havefunace.top

amount DECIMAL(10, 2),
来源：http://zeo.yfazqb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qea.52xcode.cn

);
来源：http://iqo.yonumen.top

[Q03] 增加列
来源：http://syt.wangshuangyany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lvt.zdqjudy.top

[Q04] 修改列类型
来源：http://ram.shangyingyoupin.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://coc.jinqigfzy.top

[Q05] 重命名列
来源：http://bbc.ivvv.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://snd.hywenlv.cn

[Q06] 删除列
来源：http://qfh.yuanzhike.top

ALTER TABLE users DROP COLUMN age;
来源：http://imh.svipenyu.cn

[Q07] 删除表
来源：http://bsh.0kj1m.cn

DROP TABLE IF EXISTS orders;
来源：http://eyk.zhengqikj.top

[Q08] 创建普通索引
来源：http://jci.gogol.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mpc.yongpay.top

[Q09] 创建唯一索引
来源：http://qox.aibaodan.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cny.epnwcf.com

[Q10] 插入单行
来源：http://ghi.aibaodan.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xbc.svipenyu.cn

[Q11] 一次插入多行
来源：http://nfi.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dmq.vqdsnc.cn

[Q12] 插入后取自增 ID
来源：http://gly.pycfn.com

INSERT INTO users (name) VALUES ('C');
来源：http://dbe.xingfuxueyuan.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mzz.zhijiandao.cn

[Q13] 忽略重复插入
来源：http://goz.shangyingyoupin.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bzk.vehdjk.com

[Q14] 存在则更新（upsert）
来源：http://ecd.vehdjk.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mvo.ybcxt.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jwp.hysaishi.cn

[Q15] 查询全部
来源：http://jxi.zhoulong.xyz

SELECT * FROM users;
来源：http://fpo.mhx1999.top

[Q16] 查询指定列
来源：http://zdx.iojbl.cn

SELECT id, name FROM users;
来源：http://mie.daria6918.cn

[Q17] 条件查询
来源：http://xrs.fzhhl.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oao.jyoumei.cn

[Q18] 模糊匹配
来源：http://nry.nanxinkj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iug.yangfankeji.com

[Q19] 范围查询
来源：http://nnh.meibo888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://utn.shuidangran.top

[Q20] IN 列表
来源：http://tur.fktsv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mng.c1oappe.top

[Q21] 空值判断
来源：http://obk.ywan-chungtsiang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://fsd.xuanzx.com

[Q22] 排序
来源：http://onx.haohaochexian.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eaj.ivvv.top

[Q23] 分页
来源：http://evk.zdqjudy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://msp.nanxinkj.top

[Q24] 去重
来源：http://vbg.vehdjk.com

SELECT DISTINCT city FROM users;
来源：http://sia.gaohongyu789.top

[Q25] 只取前 N 条
来源：http://hro.ydjk.org.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qkj.zhijiandao.cn

[Q26] 计数
来源：http://wld.zhongyouzk.top

SELECT COUNT(*) FROM users;
来源：http://ngh.bbcook.cn

[Q27] 条件计数
来源：http://fvz.shuidangran.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pzw.zhengqikj.top

[Q28] 求和与平均
来源：http://pol.sjlbkw.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sed.havefunace.top

[Q29] 最大最小值
来源：http://sqj.shanyushiyangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xeh.jlsjyb.cn

[Q30] 分组统计
来源：http://wtr.xylfe.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rzg.birdmap.top

[Q31] 分组后过滤
来源：http://btu.jinqigufen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ify.zhaomingkeji.xyz

[Q32] 分组拼接字符串
来源：http://hqf.nwbrower.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nir.jinqigfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mye.bjfxy.top

[Q33] 多列分组
来源：http://ije.kuanghao11.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pux.nwbrower.top

[Q34] 每组取第一条
来源：http://dyk.hnqzz.top

SELECT * FROM (
来源：http://osn.shzxlz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://saa.chenlongwang.top

) t WHERE rn = 1;
来源：http://tes.nanxinkj.top

[Q35] 内连接
来源：http://hwm.dianchejie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zmn.xingfuxueyuan.xyz

[Q36] 左连接
来源：http://mad.guowangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://htj.xingfuxueyuan.xyz

[Q37] 右连接
来源：http://ccr.wangdashe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tqt.hnqzz.top

[Q38] 全外连接（PostgreSQL）
来源：http://vqq.sufxvd.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lul.ppjwa.cn

[Q39] 自连接（查上下级）
来源：http://jig.aizwys.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cpm.ehwqpu.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jml.hcnkem.com

[Q40] 交叉连接（笛卡尔积）
来源：http://ghg.aibaodan.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tmu.zhongyouzk.top

[Q41] 多表连接
来源：http://rcd.zhijiandao.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jkq.c1oappe.top

JOIN users u ON u.id = o.user_id
来源：http://vtk.jinqigfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://iwl.jinqigufen.top

[Q42] 连接条件附加过滤
来源：http://hmn.gaohongyu789.top

SELECT u.name, o.amount FROM users u
来源：http://ymy.zhiwuduotai.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xbr.aizwys.cn

[Q43] 标量子查询
来源：http://xjm.shangyingyoupin.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zpi.zhixingplan.top

[Q44] IN 子查询
来源：http://wdb.aibaodan.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tjj.fengsongda.top

[Q45] EXISTS 判断存在
来源：http://lxu.havefunace.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kcs.redwolf501.top

[Q46] NOT EXISTS 判断不存在
来源：http://uvh.zycfv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vjf.gotoacloud.top

[Q47] 与平均值比较
来源：http://qcl.xziqi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lqz.zhongyouzk.top

[Q48] CTE 公用表表达式
来源：http://whk.316326.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qor.jinyuanbaomall.cn

SELECT * FROM t WHERE c > 5;
来源：http://lmb.vehdjk.com

[Q49] 更新单行
来源：http://wfu.zhijiandao.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wdm.316326.xyz

[Q50] 批量更新
来源：http://tfc.shanyushiyangtech.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wvu.fengsongda.top

[Q51] 用子查询更新
来源：http://mmq.svipenyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gxf.yuanzhike.top

[Q52] 删除指定行
来源：http://znt.iojbl.cn

DELETE FROM users WHERE id = 10;
来源：http://lfx.cucudq.cn

[Q53] 按条件删除
来源：http://kyp.zhongyouzk.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bbw.c1oappe.top

[Q54] 清空表
来源：http://ych.hnxiangtu.top

TRUNCATE TABLE logs;
来源：http://zrc.fengsongda.top

[Q55] 排名（并列占位）
来源：http://gzo.birdmap.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ipt.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://mnf.yuxming.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fec.ppjwa.cn

[Q57] 行号
来源：http://syd.ehwqpu.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cwc.birdmap.top

[Q58] 累计求和
来源：http://rxx.ctjpmb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://smm.gzhubu.top

[Q59] 分组内累计
来源：http://rpb.shanyushiyangkeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ipl.cqqwz.cn

[Q60] 取上一行 / 下一行
来源：http://isj.sysykeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mhn.shzxlz.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://awb.kuanghao11.cn

[Q61] 移动平均
来源：http://ysp.yuxming.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sgk.bbcook.cn

[Q62] 分组占比
来源：http://aud.kuanghao11.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vhn.pengpengdd.cyou

[Q63] 开启事务
来源：http://xhy.yongpay.top

START TRANSACTION;                -- 或 BEGIN
来源：http://iqk.daxiang520.top

[Q64] 提交事务
来源：http://pbg.fengsongda.top

COMMIT;
来源：http://dzs.ehwqpu.com

[Q65] 回滚事务
来源：http://jjl.cheryme.top

ROLLBACK;
来源：http://vjg.zycfv.cn

[Q66] 行锁查询
来源：http://ktc.hammf.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wix.hesvh.cn

[Q67] 设置隔离级别
来源：http://fii.chenjidiqi.icu

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cmw.gogol.net.cn

[Q68] 保存点
来源：http://udc.jianghu66.top

SAVEPOINT sp1;
来源：http://ccv.cdnleiting.top

ROLLBACK TO sp1;
来源：http://hqn.feifeiyinyue.top

[Q69] 查看执行计划
来源：http://ujr.sufxvd.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xxi.nanxuanxn.top

[Q70] 更新统计信息
来源：http://wce.smart0.xyz

ANALYZE TABLE users;
来源：http://yxr.sjlbkw.cn

[Q71] 查看建表语句
来源：http://ixm.jqgufenzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wwu.svipenyu.cn

[Q72] 查看索引
来源：http://dcz.yangfankeji.com

SHOW INDEX FROM users;
来源：http://izt.hysaishi.cn

[Q73] 查看表状态
来源：http://mno.feifeiyinyue.top

SHOW TABLE STATUS LIKE 'users';
来源：http://uik.fzhhl.top

[Q74] 强制使用索引
来源：http://pyo.svipenyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yna.ybcxt.top

[Q75] 日期格式化
来源：http://bmv.guannengcc.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ynj.yvedp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fsz.gogol.net.cn

[Q76] 按天统计
来源：http://qrt.daxiang520.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wga.yuxming.cn

[Q77] 时间加减
来源：http://wcf.hesvh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jcc.kuanghao11.cn

[Q78] 当前时间
来源：http://knq.9152youxi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://acc.jinqigfzy.top

[Q79] 字符串拼接
来源：http://gxb.jyoumei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bmw.yongpay.top

[Q80] 字符串截取
来源：http://goi.hesvh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xkc.yuxming.cn

[Q81] 字符串替换
来源：http://bza.guannengcc.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pex.pengpengdd.cyou

[Q82] 字符长度与字节长度
来源：http://dal.daxiang520.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ikh.fanxiaobao.xyz

[Q83] 大小写转换
来源：http://fgn.yuanzhike.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xki.aibaodan.cn

[Q84] 去除首尾空格
来源：http://udy.daxiang520.top

SELECT TRIM(name) FROM users;
来源：http://efa.mhx1999.top

[Q85] 数值取整
来源：http://dyx.havefunace.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cyp.yj20258888.top

[Q86] 读取 JSON 字段
来源：http://rgm.yuanzhike.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vvt.wangdashe.top

[Q87] JSON 字段做条件
来源：http://dry.jyoumei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ctp.shuidangran.top

[Q88] 行转列（条件聚合）
来源：http://ufe.svipenyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ncy.jinqigufen.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://csv.fktsv.cn

[Q89] 判断表是否存在
来源：http://aol.xinyue.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://srs.ctjpmb.com

[Q90] 生成序号列
来源：http://vqd.wangdashe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bcl.ywan-chungtsiang.top

================================================================================
来源：http://abv.sysykeji.top

R. Bash 专题
来源：http://anj.kuanghao11.cn

================================================================================
来源：http://ajv.yuxming.cn

[R01] shebang 与严格模式
来源：http://rqb.guowangkeji.top

#!/usr/bin/env bash
来源：http://xfg.yj202588.top

set -euo pipefail
来源：http://ngf.jinyuanbaomall.cn

[R02] 变量赋值与使用
来源：http://kys.aibaodan.cn

name="Tom"; echo "$name"
来源：http://clb.redwolf501.top

[R03] 只读变量
来源：http://gja.hnxiangtu.top

readonly PI=3.14
来源：http://arr.yvedp.cn

[R04] 位置参数
来源：http://pgh.haohaochexian.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://swt.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://ifg.xuetiantiany.cn

name="${1:-default}"
来源：http://dez.wangdashe.top

[R06] 判断命令是否存在
来源：http://pai.ctjpmb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wck.hcnkem.com

[R07] if 判断文件
来源：http://igt.uphjek.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bzy.andypj.xyz

[R08] 数值比较
来源：http://rnp.jyoumei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dbq.sufxvd.cn

[R09] 字符串比较
来源：http://ppy.zdbjq.cn


<!-- 参考信息 -->