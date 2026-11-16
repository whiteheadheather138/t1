代发 wailian999

TS:   crypto.randomUUID()
来源：http://rja.jinghuilouyu.cn

Java: UUID.randomUUID().toString()
来源：http://dey.mhx1999.top

Go:   // 用 github.com/google/uuid
来源：http://vfs.daria6918.cn

Ruby: SecureRandom.uuid
来源：http://isx.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://yfl.shangyingyoupin.top

[P02] MD5 / SHA256 摘要
来源：http://dga.tianlin.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://odp.xuanzx.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://vvq.gaohongyu789.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://opg.yanxiufei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jwk.shanyushiyangtech.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kkb.fzhhl.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://che.dianchejie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://psf.aibaodan.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nop.yj20258.top

[P03] 生成短随机字符串
来源：http://tkn.ehwqpu.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://drn.xylfe.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kvm.vqdsnc.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pmw.jinqigfzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://amk.jianghu66.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yuk.vqdsnc.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://huv.yongpay.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mzb.yj202588.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://trm.mhx1999.top

[P04] 求长度
来源：http://eug.bbcook.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bdt.daria6918.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ycs.cdnleiting.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://djc.cheryme.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eon.sxryk.cn

Java: list.size();  map.size();  s.length()
来源：http://yxw.xziqi.cn

Go:   len(arr);  len(m)
来源：http://aqw.mhx1999.top

Ruby: x.length;  x.size
来源：http://aqm.ehwqpu.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://mvp.xuanzx.com

[P05] 判断两个对象内容是否相等
来源：http://omk.chenjidiqi.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://sjc.zdqjudy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kwb.9152youxi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://myf.kuanghao11.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cek.yuxming.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hbg.shangyingyoupin.top

Go:   reflect.DeepEqual(a, b)
来源：http://skq.0kj1m.cn

Ruby: a == b
来源：http://viy.ybcxt.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://agy.jqgfzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://khm.cheryme.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://psc.ivvv.top

PHP:  if (empty($x)) {}
来源：http://roo.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://boa.aizwys.cn

TS:   if (x == null) {}
来源：http://sum.zhiwuduotai.top

Java: if (x == null || x.isEmpty()) {}
来源：http://blh.yj20258.top

Go:   if x == nil {}
来源：http://zlf.sjlbkw.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fkt.zhongyouzk.top

C#:   if (x is null) {}
来源：http://xkk.feifeiyinyue.top

[P07] 防抖与节流
来源：http://kcd.quarkkingdee.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://quu.guannengcc.top

PHP:  // 手写时间戳比较
来源：http://uto.guannengcc.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://twv.svipenyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qub.pengpengdd.cyou

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mvd.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cxy.zhengqikj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mos.hcnkem.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cbi.xylfe.cn

[P08] 处理浮点精度问题
来源：http://yzu.vehdjk.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iei.yj20258.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yfu.tarul.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ezg.fengsongda.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lgh.mhx1999.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ikb.jlsjyb.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jyh.316326.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kpz.jianghu66.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oda.gzhubu.top

================================================================================
来源：http://ino.jinqigufen.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fqb.andypj.xyz

================================================================================
来源：http://nyn.ivvv.top

[Q01] 创建表
来源：http://ubt.yuanzhike.top

CREATE TABLE users (
来源：http://tve.tianlin.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xqz.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://ggr.jinyuanbaomall.cn

email VARCHAR(100) UNIQUE,
来源：http://nht.ppjwa.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jft.gogol.net.cn

);
来源：http://xso.nwbrower.top

[Q02] 创建带外键的表
来源：http://wrm.zhixingplan.top

CREATE TABLE orders (
来源：http://qgb.shangyingyoupin.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gqn.jianghu66.top

user_id INT NOT NULL,
来源：http://fhx.daxiang520.top

amount DECIMAL(10, 2),
来源：http://lme.hfpthk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nyx.xylfe.cn

);
来源：http://bwb.shanyushiyangtech.top

[Q03] 增加列
来源：http://xem.dianchejie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sbd.hnxiangtu.top

[Q04] 修改列类型
来源：http://xxg.smart0.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://glj.gotoacloud.top

[Q05] 重命名列
来源：http://hyj.jinyuanbaomall.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xgf.shanyushiyangkeji.top

[Q06] 删除列
来源：http://bze.chenjidiqi.icu

ALTER TABLE users DROP COLUMN age;
来源：http://uti.fehbvm.com

[Q07] 删除表
来源：http://sno.cdnleiting.top

DROP TABLE IF EXISTS orders;
来源：http://fgq.zhixingplan.top

[Q08] 创建普通索引
来源：http://kkp.bjfxy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mew.shanyushiyangtech.top

[Q09] 创建唯一索引
来源：http://dmq.yvedp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ctl.yfazqb.com

[Q10] 插入单行
来源：http://qkm.snrcjt.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oym.ctjpmb.com

[Q11] 一次插入多行
来源：http://oei.shanyushiyangkeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nzj.hcnkem.com

[Q12] 插入后取自增 ID
来源：http://kyd.yangfankeji.com

INSERT INTO users (name) VALUES ('C');
来源：http://ncg.sysykeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oaw.shzxlz.cn

[Q13] 忽略重复插入
来源：http://yll.hesvh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zog.zdqjudy.top

[Q14] 存在则更新（upsert）
来源：http://tmk.ywan-chungtsiang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kog.yueranfly.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lbn.wangshuangyany.cn

[Q15] 查询全部
来源：http://xhe.52xcode.cn

SELECT * FROM users;
来源：http://gzq.chenjidiqi.icu

[Q16] 查询指定列
来源：http://qwt.hfpthk.cn

SELECT id, name FROM users;
来源：http://rxu.tanke756.top

[Q17] 条件查询
来源：http://avx.chenzaomai.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://aig.chenlongwang.top

[Q18] 模糊匹配
来源：http://geq.c1oappe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yyt.jiagoushi.top

[Q19] 范围查询
来源：http://qaj.ydjk.org.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tgc.zhixingplan.top

[Q20] IN 列表
来源：http://gov.9152youxi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hei.zdqjudy.top

[Q21] 空值判断
来源：http://chd.epnwcf.com

SELECT * FROM users WHERE email IS NULL;
来源：http://tss.jqgfzy.top

[Q22] 排序
来源：http://hog.bbcook.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jgh.shuidangran.top

[Q23] 分页
来源：http://kci.nanxuanxn.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kuo.zhaomingkeji.xyz

[Q24] 去重
来源：http://azq.nwbrower.top

SELECT DISTINCT city FROM users;
来源：http://nhy.pengpengdd.cyou

[Q25] 只取前 N 条
来源：http://rey.xziqi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://djk.c1oappe.top

[Q26] 计数
来源：http://yuu.xuanzx.com

SELECT COUNT(*) FROM users;
来源：http://iee.hnxiangtu.top

[Q27] 条件计数
来源：http://cak.jiagoushi.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ysy.quarkkingdee.top

[Q28] 求和与平均
来源：http://fmy.shuidangran.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yht.haohaochexian.top

[Q29] 最大最小值
来源：http://dax.zhiwuduotai.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://erm.zdbjq.cn

[Q30] 分组统计
来源：http://cgl.yj202588.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zrb.jinqigfzy.top

[Q31] 分组后过滤
来源：http://vot.jinqigufen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fiz.feifeiyinyue.top

[Q32] 分组拼接字符串
来源：http://xwz.wangdashe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://urw.cashguo.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vkm.yongpay.top

[Q33] 多列分组
来源：http://drw.yanxiufei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pga.tarul.cn

[Q34] 每组取第一条
来源：http://onw.yuanzhike.top

SELECT * FROM (
来源：http://xow.jinghuilouyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vrh.xylfe.cn

) t WHERE rn = 1;
来源：http://jlo.pengpengdd.cyou

[Q35] 内连接
来源：http://dia.birdmap.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://goj.kuanghao11.cn

[Q36] 左连接
来源：http://jcd.zhoulong.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://myp.hesvh.cn

[Q37] 右连接
来源：http://yyv.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kgd.bbcook.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dxv.jqgfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bmv.daxiang520.top

[Q39] 自连接（查上下级）
来源：http://gnp.sufxvd.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://omb.yvedp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eid.sxryk.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ewm.cashguo.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eok.yonumen.top

[Q41] 多表连接
来源：http://xyl.hammf.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kay.yj202588.top

JOIN users u ON u.id = o.user_id
来源：http://bzk.zhengqikj.top

JOIN products p ON p.id = o.product_id;
来源：http://pvq.ybcxt.top

[Q42] 连接条件附加过滤
来源：http://vcj.redwolf501.top

SELECT u.name, o.amount FROM users u
来源：http://snd.sjlbkw.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vmx.zycfv.cn

[Q43] 标量子查询
来源：http://vou.andypj.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tfu.havefunace.top

[Q44] IN 子查询
来源：http://hxq.sufxvd.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ceq.shuidangran.top

[Q45] EXISTS 判断存在
来源：http://cnk.feifeiyinyue.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jaf.shzxlz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gmo.jiagoushi.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://had.andypj.xyz

[Q47] 与平均值比较
来源：http://qrx.snrcjt.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fzz.hfpthk.cn

[Q48] CTE 公用表表达式
来源：http://pdw.hfpthk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kdu.yj202588.top

SELECT * FROM t WHERE c > 5;
来源：http://eql.316326.xyz

[Q49] 更新单行
来源：http://mhs.feifeiyinyue.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cse.cucudq.cn

[Q50] 批量更新
来源：http://ucu.vqdsnc.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://auk.ivvv.top

[Q51] 用子查询更新
来源：http://tep.xylfe.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mcx.yj202588.top

[Q52] 删除指定行
来源：http://shw.yongpay.top

DELETE FROM users WHERE id = 10;
来源：http://fcu.smart0.xyz

[Q53] 按条件删除
来源：http://bsk.zhengqikj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kva.hywenlv.cn

[Q54] 清空表
来源：http://inh.hesvh.cn

TRUNCATE TABLE logs;
来源：http://mpa.meibo888.top

[Q55] 排名（并列占位）
来源：http://mfz.zhaomingkeji.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dze.fehbvm.com

[Q56] 密集排名（并列不占位）
来源：http://drh.tarul.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dts.chenlongwang.top

[Q57] 行号
来源：http://nts.zdqjudy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kjk.cheryme.top

[Q58] 累计求和
来源：http://giz.yj20258.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kkg.316326.xyz

[Q59] 分组内累计
来源：http://lwy.yvedp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ylz.quarkkingdee.top

[Q60] 取上一行 / 下一行
来源：http://nhl.tarul.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uee.havefunace.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mrk.ivvv.top

[Q61] 移动平均
来源：http://wcm.uphjek.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://duw.ywan-chungtsiang.top

[Q62] 分组占比
来源：http://dbd.sysykeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vlm.fanxiaobao.xyz

[Q63] 开启事务
来源：http://raa.haohaochexian.top

START TRANSACTION;                -- 或 BEGIN
来源：http://biz.daxiang520.top

[Q64] 提交事务
来源：http://oli.gzhubu.top

COMMIT;
来源：http://iqp.chenjidiqi.icu

[Q65] 回滚事务
来源：http://blu.daria6918.cn

ROLLBACK;
来源：http://fxs.c1oappe.top

[Q66] 行锁查询
来源：http://fnj.wangshuangyany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qke.snrcjt.cn

[Q67] 设置隔离级别
来源：http://ewk.zycfv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kdk.tanke756.top

[Q68] 保存点
来源：http://myx.hongshengwenyu.top

SAVEPOINT sp1;
来源：http://icd.fehbvm.com

ROLLBACK TO sp1;
来源：http://egs.hesvh.cn

[Q69] 查看执行计划
来源：http://mxq.tianlin.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://srp.52xcode.cn

[Q70] 更新统计信息
来源：http://qsk.shangyingyoupin.top

ANALYZE TABLE users;
来源：http://ijs.yfazqb.com

[Q71] 查看建表语句
来源：http://ndp.sufxvd.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rqj.ctjpmb.com

[Q72] 查看索引
来源：http://gwz.9152youxi.cn

SHOW INDEX FROM users;
来源：http://ldr.fanxiaobao.xyz

[Q73] 查看表状态
来源：http://dtw.svipenyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ijd.wangdashe.top

[Q74] 强制使用索引
来源：http://akb.daria6918.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lyw.sysykeji.top

[Q75] 日期格式化
来源：http://uuq.vehdjk.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lkc.hfpthk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vqd.aibaodan.cn

[Q76] 按天统计
来源：http://wpv.cheryme.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lke.cucudq.cn

[Q77] 时间加减
来源：http://ymb.ybcxt.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mbr.yonumen.top

[Q78] 当前时间
来源：http://yzb.quarkkingdee.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://twt.zdqjudy.top

[Q79] 字符串拼接
来源：http://dxc.wangdashe.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://roj.yongpay.top

[Q80] 字符串截取
来源：http://kml.zhoulong.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xny.pengpengdd.cyou

[Q81] 字符串替换
来源：http://abp.gogol.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zkn.havefunace.top

[Q82] 字符长度与字节长度
来源：http://khi.jyoumei.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ztg.zhijiandao.cn

[Q83] 大小写转换
来源：http://azs.tianlin.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bzb.mhx1999.top

[Q84] 去除首尾空格
来源：http://brj.yuanzhike.top

SELECT TRIM(name) FROM users;
来源：http://ztr.fktsv.cn

[Q85] 数值取整
来源：http://uhs.fanxiaobao.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sgd.jqgfzy.top

[Q86] 读取 JSON 字段
来源：http://kyw.chenlongwang.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nkk.hysaishi.cn

[Q87] JSON 字段做条件
来源：http://osl.guannengcc.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xoi.shanyushiyangtech.top

[Q88] 行转列（条件聚合）
来源：http://jcf.ivvv.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lcs.hnqzz.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mdh.pycfn.com

[Q89] 判断表是否存在
来源：http://ial.hesvh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mzv.jqgfzy.top

[Q90] 生成序号列
来源：http://syt.jinyuanbaomall.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jbp.9152youxi.cn

================================================================================
来源：http://kzc.zdbjq.cn

R. Bash 专题
来源：http://sqy.ywan-chungtsiang.top

================================================================================
来源：http://lni.pengpengdd.cyou

[R01] shebang 与严格模式
来源：http://eml.xylfe.cn

#!/usr/bin/env bash
来源：http://ygx.xinyue.icu

set -euo pipefail
来源：http://djo.tian-w.cn

[R02] 变量赋值与使用
来源：http://mxh.yuxming.cn

name="Tom"; echo "$name"
来源：http://ept.nanxinkj.top

[R03] 只读变量
来源：http://jui.feifeiyinyue.top

readonly PI=3.14
来源：http://xfo.yj20258888.top

[R04] 位置参数
来源：http://jxd.hcnkem.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zkb.bbcook.cn

[R05] 参数默认值
来源：http://msi.meibo888.top

name="${1:-default}"
来源：http://gwp.wangshuangyany.cn

[R06] 判断命令是否存在
来源：http://dnr.ywan-chungtsiang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kzm.ivvv.top

[R07] if 判断文件
来源：http://fko.zdqjudy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://myg.zhiwuduotai.top

[R08] 数值比较
来源：http://eby.ydzc1.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hjl.ywan-chungtsiang.top

[R09] 字符串比较
来源：http://poc.yueranfly.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uts.sufxvd.cn

[R10] 正则匹配
来源：http://luu.yuanzhike.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mbe.shanyushiyangkeji.top

[R11] case 多分支
来源：http://hmb.jinqigfzy.top


<!-- 参考信息 -->