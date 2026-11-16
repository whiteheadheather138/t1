代发 wailian999

[O06] 使用进程池
来源：http://iks.daxiang520.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vxk.yuanzhike.top

PHP:  // pcntl_fork 或多进程队列
来源：http://yfu.xuetiantiany.cn

JS:   // child_process / cluster 模块
来源：http://fyk.fanxiaobao.xyz

TS:   // child_process / cluster 模块
来源：http://fqf.nanxuanxn.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jev.kuanghao11.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uri.uphjek.com

Ruby: // fork 块
来源：http://vus.zhijiandao.cn

C#:   Parallel.For
来源：http://anw.ctjpmb.com

================================================================================
来源：http://xnp.yj20258888.top

P. 常用工具函数
来源：http://bxv.gogol.net.cn

================================================================================
来源：http://ekn.ywan-chungtsiang.top

[P01] 生成 UUID
来源：http://xjt.chenjidiqi.icu

Py:   str(uuid.uuid4())
来源：http://qfu.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sbe.xuetiantiany.cn

JS:   crypto.randomUUID()
来源：http://cbw.mhx1999.top

TS:   crypto.randomUUID()
来源：http://edd.yanxiufei.cn

Java: UUID.randomUUID().toString()
来源：http://czp.cqqwz.cn

Go:   // 用 github.com/google/uuid
来源：http://ygo.ehwqpu.com

Ruby: SecureRandom.uuid
来源：http://isc.9152youxi.cn

C#:   Guid.NewGuid().ToString()
来源：http://shq.shanyushiyangtech.top

[P02] MD5 / SHA256 摘要
来源：http://ktb.vehdjk.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://onf.aizwys.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yrs.havefunace.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pbo.fengsongda.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jbb.hesvh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tto.vehdjk.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://udo.hysaishi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ort.fzhhl.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zty.pycfn.com

[P03] 生成短随机字符串
来源：http://ppt.sweek.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kvi.shuidangran.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tpo.snrcjt.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gvp.aibaodan.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kqd.ivvv.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uhy.jinyuanbaomall.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qsn.zycfv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zuc.hfpthk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nme.nanxuanxn.top

[P04] 求长度
来源：http://kiv.ywan-chungtsiang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qmb.daxiang520.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kdb.hammf.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jdk.9152youxi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bbn.ppjwa.cn

Java: list.size();  map.size();  s.length()
来源：http://bma.sysykeji.top

Go:   len(arr);  len(m)
来源：http://cgl.zdqjudy.top

Ruby: x.length;  x.size
来源：http://ewg.daxiang520.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://agh.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://jls.guannengcc.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ojf.316326.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gcg.iojbl.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://htl.mhx1999.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cdb.guowangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://odh.xingfuxueyuan.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://zpj.gogol.net.cn

Ruby: a == b
来源：http://mwb.316326.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ydw.ivvv.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ctg.xuanzx.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://los.xuetiantiany.cn

PHP:  if (empty($x)) {}
来源：http://kkg.jlsjyb.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wes.shanyushiyangtech.top

TS:   if (x == null) {}
来源：http://tht.yangfankeji.com

Java: if (x == null || x.isEmpty()) {}
来源：http://efp.zhixingplan.top

Go:   if x == nil {}
来源：http://yqq.tianlin.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://beu.aizwys.cn

C#:   if (x is null) {}
来源：http://dzb.hfpthk.cn

[P07] 防抖与节流
来源：http://msa.xylfe.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ehq.hnqzz.top

PHP:  // 手写时间戳比较
来源：http://pmu.pengpengdd.cyou

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fgf.jiagoushi.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uvi.iojbl.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://arv.yfazqb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lde.yanxiufei.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pow.iojbl.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ofp.bbcook.cn

[P08] 处理浮点精度问题
来源：http://rrh.chenlongwang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yxe.zhijiandao.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nuz.yueranfly.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jye.bjfxy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rou.tarul.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://btc.yongpay.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rsb.xuetiantiany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wjd.epnwcf.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jlo.jinghuilouyu.cn

================================================================================
来源：http://mxw.uphjek.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jvw.fktsv.cn

================================================================================
来源：http://ebw.shzxlz.cn

[Q01] 创建表
来源：http://juh.9152youxi.cn

CREATE TABLE users (
来源：http://nvq.cqqwz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://btb.yvedp.cn

name VARCHAR(50) NOT NULL,
来源：http://yme.yueranfly.top

email VARCHAR(100) UNIQUE,
来源：http://agq.bjfxy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nxm.jinyuanbaomall.cn

);
来源：http://cxq.zycfv.cn

[Q02] 创建带外键的表
来源：http://ano.yvedp.cn

CREATE TABLE orders (
来源：http://pxx.xziqi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jty.yongpay.top

user_id INT NOT NULL,
来源：http://qvu.chenzaomai.com

amount DECIMAL(10, 2),
来源：http://fdj.sysykeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uww.52xcode.cn

);
来源：http://wfx.daria6918.cn

[Q03] 增加列
来源：http://iyz.yueranfly.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uef.kuanghao11.cn

[Q04] 修改列类型
来源：http://jwg.tian-w.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://grr.redwolf501.top

[Q05] 重命名列
来源：http://iae.jlsjyb.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pgc.tianlin.xyz

[Q06] 删除列
来源：http://djl.gzhubu.top

ALTER TABLE users DROP COLUMN age;
来源：http://ubp.hywenlv.cn

[Q07] 删除表
来源：http://jpk.meibo888.top

DROP TABLE IF EXISTS orders;
来源：http://blc.shanyushiyangtech.top

[Q08] 创建普通索引
来源：http://xdb.svipenyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://umu.gzhubu.top

[Q09] 创建唯一索引
来源：http://vjy.tianlin.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ziz.chenlongwang.top

[Q10] 插入单行
来源：http://lxq.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jyd.hongshengwenyu.top

[Q11] 一次插入多行
来源：http://ctk.cdnleiting.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hxj.ybcxt.top

[Q12] 插入后取自增 ID
来源：http://aix.yongpay.top

INSERT INTO users (name) VALUES ('C');
来源：http://izb.zhijiandao.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vjy.yfazqb.com

[Q13] 忽略重复插入
来源：http://bvb.fengsongda.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vyy.ehwqpu.com

[Q14] 存在则更新（upsert）
来源：http://eat.jiagoushi.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kra.wangshuangyany.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bek.gotoacloud.top

[Q15] 查询全部
来源：http://yhv.guowangkeji.top

SELECT * FROM users;
来源：http://hkv.feifeiyinyue.top

[Q16] 查询指定列
来源：http://gnb.shanyushiyangkeji.top

SELECT id, name FROM users;
来源：http://yzw.shzxlz.cn

[Q17] 条件查询
来源：http://fug.cashguo.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yde.zhongyouzk.top

[Q18] 模糊匹配
来源：http://rhd.dashuyun.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tgy.hnqzz.top

[Q19] 范围查询
来源：http://rtr.yvedp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zdf.pengpengdd.cyou

[Q20] IN 列表
来源：http://wux.uphjek.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lhs.c1oappe.top

[Q21] 空值判断
来源：http://kst.jianghu66.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zce.ybcxt.top

[Q22] 排序
来源：http://fea.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://opw.tarul.cn

[Q23] 分页
来源：http://fng.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zci.9152youxi.cn

[Q24] 去重
来源：http://xpa.vehdjk.com

SELECT DISTINCT city FROM users;
来源：http://bsd.yongpay.top

[Q25] 只取前 N 条
来源：http://acm.sweek.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sty.aizwys.cn

[Q26] 计数
来源：http://tjf.ybcxt.top

SELECT COUNT(*) FROM users;
来源：http://gjb.shuidangran.top

[Q27] 条件计数
来源：http://krr.shanyushiyangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fzh.cheryme.top

[Q28] 求和与平均
来源：http://fjq.meibo888.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ezd.shangyingyoupin.top

[Q29] 最大最小值
来源：http://avu.sjlbkw.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kgd.pycfn.com

[Q30] 分组统计
来源：http://alu.bbcook.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://flf.cheryme.top

[Q31] 分组后过滤
来源：http://zbc.aibaodan.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nzy.c1oappe.top

[Q32] 分组拼接字符串
来源：http://flr.redwolf501.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oqm.sysykeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://orm.jinghuilouyu.cn

[Q33] 多列分组
来源：http://mvx.nwbrower.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sca.cucudq.cn

[Q34] 每组取第一条
来源：http://iap.yongpay.top

SELECT * FROM (
来源：http://oxj.fzhhl.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kpm.xylfe.cn

) t WHERE rn = 1;
来源：http://xgz.gotoacloud.top

[Q35] 内连接
来源：http://qat.ppjwa.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qbr.9152youxi.cn

[Q36] 左连接
来源：http://alc.hnxiangtu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xwo.sysykeji.top

[Q37] 右连接
来源：http://tyk.xingfuxueyuan.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://llz.zhengqikj.top

[Q38] 全外连接（PostgreSQL）
来源：http://qmk.gaohongyu789.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zfp.ehwqpu.com

[Q39] 自连接（查上下级）
来源：http://izy.jqgufenzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tob.wangdashe.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lqj.hammf.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://phh.meibo888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yck.pengpengdd.cyou

[Q41] 多表连接
来源：http://mpb.nanxinkj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://xhj.tanke756.top

JOIN users u ON u.id = o.user_id
来源：http://rff.pengpengdd.cyou

JOIN products p ON p.id = o.product_id;
来源：http://lxl.fanxiaobao.xyz

[Q42] 连接条件附加过滤
来源：http://jvf.vqdsnc.cn

SELECT u.name, o.amount FROM users u
来源：http://llm.gaohongyu789.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kna.haohaochexian.top

[Q43] 标量子查询
来源：http://fmw.cdnleiting.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tcc.guannengcc.top

[Q44] IN 子查询
来源：http://nag.tanke756.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yry.fzhhl.top

[Q45] EXISTS 判断存在
来源：http://icl.ehwqpu.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kvz.jinyuanbaomall.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nzg.yonumen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nju.ppjwa.cn

[Q47] 与平均值比较
来源：http://zva.jlsjyb.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xml.yj202588.top

[Q48] CTE 公用表表达式
来源：http://pnh.zhiwuduotai.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uyz.52xcode.cn

SELECT * FROM t WHERE c > 5;
来源：http://azz.hnxiangtu.top

[Q49] 更新单行
来源：http://npl.9152youxi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fnk.zhiwuduotai.top

[Q50] 批量更新
来源：http://mbc.fzhhl.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vgi.ppjwa.cn

[Q51] 用子查询更新
来源：http://dbg.zycfv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://evu.cashguo.top

[Q52] 删除指定行
来源：http://ymp.svipenyu.cn

DELETE FROM users WHERE id = 10;
来源：http://sdw.jqgufenzy.top

[Q53] 按条件删除
来源：http://bsc.wangshuangyany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://aaa.cheryme.top

[Q54] 清空表
来源：http://mda.hnqzz.top

TRUNCATE TABLE logs;
来源：http://xix.shuidangran.top

[Q55] 排名（并列占位）
来源：http://whr.tarul.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xuf.zhijiandao.cn

[Q56] 密集排名（并列不占位）
来源：http://ges.haohaochexian.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lzd.chenzaomai.com

[Q57] 行号
来源：http://wmh.xinyue.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hrh.316326.xyz

[Q58] 累计求和
来源：http://iwi.yueranfly.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gwe.xuanzx.com

[Q59] 分组内累计
来源：http://kar.yvedp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://upo.9152youxi.cn

[Q60] 取上一行 / 下一行
来源：http://hrr.guowangkeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xpg.smart0.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ecv.svipenyu.cn

[Q61] 移动平均
来源：http://eaz.quarkkingdee.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wem.zhaomingkeji.xyz

[Q62] 分组占比
来源：http://atp.sjlbkw.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hng.shangyingyoupin.top

[Q63] 开启事务
来源：http://qsz.zhijiandao.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dpu.bjfxy.top

[Q64] 提交事务
来源：http://gab.cheryme.top

COMMIT;
来源：http://cjw.fzhhl.top

[Q65] 回滚事务
来源：http://trl.quarkkingdee.top

ROLLBACK;
来源：http://ukx.redwolf501.top

[Q66] 行锁查询
来源：http://umq.ctjpmb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://apo.gzhubu.top

[Q67] 设置隔离级别
来源：http://mau.quarkkingdee.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uol.bjfxy.top

[Q68] 保存点
来源：http://gfz.nwbrower.top

SAVEPOINT sp1;
来源：http://qhl.hysaishi.cn

ROLLBACK TO sp1;
来源：http://tkl.zhengqikj.top

[Q69] 查看执行计划
来源：http://uez.fehbvm.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eau.gaohongyu789.top

[Q70] 更新统计信息
来源：http://hit.epnwcf.com

ANALYZE TABLE users;
来源：http://msp.cdnleiting.top

[Q71] 查看建表语句
来源：http://mty.bbcook.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lzg.wangdashe.top

[Q72] 查看索引
来源：http://bzl.hywenlv.cn

SHOW INDEX FROM users;
来源：http://pvt.cdnleiting.top

[Q73] 查看表状态
来源：http://dmq.gogol.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ofv.hysaishi.cn

[Q74] 强制使用索引
来源：http://dqg.hesvh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gvm.daria6918.cn

[Q75] 日期格式化
来源：http://jew.gogol.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hlr.haohaochexian.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pln.dashuyun.cn

[Q76] 按天统计
来源：http://jnb.bbcook.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tan.fktsv.cn

[Q77] 时间加减
来源：http://lnf.shanyushiyangtech.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://peb.chenlongwang.top

[Q78] 当前时间
来源：http://ecn.quarkkingdee.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aal.ybcxt.top

[Q79] 字符串拼接
来源：http://pss.pengpengdd.cyou

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uar.jqgufenzy.top

[Q80] 字符串截取
来源：http://zsf.nanxinkj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://noi.haohaochexian.top

[Q81] 字符串替换
来源：http://ftu.gotoacloud.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sce.zdqjudy.top

[Q82] 字符长度与字节长度
来源：http://zxf.daria6918.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jfv.zhixingplan.top

[Q83] 大小写转换
来源：http://zvy.gogol.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tgn.bbcook.cn

[Q84] 去除首尾空格
来源：http://fvm.ydzc1.top

SELECT TRIM(name) FROM users;
来源：http://qxh.pycfn.com

[Q85] 数值取整
来源：http://nhd.9152youxi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://txm.aizwys.cn

[Q86] 读取 JSON 字段
来源：http://nob.andypj.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sey.meibo888.top

[Q87] JSON 字段做条件
来源：http://vmc.gaohongyu789.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vgh.epnwcf.com

[Q88] 行转列（条件聚合）
来源：http://bhu.shuidangran.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iqf.jqgufenzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hat.hcnkem.com

[Q89] 判断表是否存在
来源：http://crq.sufxvd.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://aks.vehdjk.com

[Q90] 生成序号列
来源：http://whc.aizwys.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://etc.quarkkingdee.top

================================================================================
来源：http://zwp.zhijiandao.cn

R. Bash 专题
来源：http://ckv.ybcxt.top

================================================================================
来源：http://ciw.yj202588.top

[R01] shebang 与严格模式
来源：http://fve.zhijiandao.cn

#!/usr/bin/env bash
来源：http://qxk.hnxiangtu.top

set -euo pipefail
来源：http://hoq.haohaochexian.top

[R02] 变量赋值与使用
来源：http://ogr.xingfuxueyuan.xyz

name="Tom"; echo "$name"
来源：http://ori.daria6918.cn

[R03] 只读变量
来源：http://xyj.svipenyu.cn


<!-- 参考信息 -->