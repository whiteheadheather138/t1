代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://sis.tian-w.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uch.zhixingplan.top

JS:   await Promise.all(tasks)
来源：http://mph.yonumen.top

TS:   await Promise.all(tasks)
来源：http://mcm.dianchejie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rtx.fzhhl.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ndw.daria6918.cn

Ruby: threads.map(&:join)
来源：http://brh.aizwys.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vfe.tarul.cn

[O06] 使用进程池
来源：http://jzy.dashuyun.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bkz.fengsongda.top

PHP:  // pcntl_fork 或多进程队列
来源：http://sfo.yj20258888.top

JS:   // child_process / cluster 模块
来源：http://zgw.xziqi.cn

TS:   // child_process / cluster 模块
来源：http://ttq.guannengcc.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lyb.yvedp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://irs.yueranfly.top

Ruby: // fork 块
来源：http://ixz.gogol.net.cn

C#:   Parallel.For
来源：http://ddg.jiagoushi.top

================================================================================
来源：http://ooh.nanxuanxn.top

P. 常用工具函数
来源：http://iue.ybcxt.top

================================================================================
来源：http://kgg.yuanzhike.top

[P01] 生成 UUID
来源：http://oql.yueranfly.top

Py:   str(uuid.uuid4())
来源：http://xjf.shangyingyoupin.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jjq.hammf.cn

JS:   crypto.randomUUID()
来源：http://bdz.cucudq.cn

TS:   crypto.randomUUID()
来源：http://vim.316326.xyz

Java: UUID.randomUUID().toString()
来源：http://ktu.hongshengwenyu.top

Go:   // 用 github.com/google/uuid
来源：http://hoz.9152youxi.cn

Ruby: SecureRandom.uuid
来源：http://xry.jlsjyb.cn

C#:   Guid.NewGuid().ToString()
来源：http://mla.dashuyun.cn

[P02] MD5 / SHA256 摘要
来源：http://flw.gaohongyu789.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rdw.mhx1999.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ire.316326.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mqg.ppjwa.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bxt.nwbrower.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tjq.tianlin.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lgr.dashuyun.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oqo.yonumen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fgd.316326.xyz

[P03] 生成短随机字符串
来源：http://yut.snrcjt.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://szg.quarkkingdee.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://crr.gogol.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xss.xingfuxueyuan.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://shp.shuidangran.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mzi.ppjwa.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tvd.zdqjudy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zoy.hcnkem.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sxa.ybcxt.top

[P04] 求长度
来源：http://muy.yvedp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pds.sxryk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xgl.jyoumei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hlr.epnwcf.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dnc.bjfxy.top

Java: list.size();  map.size();  s.length()
来源：http://cqu.hnqzz.top

Go:   len(arr);  len(m)
来源：http://oeg.xylfe.cn

Ruby: x.length;  x.size
来源：http://yyk.yvedp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hte.316326.xyz

[P05] 判断两个对象内容是否相等
来源：http://aiq.kuanghao11.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zsm.52xcode.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cxs.hongshengwenyu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zpw.jinyuanbaomall.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dbh.zdqjudy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qur.jiagoushi.top

Go:   reflect.DeepEqual(a, b)
来源：http://toh.sweek.top

Ruby: a == b
来源：http://iwc.feifeiyinyue.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bhl.zhiwuduotai.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hmd.aibaodan.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://arx.gaohongyu789.top

PHP:  if (empty($x)) {}
来源：http://xls.redwolf501.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cny.haohaochexian.top

TS:   if (x == null) {}
来源：http://iqh.hammf.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cfx.gogol.net.cn

Go:   if x == nil {}
来源：http://eeq.wangdashe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://puk.yanxiufei.cn

C#:   if (x is null) {}
来源：http://mzg.wangdashe.top

[P07] 防抖与节流
来源：http://ose.cashguo.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://juq.zycfv.cn

PHP:  // 手写时间戳比较
来源：http://kvq.jinyuanbaomall.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tkz.chenzaomai.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oos.zhiwuduotai.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dvv.dashuyun.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xoz.fktsv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xyr.52xcode.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xqh.ivvv.top

[P08] 处理浮点精度问题
来源：http://omw.pengpengdd.cyou

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jal.aibaodan.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uoh.hywenlv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gbt.yj20258.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://job.bjfxy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zsl.tianlin.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lml.nwbrower.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jug.shangyingyoupin.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pay.ctjpmb.com

================================================================================
来源：http://hux.zdqjudy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wgp.yj20258.top

================================================================================
来源：http://rwf.epnwcf.com

[Q01] 创建表
来源：http://dkv.chenlongwang.top

CREATE TABLE users (
来源：http://yny.pengpengdd.cyou

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uml.yangfankeji.com

name VARCHAR(50) NOT NULL,
来源：http://zxf.wangshuangyany.cn

email VARCHAR(100) UNIQUE,
来源：http://fxf.shanyushiyangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vgg.yongpay.top

);
来源：http://qdy.ehwqpu.com

[Q02] 创建带外键的表
来源：http://sab.haohaochexian.top

CREATE TABLE orders (
来源：http://ntq.epnwcf.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fww.smart0.xyz

user_id INT NOT NULL,
来源：http://wnb.gotoacloud.top

amount DECIMAL(10, 2),
来源：http://cft.ydzc1.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://chn.yj202588.top

);
来源：http://tuq.zdqjudy.top

[Q03] 增加列
来源：http://xkl.svipenyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dle.52xcode.cn

[Q04] 修改列类型
来源：http://cwj.cqqwz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cau.yangfankeji.com

[Q05] 重命名列
来源：http://gqj.ivvv.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vyk.xingfuxueyuan.xyz

[Q06] 删除列
来源：http://qvs.tian-w.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mrh.sufxvd.cn

[Q07] 删除表
来源：http://kzx.daxiang520.top

DROP TABLE IF EXISTS orders;
来源：http://cxb.sjlbkw.cn

[Q08] 创建普通索引
来源：http://mvm.nanxuanxn.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ebj.tianlin.xyz

[Q09] 创建唯一索引
来源：http://jji.jinqigfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kth.xylfe.cn

[Q10] 插入单行
来源：http://rpi.meibo888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sae.nanxuanxn.top

[Q11] 一次插入多行
来源：http://bap.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xuf.zdqjudy.top

[Q12] 插入后取自增 ID
来源：http://yio.cheryme.top

INSERT INTO users (name) VALUES ('C');
来源：http://bum.svipenyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jfd.xylfe.cn

[Q13] 忽略重复插入
来源：http://qxv.zhiwuduotai.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zgv.shanyushiyangkeji.top

[Q14] 存在则更新（upsert）
来源：http://gjf.nwbrower.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://het.fzhhl.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fff.hysaishi.cn

[Q15] 查询全部
来源：http://fjq.birdmap.top

SELECT * FROM users;
来源：http://pzl.guowangkeji.top

[Q16] 查询指定列
来源：http://zsr.kuanghao11.cn

SELECT id, name FROM users;
来源：http://nzd.sjlbkw.cn

[Q17] 条件查询
来源：http://aei.ydjk.org.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://her.hcnkem.com

[Q18] 模糊匹配
来源：http://sli.epnwcf.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yur.zhoulong.xyz

[Q19] 范围查询
来源：http://aqz.zhiwuduotai.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eti.xingfuxueyuan.xyz

[Q20] IN 列表
来源：http://kbi.zhongyouzk.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bxa.cdnleiting.top

[Q21] 空值判断
来源：http://xft.sjlbkw.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rou.chenzaomai.com

[Q22] 排序
来源：http://rxk.hnxiangtu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uex.tian-w.cn

[Q23] 分页
来源：http://aul.sjlbkw.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tlu.jinqigufen.top

[Q24] 去重
来源：http://rxh.jlsjyb.cn

SELECT DISTINCT city FROM users;
来源：http://mlj.uphjek.com

[Q25] 只取前 N 条
来源：http://pxm.havefunace.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cet.fehbvm.com

[Q26] 计数
来源：http://lxb.ybcxt.top

SELECT COUNT(*) FROM users;
来源：http://dvn.dianchejie.cn

[Q27] 条件计数
来源：http://mkf.gogol.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://euh.zhiwuduotai.top

[Q28] 求和与平均
来源：http://rsb.gaohongyu789.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rcm.ehwqpu.com

[Q29] 最大最小值
来源：http://xlb.yfazqb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://syl.hnxiangtu.top

[Q30] 分组统计
来源：http://zck.zhaomingkeji.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nxq.pengpengdd.cyou

[Q31] 分组后过滤
来源：http://dra.iojbl.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zjr.smart0.xyz

[Q32] 分组拼接字符串
来源：http://zvr.tian-w.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://okb.daria6918.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uqy.tian-w.cn

[Q33] 多列分组
来源：http://ksr.birdmap.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qcc.nanxinkj.top

[Q34] 每组取第一条
来源：http://glw.wangshuangyany.cn

SELECT * FROM (
来源：http://stl.ctjpmb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ieu.redwolf501.top

) t WHERE rn = 1;
来源：http://xfh.yj202588.top

[Q35] 内连接
来源：http://ihf.guannengcc.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ozt.fehbvm.com

[Q36] 左连接
来源：http://gsk.xziqi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://njm.kuanghao11.cn

[Q37] 右连接
来源：http://uyc.wangdashe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cgu.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ivv.ybcxt.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iga.fktsv.cn

[Q39] 自连接（查上下级）
来源：http://bmq.cheryme.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://agq.yuanzhike.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zlv.fengsongda.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ktf.sjlbkw.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pqc.ppjwa.cn

[Q41] 多表连接
来源：http://mtw.cqqwz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ckk.yj20258.top

JOIN users u ON u.id = o.user_id
来源：http://xdm.aizwys.cn

JOIN products p ON p.id = o.product_id;
来源：http://pwv.yueranfly.top

[Q42] 连接条件附加过滤
来源：http://nje.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u
来源：http://wvc.dashuyun.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jbs.aibaodan.cn

[Q43] 标量子查询
来源：http://agy.yueranfly.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hjg.quarkkingdee.top

[Q44] IN 子查询
来源：http://aci.xuetiantiany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ntl.redwolf501.top

[Q45] EXISTS 判断存在
来源：http://xcq.fzhhl.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rws.xinyue.icu

[Q46] NOT EXISTS 判断不存在
来源：http://xvg.yuanzhike.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jbh.chenlongwang.top

[Q47] 与平均值比较
来源：http://nqo.xziqi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://inj.yuanzhike.top

[Q48] CTE 公用表表达式
来源：http://qoy.sxryk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hcl.sysykeji.top

SELECT * FROM t WHERE c > 5;
来源：http://ujw.havefunace.top

[Q49] 更新单行
来源：http://fau.bbcook.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mjd.cdnleiting.top

[Q50] 批量更新
来源：http://jjr.zdbjq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://stn.sjlbkw.cn

[Q51] 用子查询更新
来源：http://gkw.ydzc1.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lyx.sufxvd.cn

[Q52] 删除指定行
来源：http://lim.hnqzz.top

DELETE FROM users WHERE id = 10;
来源：http://tls.yj20258.top

[Q53] 按条件删除
来源：http://til.yuanzhike.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nkl.pengpengdd.cyou

[Q54] 清空表
来源：http://ica.gogol.net.cn

TRUNCATE TABLE logs;
来源：http://klr.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://guh.wangshuangyany.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yzk.tanke756.top

[Q56] 密集排名（并列不占位）
来源：http://xko.jyoumei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ucn.jqgufenzy.top

[Q57] 行号
来源：http://fgw.iojbl.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://azr.0kj1m.cn

[Q58] 累计求和
来源：http://dcr.316326.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dsh.316326.xyz

[Q59] 分组内累计
来源：http://oih.cucudq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pcm.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://zyr.hnqzz.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pjs.sysykeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ulp.sweek.top

[Q61] 移动平均
来源：http://trk.mhx1999.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vqp.cashguo.top

[Q62] 分组占比
来源：http://sat.zdqjudy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ahj.yj20258.top

[Q63] 开启事务
来源：http://ckd.c1oappe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ktm.kuanghao11.cn

[Q64] 提交事务
来源：http://czt.shzxlz.cn

COMMIT;
来源：http://kfh.bbcook.cn

[Q65] 回滚事务
来源：http://kac.yanxiufei.cn

ROLLBACK;
来源：http://yff.shanyushiyangtech.top

[Q66] 行锁查询
来源：http://ncz.yonumen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gop.uphjek.com

[Q67] 设置隔离级别
来源：http://uba.meibo888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tpw.shanyushiyangkeji.top

[Q68] 保存点
来源：http://kyx.nanxinkj.top

SAVEPOINT sp1;
来源：http://gze.gogol.net.cn

ROLLBACK TO sp1;
来源：http://zqc.cqqwz.cn

[Q69] 查看执行计划
来源：http://gby.aizwys.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ctd.hongshengwenyu.top

[Q70] 更新统计信息
来源：http://qjq.jqgufenzy.top

ANALYZE TABLE users;
来源：http://ixu.ppjwa.cn

[Q71] 查看建表语句
来源：http://nsx.yueranfly.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tgq.zhixingplan.top

[Q72] 查看索引
来源：http://xce.zdqjudy.top

SHOW INDEX FROM users;
来源：http://trr.redwolf501.top

[Q73] 查看表状态
来源：http://plx.kuanghao11.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wcc.9152youxi.cn

[Q74] 强制使用索引
来源：http://cmq.uphjek.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jnf.xingfuxueyuan.xyz

[Q75] 日期格式化
来源：http://znp.quarkkingdee.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zbt.meibo888.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ljg.shzxlz.cn

[Q76] 按天统计
来源：http://mjr.smart0.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fvi.hnxiangtu.top

[Q77] 时间加减
来源：http://lsm.kuanghao11.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rkk.9152youxi.cn

[Q78] 当前时间
来源：http://mrq.hysaishi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dep.yonumen.top

[Q79] 字符串拼接
来源：http://auv.xuanzx.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pbr.nwbrower.top

[Q80] 字符串截取
来源：http://mty.yueranfly.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qxs.ydjk.org.cn

[Q81] 字符串替换
来源：http://wib.pycfn.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yun.zycfv.cn

[Q82] 字符长度与字节长度
来源：http://vly.hesvh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bop.sufxvd.cn

[Q83] 大小写转换
来源：http://qlq.mhx1999.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oyq.tianlin.xyz

[Q84] 去除首尾空格
来源：http://pvs.sjlbkw.cn

SELECT TRIM(name) FROM users;
来源：http://rpq.jqgfzy.top

[Q85] 数值取整
来源：http://rla.ydzc1.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yws.pengpengdd.cyou

[Q86] 读取 JSON 字段
来源：http://vdb.zhoulong.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xkv.gzhubu.top

[Q87] JSON 字段做条件
来源：http://klh.zhijiandao.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rnk.iojbl.cn

[Q88] 行转列（条件聚合）
来源：http://xhh.jlsjyb.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wko.jiagoushi.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lqq.hywenlv.cn

[Q89] 判断表是否存在
来源：http://cgh.cashguo.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ihk.shangyingyoupin.top

[Q90] 生成序号列
来源：http://cxd.bjfxy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yrt.chenzaomai.com

================================================================================
来源：http://fix.sjlbkw.cn


<!-- 参考信息 -->