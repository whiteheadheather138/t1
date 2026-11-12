代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://zti.tianlin.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://txv.dianchejie.cn

JS:   await Promise.all(tasks)
来源：http://iqf.hcnkem.com

TS:   await Promise.all(tasks)
来源：http://ldn.hesvh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uyt.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hlc.nwbrower.top

Ruby: threads.map(&:join)
来源：http://qna.0kj1m.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xla.ydjk.org.cn

[O06] 使用进程池
来源：http://zpd.wangdashe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mhi.sjlbkw.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nqg.0kj1m.cn

JS:   // child_process / cluster 模块
来源：http://cxf.andypj.xyz

TS:   // child_process / cluster 模块
来源：http://lgy.zhijiandao.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://muc.zycfv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://etw.yuxming.cn

Ruby: // fork 块
来源：http://zlj.tian-w.cn

C#:   Parallel.For
来源：http://wgi.nanxuanxn.top

================================================================================
来源：http://rfv.xylfe.cn

P. 常用工具函数
来源：http://ufz.yvedp.cn

================================================================================
来源：http://bnk.sjlbkw.cn

[P01] 生成 UUID
来源：http://uqi.jyoumei.cn

Py:   str(uuid.uuid4())
来源：http://mwc.fengsongda.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tpq.hammf.cn

JS:   crypto.randomUUID()
来源：http://apk.yfazqb.com

TS:   crypto.randomUUID()
来源：http://rgb.jqgfzy.top

Java: UUID.randomUUID().toString()
来源：http://bkf.bbcook.cn

Go:   // 用 github.com/google/uuid
来源：http://bqd.daria6918.cn

Ruby: SecureRandom.uuid
来源：http://ksd.uphjek.com

C#:   Guid.NewGuid().ToString()
来源：http://vft.guowangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://cfw.fehbvm.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jmm.9152youxi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mtw.wangshuangyany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wvr.tarul.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yxg.9152youxi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zhy.tian-w.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fhi.redwolf501.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rck.cdnleiting.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vqp.yongpay.top

[P03] 生成短随机字符串
来源：http://vml.cashguo.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://osh.pycfn.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ucj.zhoulong.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://syo.jiagoushi.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yso.chenjidiqi.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qaq.ydjk.org.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rfq.sweek.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xrq.shanyushiyangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://akw.feifeiyinyue.top

[P04] 求长度
来源：http://dzj.chenzaomai.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://emg.vehdjk.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gfu.yj20258.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jcz.zhixingplan.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dgf.kuanghao11.cn

Java: list.size();  map.size();  s.length()
来源：http://zmh.svipenyu.cn

Go:   len(arr);  len(m)
来源：http://hrt.yueranfly.top

Ruby: x.length;  x.size
来源：http://cqk.iojbl.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gat.ctjpmb.com

[P05] 判断两个对象内容是否相等
来源：http://yjc.jqgfzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://cnx.jinqigufen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ckm.nanxuanxn.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xhy.jiagoushi.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uti.hesvh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://arb.shangyingyoupin.top

Go:   reflect.DeepEqual(a, b)
来源：http://qkn.aibaodan.cn

Ruby: a == b
来源：http://yvm.wangdashe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://itd.cqqwz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://inj.yangfankeji.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zcn.hnqzz.top

PHP:  if (empty($x)) {}
来源：http://fdm.guannengcc.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://urf.nanxinkj.top

TS:   if (x == null) {}
来源：http://vst.zdbjq.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vyz.cucudq.cn

Go:   if x == nil {}
来源：http://nev.yueranfly.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ktw.aizwys.cn

C#:   if (x is null) {}
来源：http://gmg.chenzaomai.com

[P07] 防抖与节流
来源：http://dan.kuanghao11.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ekk.c1oappe.top

PHP:  // 手写时间戳比较
来源：http://xii.vehdjk.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rna.yvedp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lne.shangyingyoupin.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lso.cheryme.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ohs.zdqjudy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zlg.tarul.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oam.daxiang520.top

[P08] 处理浮点精度问题
来源：http://ntf.yfazqb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lvw.ybcxt.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wpb.meibo888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qob.ybcxt.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vpv.shangyingyoupin.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://smc.feifeiyinyue.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mqa.wangshuangyany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gfw.hywenlv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lge.zhoulong.xyz

================================================================================
来源：http://fxn.xuetiantiany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lpn.jianghu66.top

================================================================================
来源：http://qay.zycfv.cn

[Q01] 创建表
来源：http://ork.zdqjudy.top

CREATE TABLE users (
来源：http://edz.nwbrower.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kru.sweek.top

name VARCHAR(50) NOT NULL,
来源：http://fqy.jqgufenzy.top

email VARCHAR(100) UNIQUE,
来源：http://wyx.ydjk.org.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iol.jqgfzy.top

);
来源：http://hha.hfpthk.cn

[Q02] 创建带外键的表
来源：http://jkl.ywan-chungtsiang.top

CREATE TABLE orders (
来源：http://nri.hnxiangtu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://clh.tarul.cn

user_id INT NOT NULL,
来源：http://czn.pengpengdd.cyou

amount DECIMAL(10, 2),
来源：http://yop.dianchejie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kae.smart0.xyz

);
来源：http://utd.hysaishi.cn

[Q03] 增加列
来源：http://siw.hnxiangtu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sug.jiagoushi.top

[Q04] 修改列类型
来源：http://zfn.zhongyouzk.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://asx.nanxinkj.top

[Q05] 重命名列
来源：http://hed.yueranfly.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ytv.kuanghao11.cn

[Q06] 删除列
来源：http://rev.pengpengdd.cyou

ALTER TABLE users DROP COLUMN age;
来源：http://rvg.yfazqb.com

[Q07] 删除表
来源：http://ksf.mhx1999.top

DROP TABLE IF EXISTS orders;
来源：http://vtq.hfpthk.cn

[Q08] 创建普通索引
来源：http://clw.chenzaomai.com

CREATE INDEX idx_users_email ON users(email);
来源：http://wks.yangfankeji.com

[Q09] 创建唯一索引
来源：http://wjd.jyoumei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ltw.sufxvd.cn

[Q10] 插入单行
来源：http://igr.bjfxy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oti.ctjpmb.com

[Q11] 一次插入多行
来源：http://trp.svipenyu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sqq.zhengqikj.top

[Q12] 插入后取自增 ID
来源：http://oxt.smart0.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://wdz.zhongyouzk.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cmz.jqgufenzy.top

[Q13] 忽略重复插入
来源：http://wai.ydzc1.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ctt.jqgfzy.top

[Q14] 存在则更新（upsert）
来源：http://vti.cdnleiting.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kjq.chenjidiqi.icu

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ieo.yanxiufei.cn

[Q15] 查询全部
来源：http://rvg.gaohongyu789.top

SELECT * FROM users;
来源：http://hfs.jqgufenzy.top

[Q16] 查询指定列
来源：http://aox.zhoulong.xyz

SELECT id, name FROM users;
来源：http://ytl.gaohongyu789.top

[Q17] 条件查询
来源：http://csl.tianlin.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wwd.daria6918.cn

[Q18] 模糊匹配
来源：http://ozk.shzxlz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qge.jlsjyb.cn

[Q19] 范围查询
来源：http://vyn.fengsongda.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wis.aibaodan.cn

[Q20] IN 列表
来源：http://ryw.yonumen.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vol.ehwqpu.com

[Q21] 空值判断
来源：http://vbt.yj20258.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qde.hfpthk.cn

[Q22] 排序
来源：http://pyi.havefunace.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://awf.tian-w.cn

[Q23] 分页
来源：http://nna.wangshuangyany.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rfr.fengsongda.top

[Q24] 去重
来源：http://mko.tian-w.cn

SELECT DISTINCT city FROM users;
来源：http://faw.yueranfly.top

[Q25] 只取前 N 条
来源：http://nap.chenlongwang.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gej.aizwys.cn

[Q26] 计数
来源：http://mko.hnxiangtu.top

SELECT COUNT(*) FROM users;
来源：http://pgk.jqgfzy.top

[Q27] 条件计数
来源：http://crp.yj20258.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wwo.shangyingyoupin.top

[Q28] 求和与平均
来源：http://hcl.9152youxi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xji.cashguo.top

[Q29] 最大最小值
来源：http://zzr.ctjpmb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://rqd.jiagoushi.top

[Q30] 分组统计
来源：http://xyc.shuidangran.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cgo.wangdashe.top

[Q31] 分组后过滤
来源：http://zfc.gotoacloud.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xag.birdmap.top

[Q32] 分组拼接字符串
来源：http://yvv.dianchejie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wde.nwbrower.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qes.cheryme.top

[Q33] 多列分组
来源：http://gub.bjfxy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ris.zhengqikj.top

[Q34] 每组取第一条
来源：http://npp.yj20258.top

SELECT * FROM (
来源：http://wsc.mhx1999.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pal.shangyingyoupin.top

) t WHERE rn = 1;
来源：http://vud.fengsongda.top

[Q35] 内连接
来源：http://nbt.tanke756.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://llk.jinqigfzy.top

[Q36] 左连接
来源：http://qsk.yuanzhike.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fdt.ybcxt.top

[Q37] 右连接
来源：http://zhp.shangyingyoupin.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wsa.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ork.smart0.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ojj.vqdsnc.cn

[Q39] 自连接（查上下级）
来源：http://ndc.redwolf501.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ytw.316326.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qtc.haohaochexian.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vso.yj20258.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jrr.chenjidiqi.icu

[Q41] 多表连接
来源：http://gty.pengpengdd.cyou

SELECT o.id, u.name, p.title FROM orders o
来源：http://kyf.gzhubu.top

JOIN users u ON u.id = o.user_id
来源：http://svx.tian-w.cn

JOIN products p ON p.id = o.product_id;
来源：http://tzl.9152youxi.cn

[Q42] 连接条件附加过滤
来源：http://qrz.uphjek.com

SELECT u.name, o.amount FROM users u
来源：http://put.dianchejie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://itm.jqgfzy.top

[Q43] 标量子查询
来源：http://oiz.c1oappe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jfg.zhoulong.xyz

[Q44] IN 子查询
来源：http://ppu.vqdsnc.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iqc.nanxuanxn.top

[Q45] EXISTS 判断存在
来源：http://sfy.chenlongwang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mej.nanxuanxn.top

[Q46] NOT EXISTS 判断不存在
来源：http://jur.haohaochexian.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ijt.hesvh.cn

[Q47] 与平均值比较
来源：http://izk.zhixingplan.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pri.dashuyun.cn

[Q48] CTE 公用表表达式
来源：http://www.ybcxt.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yqx.zhiwuduotai.top

SELECT * FROM t WHERE c > 5;
来源：http://uen.ivvv.top

[Q49] 更新单行
来源：http://wgr.fanxiaobao.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fsv.epnwcf.com

[Q50] 批量更新
来源：http://era.mhx1999.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bss.chenjidiqi.icu

[Q51] 用子查询更新
来源：http://xxi.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zdv.jinghuilouyu.cn

[Q52] 删除指定行
来源：http://pme.jiagoushi.top

DELETE FROM users WHERE id = 10;
来源：http://mce.aibaodan.cn

[Q53] 按条件删除
来源：http://zsy.gaohongyu789.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://isj.hnxiangtu.top

[Q54] 清空表
来源：http://xnv.zhaomingkeji.xyz

TRUNCATE TABLE logs;
来源：http://ltj.zycfv.cn

[Q55] 排名（并列占位）
来源：http://nnt.pengpengdd.cyou

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oiu.zhoulong.xyz

[Q56] 密集排名（并列不占位）
来源：http://yob.gaohongyu789.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mtb.guowangkeji.top

[Q57] 行号
来源：http://eym.ywan-chungtsiang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qqy.xingfuxueyuan.xyz

[Q58] 累计求和
来源：http://awa.jyoumei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wkr.jianghu66.top

[Q59] 分组内累计
来源：http://jej.jinqigufen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://roq.jinqigfzy.top

[Q60] 取上一行 / 下一行
来源：http://psx.jinyuanbaomall.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://duc.bjfxy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pye.yj20258.top

[Q61] 移动平均
来源：http://lwf.9152youxi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xqa.ydzc1.top

[Q62] 分组占比
来源：http://tec.sysykeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ydy.nwbrower.top

[Q63] 开启事务
来源：http://eea.bbcook.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jol.meibo888.top

[Q64] 提交事务
来源：http://tsd.xziqi.cn

COMMIT;
来源：http://sbc.bbcook.cn

[Q65] 回滚事务
来源：http://pvy.fehbvm.com

ROLLBACK;
来源：http://pfc.zdqjudy.top

[Q66] 行锁查询
来源：http://ilh.ydjk.org.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mcg.andypj.xyz

[Q67] 设置隔离级别
来源：http://yxc.uphjek.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://axy.yongpay.top

[Q68] 保存点
来源：http://rbg.shzxlz.cn

SAVEPOINT sp1;
来源：http://muv.sjlbkw.cn

ROLLBACK TO sp1;
来源：http://fkc.shzxlz.cn

[Q69] 查看执行计划
来源：http://yxk.guowangkeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hcx.aizwys.cn

[Q70] 更新统计信息
来源：http://mri.cdnleiting.top

ANALYZE TABLE users;
来源：http://aqg.ivvv.top

[Q71] 查看建表语句
来源：http://zor.jqgfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yzg.zhixingplan.top

[Q72] 查看索引
来源：http://bum.nanxinkj.top

SHOW INDEX FROM users;
来源：http://lhe.svipenyu.cn

[Q73] 查看表状态
来源：http://vja.ivvv.top

SHOW TABLE STATUS LIKE 'users';
来源：http://yeu.yuxming.cn

[Q74] 强制使用索引
来源：http://izr.hammf.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pnx.shuidangran.top

[Q75] 日期格式化
来源：http://vim.gaohongyu789.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tyr.jqgfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tpu.ydzc1.top

[Q76] 按天统计
来源：http://gtf.zycfv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vlm.zhaomingkeji.xyz

[Q77] 时间加减
来源：http://pwu.daria6918.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://igm.yanxiufei.cn

[Q78] 当前时间
来源：http://nel.shuidangran.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://twa.ydjk.org.cn

[Q79] 字符串拼接
来源：http://nlq.gzhubu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://own.shuidangran.top

[Q80] 字符串截取
来源：http://buq.ywan-chungtsiang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yad.yvedp.cn

[Q81] 字符串替换
来源：http://fvr.guannengcc.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nvx.hfpthk.cn

[Q82] 字符长度与字节长度
来源：http://hvy.yuxming.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zvm.kuanghao11.cn

[Q83] 大小写转换
来源：http://srh.chenzaomai.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fsw.zhongyouzk.top

[Q84] 去除首尾空格
来源：http://els.yanxiufei.cn

SELECT TRIM(name) FROM users;
来源：http://ecv.zdqjudy.top

[Q85] 数值取整
来源：http://nwx.andypj.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mqt.pycfn.com

[Q86] 读取 JSON 字段
来源：http://lec.chenlongwang.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rdw.zhengqikj.top

[Q87] JSON 字段做条件
来源：http://dyw.gaohongyu789.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fan.zdqjudy.top

[Q88] 行转列（条件聚合）
来源：http://aqo.uphjek.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://swj.xylfe.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eih.hnxiangtu.top

[Q89] 判断表是否存在
来源：http://xdy.fzhhl.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://shs.jiagoushi.top

[Q90] 生成序号列
来源：http://ulb.zhixingplan.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kqq.iojbl.cn

================================================================================
来源：http://bke.zhijiandao.cn


<!-- 参考信息 -->