代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://ixu.ybcxt.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rvn.jlsjyb.cn

JS:   await Promise.all(tasks)
来源：http://ixo.yj20258888.top

TS:   await Promise.all(tasks)
来源：http://zca.sufxvd.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gpg.xuanzx.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://okv.zhaomingkeji.xyz

Ruby: threads.map(&:join)
来源：http://vaz.gaohongyu789.top

C#:   await Task.WhenAll(t1, t2)
来源：http://azl.zhijiandao.cn

[O06] 使用进程池
来源：http://swg.zhaomingkeji.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://okz.hywenlv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://anf.mhx1999.top

JS:   // child_process / cluster 模块
来源：http://ggz.fktsv.cn

TS:   // child_process / cluster 模块
来源：http://tqo.52xcode.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wqz.cucudq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cny.zhengqikj.top

Ruby: // fork 块
来源：http://emf.fzhhl.top

C#:   Parallel.For
来源：http://gek.jinyuanbaomall.cn

================================================================================
来源：http://veh.guannengcc.top

P. 常用工具函数
来源：http://zhg.zycfv.cn

================================================================================
来源：http://cyt.xuanzx.com

[P01] 生成 UUID
来源：http://cxc.fehbvm.com

Py:   str(uuid.uuid4())
来源：http://vcf.daria6918.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kka.meibo888.top

JS:   crypto.randomUUID()
来源：http://gut.yonumen.top

TS:   crypto.randomUUID()
来源：http://xrh.jinyuanbaomall.cn

Java: UUID.randomUUID().toString()
来源：http://zid.yj20258888.top

Go:   // 用 github.com/google/uuid
来源：http://rdt.hammf.cn

Ruby: SecureRandom.uuid
来源：http://vhv.iojbl.cn

C#:   Guid.NewGuid().ToString()
来源：http://xuc.sufxvd.cn

[P02] MD5 / SHA256 摘要
来源：http://tyq.shuidangran.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mhk.jqgfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://daf.wangdashe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nit.zhoulong.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wmc.snrcjt.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jcj.shuidangran.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yjr.epnwcf.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pjh.zhoulong.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://deb.pengpengdd.cyou

[P03] 生成短随机字符串
来源：http://nze.yfazqb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lhw.tanke756.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://chb.zhijiandao.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vpu.guowangkeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gzt.ppjwa.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qec.andypj.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qwk.yuanzhike.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://pdu.chenlongwang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qqn.cashguo.top

[P04] 求长度
来源：http://wev.ywan-chungtsiang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qyg.smart0.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qes.cucudq.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uml.quarkkingdee.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rgz.cqqwz.cn

Java: list.size();  map.size();  s.length()
来源：http://rnk.yonumen.top

Go:   len(arr);  len(m)
来源：http://uvc.nanxuanxn.top

Ruby: x.length;  x.size
来源：http://qni.wangdashe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lkr.jinyuanbaomall.cn

[P05] 判断两个对象内容是否相等
来源：http://fcd.dashuyun.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zru.hammf.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sdc.jqgfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oar.hnxiangtu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uhm.feifeiyinyue.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hnz.sufxvd.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xcn.yangfankeji.com

Ruby: a == b
来源：http://cha.jqgufenzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eey.aizwys.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gmm.wangdashe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fof.cqqwz.cn

PHP:  if (empty($x)) {}
来源：http://aed.jinqigfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qgz.0kj1m.cn

TS:   if (x == null) {}
来源：http://ogn.ivvv.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pyn.mhx1999.top

Go:   if x == nil {}
来源：http://ljl.0kj1m.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nsd.ywan-chungtsiang.top

C#:   if (x is null) {}
来源：http://wwf.sxryk.cn

[P07] 防抖与节流
来源：http://ryi.cdnleiting.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sja.yvedp.cn

PHP:  // 手写时间戳比较
来源：http://uui.tanke756.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://phd.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yjb.daxiang520.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wuj.52xcode.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oru.wangshuangyany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ixp.svipenyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bbn.xylfe.cn

[P08] 处理浮点精度问题
来源：http://qif.uphjek.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://luh.cucudq.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hhd.yvedp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jsb.9152youxi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pcs.shzxlz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://opx.zycfv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://adf.guannengcc.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ybx.jyoumei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ioy.cashguo.top

================================================================================
来源：http://swr.tarul.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kcc.xuanzx.com

================================================================================
来源：http://iqf.zdqjudy.top

[Q01] 创建表
来源：http://wlq.bbcook.cn

CREATE TABLE users (
来源：http://ykn.yuxming.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dfy.52xcode.cn

name VARCHAR(50) NOT NULL,
来源：http://dmx.gogol.net.cn

email VARCHAR(100) UNIQUE,
来源：http://fub.hongshengwenyu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cxc.hnqzz.top

);
来源：http://rbw.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://qdc.shanyushiyangtech.top

CREATE TABLE orders (
来源：http://cph.shangyingyoupin.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vry.ybcxt.top

user_id INT NOT NULL,
来源：http://idw.zhixingplan.top

amount DECIMAL(10, 2),
来源：http://cjx.ctjpmb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qyt.gotoacloud.top

);
来源：http://nlc.yanxiufei.cn

[Q03] 增加列
来源：http://zje.fzhhl.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kio.sxryk.cn

[Q04] 修改列类型
来源：http://aek.chenzaomai.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kue.daria6918.cn

[Q05] 重命名列
来源：http://pkl.dianchejie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ffi.cdnleiting.top

[Q06] 删除列
来源：http://hjl.cdnleiting.top

ALTER TABLE users DROP COLUMN age;
来源：http://kii.vehdjk.com

[Q07] 删除表
来源：http://xeu.yvedp.cn

DROP TABLE IF EXISTS orders;
来源：http://hsw.9152youxi.cn

[Q08] 创建普通索引
来源：http://tnm.jyoumei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pse.hnxiangtu.top

[Q09] 创建唯一索引
来源：http://cnc.daria6918.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zqj.cqqwz.cn

[Q10] 插入单行
来源：http://kli.feifeiyinyue.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ouj.epnwcf.com

[Q11] 一次插入多行
来源：http://qew.0kj1m.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vin.dashuyun.cn

[Q12] 插入后取自增 ID
来源：http://jxs.jinyuanbaomall.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fpv.zhoulong.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dms.cdnleiting.top

[Q13] 忽略重复插入
来源：http://sul.chenzaomai.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qmd.jlsjyb.cn

[Q14] 存在则更新（upsert）
来源：http://lnt.ivvv.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://plp.gaohongyu789.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://noe.ybcxt.top

[Q15] 查询全部
来源：http://hxy.nanxuanxn.top

SELECT * FROM users;
来源：http://icg.hywenlv.cn

[Q16] 查询指定列
来源：http://apc.nanxuanxn.top

SELECT id, name FROM users;
来源：http://jte.andypj.xyz

[Q17] 条件查询
来源：http://pjj.c1oappe.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hkj.xinyue.icu

[Q18] 模糊匹配
来源：http://fyy.fanxiaobao.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ado.guowangkeji.top

[Q19] 范围查询
来源：http://xuz.shzxlz.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wuw.ivvv.top

[Q20] IN 列表
来源：http://bmq.gotoacloud.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yjn.gaohongyu789.top

[Q21] 空值判断
来源：http://ujq.cheryme.top

SELECT * FROM users WHERE email IS NULL;
来源：http://hxq.chenzaomai.com

[Q22] 排序
来源：http://xsv.yuanzhike.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hba.xziqi.cn

[Q23] 分页
来源：http://lge.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bfd.hcnkem.com

[Q24] 去重
来源：http://vik.jiagoushi.top

SELECT DISTINCT city FROM users;
来源：http://crk.chenzaomai.com

[Q25] 只取前 N 条
来源：http://ail.cashguo.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tpx.jyoumei.cn

[Q26] 计数
来源：http://art.hongshengwenyu.top

SELECT COUNT(*) FROM users;
来源：http://msi.zhaomingkeji.xyz

[Q27] 条件计数
来源：http://izw.yj20258888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://act.shuidangran.top

[Q28] 求和与平均
来源：http://vwu.hnxiangtu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ost.zdbjq.cn

[Q29] 最大最小值
来源：http://eqa.hnqzz.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vzp.hnqzz.top

[Q30] 分组统计
来源：http://tya.snrcjt.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hoj.ybcxt.top

[Q31] 分组后过滤
来源：http://fuf.yj20258.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bgo.daxiang520.top

[Q32] 分组拼接字符串
来源：http://bmj.pycfn.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://njn.wangshuangyany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gqk.mhx1999.top

[Q33] 多列分组
来源：http://xhy.hnqzz.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mjl.yangfankeji.com

[Q34] 每组取第一条
来源：http://mmn.uphjek.com

SELECT * FROM (
来源：http://tos.zdbjq.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hqm.ybcxt.top

) t WHERE rn = 1;
来源：http://kdo.hnqzz.top

[Q35] 内连接
来源：http://rwc.chenzaomai.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fmk.tian-w.cn

[Q36] 左连接
来源：http://dil.hywenlv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://squ.gotoacloud.top

[Q37] 右连接
来源：http://tmk.dianchejie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://woi.jianghu66.top

[Q38] 全外连接（PostgreSQL）
来源：http://hkv.yj202588.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dfr.aibaodan.cn

[Q39] 自连接（查上下级）
来源：http://jvk.feifeiyinyue.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dbd.jlsjyb.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://evm.vqdsnc.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://egc.jlsjyb.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dym.fehbvm.com

[Q41] 多表连接
来源：http://xhp.vehdjk.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://gqv.quarkkingdee.top

JOIN users u ON u.id = o.user_id
来源：http://fbv.chenzaomai.com

JOIN products p ON p.id = o.product_id;
来源：http://flo.quarkkingdee.top

[Q42] 连接条件附加过滤
来源：http://qny.jlsjyb.cn

SELECT u.name, o.amount FROM users u
来源：http://dmu.ybcxt.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eax.zhixingplan.top

[Q43] 标量子查询
来源：http://kbg.guannengcc.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vyh.jinghuilouyu.cn

[Q44] IN 子查询
来源：http://kwx.iojbl.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zog.smart0.xyz

[Q45] EXISTS 判断存在
来源：http://dwb.fehbvm.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://klf.hongshengwenyu.top

[Q46] NOT EXISTS 判断不存在
来源：http://swg.birdmap.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jnq.fengsongda.top

[Q47] 与平均值比较
来源：http://wbt.zhixingplan.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uzl.xylfe.cn

[Q48] CTE 公用表表达式
来源：http://sgj.sxryk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oqy.kuanghao11.cn

SELECT * FROM t WHERE c > 5;
来源：http://bou.tian-w.cn

[Q49] 更新单行
来源：http://wvi.feifeiyinyue.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://teh.jinghuilouyu.cn

[Q50] 批量更新
来源：http://epf.aizwys.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://taf.cucudq.cn

[Q51] 用子查询更新
来源：http://zbo.hcnkem.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bgj.andypj.xyz

[Q52] 删除指定行
来源：http://atr.bbcook.cn

DELETE FROM users WHERE id = 10;
来源：http://opj.jyoumei.cn

[Q53] 按条件删除
来源：http://gmh.aizwys.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hzt.shangyingyoupin.top

[Q54] 清空表
来源：http://dsj.chenlongwang.top

TRUNCATE TABLE logs;
来源：http://eac.chenlongwang.top

[Q55] 排名（并列占位）
来源：http://gyl.tian-w.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mow.fzhhl.top

[Q56] 密集排名（并列不占位）
来源：http://vqz.gotoacloud.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mog.zhengqikj.top

[Q57] 行号
来源：http://hls.zhoulong.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rfr.jqgfzy.top

[Q58] 累计求和
来源：http://xmi.tian-w.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uzu.cheryme.top

[Q59] 分组内累计
来源：http://bgh.yangfankeji.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vbk.hcnkem.com

[Q60] 取上一行 / 下一行
来源：http://rfp.fengsongda.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rjb.snrcjt.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://noy.guannengcc.top

[Q61] 移动平均
来源：http://thm.ywan-chungtsiang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ckp.tian-w.cn

[Q62] 分组占比
来源：http://vfm.yj20258.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dvd.xylfe.cn

[Q63] 开启事务
来源：http://gpj.hesvh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qpe.jinqigfzy.top

[Q64] 提交事务
来源：http://iom.9152youxi.cn

COMMIT;
来源：http://jsa.yongpay.top

[Q65] 回滚事务
来源：http://coh.wangdashe.top

ROLLBACK;
来源：http://xvz.havefunace.top

[Q66] 行锁查询
来源：http://ciu.xingfuxueyuan.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://euj.fehbvm.com

[Q67] 设置隔离级别
来源：http://mzt.sweek.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rlu.ctjpmb.com

[Q68] 保存点
来源：http://yod.cashguo.top

SAVEPOINT sp1;
来源：http://vmv.kuanghao11.cn

ROLLBACK TO sp1;
来源：http://ccd.yanxiufei.cn

[Q69] 查看执行计划
来源：http://sqi.dianchejie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ftm.chenlongwang.top

[Q70] 更新统计信息
来源：http://nzz.ywan-chungtsiang.top

ANALYZE TABLE users;
来源：http://ncf.tarul.cn

[Q71] 查看建表语句
来源：http://uds.fehbvm.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mpx.chenjidiqi.icu

[Q72] 查看索引
来源：http://hdw.bjfxy.top

SHOW INDEX FROM users;
来源：http://gzw.zhiwuduotai.top

[Q73] 查看表状态
来源：http://ymw.0kj1m.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fvk.shanyushiyangtech.top

[Q74] 强制使用索引
来源：http://olq.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tcb.wangshuangyany.cn

[Q75] 日期格式化
来源：http://ply.yj20258888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kby.yfazqb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mtd.zycfv.cn

[Q76] 按天统计
来源：http://qbp.tian-w.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bzr.nanxinkj.top

[Q77] 时间加减
来源：http://wdo.zycfv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nov.quarkkingdee.top

[Q78] 当前时间
来源：http://pzx.redwolf501.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xye.pycfn.com

[Q79] 字符串拼接
来源：http://sjs.hnxiangtu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ojv.gotoacloud.top

[Q80] 字符串截取
来源：http://dwn.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zht.dashuyun.cn

[Q81] 字符串替换
来源：http://eah.aibaodan.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://npl.hywenlv.cn

[Q82] 字符长度与字节长度
来源：http://tsj.jinghuilouyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bey.jiagoushi.top

[Q83] 大小写转换
来源：http://egx.xziqi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qjh.yuxming.cn

[Q84] 去除首尾空格
来源：http://cpq.tian-w.cn

SELECT TRIM(name) FROM users;
来源：http://yka.yj202588.top

[Q85] 数值取整
来源：http://euq.xylfe.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://oga.ctjpmb.com

[Q86] 读取 JSON 字段
来源：http://bzr.sufxvd.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ymt.nwbrower.top

[Q87] JSON 字段做条件
来源：http://vth.vqdsnc.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gpy.vqdsnc.cn

[Q88] 行转列（条件聚合）
来源：http://nks.316326.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://trx.pycfn.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dhf.wangshuangyany.cn

[Q89] 判断表是否存在
来源：http://irw.yj20258.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bzh.zycfv.cn

[Q90] 生成序号列
来源：http://slh.shzxlz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mum.yueranfly.top

================================================================================
来源：http://nmq.xinyue.icu


<!-- 参考信息 -->