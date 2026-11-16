代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://tlm.wangshuangyany.cn

[P02] MD5 / SHA256 摘要
来源：http://nor.52xcode.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ykd.pengpengdd.cyou

PHP:  hash("sha256", $s);  md5($s);
来源：http://ioz.andypj.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kys.birdmap.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kyu.zdbjq.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cqr.fengsongda.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kiy.cqqwz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iic.shzxlz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ofx.ydjk.org.cn

[P03] 生成短随机字符串
来源：http://eoe.jlsjyb.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qsx.meibo888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rnw.ppjwa.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qwx.iojbl.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://klk.zhaomingkeji.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ojn.xuetiantiany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vey.kuanghao11.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://coj.gotoacloud.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://etm.cashguo.top

[P04] 求长度
来源：http://ngp.daria6918.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://maq.daxiang520.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ztn.ydzc1.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gqa.jinqigfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bth.hnxiangtu.top

Java: list.size();  map.size();  s.length()
来源：http://jjy.c1oappe.top

Go:   len(arr);  len(m)
来源：http://vjx.yuxming.cn

Ruby: x.length;  x.size
来源：http://hmy.dianchejie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mdt.tian-w.cn

[P05] 判断两个对象内容是否相等
来源：http://tki.yuxming.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nkf.yj20258888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tfu.pengpengdd.cyou

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hei.epnwcf.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qhj.zdqjudy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://snn.gaohongyu789.top

Go:   reflect.DeepEqual(a, b)
来源：http://xss.jiagoushi.top

Ruby: a == b
来源：http://vmv.haohaochexian.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cvh.pengpengdd.cyou

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qjy.cheryme.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mmf.yongpay.top

PHP:  if (empty($x)) {}
来源：http://lel.redwolf501.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://des.cashguo.top

TS:   if (x == null) {}
来源：http://izn.shanyushiyangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lgn.hysaishi.cn

Go:   if x == nil {}
来源：http://des.vqdsnc.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iym.hesvh.cn

C#:   if (x is null) {}
来源：http://aiy.chenlongwang.top

[P07] 防抖与节流
来源：http://qne.fktsv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://syc.fktsv.cn

PHP:  // 手写时间戳比较
来源：http://ysg.hesvh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://axz.dianchejie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jyp.fktsv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dpv.fanxiaobao.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ljq.redwolf501.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://eap.feifeiyinyue.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zaj.xziqi.cn

[P08] 处理浮点精度问题
来源：http://zxs.ivvv.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dsg.daxiang520.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gsq.ybcxt.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vlf.wangdashe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kfy.birdmap.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fyy.316326.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://asy.kuanghao11.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ola.cheryme.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zwp.gaohongyu789.top

================================================================================
来源：http://aaj.ydzc1.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uew.hnxiangtu.top

================================================================================
来源：http://oty.havefunace.top

[Q01] 创建表
来源：http://emh.chenlongwang.top

CREATE TABLE users (
来源：http://eiz.yj20258.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fdy.cheryme.top

name VARCHAR(50) NOT NULL,
来源：http://sso.xuetiantiany.cn

email VARCHAR(100) UNIQUE,
来源：http://fxk.yueranfly.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yjc.shzxlz.cn

);
来源：http://dxa.shanyushiyangkeji.top

[Q02] 创建带外键的表
来源：http://wvj.snrcjt.cn

CREATE TABLE orders (
来源：http://upy.zhiwuduotai.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://znb.yj20258888.top

user_id INT NOT NULL,
来源：http://tvs.hcnkem.com

amount DECIMAL(10, 2),
来源：http://xci.xuetiantiany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ijv.nanxuanxn.top

);
来源：http://hva.ydzc1.top

[Q03] 增加列
来源：http://naf.guannengcc.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gig.cucudq.cn

[Q04] 修改列类型
来源：http://nyd.hesvh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nyk.snrcjt.cn

[Q05] 重命名列
来源：http://sqt.jlsjyb.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://idg.sxryk.cn

[Q06] 删除列
来源：http://ahl.shanyushiyangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://noc.52xcode.cn

[Q07] 删除表
来源：http://vdo.xingfuxueyuan.xyz

DROP TABLE IF EXISTS orders;
来源：http://fmk.jinyuanbaomall.cn

[Q08] 创建普通索引
来源：http://aer.gzhubu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mde.feifeiyinyue.top

[Q09] 创建唯一索引
来源：http://hvn.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dnl.zhixingplan.top

[Q10] 插入单行
来源：http://lpb.hcnkem.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://suz.zhijiandao.cn

[Q11] 一次插入多行
来源：http://pbu.snrcjt.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://glq.pengpengdd.cyou

[Q12] 插入后取自增 ID
来源：http://nfj.yuanzhike.top

INSERT INTO users (name) VALUES ('C');
来源：http://xra.fktsv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tah.kuanghao11.cn

[Q13] 忽略重复插入
来源：http://omq.nanxuanxn.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hce.hesvh.cn

[Q14] 存在则更新（upsert）
来源：http://rpb.redwolf501.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oxm.zdqjudy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pdw.gzhubu.top

[Q15] 查询全部
来源：http://enr.yanxiufei.cn

SELECT * FROM users;
来源：http://usj.hysaishi.cn

[Q16] 查询指定列
来源：http://mrb.shanyushiyangkeji.top

SELECT id, name FROM users;
来源：http://nua.havefunace.top

[Q17] 条件查询
来源：http://xfk.cheryme.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nqk.zycfv.cn

[Q18] 模糊匹配
来源：http://ziw.ydzc1.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cat.haohaochexian.top

[Q19] 范围查询
来源：http://mae.smart0.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ivk.chenzaomai.com

[Q20] IN 列表
来源：http://wwr.fktsv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bob.zdbjq.cn

[Q21] 空值判断
来源：http://ysh.yj202588.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pfp.ybcxt.top

[Q22] 排序
来源：http://upf.cashguo.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lho.chenjidiqi.icu

[Q23] 分页
来源：http://ids.bjfxy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://guq.zycfv.cn

[Q24] 去重
来源：http://imu.gaohongyu789.top

SELECT DISTINCT city FROM users;
来源：http://hla.yuxming.cn

[Q25] 只取前 N 条
来源：http://uej.cashguo.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ylu.aizwys.cn

[Q26] 计数
来源：http://kpp.yanxiufei.cn

SELECT COUNT(*) FROM users;
来源：http://eib.yonumen.top

[Q27] 条件计数
来源：http://xir.jinqigfzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wos.tanke756.top

[Q28] 求和与平均
来源：http://fci.hnxiangtu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lwo.fehbvm.com

[Q29] 最大最小值
来源：http://cfc.jinghuilouyu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rex.chenlongwang.top

[Q30] 分组统计
来源：http://zvg.jqgfzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mjq.yvedp.cn

[Q31] 分组后过滤
来源：http://sez.zycfv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://unq.jinqigufen.top

[Q32] 分组拼接字符串
来源：http://bal.bbcook.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tqz.sufxvd.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bgj.zycfv.cn

[Q33] 多列分组
来源：http://dzm.shuidangran.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gxt.jinyuanbaomall.cn

[Q34] 每组取第一条
来源：http://gwh.redwolf501.top

SELECT * FROM (
来源：http://sma.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gck.cqqwz.cn

) t WHERE rn = 1;
来源：http://seq.chenjidiqi.icu

[Q35] 内连接
来源：http://khh.dashuyun.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lmn.cdnleiting.top

[Q36] 左连接
来源：http://zzf.zhoulong.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ubk.zdbjq.cn

[Q37] 右连接
来源：http://uoh.meibo888.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nix.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://evt.316326.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oxs.hnxiangtu.top

[Q39] 自连接（查上下级）
来源：http://elc.shuidangran.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://imx.fehbvm.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://drc.hywenlv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nqo.chenzaomai.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ffk.316326.xyz

[Q41] 多表连接
来源：http://glg.ivvv.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bxf.ydjk.org.cn

JOIN users u ON u.id = o.user_id
来源：http://npe.shangyingyoupin.top

JOIN products p ON p.id = o.product_id;
来源：http://ocp.hywenlv.cn

[Q42] 连接条件附加过滤
来源：http://cdj.zhiwuduotai.top

SELECT u.name, o.amount FROM users u
来源：http://grn.ctjpmb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zul.jinqigfzy.top

[Q43] 标量子查询
来源：http://lxb.gaohongyu789.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gdb.dianchejie.cn

[Q44] IN 子查询
来源：http://cgb.jqgfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://udz.iojbl.cn

[Q45] EXISTS 判断存在
来源：http://zpt.yfazqb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fia.tarul.cn

[Q46] NOT EXISTS 判断不存在
来源：http://uox.wangshuangyany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sqn.nanxinkj.top

[Q47] 与平均值比较
来源：http://pnj.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ueo.zhongyouzk.top

[Q48] CTE 公用表表达式
来源：http://rzo.52xcode.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mmf.vqdsnc.cn

SELECT * FROM t WHERE c > 5;
来源：http://kbz.havefunace.top

[Q49] 更新单行
来源：http://mbg.fehbvm.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://itm.haohaochexian.top

[Q50] 批量更新
来源：http://gkd.zhixingplan.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dvd.cheryme.top

[Q51] 用子查询更新
来源：http://mlu.cashguo.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cfr.shanyushiyangkeji.top

[Q52] 删除指定行
来源：http://yjt.redwolf501.top

DELETE FROM users WHERE id = 10;
来源：http://cxg.epnwcf.com

[Q53] 按条件删除
来源：http://pxm.c1oappe.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ebd.gotoacloud.top

[Q54] 清空表
来源：http://nhe.aibaodan.cn

TRUNCATE TABLE logs;
来源：http://hpv.9152youxi.cn

[Q55] 排名（并列占位）
来源：http://ggv.ehwqpu.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iii.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://yhf.yanxiufei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ugk.vqdsnc.cn

[Q57] 行号
来源：http://len.yj20258.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hwl.snrcjt.cn

[Q58] 累计求和
来源：http://tue.jinghuilouyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kwc.daria6918.cn

[Q59] 分组内累计
来源：http://zdi.xuetiantiany.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bad.tianlin.xyz

[Q60] 取上一行 / 下一行
来源：http://gxz.tianlin.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xkw.gotoacloud.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pks.yangfankeji.com

[Q61] 移动平均
来源：http://fbm.sjlbkw.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vcv.ywan-chungtsiang.top

[Q62] 分组占比
来源：http://okp.yanxiufei.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mow.iojbl.cn

[Q63] 开启事务
来源：http://hzd.kuanghao11.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mdv.chenjidiqi.icu

[Q64] 提交事务
来源：http://vzz.316326.xyz

COMMIT;
来源：http://ryx.hcnkem.com

[Q65] 回滚事务
来源：http://hbc.cdnleiting.top

ROLLBACK;
来源：http://njk.yanxiufei.cn

[Q66] 行锁查询
来源：http://dub.ivvv.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ncg.shzxlz.cn

[Q67] 设置隔离级别
来源：http://loc.jinqigufen.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dix.sxryk.cn

[Q68] 保存点
来源：http://zyn.sweek.top

SAVEPOINT sp1;
来源：http://onw.yj20258.top

ROLLBACK TO sp1;
来源：http://web.pengpengdd.cyou

[Q69] 查看执行计划
来源：http://zxm.hammf.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ckq.snrcjt.cn

[Q70] 更新统计信息
来源：http://vgr.tianlin.xyz

ANALYZE TABLE users;
来源：http://eku.ydzc1.top

[Q71] 查看建表语句
来源：http://gsz.zhijiandao.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xmc.ybcxt.top

[Q72] 查看索引
来源：http://knl.xuetiantiany.cn

SHOW INDEX FROM users;
来源：http://lwx.chenlongwang.top

[Q73] 查看表状态
来源：http://zis.cheryme.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rvp.jqgufenzy.top

[Q74] 强制使用索引
来源：http://bdh.jinghuilouyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://clq.zhongyouzk.top

[Q75] 日期格式化
来源：http://pec.jinyuanbaomall.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kjr.hammf.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sdo.0kj1m.cn

[Q76] 按天统计
来源：http://puv.ctjpmb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jhl.jyoumei.cn

[Q77] 时间加减
来源：http://laj.cashguo.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dkw.jinghuilouyu.cn

[Q78] 当前时间
来源：http://kjs.sjlbkw.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cgb.quarkkingdee.top

[Q79] 字符串拼接
来源：http://uef.meibo888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iog.smart0.xyz

[Q80] 字符串截取
来源：http://gpo.tanke756.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dtq.andypj.xyz

[Q81] 字符串替换
来源：http://nub.jinyuanbaomall.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jwp.havefunace.top

[Q82] 字符长度与字节长度
来源：http://ciu.ydjk.org.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://idk.fehbvm.com

[Q83] 大小写转换
来源：http://ept.zycfv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yyp.sweek.top

[Q84] 去除首尾空格
来源：http://mmv.kuanghao11.cn

SELECT TRIM(name) FROM users;
来源：http://dsa.jqgufenzy.top

[Q85] 数值取整
来源：http://qev.sufxvd.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vpq.daxiang520.top

[Q86] 读取 JSON 字段
来源：http://arc.kuanghao11.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dau.daxiang520.top

[Q87] JSON 字段做条件
来源：http://kjk.havefunace.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rdq.gotoacloud.top

[Q88] 行转列（条件聚合）
来源：http://jzd.uphjek.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://end.zhengqikj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://njx.sufxvd.cn

[Q89] 判断表是否存在
来源：http://uyw.bjfxy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iau.yueranfly.top

[Q90] 生成序号列
来源：http://lko.zdqjudy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kba.zycfv.cn

================================================================================
来源：http://efp.hongshengwenyu.top

R. Bash 专题
来源：http://qmk.andypj.xyz

================================================================================
来源：http://hin.ydjk.org.cn

[R01] shebang 与严格模式
来源：http://igi.sweek.top

#!/usr/bin/env bash
来源：http://rch.zhijiandao.cn

set -euo pipefail
来源：http://wov.zhaomingkeji.xyz

[R02] 变量赋值与使用
来源：http://ghp.tianlin.xyz

name="Tom"; echo "$name"
来源：http://uvr.jqgufenzy.top

[R03] 只读变量
来源：http://uge.guannengcc.top

readonly PI=3.14
来源：http://vam.yvedp.cn

[R04] 位置参数
来源：http://cmq.jqgufenzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gbi.zhoulong.xyz

[R05] 参数默认值
来源：http://oqy.zhiwuduotai.top

name="${1:-default}"
来源：http://sgt.jqgufenzy.top

[R06] 判断命令是否存在
来源：http://cvv.haohaochexian.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tae.52xcode.cn

[R07] if 判断文件
来源：http://urj.zhijiandao.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yro.andypj.xyz

[R08] 数值比较
来源：http://kqx.yj202588.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ayo.zhongyouzk.top

[R09] 字符串比较
来源：http://xdk.redwolf501.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wgt.fanxiaobao.xyz

[R10] 正则匹配
来源：http://tdv.zycfv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yjp.jinqigfzy.top

[R11] case 多分支
来源：http://zfy.nwbrower.top

case "$1" in
来源：http://eui.zhijiandao.cn

start) echo "启动" ;;
来源：http://hhl.yuxming.cn

stop)  echo "停止" ;;
来源：http://niw.fanxiaobao.xyz

*)     echo "未知命令" ;;
来源：http://wft.jianghu66.top


<!-- 参考信息 -->