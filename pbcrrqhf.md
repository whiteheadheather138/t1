代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://ihg.andypj.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://umw.svipenyu.cn

JS:   await Promise.all(tasks)
来源：http://nxq.hcnkem.com

TS:   await Promise.all(tasks)
来源：http://ood.jyoumei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://szu.zhiwuduotai.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gjg.zhaomingkeji.xyz

Ruby: threads.map(&:join)
来源：http://aej.sweek.top

C#:   await Task.WhenAll(t1, t2)
来源：http://srd.vqdsnc.cn

[O06] 使用进程池
来源：http://xru.jinyuanbaomall.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xpr.tianlin.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://kjc.cqqwz.cn

JS:   // child_process / cluster 模块
来源：http://ltn.wangdashe.top

TS:   // child_process / cluster 模块
来源：http://ypv.yj20258888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://doi.hywenlv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eok.yj20258888.top

Ruby: // fork 块
来源：http://hri.sjlbkw.cn

C#:   Parallel.For
来源：http://jio.meibo888.top

================================================================================
来源：http://xls.epnwcf.com

P. 常用工具函数
来源：http://wlz.hcnkem.com

================================================================================
来源：http://llj.nwbrower.top

[P01] 生成 UUID
来源：http://hdr.jqgufenzy.top

Py:   str(uuid.uuid4())
来源：http://xwk.snrcjt.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iut.yj20258.top

JS:   crypto.randomUUID()
来源：http://jgj.chenlongwang.top

TS:   crypto.randomUUID()
来源：http://ugn.svipenyu.cn

Java: UUID.randomUUID().toString()
来源：http://goa.feifeiyinyue.top

Go:   // 用 github.com/google/uuid
来源：http://tca.shanyushiyangkeji.top

Ruby: SecureRandom.uuid
来源：http://ntk.fktsv.cn

C#:   Guid.NewGuid().ToString()
来源：http://uik.jinghuilouyu.cn

[P02] MD5 / SHA256 摘要
来源：http://muf.gotoacloud.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hmf.iojbl.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mfg.hesvh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gak.nanxinkj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gya.yj20258.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vhj.jlsjyb.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fqi.ppjwa.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://svs.hysaishi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fxn.dianchejie.cn

[P03] 生成短随机字符串
来源：http://hnu.ctjpmb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hnp.nanxuanxn.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eon.nwbrower.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lqh.yueranfly.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vpx.fzhhl.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://syn.kuanghao11.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lwf.jianghu66.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://psn.zdbjq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gwr.hywenlv.cn

[P04] 求长度
来源：http://raw.shanyushiyangtech.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rsm.xingfuxueyuan.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cdd.bbcook.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xja.quarkkingdee.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bhe.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://pii.pycfn.com

Go:   len(arr);  len(m)
来源：http://ygk.yvedp.cn

Ruby: x.length;  x.size
来源：http://nrb.xuanzx.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://daf.guowangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://rsy.zhengqikj.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://cpk.mhx1999.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tjd.yanxiufei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rxp.sweek.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tyz.52xcode.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uyy.hywenlv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://syc.chenlongwang.top

Ruby: a == b
来源：http://sry.sxryk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dxn.andypj.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eqx.feifeiyinyue.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uqd.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://map.aizwys.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ulu.aibaodan.cn

TS:   if (x == null) {}
来源：http://cfp.gotoacloud.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ism.0kj1m.cn

Go:   if x == nil {}
来源：http://ftp.0kj1m.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zwg.cashguo.top

C#:   if (x is null) {}
来源：http://lwl.nanxinkj.top

[P07] 防抖与节流
来源：http://phc.c1oappe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rxf.ydjk.org.cn

PHP:  // 手写时间戳比较
来源：http://mzq.ehwqpu.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jef.guowangkeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ujt.tarul.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://grz.cdnleiting.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dqk.yonumen.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qby.ctjpmb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kvu.shanyushiyangkeji.top

[P08] 处理浮点精度问题
来源：http://ful.hongshengwenyu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cpz.9152youxi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://usp.jinyuanbaomall.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sxq.c1oappe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dmm.haohaochexian.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zjd.gogol.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fwo.zhijiandao.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://eyx.hywenlv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dan.feifeiyinyue.top

================================================================================
来源：http://mkw.shuidangran.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://njf.jinghuilouyu.cn

================================================================================
来源：http://wdk.jinqigfzy.top

[Q01] 创建表
来源：http://oqi.zdbjq.cn

CREATE TABLE users (
来源：http://ois.hammf.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fal.jqgufenzy.top

name VARCHAR(50) NOT NULL,
来源：http://qvj.gaohongyu789.top

email VARCHAR(100) UNIQUE,
来源：http://xnd.nanxinkj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hxk.yuxming.cn

);
来源：http://dih.fzhhl.top

[Q02] 创建带外键的表
来源：http://fwj.gaohongyu789.top

CREATE TABLE orders (
来源：http://ywt.wangdashe.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://iyc.zhengqikj.top

user_id INT NOT NULL,
来源：http://smx.vqdsnc.cn

amount DECIMAL(10, 2),
来源：http://fzu.nanxinkj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fff.chenzaomai.com

);
来源：http://hpk.havefunace.top

[Q03] 增加列
来源：http://eme.iojbl.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://drh.xziqi.cn

[Q04] 修改列类型
来源：http://gkb.zhoulong.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ibk.shanyushiyangkeji.top

[Q05] 重命名列
来源：http://ubk.nwbrower.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vdk.kuanghao11.cn

[Q06] 删除列
来源：http://xls.tarul.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ivl.daxiang520.top

[Q07] 删除表
来源：http://xzs.fzhhl.top

DROP TABLE IF EXISTS orders;
来源：http://kdh.hongshengwenyu.top

[Q08] 创建普通索引
来源：http://pfb.gaohongyu789.top

CREATE INDEX idx_users_email ON users(email);
来源：http://evv.sysykeji.top

[Q09] 创建唯一索引
来源：http://tle.ydjk.org.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://efg.hywenlv.cn

[Q10] 插入单行
来源：http://esi.dianchejie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jlw.hcnkem.com

[Q11] 一次插入多行
来源：http://jda.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cdi.daria6918.cn

[Q12] 插入后取自增 ID
来源：http://onw.mhx1999.top

INSERT INTO users (name) VALUES ('C');
来源：http://ixh.bbcook.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://adk.cucudq.cn

[Q13] 忽略重复插入
来源：http://mci.zdqjudy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rss.pycfn.com

[Q14] 存在则更新（upsert）
来源：http://uud.yj20258888.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://osj.gzhubu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ouh.jiagoushi.top

[Q15] 查询全部
来源：http://hdc.redwolf501.top

SELECT * FROM users;
来源：http://xkw.pengpengdd.cyou

[Q16] 查询指定列
来源：http://uvs.zhongyouzk.top

SELECT id, name FROM users;
来源：http://sdk.ivvv.top

[Q17] 条件查询
来源：http://kyd.vehdjk.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jnq.mhx1999.top

[Q18] 模糊匹配
来源：http://nkn.uphjek.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bpa.ydjk.org.cn

[Q19] 范围查询
来源：http://xyp.jinyuanbaomall.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://egw.mhx1999.top

[Q20] IN 列表
来源：http://tmz.0kj1m.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wnr.feifeiyinyue.top

[Q21] 空值判断
来源：http://hwp.gogol.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://uxu.mhx1999.top

[Q22] 排序
来源：http://jvx.ppjwa.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kdc.shanyushiyangkeji.top

[Q23] 分页
来源：http://idi.wangshuangyany.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kej.zdbjq.cn

[Q24] 去重
来源：http://ohh.jqgfzy.top

SELECT DISTINCT city FROM users;
来源：http://nkr.jyoumei.cn

[Q25] 只取前 N 条
来源：http://vpz.zhongyouzk.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pys.birdmap.top

[Q26] 计数
来源：http://xos.0kj1m.cn

SELECT COUNT(*) FROM users;
来源：http://qxa.fehbvm.com

[Q27] 条件计数
来源：http://cbc.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hcz.aizwys.cn

[Q28] 求和与平均
来源：http://wmy.dianchejie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oux.shanyushiyangtech.top

[Q29] 最大最小值
来源：http://cov.smart0.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://weh.dashuyun.cn

[Q30] 分组统计
来源：http://dhs.zhaomingkeji.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://igo.yanxiufei.cn

[Q31] 分组后过滤
来源：http://aow.zhoulong.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ccd.aibaodan.cn

[Q32] 分组拼接字符串
来源：http://uxn.xziqi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qvt.bjfxy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://myc.jqgufenzy.top

[Q33] 多列分组
来源：http://mde.yuanzhike.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://edd.yangfankeji.com

[Q34] 每组取第一条
来源：http://ubr.bbcook.cn

SELECT * FROM (
来源：http://mbj.vehdjk.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ttr.bjfxy.top

) t WHERE rn = 1;
来源：http://ixi.hywenlv.cn

[Q35] 内连接
来源：http://iuo.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://twj.jinyuanbaomall.cn

[Q36] 左连接
来源：http://jsa.hfpthk.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wpo.snrcjt.cn

[Q37] 右连接
来源：http://owf.sxryk.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mcz.daxiang520.top

[Q38] 全外连接（PostgreSQL）
来源：http://grd.chenjidiqi.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kto.svipenyu.cn

[Q39] 自连接（查上下级）
来源：http://rxa.gotoacloud.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ljv.jinqigfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jen.shanyushiyangtech.top

[Q40] 交叉连接（笛卡尔积）
来源：http://mvm.fktsv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://evf.52xcode.cn

[Q41] 多表连接
来源：http://qsn.hnqzz.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nqz.fengsongda.top

JOIN users u ON u.id = o.user_id
来源：http://btt.fehbvm.com

JOIN products p ON p.id = o.product_id;
来源：http://hgz.yuanzhike.top

[Q42] 连接条件附加过滤
来源：http://rya.yanxiufei.cn

SELECT u.name, o.amount FROM users u
来源：http://ahf.jinqigufen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ykg.quarkkingdee.top

[Q43] 标量子查询
来源：http://mfl.shangyingyoupin.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://slr.yvedp.cn

[Q44] IN 子查询
来源：http://txo.fktsv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://aip.jqgufenzy.top

[Q45] EXISTS 判断存在
来源：http://cyk.yfazqb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hfm.haohaochexian.top

[Q46] NOT EXISTS 判断不存在
来源：http://icy.guowangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dqt.dashuyun.cn

[Q47] 与平均值比较
来源：http://qoc.shuidangran.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hsy.zdbjq.cn

[Q48] CTE 公用表表达式
来源：http://pal.andypj.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://avc.shzxlz.cn

SELECT * FROM t WHERE c > 5;
来源：http://fih.jinyuanbaomall.cn

[Q49] 更新单行
来源：http://egs.sweek.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xie.hysaishi.cn

[Q50] 批量更新
来源：http://ipa.fengsongda.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dwn.hesvh.cn

[Q51] 用子查询更新
来源：http://lwf.wangshuangyany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zlm.birdmap.top

[Q52] 删除指定行
来源：http://dwc.mhx1999.top

DELETE FROM users WHERE id = 10;
来源：http://via.pengpengdd.cyou

[Q53] 按条件删除
来源：http://pyw.zhaomingkeji.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dai.yj202588.top

[Q54] 清空表
来源：http://hyk.dashuyun.cn

TRUNCATE TABLE logs;
来源：http://wui.hnxiangtu.top

[Q55] 排名（并列占位）
来源：http://vbv.fzhhl.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ttv.sysykeji.top

[Q56] 密集排名（并列不占位）
来源：http://kfh.haohaochexian.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dbf.zhengqikj.top

[Q57] 行号
来源：http://vat.birdmap.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rzl.shzxlz.cn

[Q58] 累计求和
来源：http://xwf.yj20258.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ilc.c1oappe.top

[Q59] 分组内累计
来源：http://gkh.xuetiantiany.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://adt.tianlin.xyz

[Q60] 取上一行 / 下一行
来源：http://qrf.yuxming.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nfr.c1oappe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mic.cdnleiting.top

[Q61] 移动平均
来源：http://uls.wangshuangyany.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bxt.fehbvm.com

[Q62] 分组占比
来源：http://rml.wangdashe.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yvg.yuxming.cn

[Q63] 开启事务
来源：http://oli.shanyushiyangtech.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wjn.daxiang520.top

[Q64] 提交事务
来源：http://mpy.svipenyu.cn

COMMIT;
来源：http://fhe.redwolf501.top

[Q65] 回滚事务
来源：http://xgs.yongpay.top

ROLLBACK;
来源：http://img.shuidangran.top

[Q66] 行锁查询
来源：http://spz.svipenyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://aif.zhengqikj.top

[Q67] 设置隔离级别
来源：http://cru.yuxming.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mir.birdmap.top

[Q68] 保存点
来源：http://syl.yj20258888.top

SAVEPOINT sp1;
来源：http://mub.hysaishi.cn

ROLLBACK TO sp1;
来源：http://pgr.nanxuanxn.top

[Q69] 查看执行计划
来源：http://yfg.hfpthk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pvx.ivvv.top

[Q70] 更新统计信息
来源：http://hlh.yongpay.top

ANALYZE TABLE users;
来源：http://wge.mhx1999.top

[Q71] 查看建表语句
来源：http://fgk.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://aih.hammf.cn

[Q72] 查看索引
来源：http://hvj.havefunace.top

SHOW INDEX FROM users;
来源：http://bwy.0kj1m.cn

[Q73] 查看表状态
来源：http://fph.zdqjudy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kci.guannengcc.top

[Q74] 强制使用索引
来源：http://jxh.bbcook.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rcu.xylfe.cn

[Q75] 日期格式化
来源：http://bld.cqqwz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uzw.zycfv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cvj.fanxiaobao.xyz

[Q76] 按天统计
来源：http://hty.hysaishi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nqt.nanxuanxn.top

[Q77] 时间加减
来源：http://iwm.dashuyun.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yuu.yj20258888.top

[Q78] 当前时间
来源：http://zkg.yueranfly.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ukb.xuetiantiany.cn

[Q79] 字符串拼接
来源：http://yzw.epnwcf.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bio.xingfuxueyuan.xyz

[Q80] 字符串截取
来源：http://qdy.uphjek.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ksq.zhengqikj.top

[Q81] 字符串替换
来源：http://wcn.52xcode.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ydg.zhaomingkeji.xyz

[Q82] 字符长度与字节长度
来源：http://enp.snrcjt.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vwk.fzhhl.top

[Q83] 大小写转换
来源：http://pua.ctjpmb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zfm.cashguo.top

[Q84] 去除首尾空格
来源：http://wtq.cqqwz.cn

SELECT TRIM(name) FROM users;
来源：http://vpm.nanxinkj.top

[Q85] 数值取整
来源：http://biy.gzhubu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mcs.ehwqpu.com

[Q86] 读取 JSON 字段
来源：http://jtr.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lvx.dianchejie.cn

[Q87] JSON 字段做条件
来源：http://pnr.tianlin.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kjm.vehdjk.com

[Q88] 行转列（条件聚合）
来源：http://eqs.jiagoushi.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://igq.mhx1999.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wdn.hywenlv.cn

[Q89] 判断表是否存在
来源：http://kgc.9152youxi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jhi.cqqwz.cn

[Q90] 生成序号列
来源：http://wsj.zhixingplan.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lav.pengpengdd.cyou

================================================================================
来源：http://dfe.shangyingyoupin.top


<!-- 参考信息 -->