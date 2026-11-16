代发 wailian999

[O02] 使用线程池
来源：http://vbq.hnqzz.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wqv.birdmap.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://snb.sxryk.cn

JS:   // worker_threads 线程池
来源：http://ozy.zhoulong.xyz

TS:   // worker_threads 线程池
来源：http://cmd.mhx1999.top

Java: Executors.newFixedThreadPool(4)
来源：http://fid.zhixingplan.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qlz.vqdsnc.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://now.cheryme.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mmo.yfazqb.com

[O03] 加锁保护共享数据
来源：http://qkh.shanyushiyangtech.top

Py:   with lock: shared += 1
来源：http://ngf.vqdsnc.cn

PHP:  // 用 flock() 做文件锁
来源：http://mmg.daria6918.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iln.wangdashe.top

TS:   // 同 JS
来源：http://fam.jlsjyb.cn

Java: synchronized (this) { shared++; }
来源：http://wrw.snrcjt.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eqh.9152youxi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wbb.yongpay.top

C#:   lock (gate) { shared++; }
来源：http://qvd.quarkkingdee.top

[O04] 定义异步函数并等待
来源：http://gaz.xinyue.icu

Py:   async def f():⏎    await g()
来源：http://arb.nanxinkj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pem.feifeiyinyue.top

JS:   async function f() { await g(); }
来源：http://ezl.aibaodan.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mqr.xziqi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bnf.aizwys.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hly.hammf.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ulo.9152youxi.cn

C#:   async Task F() { await G(); }
来源：http://qam.vqdsnc.cn

[O05] 并发执行并等待全部完成
来源：http://sic.fengsongda.top

Py:   asyncio.gather(*tasks)
来源：http://vau.xinyue.icu

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gei.52xcode.cn

JS:   await Promise.all(tasks)
来源：http://tff.jqgfzy.top

TS:   await Promise.all(tasks)
来源：http://mxv.fktsv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bcx.ppjwa.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tgn.316326.xyz

Ruby: threads.map(&:join)
来源：http://pzs.ydzc1.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lzs.kuanghao11.cn

[O06] 使用进程池
来源：http://tli.shzxlz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vdj.xinyue.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://gab.aibaodan.cn

JS:   // child_process / cluster 模块
来源：http://jak.fengsongda.top

TS:   // child_process / cluster 模块
来源：http://eli.316326.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jfx.nanxinkj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hgd.fanxiaobao.xyz

Ruby: // fork 块
来源：http://aqp.daxiang520.top

C#:   Parallel.For
来源：http://upw.zhoulong.xyz

================================================================================
来源：http://kly.aibaodan.cn

P. 常用工具函数
来源：http://tue.shangyingyoupin.top

================================================================================
来源：http://jsg.dashuyun.cn

[P01] 生成 UUID
来源：http://zma.bbcook.cn

Py:   str(uuid.uuid4())
来源：http://mpx.yangfankeji.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fwt.ydjk.org.cn

JS:   crypto.randomUUID()
来源：http://itk.yonumen.top

TS:   crypto.randomUUID()
来源：http://xyr.vehdjk.com

Java: UUID.randomUUID().toString()
来源：http://ooq.xuetiantiany.cn

Go:   // 用 github.com/google/uuid
来源：http://pls.nwbrower.top

Ruby: SecureRandom.uuid
来源：http://wpn.meibo888.top

C#:   Guid.NewGuid().ToString()
来源：http://htp.pycfn.com

[P02] MD5 / SHA256 摘要
来源：http://jra.sufxvd.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qcr.vehdjk.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://ols.jyoumei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oog.52xcode.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cuc.jqgfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://isr.fktsv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nma.jinqigfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uek.fzhhl.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ojn.aizwys.cn

[P03] 生成短随机字符串
来源：http://qqj.haohaochexian.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yik.52xcode.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vha.yueranfly.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hjc.cashguo.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dje.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jxt.guannengcc.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hgf.chenzaomai.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://smj.xziqi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dym.birdmap.top

[P04] 求长度
来源：http://lhe.yfazqb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nfy.52xcode.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xqu.yuanzhike.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.chenzaomai.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://efx.zhiwuduotai.top

Java: list.size();  map.size();  s.length()
来源：http://vjk.aibaodan.cn

Go:   len(arr);  len(m)
来源：http://qok.wangshuangyany.cn

Ruby: x.length;  x.size
来源：http://bzm.jianghu66.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rri.shanyushiyangtech.top

[P05] 判断两个对象内容是否相等
来源：http://ugx.jqgufenzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rwj.ehwqpu.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://orr.cucudq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://crz.gotoacloud.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kyq.gotoacloud.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wxz.zhengqikj.top

Go:   reflect.DeepEqual(a, b)
来源：http://ggf.fktsv.cn

Ruby: a == b
来源：http://nas.jianghu66.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qem.shanyushiyangtech.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ekl.ybcxt.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fog.nwbrower.top

PHP:  if (empty($x)) {}
来源：http://pif.aibaodan.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vbx.fengsongda.top

TS:   if (x == null) {}
来源：http://bya.jyoumei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wdm.nanxinkj.top

Go:   if x == nil {}
来源：http://ypu.shangyingyoupin.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xxc.yangfankeji.com

C#:   if (x is null) {}
来源：http://rtj.shangyingyoupin.top

[P07] 防抖与节流
来源：http://cxv.fengsongda.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cqh.hnqzz.top

PHP:  // 手写时间戳比较
来源：http://gzv.jqgfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fnb.yj20258.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bmt.yfazqb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ged.aibaodan.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lsm.yongpay.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://lqo.hcnkem.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kpq.mhx1999.top

[P08] 处理浮点精度问题
来源：http://nbv.zycfv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bdp.sufxvd.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hha.zycfv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vdz.nanxuanxn.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://flm.xingfuxueyuan.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://slo.bbcook.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uhs.fktsv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kkw.daria6918.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wwm.xinyue.icu

================================================================================
来源：http://jgl.guannengcc.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qto.andypj.xyz

================================================================================
来源：http://hme.gotoacloud.top

[Q01] 创建表
来源：http://beq.yonumen.top

CREATE TABLE users (
来源：http://tod.yonumen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kyj.shanyushiyangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://yvd.xingfuxueyuan.xyz

email VARCHAR(100) UNIQUE,
来源：http://hyf.mhx1999.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cpm.52xcode.cn

);
来源：http://fwl.gotoacloud.top

[Q02] 创建带外键的表
来源：http://jfs.tarul.cn

CREATE TABLE orders (
来源：http://rya.zhengqikj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dpn.yj20258888.top

user_id INT NOT NULL,
来源：http://qgq.nwbrower.top

amount DECIMAL(10, 2),
来源：http://ypa.birdmap.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://clx.yvedp.cn

);
来源：http://auc.fzhhl.top

[Q03] 增加列
来源：http://lml.sysykeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eoe.fanxiaobao.xyz

[Q04] 修改列类型
来源：http://ndp.wangdashe.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mnz.hammf.cn

[Q05] 重命名列
来源：http://cpm.ydzc1.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mal.zhoulong.xyz

[Q06] 删除列
来源：http://izd.ctjpmb.com

ALTER TABLE users DROP COLUMN age;
来源：http://wbw.xuanzx.com

[Q07] 删除表
来源：http://kzz.havefunace.top

DROP TABLE IF EXISTS orders;
来源：http://lir.tanke756.top

[Q08] 创建普通索引
来源：http://htj.mhx1999.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gdl.zhixingplan.top

[Q09] 创建唯一索引
来源：http://ieh.hnqzz.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cqs.andypj.xyz

[Q10] 插入单行
来源：http://exd.jinqigfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gpo.uphjek.com

[Q11] 一次插入多行
来源：http://vvk.nanxinkj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://syj.ivvv.top

[Q12] 插入后取自增 ID
来源：http://ogb.cashguo.top

INSERT INTO users (name) VALUES ('C');
来源：http://lay.wangshuangyany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pam.jlsjyb.cn

[Q13] 忽略重复插入
来源：http://pkq.zhiwuduotai.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://teb.vqdsnc.cn

[Q14] 存在则更新（upsert）
来源：http://dcv.yj20258888.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ltu.xinyue.icu

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ibx.zhiwuduotai.top

[Q15] 查询全部
来源：http://opf.xuetiantiany.cn

SELECT * FROM users;
来源：http://tai.hnqzz.top

[Q16] 查询指定列
来源：http://rou.ywan-chungtsiang.top

SELECT id, name FROM users;
来源：http://uyb.yuxming.cn

[Q17] 条件查询
来源：http://ljc.bbcook.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tds.zdqjudy.top

[Q18] 模糊匹配
来源：http://lca.jinghuilouyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oqj.jqgufenzy.top

[Q19] 范围查询
来源：http://qab.hongshengwenyu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qif.hysaishi.cn

[Q20] IN 列表
来源：http://iij.pycfn.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fag.andypj.xyz

[Q21] 空值判断
来源：http://tav.0kj1m.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://osh.gotoacloud.top

[Q22] 排序
来源：http://eqb.yueranfly.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://omo.aibaodan.cn

[Q23] 分页
来源：http://fqz.fktsv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cch.cashguo.top

[Q24] 去重
来源：http://jnc.zhaomingkeji.xyz

SELECT DISTINCT city FROM users;
来源：http://una.jinqigfzy.top

[Q25] 只取前 N 条
来源：http://ezh.pycfn.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uyw.pengpengdd.cyou

[Q26] 计数
来源：http://noq.jqgfzy.top

SELECT COUNT(*) FROM users;
来源：http://ddw.fehbvm.com

[Q27] 条件计数
来源：http://xrs.jlsjyb.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ada.uphjek.com

[Q28] 求和与平均
来源：http://csl.hnqzz.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zyn.cashguo.top

[Q29] 最大最小值
来源：http://bqa.tarul.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vdl.hfpthk.cn

[Q30] 分组统计
来源：http://lls.yueranfly.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ith.snrcjt.cn

[Q31] 分组后过滤
来源：http://tzq.ivvv.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://juw.zhengqikj.top

[Q32] 分组拼接字符串
来源：http://qfw.jianghu66.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yfc.pengpengdd.cyou

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mrz.yuanzhike.top

[Q33] 多列分组
来源：http://gcg.jinyuanbaomall.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qdl.sufxvd.cn

[Q34] 每组取第一条
来源：http://gtc.yj202588.top

SELECT * FROM (
来源：http://syv.c1oappe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mtf.daxiang520.top

) t WHERE rn = 1;
来源：http://pwp.zhijiandao.cn

[Q35] 内连接
来源：http://lpn.zhongyouzk.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kij.vehdjk.com

[Q36] 左连接
来源：http://aom.jianghu66.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rzq.yuxming.cn

[Q37] 右连接
来源：http://srb.quarkkingdee.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wly.ybcxt.top

[Q38] 全外连接（PostgreSQL）
来源：http://tkc.zdqjudy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fgz.birdmap.top

[Q39] 自连接（查上下级）
来源：http://pmt.hysaishi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ton.jinqigufen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lnm.jianghu66.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ttq.nanxuanxn.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wjg.cqqwz.cn

[Q41] 多表连接
来源：http://ioj.chenzaomai.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://olz.shanyushiyangtech.top

JOIN users u ON u.id = o.user_id
来源：http://uyu.ywan-chungtsiang.top

JOIN products p ON p.id = o.product_id;
来源：http://vfl.jinqigfzy.top

[Q42] 连接条件附加过滤
来源：http://cmv.ybcxt.top

SELECT u.name, o.amount FROM users u
来源：http://vcp.zhongyouzk.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gpk.fzhhl.top

[Q43] 标量子查询
来源：http://frq.chenzaomai.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rdc.chenzaomai.com

[Q44] IN 子查询
来源：http://pjz.guannengcc.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uca.fehbvm.com

[Q45] EXISTS 判断存在
来源：http://kgi.shanyushiyangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mjr.hnqzz.top

[Q46] NOT EXISTS 判断不存在
来源：http://gqx.52xcode.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mkc.tanke756.top

[Q47] 与平均值比较
来源：http://pvq.zhijiandao.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ldh.52xcode.cn

[Q48] CTE 公用表表达式
来源：http://muw.yuxming.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vaw.hnqzz.top

SELECT * FROM t WHERE c > 5;
来源：http://gpm.yueranfly.top

[Q49] 更新单行
来源：http://buk.cashguo.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bac.gogol.net.cn

[Q50] 批量更新
来源：http://weq.wangshuangyany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hkv.zhoulong.xyz

[Q51] 用子查询更新
来源：http://oft.meibo888.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://glz.yueranfly.top

[Q52] 删除指定行
来源：http://dex.zycfv.cn

DELETE FROM users WHERE id = 10;
来源：http://dvx.zdqjudy.top

[Q53] 按条件删除
来源：http://nbl.yj202588.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tkj.zycfv.cn

[Q54] 清空表
来源：http://jwm.xylfe.cn

TRUNCATE TABLE logs;
来源：http://azb.ehwqpu.com

[Q55] 排名（并列占位）
来源：http://vuq.xuetiantiany.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zdu.daria6918.cn

[Q56] 密集排名（并列不占位）
来源：http://zyr.zhengqikj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mpw.andypj.xyz

[Q57] 行号
来源：http://veb.gaohongyu789.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rhm.vqdsnc.cn

[Q58] 累计求和
来源：http://who.chenjidiqi.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ehp.fanxiaobao.xyz

[Q59] 分组内累计
来源：http://fue.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://unk.meibo888.top

[Q60] 取上一行 / 下一行
来源：http://kyx.jianghu66.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cwt.daxiang520.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cch.bbcook.cn

[Q61] 移动平均
来源：http://psb.yfazqb.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://htq.aizwys.cn

[Q62] 分组占比
来源：http://qwi.ydzc1.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vzl.aizwys.cn

[Q63] 开启事务
来源：http://cez.xingfuxueyuan.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://ezg.xingfuxueyuan.xyz

[Q64] 提交事务
来源：http://fws.guannengcc.top

COMMIT;
来源：http://stp.sxryk.cn

[Q65] 回滚事务
来源：http://dka.ydzc1.top

ROLLBACK;
来源：http://rrx.tarul.cn

[Q66] 行锁查询
来源：http://gva.tanke756.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ihg.zycfv.cn

[Q67] 设置隔离级别
来源：http://asw.zhiwuduotai.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ksk.hfpthk.cn

[Q68] 保存点
来源：http://rhz.uphjek.com

SAVEPOINT sp1;
来源：http://afv.zhiwuduotai.top

ROLLBACK TO sp1;
来源：http://cuq.9152youxi.cn

[Q69] 查看执行计划
来源：http://gql.sxryk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://txn.dianchejie.cn

[Q70] 更新统计信息
来源：http://qql.feifeiyinyue.top

ANALYZE TABLE users;
来源：http://wwm.fanxiaobao.xyz

[Q71] 查看建表语句
来源：http://wnn.vehdjk.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nfk.yueranfly.top

[Q72] 查看索引
来源：http://pxh.cdnleiting.top

SHOW INDEX FROM users;
来源：http://vnq.zdqjudy.top

[Q73] 查看表状态
来源：http://lmr.quarkkingdee.top

SHOW TABLE STATUS LIKE 'users';
来源：http://yjk.jiagoushi.top

[Q74] 强制使用索引
来源：http://zdd.hnxiangtu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hiu.dashuyun.cn

[Q75] 日期格式化
来源：http://jex.shangyingyoupin.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://epu.zhijiandao.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jov.tian-w.cn

[Q76] 按天统计
来源：http://ycg.bbcook.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tdw.xylfe.cn

[Q77] 时间加减
来源：http://yaa.hfpthk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mis.tanke756.top


<!-- 参考信息 -->