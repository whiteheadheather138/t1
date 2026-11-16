代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rui.yuanzhike.top

[O03] 加锁保护共享数据
来源：http://ebp.shanyushiyangkeji.top

Py:   with lock: shared += 1
来源：http://ohd.yuxming.cn

PHP:  // 用 flock() 做文件锁
来源：http://rez.tianlin.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ldu.316326.xyz

TS:   // 同 JS
来源：http://mgs.9152youxi.cn

Java: synchronized (this) { shared++; }
来源：http://sdk.pengpengdd.cyou

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cdq.hammf.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rcw.hywenlv.cn

C#:   lock (gate) { shared++; }
来源：http://pcu.jiagoushi.top

[O04] 定义异步函数并等待
来源：http://fwp.pycfn.com

Py:   async def f():⏎    await g()
来源：http://atc.feifeiyinyue.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fyh.fengsongda.top

JS:   async function f() { await g(); }
来源：http://wpp.wangdashe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://kvt.pengpengdd.cyou

Java: // 用 CompletableFuture 或虚拟线程
来源：http://boe.quarkkingdee.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qsc.dianchejie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wwr.cashguo.top

C#:   async Task F() { await G(); }
来源：http://gxv.xinyue.icu

[O05] 并发执行并等待全部完成
来源：http://plg.meibo888.top

Py:   asyncio.gather(*tasks)
来源：http://rwl.tarul.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://erv.mhx1999.top

JS:   await Promise.all(tasks)
来源：http://iqx.mhx1999.top

TS:   await Promise.all(tasks)
来源：http://qsy.xuanzx.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tck.sufxvd.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://een.sjlbkw.cn

Ruby: threads.map(&:join)
来源：http://ppu.jianghu66.top

C#:   await Task.WhenAll(t1, t2)
来源：http://odo.tarul.cn

[O06] 使用进程池
来源：http://wdb.ivvv.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xwn.316326.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://oht.snrcjt.cn

JS:   // child_process / cluster 模块
来源：http://leu.meibo888.top

TS:   // child_process / cluster 模块
来源：http://kci.zhijiandao.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ers.zhaomingkeji.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qfb.cucudq.cn

Ruby: // fork 块
来源：http://pca.yanxiufei.cn

C#:   Parallel.For
来源：http://slh.quarkkingdee.top

================================================================================
来源：http://hso.cashguo.top

P. 常用工具函数
来源：http://som.hammf.cn

================================================================================
来源：http://yzm.feifeiyinyue.top

[P01] 生成 UUID
来源：http://exj.yuanzhike.top

Py:   str(uuid.uuid4())
来源：http://bdb.sweek.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gya.cqqwz.cn

JS:   crypto.randomUUID()
来源：http://xtz.yuxming.cn

TS:   crypto.randomUUID()
来源：http://nwt.sjlbkw.cn

Java: UUID.randomUUID().toString()
来源：http://bry.aizwys.cn

Go:   // 用 github.com/google/uuid
来源：http://uft.mhx1999.top

Ruby: SecureRandom.uuid
来源：http://gus.wangdashe.top

C#:   Guid.NewGuid().ToString()
来源：http://xyp.zycfv.cn

[P02] MD5 / SHA256 摘要
来源：http://bsd.aibaodan.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fqo.andypj.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://qgd.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ipv.hnqzz.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nfn.tianlin.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vkt.smart0.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://byq.yuxming.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jdc.hywenlv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://agb.mhx1999.top

[P03] 生成短随机字符串
来源：http://bvk.sxryk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dzm.yongpay.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://phy.nanxuanxn.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bbl.hywenlv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ujm.nanxinkj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yaq.yongpay.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rmd.yfazqb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://qtv.cashguo.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://whe.tian-w.cn

[P04] 求长度
来源：http://shc.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://knq.zycfv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bda.gotoacloud.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rpz.tian-w.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xxd.sufxvd.cn

Java: list.size();  map.size();  s.length()
来源：http://fdh.xuanzx.com

Go:   len(arr);  len(m)
来源：http://rry.gaohongyu789.top

Ruby: x.length;  x.size
来源：http://esu.52xcode.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fao.zhoulong.xyz

[P05] 判断两个对象内容是否相等
来源：http://vmq.zdbjq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hww.wangshuangyany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://htm.yongpay.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vrz.haohaochexian.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cms.gaohongyu789.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wvj.cdnleiting.top

Go:   reflect.DeepEqual(a, b)
来源：http://rbb.ehwqpu.com

Ruby: a == b
来源：http://dna.wangshuangyany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wdf.nwbrower.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jja.wangshuangyany.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aif.316326.xyz

PHP:  if (empty($x)) {}
来源：http://mrr.ydjk.org.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tny.ywan-chungtsiang.top

TS:   if (x == null) {}
来源：http://pwu.mhx1999.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jyo.mhx1999.top

Go:   if x == nil {}
来源：http://rsh.vehdjk.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://agb.shanyushiyangkeji.top

C#:   if (x is null) {}
来源：http://ijc.quarkkingdee.top

[P07] 防抖与节流
来源：http://qhm.guannengcc.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pen.fehbvm.com

PHP:  // 手写时间戳比较
来源：http://mpr.fktsv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://guq.feifeiyinyue.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pgl.shzxlz.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xfk.svipenyu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fca.guowangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hqk.vehdjk.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sjt.fanxiaobao.xyz

[P08] 处理浮点精度问题
来源：http://wev.cucudq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iuv.hfpthk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wvw.yongpay.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fwo.c1oappe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vwu.ehwqpu.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uxr.fzhhl.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vrx.hesvh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dbh.jlsjyb.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fwp.ivvv.top

================================================================================
来源：http://jkc.xuanzx.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kbk.nanxinkj.top

================================================================================
来源：http://sas.ydzc1.top

[Q01] 创建表
来源：http://ofg.9152youxi.cn

CREATE TABLE users (
来源：http://ytx.cdnleiting.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cpp.52xcode.cn

name VARCHAR(50) NOT NULL,
来源：http://qtk.c1oappe.top

email VARCHAR(100) UNIQUE,
来源：http://rxv.zdbjq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uxb.yongpay.top

);
来源：http://glj.yonumen.top

[Q02] 创建带外键的表
来源：http://zoa.zhixingplan.top

CREATE TABLE orders (
来源：http://trf.sweek.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://arc.yongpay.top

user_id INT NOT NULL,
来源：http://nfi.snrcjt.cn

amount DECIMAL(10, 2),
来源：http://bii.uphjek.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qmu.ivvv.top

);
来源：http://jqz.fanxiaobao.xyz

[Q03] 增加列
来源：http://zua.cashguo.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zsr.hongshengwenyu.top

[Q04] 修改列类型
来源：http://scc.yangfankeji.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://swr.hcnkem.com

[Q05] 重命名列
来源：http://jts.yvedp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tni.yangfankeji.com

[Q06] 删除列
来源：http://fzk.daxiang520.top

ALTER TABLE users DROP COLUMN age;
来源：http://pln.jqgufenzy.top

[Q07] 删除表
来源：http://zij.dianchejie.cn

DROP TABLE IF EXISTS orders;
来源：http://nza.shzxlz.cn

[Q08] 创建普通索引
来源：http://akx.jianghu66.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gsc.fengsongda.top

[Q09] 创建唯一索引
来源：http://mmw.ppjwa.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zvs.gotoacloud.top

[Q10] 插入单行
来源：http://wnx.tian-w.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yfz.shanyushiyangtech.top

[Q11] 一次插入多行
来源：http://hnj.bbcook.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wps.yvedp.cn

[Q12] 插入后取自增 ID
来源：http://ihv.andypj.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://kng.wangshuangyany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cfn.fehbvm.com

[Q13] 忽略重复插入
来源：http://oxb.snrcjt.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://icv.xziqi.cn

[Q14] 存在则更新（upsert）
来源：http://ysc.kuanghao11.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zky.yj20258888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://txt.aizwys.cn

[Q15] 查询全部
来源：http://ibf.nwbrower.top

SELECT * FROM users;
来源：http://njc.ydzc1.top

[Q16] 查询指定列
来源：http://ydm.daxiang520.top

SELECT id, name FROM users;
来源：http://jdb.vqdsnc.cn

[Q17] 条件查询
来源：http://fkg.haohaochexian.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jth.hfpthk.cn

[Q18] 模糊匹配
来源：http://jbh.gogol.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uil.ybcxt.top

[Q19] 范围查询
来源：http://fvl.gaohongyu789.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tmv.redwolf501.top

[Q20] IN 列表
来源：http://woa.aizwys.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yde.yongpay.top

[Q21] 空值判断
来源：http://xkp.cucudq.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ycf.zhiwuduotai.top

[Q22] 排序
来源：http://aik.ivvv.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://reh.wangdashe.top

[Q23] 分页
来源：http://vje.chenjidiqi.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bha.jyoumei.cn

[Q24] 去重
来源：http://vhp.andypj.xyz

SELECT DISTINCT city FROM users;
来源：http://dpq.aibaodan.cn

[Q25] 只取前 N 条
来源：http://fbe.chenjidiqi.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gqz.vehdjk.com

[Q26] 计数
来源：http://ero.cheryme.top

SELECT COUNT(*) FROM users;
来源：http://xwx.daxiang520.top

[Q27] 条件计数
来源：http://apw.fengsongda.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dom.wangshuangyany.cn

[Q28] 求和与平均
来源：http://sss.sweek.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qnm.ivvv.top

[Q29] 最大最小值
来源：http://amb.xziqi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://svp.gzhubu.top

[Q30] 分组统计
来源：http://rkd.shanyushiyangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jsy.birdmap.top

[Q31] 分组后过滤
来源：http://cjc.kuanghao11.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://obj.jyoumei.cn

[Q32] 分组拼接字符串
来源：http://gev.tian-w.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mer.nanxuanxn.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://odj.cdnleiting.top

[Q33] 多列分组
来源：http://ntt.fktsv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://csm.fzhhl.top

[Q34] 每组取第一条
来源：http://kcp.andypj.xyz

SELECT * FROM (
来源：http://xfp.sjlbkw.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tlx.yj20258.top

) t WHERE rn = 1;
来源：http://toz.c1oappe.top

[Q35] 内连接
来源：http://hio.shangyingyoupin.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ajf.cheryme.top

[Q36] 左连接
来源：http://qap.cqqwz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mbm.vqdsnc.cn

[Q37] 右连接
来源：http://qna.sufxvd.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dcj.zhengqikj.top

[Q38] 全外连接（PostgreSQL）
来源：http://afu.fanxiaobao.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dcp.cucudq.cn

[Q39] 自连接（查上下级）
来源：http://eqz.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://zld.gogol.net.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gtp.yuxming.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fbj.jinyuanbaomall.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hxs.ppjwa.cn

[Q41] 多表连接
来源：http://kzv.zhijiandao.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tnf.jqgufenzy.top

JOIN users u ON u.id = o.user_id
来源：http://gug.hammf.cn

JOIN products p ON p.id = o.product_id;
来源：http://lkm.aibaodan.cn

[Q42] 连接条件附加过滤
来源：http://mdx.zdqjudy.top

SELECT u.name, o.amount FROM users u
来源：http://dkl.jlsjyb.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kar.feifeiyinyue.top

[Q43] 标量子查询
来源：http://vxq.yonumen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jfp.hysaishi.cn

[Q44] IN 子查询
来源：http://ghh.dianchejie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://whb.yueranfly.top

[Q45] EXISTS 判断存在
来源：http://egc.wangshuangyany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sxm.meibo888.top

[Q46] NOT EXISTS 判断不存在
来源：http://tyj.daria6918.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lob.sufxvd.cn

[Q47] 与平均值比较
来源：http://chv.fanxiaobao.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://srn.yj20258888.top

[Q48] CTE 公用表表达式
来源：http://oqe.yuxming.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gic.shanyushiyangkeji.top

SELECT * FROM t WHERE c > 5;
来源：http://hdc.ppjwa.cn

[Q49] 更新单行
来源：http://nxh.haohaochexian.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lmm.havefunace.top

[Q50] 批量更新
来源：http://loi.yueranfly.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lvr.hywenlv.cn

[Q51] 用子查询更新
来源：http://ykj.jqgfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qln.jyoumei.cn

[Q52] 删除指定行
来源：http://cms.xziqi.cn

DELETE FROM users WHERE id = 10;
来源：http://ibr.ctjpmb.com

[Q53] 按条件删除
来源：http://kon.xinyue.icu

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://spy.jianghu66.top

[Q54] 清空表
来源：http://fal.cucudq.cn

TRUNCATE TABLE logs;
来源：http://akb.feifeiyinyue.top

[Q55] 排名（并列占位）
来源：http://fml.yfazqb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://due.kuanghao11.cn

[Q56] 密集排名（并列不占位）
来源：http://xya.xuetiantiany.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yvd.cashguo.top

[Q57] 行号
来源：http://vpg.nanxuanxn.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rjl.zdqjudy.top

[Q58] 累计求和
来源：http://cwz.zhiwuduotai.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gmw.pycfn.com

[Q59] 分组内累计
来源：http://sgx.tarul.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mkx.sxryk.cn

[Q60] 取上一行 / 下一行
来源：http://nfe.tarul.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zyp.sweek.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vdt.snrcjt.cn

[Q61] 移动平均
来源：http://ioj.fehbvm.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nxp.fengsongda.top

[Q62] 分组占比
来源：http://cmp.xylfe.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://idy.tanke756.top

[Q63] 开启事务
来源：http://zak.yvedp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jol.nwbrower.top

[Q64] 提交事务
来源：http://pkl.jiagoushi.top

COMMIT;
来源：http://jqg.sweek.top

[Q65] 回滚事务
来源：http://ogs.nanxuanxn.top

ROLLBACK;
来源：http://mtw.fzhhl.top

[Q66] 行锁查询
来源：http://nis.shuidangran.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mvi.yuanzhike.top

[Q67] 设置隔离级别
来源：http://eqp.wangshuangyany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://syk.iojbl.cn

[Q68] 保存点
来源：http://mhe.jinqigfzy.top

SAVEPOINT sp1;
来源：http://bcb.fengsongda.top

ROLLBACK TO sp1;
来源：http://upt.pengpengdd.cyou

[Q69] 查看执行计划
来源：http://gwb.yongpay.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ngr.svipenyu.cn

[Q70] 更新统计信息
来源：http://wzc.hesvh.cn

ANALYZE TABLE users;
来源：http://hua.yvedp.cn

[Q71] 查看建表语句
来源：http://ikl.shuidangran.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ext.cucudq.cn

[Q72] 查看索引
来源：http://met.sufxvd.cn

SHOW INDEX FROM users;
来源：http://mba.tarul.cn

[Q73] 查看表状态
来源：http://mud.shzxlz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dfs.uphjek.com

[Q74] 强制使用索引
来源：http://fko.jianghu66.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cjs.jinqigfzy.top

[Q75] 日期格式化
来源：http://dnk.jqgufenzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lyt.shuidangran.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qft.jqgfzy.top

[Q76] 按天统计
来源：http://yqy.epnwcf.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bkk.jinyuanbaomall.cn

[Q77] 时间加减
来源：http://plq.yj20258888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ewn.316326.xyz

[Q78] 当前时间
来源：http://kfk.jyoumei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rkm.sxryk.cn

[Q79] 字符串拼接
来源：http://ile.xingfuxueyuan.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://djm.fktsv.cn

[Q80] 字符串截取
来源：http://lsd.hnxiangtu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ebr.sjlbkw.cn

[Q81] 字符串替换
来源：http://xiy.nwbrower.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://car.hnxiangtu.top


<!-- 参考信息 -->