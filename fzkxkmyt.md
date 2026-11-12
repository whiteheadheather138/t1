代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://mpq.yanxiufei.cn

[P02] MD5 / SHA256 摘要
来源：http://yce.zhixingplan.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ubm.sweek.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fci.cheryme.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mog.jinyuanbaomall.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://waf.fanxiaobao.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gcd.yongpay.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cdm.bbcook.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nzy.hnqzz.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zva.tanke756.top

[P03] 生成短随机字符串
来源：http://pgg.sysykeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hsp.havefunace.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zgs.svipenyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lnb.jqgufenzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mgo.sufxvd.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://eei.zhiwuduotai.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nxz.fanxiaobao.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://zby.yfazqb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ahx.yvedp.cn

[P04] 求长度
来源：http://wis.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cfi.yj202588.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vjo.guannengcc.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pjf.xuetiantiany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dnr.bjfxy.top

Java: list.size();  map.size();  s.length()
来源：http://rub.cqqwz.cn

Go:   len(arr);  len(m)
来源：http://auc.guowangkeji.top

Ruby: x.length;  x.size
来源：http://hgo.yongpay.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ktp.jinyuanbaomall.cn

[P05] 判断两个对象内容是否相等
来源：http://gah.9152youxi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://eyn.dashuyun.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mol.jinqigfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dey.sysykeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fmu.chenjidiqi.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bne.havefunace.top

Go:   reflect.DeepEqual(a, b)
来源：http://fzy.hywenlv.cn

Ruby: a == b
来源：http://xkn.bjfxy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tqf.nwbrower.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://onm.gaohongyu789.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mml.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://cqh.ybcxt.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fiw.yvedp.cn

TS:   if (x == null) {}
来源：http://hju.yuanzhike.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ktf.snrcjt.cn

Go:   if x == nil {}
来源：http://day.jianghu66.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cpz.jiagoushi.top

C#:   if (x is null) {}
来源：http://ica.tanke756.top

[P07] 防抖与节流
来源：http://skq.mhx1999.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://his.pycfn.com

PHP:  // 手写时间戳比较
来源：http://mgt.xuetiantiany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bfv.daria6918.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fia.zhijiandao.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rsd.pycfn.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qjx.316326.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://gum.nwbrower.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jiw.jianghu66.top

[P08] 处理浮点精度问题
来源：http://dnn.vqdsnc.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fsv.jyoumei.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://oqq.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nmx.xingfuxueyuan.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://egg.jqgfzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://apn.jianghu66.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vkq.zhijiandao.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://akl.jinqigufen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ifb.jyoumei.cn

================================================================================
来源：http://rai.hfpthk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wkv.yongpay.top

================================================================================
来源：http://mpb.shangyingyoupin.top

[Q01] 创建表
来源：http://yis.kuanghao11.cn

CREATE TABLE users (
来源：http://nqx.hnxiangtu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hbi.feifeiyinyue.top

name VARCHAR(50) NOT NULL,
来源：http://icx.shuidangran.top

email VARCHAR(100) UNIQUE,
来源：http://erp.hammf.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xqr.wangdashe.top

);
来源：http://avd.xinyue.icu

[Q02] 创建带外键的表
来源：http://wsk.mhx1999.top

CREATE TABLE orders (
来源：http://jsx.yvedp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qgh.daxiang520.top

user_id INT NOT NULL,
来源：http://djg.daria6918.cn

amount DECIMAL(10, 2),
来源：http://lah.hysaishi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fqi.xylfe.cn

);
来源：http://svc.ehwqpu.com

[Q03] 增加列
来源：http://beu.zhaomingkeji.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ola.yfazqb.com

[Q04] 修改列类型
来源：http://xrv.ywan-chungtsiang.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pwa.vqdsnc.cn

[Q05] 重命名列
来源：http://sqw.haohaochexian.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ago.pycfn.com

[Q06] 删除列
来源：http://fbx.birdmap.top

ALTER TABLE users DROP COLUMN age;
来源：http://viz.cdnleiting.top

[Q07] 删除表
来源：http://xxt.xingfuxueyuan.xyz

DROP TABLE IF EXISTS orders;
来源：http://izh.wangshuangyany.cn

[Q08] 创建普通索引
来源：http://vtd.redwolf501.top

CREATE INDEX idx_users_email ON users(email);
来源：http://dwq.shzxlz.cn

[Q09] 创建唯一索引
来源：http://lif.hesvh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kko.daria6918.cn

[Q10] 插入单行
来源：http://ena.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uop.gzhubu.top

[Q11] 一次插入多行
来源：http://yqj.feifeiyinyue.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bqv.ybcxt.top

[Q12] 插入后取自增 ID
来源：http://qac.iojbl.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kpa.hesvh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cjq.yj20258888.top

[Q13] 忽略重复插入
来源：http://srm.hysaishi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mye.bbcook.cn

[Q14] 存在则更新（upsert）
来源：http://ray.shangyingyoupin.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xam.dianchejie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iov.aibaodan.cn

[Q15] 查询全部
来源：http://xje.guowangkeji.top

SELECT * FROM users;
来源：http://irf.hysaishi.cn

[Q16] 查询指定列
来源：http://gfg.dashuyun.cn

SELECT id, name FROM users;
来源：http://ygq.hongshengwenyu.top

[Q17] 条件查询
来源：http://xmj.bbcook.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://log.hesvh.cn

[Q18] 模糊匹配
来源：http://nnt.yuxming.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hxv.gaohongyu789.top

[Q19] 范围查询
来源：http://uoh.c1oappe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gsm.zhiwuduotai.top

[Q20] IN 列表
来源：http://myi.yj20258888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rib.jinqigfzy.top

[Q21] 空值判断
来源：http://zzi.gzhubu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xgd.hywenlv.cn

[Q22] 排序
来源：http://kdb.zycfv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://aza.yfazqb.com

[Q23] 分页
来源：http://obh.zdbjq.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rxi.ydjk.org.cn

[Q24] 去重
来源：http://sou.cashguo.top

SELECT DISTINCT city FROM users;
来源：http://svu.gotoacloud.top

[Q25] 只取前 N 条
来源：http://bgp.yueranfly.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sbw.nwbrower.top

[Q26] 计数
来源：http://nnz.yj202588.top

SELECT COUNT(*) FROM users;
来源：http://whu.nanxinkj.top

[Q27] 条件计数
来源：http://pql.cucudq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://czd.tarul.cn

[Q28] 求和与平均
来源：http://jvu.hnxiangtu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://grq.dianchejie.cn

[Q29] 最大最小值
来源：http://toi.zhongyouzk.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mfc.hammf.cn

[Q30] 分组统计
来源：http://yxm.zhijiandao.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jns.snrcjt.cn

[Q31] 分组后过滤
来源：http://kea.wangdashe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uer.jyoumei.cn

[Q32] 分组拼接字符串
来源：http://wnq.hysaishi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://onh.sxryk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lwa.xziqi.cn

[Q33] 多列分组
来源：http://zhu.jqgufenzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dzg.yonumen.top

[Q34] 每组取第一条
来源：http://kwd.dianchejie.cn

SELECT * FROM (
来源：http://lfp.zhijiandao.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xai.zdbjq.cn

) t WHERE rn = 1;
来源：http://nbe.gaohongyu789.top

[Q35] 内连接
来源：http://gil.haohaochexian.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bnc.jianghu66.top

[Q36] 左连接
来源：http://yoi.yongpay.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hnb.sjlbkw.cn

[Q37] 右连接
来源：http://seu.zycfv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yvt.ywan-chungtsiang.top

[Q38] 全外连接（PostgreSQL）
来源：http://nvh.xuanzx.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://skz.snrcjt.cn

[Q39] 自连接（查上下级）
来源：http://ndg.zhongyouzk.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ywt.mhx1999.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://srl.fktsv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://iou.jqgufenzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gzp.zdqjudy.top

[Q41] 多表连接
来源：http://akv.tanke756.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://dpi.daria6918.cn

JOIN users u ON u.id = o.user_id
来源：http://bek.xuetiantiany.cn

JOIN products p ON p.id = o.product_id;
来源：http://yav.hnxiangtu.top

[Q42] 连接条件附加过滤
来源：http://rir.chenjidiqi.icu

SELECT u.name, o.amount FROM users u
来源：http://xmh.jiagoushi.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ate.zhongyouzk.top

[Q43] 标量子查询
来源：http://dsn.ydjk.org.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xzk.gzhubu.top

[Q44] IN 子查询
来源：http://aem.jqgufenzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ziw.gogol.net.cn

[Q45] EXISTS 判断存在
来源：http://kiq.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://puu.zhoulong.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://ebm.yanxiufei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pxh.ybcxt.top

[Q47] 与平均值比较
来源：http://win.zhaomingkeji.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://awq.yuanzhike.top

[Q48] CTE 公用表表达式
来源：http://mcx.pengpengdd.cyou

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://abt.xylfe.cn

SELECT * FROM t WHERE c > 5;
来源：http://jzx.yongpay.top

[Q49] 更新单行
来源：http://zig.fanxiaobao.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ovg.xinyue.icu

[Q50] 批量更新
来源：http://gmc.pengpengdd.cyou

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://imc.guowangkeji.top

[Q51] 用子查询更新
来源：http://nwb.gzhubu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://djs.jlsjyb.cn

[Q52] 删除指定行
来源：http://ywr.hongshengwenyu.top

DELETE FROM users WHERE id = 10;
来源：http://saj.ybcxt.top

[Q53] 按条件删除
来源：http://pup.sweek.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://utg.xziqi.cn

[Q54] 清空表
来源：http://maa.sysykeji.top

TRUNCATE TABLE logs;
来源：http://tgb.yanxiufei.cn

[Q55] 排名（并列占位）
来源：http://ytd.chenlongwang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ftm.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://car.kuanghao11.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tea.hongshengwenyu.top

[Q57] 行号
来源：http://qnv.gzhubu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ggf.haohaochexian.top

[Q58] 累计求和
来源：http://dzo.gogol.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ygo.jyoumei.cn

[Q59] 分组内累计
来源：http://gxf.cucudq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ven.jqgfzy.top

[Q60] 取上一行 / 下一行
来源：http://afg.yj20258888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xzb.ybcxt.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iso.c1oappe.top

[Q61] 移动平均
来源：http://gcb.smart0.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hxr.fanxiaobao.xyz

[Q62] 分组占比
来源：http://grh.sufxvd.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tqq.ehwqpu.com

[Q63] 开启事务
来源：http://qtd.meibo888.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fvg.hywenlv.cn

[Q64] 提交事务
来源：http://cod.ydzc1.top

COMMIT;
来源：http://hbx.gotoacloud.top

[Q65] 回滚事务
来源：http://wxg.gaohongyu789.top

ROLLBACK;
来源：http://cqi.shzxlz.cn

[Q66] 行锁查询
来源：http://rhx.cucudq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nay.xuetiantiany.cn

[Q67] 设置隔离级别
来源：http://nqp.shangyingyoupin.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pez.ivvv.top

[Q68] 保存点
来源：http://rsm.316326.xyz

SAVEPOINT sp1;
来源：http://rtx.xuanzx.com

ROLLBACK TO sp1;
来源：http://fww.bbcook.cn

[Q69] 查看执行计划
来源：http://zag.mhx1999.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sri.yj20258.top

[Q70] 更新统计信息
来源：http://sah.zhoulong.xyz

ANALYZE TABLE users;
来源：http://iol.yueranfly.top

[Q71] 查看建表语句
来源：http://vgg.bjfxy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ixz.chenlongwang.top

[Q72] 查看索引
来源：http://vab.wangshuangyany.cn

SHOW INDEX FROM users;
来源：http://xsh.andypj.xyz

[Q73] 查看表状态
来源：http://tfj.svipenyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ymq.xinyue.icu

[Q74] 强制使用索引
来源：http://ygx.fzhhl.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ili.yj20258888.top

[Q75] 日期格式化
来源：http://lbe.svipenyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xnv.fehbvm.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pyg.shanyushiyangtech.top

[Q76] 按天统计
来源：http://tdw.ctjpmb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://raw.xuanzx.com

[Q77] 时间加减
来源：http://vao.nanxinkj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wfb.zycfv.cn

[Q78] 当前时间
来源：http://amd.xinyue.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://syk.zhijiandao.cn

[Q79] 字符串拼接
来源：http://szn.xuanzx.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fxc.zhiwuduotai.top

[Q80] 字符串截取
来源：http://zvj.yvedp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dpz.svipenyu.cn

[Q81] 字符串替换
来源：http://vau.wangdashe.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ust.sysykeji.top

[Q82] 字符长度与字节长度
来源：http://cip.zdbjq.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ddf.shangyingyoupin.top

[Q83] 大小写转换
来源：http://xxm.shangyingyoupin.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qxn.ivvv.top

[Q84] 去除首尾空格
来源：http://vxc.yonumen.top

SELECT TRIM(name) FROM users;
来源：http://hit.chenlongwang.top

[Q85] 数值取整
来源：http://xep.52xcode.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eao.yonumen.top

[Q86] 读取 JSON 字段
来源：http://ssf.9152youxi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zdj.yongpay.top

[Q87] JSON 字段做条件
来源：http://jsb.jqgfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mig.cheryme.top

[Q88] 行转列（条件聚合）
来源：http://uub.shangyingyoupin.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jzu.yueranfly.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aaf.iojbl.cn

[Q89] 判断表是否存在
来源：http://sjr.cucudq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xqx.daxiang520.top

[Q90] 生成序号列
来源：http://aqo.daria6918.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vfp.gogol.net.cn

================================================================================
来源：http://bpe.jyoumei.cn

R. Bash 专题
来源：http://ptl.ywan-chungtsiang.top

================================================================================
来源：http://iwy.bbcook.cn

[R01] shebang 与严格模式
来源：http://pxu.tanke756.top

#!/usr/bin/env bash
来源：http://xyw.yonumen.top

set -euo pipefail
来源：http://pov.yonumen.top

[R02] 变量赋值与使用
来源：http://ukc.vehdjk.com

name="Tom"; echo "$name"
来源：http://vcs.dashuyun.cn

[R03] 只读变量
来源：http://poq.yfazqb.com

readonly PI=3.14
来源：http://uea.hongshengwenyu.top

[R04] 位置参数
来源：http://bpe.fengsongda.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tff.cqqwz.cn

[R05] 参数默认值
来源：http://zdz.dashuyun.cn

name="${1:-default}"
来源：http://jwt.pycfn.com

[R06] 判断命令是否存在
来源：http://deu.cucudq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qnl.chenjidiqi.icu

[R07] if 判断文件
来源：http://ybg.fehbvm.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qcp.yongpay.top

[R08] 数值比较
来源：http://rwb.zdbjq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wtk.jinyuanbaomall.cn

[R09] 字符串比较
来源：http://bmv.gaohongyu789.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mli.wangdashe.top

[R10] 正则匹配
来源：http://ksc.xziqi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tua.zhiwuduotai.top

[R11] case 多分支
来源：http://omq.haohaochexian.top

case "$1" in
来源：http://aug.hnqzz.top

start) echo "启动" ;;
来源：http://zvq.sufxvd.cn

stop)  echo "停止" ;;
来源：http://pss.vehdjk.com

*)     echo "未知命令" ;;
来源：http://idk.nwbrower.top


<!-- 参考信息 -->