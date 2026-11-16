代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://etb.fktsv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lmk.yfazqb.com

C#:   async Task F() { await G(); }
来源：http://hwz.guowangkeji.top

[O05] 并发执行并等待全部完成
来源：http://hyl.fengsongda.top

Py:   asyncio.gather(*tasks)
来源：http://aia.hammf.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://okk.yongpay.top

JS:   await Promise.all(tasks)
来源：http://bny.316326.xyz

TS:   await Promise.all(tasks)
来源：http://qjm.yj20258.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ayh.shuidangran.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oik.jqgufenzy.top

Ruby: threads.map(&:join)
来源：http://tvr.zhijiandao.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zdu.feifeiyinyue.top

[O06] 使用进程池
来源：http://kur.wangshuangyany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sds.hfpthk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://knp.epnwcf.com

JS:   // child_process / cluster 模块
来源：http://vac.sjlbkw.cn

TS:   // child_process / cluster 模块
来源：http://igh.guowangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oiz.jinqigfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dzn.yj202588.top

Ruby: // fork 块
来源：http://uit.gzhubu.top

C#:   Parallel.For
来源：http://rag.jqgufenzy.top

================================================================================
来源：http://jzp.feifeiyinyue.top

P. 常用工具函数
来源：http://zow.hywenlv.cn

================================================================================
来源：http://ppm.fzhhl.top

[P01] 生成 UUID
来源：http://pyg.shuidangran.top

Py:   str(uuid.uuid4())
来源：http://fym.xylfe.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kpa.cucudq.cn

JS:   crypto.randomUUID()
来源：http://vcj.316326.xyz

TS:   crypto.randomUUID()
来源：http://hpb.jlsjyb.cn

Java: UUID.randomUUID().toString()
来源：http://fyt.fzhhl.top

Go:   // 用 github.com/google/uuid
来源：http://wdg.daria6918.cn

Ruby: SecureRandom.uuid
来源：http://zzq.jinqigufen.top

C#:   Guid.NewGuid().ToString()
来源：http://lvu.zycfv.cn

[P02] MD5 / SHA256 摘要
来源：http://ugr.shanyushiyangtech.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ptf.gaohongyu789.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wmw.zhijiandao.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jaj.vehdjk.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lov.yj202588.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hxp.daria6918.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wpp.redwolf501.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fjv.xziqi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://urz.hysaishi.cn

[P03] 生成短随机字符串
来源：http://lku.pengpengdd.cyou

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mpt.ctjpmb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://toj.zycfv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rnq.nanxuanxn.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rsa.ywan-chungtsiang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rlv.jinyuanbaomall.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aiz.nanxinkj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xny.tian-w.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://aaw.jinqigfzy.top

[P04] 求长度
来源：http://buo.gotoacloud.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://aqb.dianchejie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bzh.yangfankeji.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uxf.zhongyouzk.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mcc.haohaochexian.top

Java: list.size();  map.size();  s.length()
来源：http://baa.dashuyun.cn

Go:   len(arr);  len(m)
来源：http://dhd.andypj.xyz

Ruby: x.length;  x.size
来源：http://kxz.haohaochexian.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bsa.guowangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://ehg.zhoulong.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://ztq.gogol.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://aog.xinyue.icu

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xxh.haohaochexian.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dkt.xinyue.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xjx.jiagoushi.top

Go:   reflect.DeepEqual(a, b)
来源：http://xcm.hywenlv.cn

Ruby: a == b
来源：http://kbr.chenzaomai.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rkq.cashguo.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wwu.hcnkem.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ajw.dashuyun.cn

PHP:  if (empty($x)) {}
来源：http://hon.sjlbkw.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://roi.zycfv.cn

TS:   if (x == null) {}
来源：http://lel.chenzaomai.com

Java: if (x == null || x.isEmpty()) {}
来源：http://crm.aizwys.cn

Go:   if x == nil {}
来源：http://snn.zhijiandao.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sva.hnqzz.top

C#:   if (x is null) {}
来源：http://gjf.daria6918.cn

[P07] 防抖与节流
来源：http://idl.cashguo.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qrh.gzhubu.top

PHP:  // 手写时间戳比较
来源：http://xbo.tarul.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rqo.yueranfly.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qsc.tanke756.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://eqx.jqgufenzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ril.zhiwuduotai.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ptn.hfpthk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ioj.chenlongwang.top

[P08] 处理浮点精度问题
来源：http://vha.sysykeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xga.hysaishi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vrt.daxiang520.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yjj.52xcode.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ovf.epnwcf.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rqt.birdmap.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fpe.hongshengwenyu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://svp.zdqjudy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bzx.hammf.cn

================================================================================
来源：http://cym.ctjpmb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xqg.316326.xyz

================================================================================
来源：http://bry.wangdashe.top

[Q01] 创建表
来源：http://gix.guowangkeji.top

CREATE TABLE users (
来源：http://vxu.cdnleiting.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://afl.shanyushiyangtech.top

name VARCHAR(50) NOT NULL,
来源：http://tgf.yj20258.top

email VARCHAR(100) UNIQUE,
来源：http://ilk.9152youxi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ott.fehbvm.com

);
来源：http://wno.xylfe.cn

[Q02] 创建带外键的表
来源：http://dwi.xuanzx.com

CREATE TABLE orders (
来源：http://hho.ppjwa.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xrb.fengsongda.top

user_id INT NOT NULL,
来源：http://xgi.c1oappe.top

amount DECIMAL(10, 2),
来源：http://qsd.ivvv.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mei.aizwys.cn

);
来源：http://kym.yueranfly.top

[Q03] 增加列
来源：http://ayf.shangyingyoupin.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jks.hysaishi.cn

[Q04] 修改列类型
来源：http://llx.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ogm.ppjwa.cn

[Q05] 重命名列
来源：http://hqw.daxiang520.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zie.daria6918.cn

[Q06] 删除列
来源：http://xuh.jianghu66.top

ALTER TABLE users DROP COLUMN age;
来源：http://osv.shangyingyoupin.top

[Q07] 删除表
来源：http://jwy.shangyingyoupin.top

DROP TABLE IF EXISTS orders;
来源：http://lyn.c1oappe.top

[Q08] 创建普通索引
来源：http://xdl.nanxuanxn.top

CREATE INDEX idx_users_email ON users(email);
来源：http://dji.shanyushiyangtech.top

[Q09] 创建唯一索引
来源：http://lbw.shanyushiyangtech.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ljp.zhoulong.xyz

[Q10] 插入单行
来源：http://jgm.birdmap.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://box.zhengqikj.top

[Q11] 一次插入多行
来源：http://rdp.tanke756.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ttb.jiagoushi.top

[Q12] 插入后取自增 ID
来源：http://thc.zhaomingkeji.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://gyu.jinqigufen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wqi.hnxiangtu.top

[Q13] 忽略重复插入
来源：http://gif.yj20258888.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://req.kuanghao11.cn

[Q14] 存在则更新（upsert）
来源：http://fjj.shanyushiyangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nul.hfpthk.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wmd.ppjwa.cn

[Q15] 查询全部
来源：http://qty.jinqigfzy.top

SELECT * FROM users;
来源：http://ahy.dianchejie.cn

[Q16] 查询指定列
来源：http://edq.shangyingyoupin.top

SELECT id, name FROM users;
来源：http://kjo.nwbrower.top

[Q17] 条件查询
来源：http://pwf.hywenlv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jyg.ydzc1.top

[Q18] 模糊匹配
来源：http://hdw.cqqwz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rad.ivvv.top

[Q19] 范围查询
来源：http://cxl.vqdsnc.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lxj.hammf.cn

[Q20] IN 列表
来源：http://izl.sxryk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eck.zhoulong.xyz

[Q21] 空值判断
来源：http://llk.kuanghao11.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xqt.uphjek.com

[Q22] 排序
来源：http://zlx.hammf.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hks.gotoacloud.top

[Q23] 分页
来源：http://ojf.cheryme.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://aop.fzhhl.top

[Q24] 去重
来源：http://hew.daxiang520.top

SELECT DISTINCT city FROM users;
来源：http://fqs.cashguo.top

[Q25] 只取前 N 条
来源：http://ktz.tarul.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gfs.ywan-chungtsiang.top

[Q26] 计数
来源：http://tww.bbcook.cn

SELECT COUNT(*) FROM users;
来源：http://jsa.ppjwa.cn

[Q27] 条件计数
来源：http://brh.yueranfly.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yyg.zhaomingkeji.xyz

[Q28] 求和与平均
来源：http://zif.sxryk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dpa.shzxlz.cn

[Q29] 最大最小值
来源：http://nrs.yj202588.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xyr.yuxming.cn

[Q30] 分组统计
来源：http://cnq.ydzc1.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xka.xingfuxueyuan.xyz

[Q31] 分组后过滤
来源：http://mvh.shzxlz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pdc.ppjwa.cn

[Q32] 分组拼接字符串
来源：http://nzp.xuanzx.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gua.yfazqb.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ttb.yuanzhike.top

[Q33] 多列分组
来源：http://kzr.ivvv.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://opw.guowangkeji.top

[Q34] 每组取第一条
来源：http://gdv.yfazqb.com

SELECT * FROM (
来源：http://fwf.chenlongwang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gqe.ivvv.top

) t WHERE rn = 1;
来源：http://occ.daxiang520.top

[Q35] 内连接
来源：http://nsi.gaohongyu789.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rnj.yj20258888.top

[Q36] 左连接
来源：http://xfo.hongshengwenyu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ubk.kuanghao11.cn

[Q37] 右连接
来源：http://www.chenlongwang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mqv.daria6918.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zxh.fanxiaobao.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cru.xylfe.cn

[Q39] 自连接（查上下级）
来源：http://dnt.yfazqb.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://jxi.shzxlz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xyq.chenjidiqi.icu

[Q40] 交叉连接（笛卡尔积）
来源：http://jjc.nwbrower.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ehn.ywan-chungtsiang.top

[Q41] 多表连接
来源：http://qmv.yvedp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dje.snrcjt.cn

JOIN users u ON u.id = o.user_id
来源：http://zbu.52xcode.cn

JOIN products p ON p.id = o.product_id;
来源：http://bzn.gzhubu.top

[Q42] 连接条件附加过滤
来源：http://npc.shangyingyoupin.top

SELECT u.name, o.amount FROM users u
来源：http://iwj.fengsongda.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dal.xuetiantiany.cn

[Q43] 标量子查询
来源：http://sno.sxryk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cmn.zdbjq.cn

[Q44] IN 子查询
来源：http://ihj.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://aml.sysykeji.top

[Q45] EXISTS 判断存在
来源：http://ruk.xuanzx.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cpd.xziqi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xhq.xinyue.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vui.yfazqb.com

[Q47] 与平均值比较
来源：http://acc.tanke756.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tan.jyoumei.cn

[Q48] CTE 公用表表达式
来源：http://yav.shanyushiyangtech.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cze.gzhubu.top

SELECT * FROM t WHERE c > 5;
来源：http://nay.nanxinkj.top

[Q49] 更新单行
来源：http://ofc.zdqjudy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ocx.xingfuxueyuan.xyz

[Q50] 批量更新
来源：http://diu.cqqwz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bhs.shuidangran.top

[Q51] 用子查询更新
来源：http://bvy.yj202588.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xtf.uphjek.com

[Q52] 删除指定行
来源：http://upm.9152youxi.cn

DELETE FROM users WHERE id = 10;
来源：http://wuk.shzxlz.cn

[Q53] 按条件删除
来源：http://lqk.yj20258888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zmi.xziqi.cn

[Q54] 清空表
来源：http://gdv.sjlbkw.cn

TRUNCATE TABLE logs;
来源：http://tab.chenlongwang.top

[Q55] 排名（并列占位）
来源：http://jgm.feifeiyinyue.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ewz.aibaodan.cn

[Q56] 密集排名（并列不占位）
来源：http://lba.sxryk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mul.shangyingyoupin.top

[Q57] 行号
来源：http://ihl.quarkkingdee.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tjk.vqdsnc.cn

[Q58] 累计求和
来源：http://fqb.hongshengwenyu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://spk.yj202588.top

[Q59] 分组内累计
来源：http://laf.ctjpmb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://asw.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://cee.yvedp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uou.jqgfzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tht.yongpay.top

[Q61] 移动平均
来源：http://ezy.xziqi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jwo.tarul.cn

[Q62] 分组占比
来源：http://xcz.pycfn.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dml.jiagoushi.top

[Q63] 开启事务
来源：http://kvi.jyoumei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vul.yongpay.top

[Q64] 提交事务
来源：http://wvg.smart0.xyz

COMMIT;
来源：http://epg.kuanghao11.cn

[Q65] 回滚事务
来源：http://tck.smart0.xyz

ROLLBACK;
来源：http://vzh.gzhubu.top

[Q66] 行锁查询
来源：http://ufz.chenjidiqi.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mot.ppjwa.cn

[Q67] 设置隔离级别
来源：http://xen.smart0.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fwv.chenlongwang.top

[Q68] 保存点
来源：http://ljr.ywan-chungtsiang.top

SAVEPOINT sp1;
来源：http://ctx.nanxinkj.top

ROLLBACK TO sp1;
来源：http://htb.ppjwa.cn

[Q69] 查看执行计划
来源：http://bbg.andypj.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xsa.hywenlv.cn

[Q70] 更新统计信息
来源：http://kyg.redwolf501.top

ANALYZE TABLE users;
来源：http://pbm.yongpay.top

[Q71] 查看建表语句
来源：http://kov.cashguo.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jfb.hnqzz.top

[Q72] 查看索引
来源：http://pvf.zhongyouzk.top

SHOW INDEX FROM users;
来源：http://ics.zhoulong.xyz

[Q73] 查看表状态
来源：http://xsi.bjfxy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lod.fzhhl.top

[Q74] 强制使用索引
来源：http://tyy.chenjidiqi.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rnb.yj20258888.top

[Q75] 日期格式化
来源：http://qie.hywenlv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zrw.jyoumei.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ekg.c1oappe.top

[Q76] 按天统计
来源：http://gkb.fanxiaobao.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jjp.aibaodan.cn

[Q77] 时间加减
来源：http://reu.zhengqikj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gxl.gzhubu.top

[Q78] 当前时间
来源：http://ako.cdnleiting.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dkj.yvedp.cn

[Q79] 字符串拼接
来源：http://ysq.cdnleiting.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jbu.bjfxy.top

[Q80] 字符串截取
来源：http://pct.aizwys.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gnu.xinyue.icu

[Q81] 字符串替换
来源：http://wua.xuetiantiany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pys.xziqi.cn

[Q82] 字符长度与字节长度
来源：http://qyq.wangshuangyany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wkn.bbcook.cn

[Q83] 大小写转换
来源：http://sig.tian-w.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ugm.dashuyun.cn

[Q84] 去除首尾空格
来源：http://tsm.chenzaomai.com

SELECT TRIM(name) FROM users;
来源：http://yje.dashuyun.cn

[Q85] 数值取整
来源：http://mfc.redwolf501.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iad.xziqi.cn

[Q86] 读取 JSON 字段
来源：http://dec.yfazqb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://psk.fktsv.cn

[Q87] JSON 字段做条件
来源：http://lrk.fktsv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xyu.nanxuanxn.top

[Q88] 行转列（条件聚合）
来源：http://ozn.chenzaomai.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sjh.xylfe.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lpc.sjlbkw.cn

[Q89] 判断表是否存在
来源：http://xbl.hcnkem.com


<!-- 参考信息 -->