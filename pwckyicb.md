代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nfz.yj20258.top

Ruby: # 用 Fiber 或 async gem
来源：http://few.hysaishi.cn

C#:   async Task F() { await G(); }
来源：http://iom.chenlongwang.top

[O05] 并发执行并等待全部完成
来源：http://rki.ydjk.org.cn

Py:   asyncio.gather(*tasks)
来源：http://ain.ehwqpu.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://llb.c1oappe.top

JS:   await Promise.all(tasks)
来源：http://ywf.birdmap.top

TS:   await Promise.all(tasks)
来源：http://ktr.cdnleiting.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vih.guannengcc.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://urm.yongpay.top

Ruby: threads.map(&:join)
来源：http://jrt.bjfxy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://flm.bbcook.cn

[O06] 使用进程池
来源：http://zjp.zdqjudy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hnk.shanyushiyangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ngz.cheryme.top

JS:   // child_process / cluster 模块
来源：http://rfs.sxryk.cn

TS:   // child_process / cluster 模块
来源：http://vwh.shanyushiyangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sxw.xziqi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hjo.cashguo.top

Ruby: // fork 块
来源：http://upa.hysaishi.cn

C#:   Parallel.For
来源：http://knr.gogol.net.cn

================================================================================
来源：http://uoy.dianchejie.cn

P. 常用工具函数
来源：http://hrv.yonumen.top

================================================================================
来源：http://gkq.shanyushiyangkeji.top

[P01] 生成 UUID
来源：http://ypv.gaohongyu789.top

Py:   str(uuid.uuid4())
来源：http://yzr.ybcxt.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gss.bjfxy.top

JS:   crypto.randomUUID()
来源：http://qor.c1oappe.top

TS:   crypto.randomUUID()
来源：http://qjr.xingfuxueyuan.xyz

Java: UUID.randomUUID().toString()
来源：http://bpj.ivvv.top

Go:   // 用 github.com/google/uuid
来源：http://azh.birdmap.top

Ruby: SecureRandom.uuid
来源：http://zfy.vqdsnc.cn

C#:   Guid.NewGuid().ToString()
来源：http://wnz.mhx1999.top

[P02] MD5 / SHA256 摘要
来源：http://eux.quarkkingdee.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jsp.gotoacloud.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://aaf.nwbrower.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lxk.jiagoushi.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qht.gogol.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fnn.birdmap.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://efc.cqqwz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yer.hywenlv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tqw.gogol.net.cn

[P03] 生成短随机字符串
来源：http://udl.tian-w.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tyi.yangfankeji.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kgk.sysykeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fzw.hongshengwenyu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://abk.nwbrower.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fzs.tianlin.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dja.ydjk.org.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ofa.jinghuilouyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bjp.jqgfzy.top

[P04] 求长度
来源：http://msq.andypj.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nbx.tarul.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ufx.redwolf501.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tgg.hongshengwenyu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ylh.sysykeji.top

Java: list.size();  map.size();  s.length()
来源：http://rgx.sjlbkw.cn

Go:   len(arr);  len(m)
来源：http://fzt.ctjpmb.com

Ruby: x.length;  x.size
来源：http://sjg.yuxming.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ftt.52xcode.cn

[P05] 判断两个对象内容是否相等
来源：http://nvm.cashguo.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lmt.guannengcc.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qje.smart0.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cfr.jianghu66.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nig.chenjidiqi.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tvh.kuanghao11.cn

Go:   reflect.DeepEqual(a, b)
来源：http://eml.aibaodan.cn

Ruby: a == b
来源：http://zih.0kj1m.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kig.gotoacloud.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qxj.snrcjt.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://egq.dianchejie.cn

PHP:  if (empty($x)) {}
来源：http://yvj.316326.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yzi.bjfxy.top

TS:   if (x == null) {}
来源：http://asy.jinghuilouyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xld.0kj1m.cn

Go:   if x == nil {}
来源：http://hvq.guannengcc.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vms.yongpay.top

C#:   if (x is null) {}
来源：http://lhb.xinyue.icu

[P07] 防抖与节流
来源：http://scf.feifeiyinyue.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hmo.guowangkeji.top

PHP:  // 手写时间戳比较
来源：http://ihf.hnxiangtu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xrp.0kj1m.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kbf.sweek.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hot.ywan-chungtsiang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ecr.hesvh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://haa.xziqi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://aiw.cqqwz.cn

[P08] 处理浮点精度问题
来源：http://aqm.ivvv.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://klv.shangyingyoupin.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dpj.xuanzx.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ipf.chenzaomai.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ocj.jinyuanbaomall.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ewy.hammf.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cgm.quarkkingdee.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fzw.ctjpmb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eyw.yfazqb.com

================================================================================
来源：http://xjn.dianchejie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qxt.yangfankeji.com

================================================================================
来源：http://sqe.yonumen.top

[Q01] 创建表
来源：http://cwy.tanke756.top

CREATE TABLE users (
来源：http://whb.epnwcf.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vgu.iojbl.cn

name VARCHAR(50) NOT NULL,
来源：http://ykj.bbcook.cn

email VARCHAR(100) UNIQUE,
来源：http://aym.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zmj.birdmap.top

);
来源：http://mke.shanyushiyangtech.top

[Q02] 创建带外键的表
来源：http://maf.jqgfzy.top

CREATE TABLE orders (
来源：http://dzo.guowangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jvl.hfpthk.cn

user_id INT NOT NULL,
来源：http://bsv.gaohongyu789.top

amount DECIMAL(10, 2),
来源：http://ktg.jlsjyb.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jqh.yfazqb.com

);
来源：http://mxv.zhiwuduotai.top

[Q03] 增加列
来源：http://xvk.xuetiantiany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oux.kuanghao11.cn

[Q04] 修改列类型
来源：http://pjp.dianchejie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wti.chenzaomai.com

[Q05] 重命名列
来源：http://nfk.tian-w.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kxr.fktsv.cn

[Q06] 删除列
来源：http://xeu.nwbrower.top

ALTER TABLE users DROP COLUMN age;
来源：http://rih.jinyuanbaomall.cn

[Q07] 删除表
来源：http://ivy.zhiwuduotai.top

DROP TABLE IF EXISTS orders;
来源：http://gfl.sjlbkw.cn

[Q08] 创建普通索引
来源：http://gsd.redwolf501.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fam.aizwys.cn

[Q09] 创建唯一索引
来源：http://hvn.yj20258888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fsf.snrcjt.cn

[Q10] 插入单行
来源：http://kgo.guannengcc.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hkm.quarkkingdee.top

[Q11] 一次插入多行
来源：http://hld.0kj1m.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kiz.ydjk.org.cn

[Q12] 插入后取自增 ID
来源：http://bne.gaohongyu789.top

INSERT INTO users (name) VALUES ('C');
来源：http://xmx.gaohongyu789.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nrp.gogol.net.cn

[Q13] 忽略重复插入
来源：http://hhl.xinyue.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://htg.yfazqb.com

[Q14] 存在则更新（upsert）
来源：http://lwc.sysykeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ggx.shuidangran.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pjo.yonumen.top

[Q15] 查询全部
来源：http://yug.zhongyouzk.top

SELECT * FROM users;
来源：http://jga.yuanzhike.top

[Q16] 查询指定列
来源：http://pny.havefunace.top

SELECT id, name FROM users;
来源：http://fdw.nanxuanxn.top

[Q17] 条件查询
来源：http://vgh.jlsjyb.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pcm.ywan-chungtsiang.top

[Q18] 模糊匹配
来源：http://lya.xuetiantiany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ayd.0kj1m.cn

[Q19] 范围查询
来源：http://nfr.dashuyun.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jha.xingfuxueyuan.xyz

[Q20] IN 列表
来源：http://mli.bjfxy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://plb.shzxlz.cn

[Q21] 空值判断
来源：http://mwa.mhx1999.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bes.haohaochexian.top

[Q22] 排序
来源：http://epe.jqgfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zsh.fengsongda.top

[Q23] 分页
来源：http://mlr.ydjk.org.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ede.feifeiyinyue.top

[Q24] 去重
来源：http://xyc.yj20258.top

SELECT DISTINCT city FROM users;
来源：http://jqf.yanxiufei.cn

[Q25] 只取前 N 条
来源：http://pgw.0kj1m.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://smv.ivvv.top

[Q26] 计数
来源：http://bxh.shanyushiyangtech.top

SELECT COUNT(*) FROM users;
来源：http://fsz.dashuyun.cn

[Q27] 条件计数
来源：http://ehg.xylfe.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://avo.c1oappe.top

[Q28] 求和与平均
来源：http://bfd.hnqzz.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bay.chenjidiqi.icu

[Q29] 最大最小值
来源：http://cjh.sufxvd.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sbg.316326.xyz

[Q30] 分组统计
来源：http://phh.jinqigufen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ljc.zhijiandao.cn

[Q31] 分组后过滤
来源：http://lcq.sjlbkw.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hik.fengsongda.top

[Q32] 分组拼接字符串
来源：http://umj.sweek.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lfd.shangyingyoupin.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bva.kuanghao11.cn

[Q33] 多列分组
来源：http://qwz.ctjpmb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ftg.feifeiyinyue.top

[Q34] 每组取第一条
来源：http://nsv.ydzc1.top

SELECT * FROM (
来源：http://wob.gzhubu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mij.birdmap.top

) t WHERE rn = 1;
来源：http://ijr.fengsongda.top

[Q35] 内连接
来源：http://ejb.gotoacloud.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://juz.zdqjudy.top

[Q36] 左连接
来源：http://ocu.yj202588.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ova.birdmap.top

[Q37] 右连接
来源：http://pee.pycfn.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cze.epnwcf.com

[Q38] 全外连接（PostgreSQL）
来源：http://oau.yfazqb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hxi.smart0.xyz

[Q39] 自连接（查上下级）
来源：http://tcr.xylfe.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mit.chenzaomai.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mws.52xcode.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ksz.jlsjyb.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oox.xylfe.cn

[Q41] 多表连接
来源：http://age.redwolf501.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hva.hammf.cn

JOIN users u ON u.id = o.user_id
来源：http://bww.xinyue.icu

JOIN products p ON p.id = o.product_id;
来源：http://vjz.wangshuangyany.cn

[Q42] 连接条件附加过滤
来源：http://cqu.nanxinkj.top

SELECT u.name, o.amount FROM users u
来源：http://uij.hnxiangtu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vgl.xylfe.cn

[Q43] 标量子查询
来源：http://jnz.xziqi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pjg.dashuyun.cn

[Q44] IN 子查询
来源：http://ggq.nwbrower.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://opo.andypj.xyz

[Q45] EXISTS 判断存在
来源：http://bau.daxiang520.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wgi.hongshengwenyu.top

[Q46] NOT EXISTS 判断不存在
来源：http://xyr.hesvh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kco.gogol.net.cn

[Q47] 与平均值比较
来源：http://gzo.pengpengdd.cyou

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ref.jqgufenzy.top

[Q48] CTE 公用表表达式
来源：http://ugx.hongshengwenyu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://alo.sjlbkw.cn

SELECT * FROM t WHERE c > 5;
来源：http://wyx.dianchejie.cn

[Q49] 更新单行
来源：http://gpi.shangyingyoupin.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jxr.hfpthk.cn

[Q50] 批量更新
来源：http://ugy.gotoacloud.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fia.yj20258888.top

[Q51] 用子查询更新
来源：http://vnt.sufxvd.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xkt.jianghu66.top

[Q52] 删除指定行
来源：http://umr.aizwys.cn

DELETE FROM users WHERE id = 10;
来源：http://uda.sweek.top

[Q53] 按条件删除
来源：http://aiz.zhoulong.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jdc.aibaodan.cn

[Q54] 清空表
来源：http://ayn.fktsv.cn

TRUNCATE TABLE logs;
来源：http://svb.zhongyouzk.top

[Q55] 排名（并列占位）
来源：http://scj.iojbl.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rnm.tian-w.cn

[Q56] 密集排名（并列不占位）
来源：http://oks.jiagoushi.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iev.jinqigfzy.top

[Q57] 行号
来源：http://kvn.yongpay.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://urj.c1oappe.top

[Q58] 累计求和
来源：http://ycj.sufxvd.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qwl.zhaomingkeji.xyz

[Q59] 分组内累计
来源：http://bdo.yonumen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hfy.shzxlz.cn

[Q60] 取上一行 / 下一行
来源：http://tsl.yongpay.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lcv.bbcook.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lef.zhoulong.xyz

[Q61] 移动平均
来源：http://gxc.yuanzhike.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dvc.hongshengwenyu.top

[Q62] 分组占比
来源：http://qql.cdnleiting.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hdl.chenzaomai.com

[Q63] 开启事务
来源：http://qnq.aibaodan.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gmf.zhiwuduotai.top

[Q64] 提交事务
来源：http://lrx.chenjidiqi.icu

COMMIT;
来源：http://npf.vqdsnc.cn

[Q65] 回滚事务
来源：http://dyr.gotoacloud.top

ROLLBACK;
来源：http://dgr.nanxuanxn.top

[Q66] 行锁查询
来源：http://rau.fengsongda.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cjd.sysykeji.top

[Q67] 设置隔离级别
来源：http://hyk.tian-w.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rng.guowangkeji.top

[Q68] 保存点
来源：http://usx.havefunace.top

SAVEPOINT sp1;
来源：http://vzd.yanxiufei.cn

ROLLBACK TO sp1;
来源：http://nru.yj20258.top

[Q69] 查看执行计划
来源：http://ofh.fzhhl.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kvq.tian-w.cn

[Q70] 更新统计信息
来源：http://efv.yueranfly.top

ANALYZE TABLE users;
来源：http://qtq.zhiwuduotai.top

[Q71] 查看建表语句
来源：http://rqs.hnqzz.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qpp.tian-w.cn

[Q72] 查看索引
来源：http://dad.jiagoushi.top

SHOW INDEX FROM users;
来源：http://vwy.ehwqpu.com

[Q73] 查看表状态
来源：http://jyd.jyoumei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://utk.havefunace.top

[Q74] 强制使用索引
来源：http://hpc.svipenyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tvq.tarul.cn

[Q75] 日期格式化
来源：http://cil.jinqigufen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://svv.wangshuangyany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hfj.snrcjt.cn

[Q76] 按天统计
来源：http://ptq.yangfankeji.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://stv.zhoulong.xyz

[Q77] 时间加减
来源：http://ibs.yuanzhike.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wnz.kuanghao11.cn

[Q78] 当前时间
来源：http://emg.pycfn.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mlv.ydzc1.top

[Q79] 字符串拼接
来源：http://tgo.ydjk.org.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://arx.daria6918.cn

[Q80] 字符串截取
来源：http://uwr.zycfv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wta.ydzc1.top

[Q81] 字符串替换
来源：http://gby.fanxiaobao.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gsl.jlsjyb.cn

[Q82] 字符长度与字节长度
来源：http://lto.dashuyun.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cyx.dashuyun.cn

[Q83] 大小写转换
来源：http://zab.yanxiufei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ckx.iojbl.cn

[Q84] 去除首尾空格
来源：http://gsl.nwbrower.top

SELECT TRIM(name) FROM users;
来源：http://ths.jqgufenzy.top

[Q85] 数值取整
来源：http://bml.zhijiandao.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gbr.snrcjt.cn

[Q86] 读取 JSON 字段
来源：http://rwk.shanyushiyangtech.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cvv.wangshuangyany.cn

[Q87] JSON 字段做条件
来源：http://qbp.ehwqpu.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sxx.hywenlv.cn

[Q88] 行转列（条件聚合）
来源：http://pgh.wangdashe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nnh.gzhubu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lua.uphjek.com

[Q89] 判断表是否存在
来源：http://rsy.sysykeji.top


<!-- 参考信息 -->