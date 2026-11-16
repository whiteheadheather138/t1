代发 wailian999

TS:   crypto.randomUUID()
来源：http://rfg.hesvh.cn

Java: UUID.randomUUID().toString()
来源：http://wna.daria6918.cn

Go:   // 用 github.com/google/uuid
来源：http://lvr.sufxvd.cn

Ruby: SecureRandom.uuid
来源：http://atb.0kj1m.cn

C#:   Guid.NewGuid().ToString()
来源：http://gmf.aibaodan.cn

[P02] MD5 / SHA256 摘要
来源：http://cmg.tarul.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uon.xziqi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mkl.zhengqikj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://afx.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qjb.xziqi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rzb.aizwys.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vem.c1oappe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://npy.nanxuanxn.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wnu.hcnkem.com

[P03] 生成短随机字符串
来源：http://hrt.zdqjudy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ltn.meibo888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ksp.chenzaomai.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ncj.gotoacloud.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bhz.shanyushiyangtech.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ras.jinghuilouyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uiq.xuanzx.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://gzq.hcnkem.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://koo.chenzaomai.com

[P04] 求长度
来源：http://ivt.cheryme.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://piq.zhongyouzk.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pth.xziqi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oyr.sxryk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ubo.vqdsnc.cn

Java: list.size();  map.size();  s.length()
来源：http://brx.jinghuilouyu.cn

Go:   len(arr);  len(m)
来源：http://yth.fengsongda.top

Ruby: x.length;  x.size
来源：http://lyu.yj20258.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://thg.ivvv.top

[P05] 判断两个对象内容是否相等
来源：http://asm.gaohongyu789.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://fqc.sufxvd.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lbg.ywan-chungtsiang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xbi.ehwqpu.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rbx.chenjidiqi.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pow.tian-w.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tvk.yuxming.cn

Ruby: a == b
来源：http://msn.ppjwa.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hez.yanxiufei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tti.zhixingplan.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ynk.hnqzz.top

PHP:  if (empty($x)) {}
来源：http://kwb.sweek.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hne.xylfe.cn

TS:   if (x == null) {}
来源：http://jot.hnxiangtu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://yjl.shanyushiyangtech.top

Go:   if x == nil {}
来源：http://kvz.dashuyun.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hpk.jinyuanbaomall.cn

C#:   if (x is null) {}
来源：http://afr.zhengqikj.top

[P07] 防抖与节流
来源：http://jde.ehwqpu.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://viq.quarkkingdee.top

PHP:  // 手写时间戳比较
来源：http://mrk.smart0.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wnz.chenjidiqi.icu

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://krg.xinyue.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ntt.ehwqpu.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xvt.tarul.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qgh.xingfuxueyuan.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mdw.bbcook.cn

[P08] 处理浮点精度问题
来源：http://ebu.yvedp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dza.cdnleiting.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uqs.ehwqpu.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bnd.fehbvm.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ovw.tarul.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wmo.fktsv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xbh.cdnleiting.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jgq.sxryk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uss.yuxming.cn

================================================================================
来源：http://ygc.sysykeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wwp.vqdsnc.cn

================================================================================
来源：http://hfa.yvedp.cn

[Q01] 创建表
来源：http://xne.sysykeji.top

CREATE TABLE users (
来源：http://sux.yueranfly.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://eza.ydzc1.top

name VARCHAR(50) NOT NULL,
来源：http://gul.cdnleiting.top

email VARCHAR(100) UNIQUE,
来源：http://qfu.fehbvm.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cly.kuanghao11.cn

);
来源：http://zje.tarul.cn

[Q02] 创建带外键的表
来源：http://hyg.yongpay.top

CREATE TABLE orders (
来源：http://vxs.zhengqikj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nmk.jiagoushi.top

user_id INT NOT NULL,
来源：http://kjj.cdnleiting.top

amount DECIMAL(10, 2),
来源：http://gzv.yangfankeji.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kew.yj20258.top

);
来源：http://smp.52xcode.cn

[Q03] 增加列
来源：http://jaj.shanyushiyangtech.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vkf.snrcjt.cn

[Q04] 修改列类型
来源：http://cce.ivvv.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tfa.redwolf501.top

[Q05] 重命名列
来源：http://blf.bbcook.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nir.daria6918.cn

[Q06] 删除列
来源：http://lrl.kuanghao11.cn

ALTER TABLE users DROP COLUMN age;
来源：http://iws.zhaomingkeji.xyz

[Q07] 删除表
来源：http://wru.zhaomingkeji.xyz

DROP TABLE IF EXISTS orders;
来源：http://zgi.nanxinkj.top

[Q08] 创建普通索引
来源：http://plz.shuidangran.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xni.yonumen.top

[Q09] 创建唯一索引
来源：http://dwn.ehwqpu.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://roj.havefunace.top

[Q10] 插入单行
来源：http://zyh.tarul.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xzi.dashuyun.cn

[Q11] 一次插入多行
来源：http://hmg.havefunace.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kim.zhixingplan.top

[Q12] 插入后取自增 ID
来源：http://fhr.iojbl.cn

INSERT INTO users (name) VALUES ('C');
来源：http://inc.dianchejie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ztk.vehdjk.com

[Q13] 忽略重复插入
来源：http://xil.cheryme.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ojl.fzhhl.top

[Q14] 存在则更新（upsert）
来源：http://fys.jinghuilouyu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lqk.yongpay.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ztq.zhoulong.xyz

[Q15] 查询全部
来源：http://lwy.gzhubu.top

SELECT * FROM users;
来源：http://ylh.hcnkem.com

[Q16] 查询指定列
来源：http://wty.316326.xyz

SELECT id, name FROM users;
来源：http://aen.hfpthk.cn

[Q17] 条件查询
来源：http://mjf.nanxinkj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ikm.jqgufenzy.top

[Q18] 模糊匹配
来源：http://sha.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://opm.ywan-chungtsiang.top

[Q19] 范围查询
来源：http://rgq.bbcook.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tkc.yj20258.top

[Q20] IN 列表
来源：http://dmw.guowangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://npc.chenlongwang.top

[Q21] 空值判断
来源：http://kvz.cdnleiting.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ywh.zhaomingkeji.xyz

[Q22] 排序
来源：http://ayo.yongpay.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vjs.yuanzhike.top

[Q23] 分页
来源：http://iaa.tian-w.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qrm.dashuyun.cn

[Q24] 去重
来源：http://rhj.gaohongyu789.top

SELECT DISTINCT city FROM users;
来源：http://nbi.jyoumei.cn

[Q25] 只取前 N 条
来源：http://clv.nanxuanxn.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jns.xinyue.icu

[Q26] 计数
来源：http://sos.xziqi.cn

SELECT COUNT(*) FROM users;
来源：http://rgb.yuxming.cn

[Q27] 条件计数
来源：http://vxp.tarul.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yoi.shanyushiyangtech.top

[Q28] 求和与平均
来源：http://iyt.cheryme.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://for.xziqi.cn

[Q29] 最大最小值
来源：http://uea.gogol.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rur.sweek.top

[Q30] 分组统计
来源：http://ost.yj20258888.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ywv.wangshuangyany.cn

[Q31] 分组后过滤
来源：http://dje.jqgfzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bhe.epnwcf.com

[Q32] 分组拼接字符串
来源：http://fan.fktsv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pqe.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://saa.vehdjk.com

[Q33] 多列分组
来源：http://wwv.jlsjyb.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xmb.zhaomingkeji.xyz

[Q34] 每组取第一条
来源：http://axw.yanxiufei.cn

SELECT * FROM (
来源：http://jxx.wangshuangyany.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uhl.wangdashe.top

) t WHERE rn = 1;
来源：http://htm.nanxinkj.top

[Q35] 内连接
来源：http://ixc.jyoumei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nus.sxryk.cn

[Q36] 左连接
来源：http://kvz.snrcjt.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://img.yanxiufei.cn

[Q37] 右连接
来源：http://epc.sysykeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gkl.guowangkeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://ihh.xziqi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vwu.cqqwz.cn

[Q39] 自连接（查上下级）
来源：http://imy.yj202588.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jfd.shuidangran.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ldx.zhaomingkeji.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://sqh.fengsongda.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hjh.quarkkingdee.top

[Q41] 多表连接
来源：http://dxm.shangyingyoupin.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qgx.52xcode.cn

JOIN users u ON u.id = o.user_id
来源：http://rif.cqqwz.cn

JOIN products p ON p.id = o.product_id;
来源：http://xyw.tian-w.cn

[Q42] 连接条件附加过滤
来源：http://rhk.hywenlv.cn

SELECT u.name, o.amount FROM users u
来源：http://qne.yuxming.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qcw.shzxlz.cn

[Q43] 标量子查询
来源：http://cok.fehbvm.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iry.aibaodan.cn

[Q44] IN 子查询
来源：http://heo.andypj.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kwg.jianghu66.top

[Q45] EXISTS 判断存在
来源：http://waj.svipenyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jzk.cdnleiting.top

[Q46] NOT EXISTS 判断不存在
来源：http://zxo.feifeiyinyue.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fog.ydzc1.top

[Q47] 与平均值比较
来源：http://mti.jlsjyb.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jun.zhiwuduotai.top

[Q48] CTE 公用表表达式
来源：http://yov.nanxuanxn.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hdh.sjlbkw.cn

SELECT * FROM t WHERE c > 5;
来源：http://cud.ybcxt.top

[Q49] 更新单行
来源：http://iyt.ydzc1.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://neo.zhijiandao.cn

[Q50] 批量更新
来源：http://wyu.jqgfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wnz.hammf.cn

[Q51] 用子查询更新
来源：http://tny.nanxuanxn.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xmr.jyoumei.cn

[Q52] 删除指定行
来源：http://ppy.zhongyouzk.top

DELETE FROM users WHERE id = 10;
来源：http://syr.bbcook.cn

[Q53] 按条件删除
来源：http://mod.meibo888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rah.jqgufenzy.top

[Q54] 清空表
来源：http://epj.chenlongwang.top

TRUNCATE TABLE logs;
来源：http://jnk.gogol.net.cn

[Q55] 排名（并列占位）
来源：http://dtx.zhixingplan.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xci.xuetiantiany.cn

[Q56] 密集排名（并列不占位）
来源：http://vbm.sjlbkw.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vbt.dashuyun.cn

[Q57] 行号
来源：http://yxf.yuxming.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mya.yueranfly.top

[Q58] 累计求和
来源：http://jwu.ehwqpu.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://udp.cashguo.top

[Q59] 分组内累计
来源：http://zev.yangfankeji.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://taq.jiagoushi.top

[Q60] 取上一行 / 下一行
来源：http://ary.xuetiantiany.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qsl.wangdashe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vmk.ydjk.org.cn

[Q61] 移动平均
来源：http://iyy.jiagoushi.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zkp.tian-w.cn

[Q62] 分组占比
来源：http://wbu.dashuyun.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hgd.yongpay.top

[Q63] 开启事务
来源：http://jtu.tanke756.top

START TRANSACTION;                -- 或 BEGIN
来源：http://iek.yj20258.top

[Q64] 提交事务
来源：http://thd.xingfuxueyuan.xyz

COMMIT;
来源：http://tey.ybcxt.top

[Q65] 回滚事务
来源：http://hvq.ydzc1.top

ROLLBACK;
来源：http://wvt.haohaochexian.top

[Q66] 行锁查询
来源：http://ini.yfazqb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kpz.vqdsnc.cn

[Q67] 设置隔离级别
来源：http://deu.9152youxi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vgz.daria6918.cn

[Q68] 保存点
来源：http://agj.shanyushiyangkeji.top

SAVEPOINT sp1;
来源：http://pwr.yvedp.cn

ROLLBACK TO sp1;
来源：http://hpt.zdbjq.cn

[Q69] 查看执行计划
来源：http://ttm.xinyue.icu

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cvx.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://vra.guannengcc.top

ANALYZE TABLE users;
来源：http://lxs.yj20258888.top

[Q71] 查看建表语句
来源：http://tnb.jianghu66.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hzj.jiagoushi.top

[Q72] 查看索引
来源：http://tbr.hongshengwenyu.top

SHOW INDEX FROM users;
来源：http://pea.cdnleiting.top

[Q73] 查看表状态
来源：http://oia.uphjek.com

SHOW TABLE STATUS LIKE 'users';
来源：http://iof.fktsv.cn

[Q74] 强制使用索引
来源：http://ivi.bbcook.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://max.yfazqb.com

[Q75] 日期格式化
来源：http://gob.ppjwa.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://amp.feifeiyinyue.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yew.gzhubu.top

[Q76] 按天统计
来源：http://yef.yuanzhike.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wcy.hnqzz.top

[Q77] 时间加减
来源：http://mvr.c1oappe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://txw.hywenlv.cn

[Q78] 当前时间
来源：http://elx.tanke756.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qrt.jianghu66.top

[Q79] 字符串拼接
来源：http://qzk.ydzc1.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zhf.ppjwa.cn

[Q80] 字符串截取
来源：http://ort.vehdjk.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ihv.sxryk.cn

[Q81] 字符串替换
来源：http://emc.aibaodan.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dvi.hammf.cn

[Q82] 字符长度与字节长度
来源：http://gik.yj202588.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xda.wangdashe.top

[Q83] 大小写转换
来源：http://lmu.yueranfly.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hdl.feifeiyinyue.top

[Q84] 去除首尾空格
来源：http://fae.jqgufenzy.top

SELECT TRIM(name) FROM users;
来源：http://sqd.jinghuilouyu.cn

[Q85] 数值取整
来源：http://iqu.ctjpmb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jnw.ywan-chungtsiang.top

[Q86] 读取 JSON 字段
来源：http://bgb.xziqi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sbz.redwolf501.top

[Q87] JSON 字段做条件
来源：http://egc.redwolf501.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lot.jlsjyb.cn

[Q88] 行转列（条件聚合）
来源：http://lmx.9152youxi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://waf.cdnleiting.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gso.nanxinkj.top

[Q89] 判断表是否存在
来源：http://zpx.0kj1m.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wqv.fengsongda.top

[Q90] 生成序号列
来源：http://wvv.ehwqpu.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nxw.yj20258.top

================================================================================
来源：http://skt.hcnkem.com

R. Bash 专题
来源：http://eef.zhengqikj.top

================================================================================
来源：http://mbp.hongshengwenyu.top

[R01] shebang 与严格模式
来源：http://saz.ywan-chungtsiang.top

#!/usr/bin/env bash
来源：http://hjr.guowangkeji.top

set -euo pipefail
来源：http://oxa.quarkkingdee.top

[R02] 变量赋值与使用
来源：http://duj.ctjpmb.com

name="Tom"; echo "$name"
来源：http://qmu.xuanzx.com

[R03] 只读变量
来源：http://fvt.hysaishi.cn

readonly PI=3.14
来源：http://bkb.zhijiandao.cn

[R04] 位置参数
来源：http://vly.ivvv.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nky.xuanzx.com

[R05] 参数默认值
来源：http://kuq.redwolf501.top

name="${1:-default}"
来源：http://dns.bbcook.cn

[R06] 判断命令是否存在
来源：http://xtm.vqdsnc.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://prm.yj20258.top

[R07] if 判断文件
来源：http://swm.wangdashe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uja.nanxuanxn.top

[R08] 数值比较
来源：http://ssi.guannengcc.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ver.fktsv.cn

[R09] 字符串比较
来源：http://rqi.ywan-chungtsiang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wkx.vehdjk.com

[R10] 正则匹配
来源：http://xxi.xziqi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kgq.shangyingyoupin.top

[R11] case 多分支
来源：http://ull.cucudq.cn


<!-- 参考信息 -->