代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://cwh.ybcxt.top

Go:   go f()
来源：http://net.dianchejie.cn

Ruby: Thread.new { f }
来源：http://vma.wangshuangyany.cn

C#:   Task.Run(() => F());
来源：http://jxq.ehwqpu.com

[O02] 使用线程池
来源：http://ufe.chenzaomai.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://llj.yonumen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zma.gzhubu.top

JS:   // worker_threads 线程池
来源：http://eww.ywan-chungtsiang.top

TS:   // worker_threads 线程池
来源：http://urq.snrcjt.cn

Java: Executors.newFixedThreadPool(4)
来源：http://obs.fzhhl.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nzs.cucudq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sqq.shangyingyoupin.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bvk.sxryk.cn

[O03] 加锁保护共享数据
来源：http://eso.jinqigufen.top

Py:   with lock: shared += 1
来源：http://xzq.ppjwa.cn

PHP:  // 用 flock() 做文件锁
来源：http://xek.fzhhl.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xtk.9152youxi.cn

TS:   // 同 JS
来源：http://pyl.jinqigufen.top

Java: synchronized (this) { shared++; }
来源：http://zky.fengsongda.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nwh.xuanzx.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://uqw.zhijiandao.cn

C#:   lock (gate) { shared++; }
来源：http://hvn.gotoacloud.top

[O04] 定义异步函数并等待
来源：http://tha.nwbrower.top

Py:   async def f():⏎    await g()
来源：http://xfl.ydjk.org.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cox.nanxuanxn.top

JS:   async function f() { await g(); }
来源：http://rbi.haohaochexian.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jja.yonumen.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kff.daxiang520.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bkd.vqdsnc.cn

Ruby: # 用 Fiber 或 async gem
来源：http://iqg.zycfv.cn

C#:   async Task F() { await G(); }
来源：http://mzn.snrcjt.cn

[O05] 并发执行并等待全部完成
来源：http://dty.0kj1m.cn

Py:   asyncio.gather(*tasks)
来源：http://gko.iojbl.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zph.jqgufenzy.top

JS:   await Promise.all(tasks)
来源：http://toh.daxiang520.top

TS:   await Promise.all(tasks)
来源：http://zcr.ybcxt.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eny.cucudq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fwc.aibaodan.cn

Ruby: threads.map(&:join)
来源：http://kzv.zhongyouzk.top

C#:   await Task.WhenAll(t1, t2)
来源：http://iyt.sweek.top

[O06] 使用进程池
来源：http://hnx.jqgufenzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hxn.gotoacloud.top

PHP:  // pcntl_fork 或多进程队列
来源：http://job.vehdjk.com

JS:   // child_process / cluster 模块
来源：http://izg.gaohongyu789.top

TS:   // child_process / cluster 模块
来源：http://btk.quarkkingdee.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mtm.epnwcf.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wnr.dianchejie.cn

Ruby: // fork 块
来源：http://mms.yangfankeji.com

C#:   Parallel.For
来源：http://blx.nanxinkj.top

================================================================================
来源：http://cba.hcnkem.com

P. 常用工具函数
来源：http://gjr.yvedp.cn

================================================================================
来源：http://ttj.shangyingyoupin.top

[P01] 生成 UUID
来源：http://gpu.ctjpmb.com

Py:   str(uuid.uuid4())
来源：http://pqx.zdqjudy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qmu.gogol.net.cn

JS:   crypto.randomUUID()
来源：http://fpy.redwolf501.top

TS:   crypto.randomUUID()
来源：http://ede.ehwqpu.com

Java: UUID.randomUUID().toString()
来源：http://frw.hammf.cn

Go:   // 用 github.com/google/uuid
来源：http://pcc.wangshuangyany.cn

Ruby: SecureRandom.uuid
来源：http://uvv.chenzaomai.com

C#:   Guid.NewGuid().ToString()
来源：http://sbq.nanxinkj.top

[P02] MD5 / SHA256 摘要
来源：http://rli.hywenlv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://plb.bbcook.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://icj.pengpengdd.cyou

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mgr.iojbl.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wal.ctjpmb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dfh.yanxiufei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hvs.xuetiantiany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lly.tanke756.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iym.ehwqpu.com

[P03] 生成短随机字符串
来源：http://tzm.ppjwa.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wkj.yanxiufei.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ltj.tian-w.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dyk.yj20258888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yrr.jyoumei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wrw.0kj1m.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xgc.zhengqikj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vje.zhongyouzk.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://emg.dashuyun.cn

[P04] 求长度
来源：http://rkj.aibaodan.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bus.aizwys.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zvh.jiagoushi.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hlg.xinyue.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://seo.fengsongda.top

Java: list.size();  map.size();  s.length()
来源：http://chu.aizwys.cn

Go:   len(arr);  len(m)
来源：http://eld.fzhhl.top

Ruby: x.length;  x.size
来源：http://dbk.sxryk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wmj.fengsongda.top

[P05] 判断两个对象内容是否相等
来源：http://hkj.guannengcc.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://xre.cucudq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://olv.ehwqpu.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xch.hongshengwenyu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://aqm.birdmap.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rbh.xziqi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ilz.jlsjyb.cn

Ruby: a == b
来源：http://hfh.shanyushiyangkeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qri.bbcook.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://seh.jqgufenzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gby.fehbvm.com

PHP:  if (empty($x)) {}
来源：http://pzg.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://asw.iojbl.cn

TS:   if (x == null) {}
来源：http://sbo.fanxiaobao.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://eys.wangshuangyany.cn

Go:   if x == nil {}
来源：http://kxo.jqgufenzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xzi.zhongyouzk.top

C#:   if (x is null) {}
来源：http://rdy.xuanzx.com

[P07] 防抖与节流
来源：http://zkb.hongshengwenyu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xrj.pycfn.com

PHP:  // 手写时间戳比较
来源：http://uyq.snrcjt.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mhq.nanxuanxn.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nge.jyoumei.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cnm.cucudq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kmn.shzxlz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ipz.sysykeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vom.sweek.top

[P08] 处理浮点精度问题
来源：http://vhc.yuxming.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gmu.chenlongwang.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mdc.sjlbkw.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ama.shangyingyoupin.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xdf.jinqigufen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nul.guowangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cfj.hnqzz.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ypw.cheryme.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mcy.tian-w.cn

================================================================================
来源：http://kfq.jlsjyb.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nqp.pycfn.com

================================================================================
来源：http://qsg.gaohongyu789.top

[Q01] 创建表
来源：http://rag.tianlin.xyz

CREATE TABLE users (
来源：http://czy.tarul.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ouo.sysykeji.top

name VARCHAR(50) NOT NULL,
来源：http://vqt.nanxinkj.top

email VARCHAR(100) UNIQUE,
来源：http://uvq.zhoulong.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sho.daxiang520.top

);
来源：http://gpn.hongshengwenyu.top

[Q02] 创建带外键的表
来源：http://hjm.pengpengdd.cyou

CREATE TABLE orders (
来源：http://dlx.nwbrower.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ufa.uphjek.com

user_id INT NOT NULL,
来源：http://snl.zhixingplan.top

amount DECIMAL(10, 2),
来源：http://jph.bbcook.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ufa.svipenyu.cn

);
来源：http://sbs.hcnkem.com

[Q03] 增加列
来源：http://hsd.316326.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gkk.gaohongyu789.top

[Q04] 修改列类型
来源：http://nkp.fehbvm.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tqm.9152youxi.cn

[Q05] 重命名列
来源：http://xzv.ydzc1.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pai.gogol.net.cn

[Q06] 删除列
来源：http://yvz.feifeiyinyue.top

ALTER TABLE users DROP COLUMN age;
来源：http://atb.shanyushiyangtech.top

[Q07] 删除表
来源：http://unh.fengsongda.top

DROP TABLE IF EXISTS orders;
来源：http://sjg.guowangkeji.top

[Q08] 创建普通索引
来源：http://pjd.quarkkingdee.top

CREATE INDEX idx_users_email ON users(email);
来源：http://oyl.nanxinkj.top

[Q09] 创建唯一索引
来源：http://qhi.yfazqb.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://szl.nwbrower.top

[Q10] 插入单行
来源：http://tke.shuidangran.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aez.fengsongda.top

[Q11] 一次插入多行
来源：http://uhr.shzxlz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://orq.sysykeji.top

[Q12] 插入后取自增 ID
来源：http://wtm.chenzaomai.com

INSERT INTO users (name) VALUES ('C');
来源：http://isx.vqdsnc.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rfv.xylfe.cn

[Q13] 忽略重复插入
来源：http://csm.tarul.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kpm.redwolf501.top

[Q14] 存在则更新（upsert）
来源：http://aii.bbcook.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nnb.svipenyu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vfo.bjfxy.top

[Q15] 查询全部
来源：http://san.zhijiandao.cn

SELECT * FROM users;
来源：http://tti.shzxlz.cn

[Q16] 查询指定列
来源：http://mjh.cucudq.cn

SELECT id, name FROM users;
来源：http://sna.chenzaomai.com

[Q17] 条件查询
来源：http://cld.yuxming.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xnf.birdmap.top

[Q18] 模糊匹配
来源：http://xpt.shuidangran.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nuy.mhx1999.top

[Q19] 范围查询
来源：http://mxd.uphjek.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bye.c1oappe.top

[Q20] IN 列表
来源：http://juk.hammf.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://veu.yuxming.cn

[Q21] 空值判断
来源：http://csm.ydzc1.top

SELECT * FROM users WHERE email IS NULL;
来源：http://tmr.jqgufenzy.top

[Q22] 排序
来源：http://vix.smart0.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zek.gotoacloud.top

[Q23] 分页
来源：http://itf.chenlongwang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://orh.pengpengdd.cyou

[Q24] 去重
来源：http://tib.hongshengwenyu.top

SELECT DISTINCT city FROM users;
来源：http://bnl.jiagoushi.top

[Q25] 只取前 N 条
来源：http://vzw.hammf.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://roy.ydjk.org.cn

[Q26] 计数
来源：http://clh.jlsjyb.cn

SELECT COUNT(*) FROM users;
来源：http://noz.vqdsnc.cn

[Q27] 条件计数
来源：http://zzj.52xcode.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rqu.dashuyun.cn

[Q28] 求和与平均
来源：http://bzg.gotoacloud.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xng.wangdashe.top

[Q29] 最大最小值
来源：http://qcs.gogol.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wzi.xylfe.cn

[Q30] 分组统计
来源：http://zvv.andypj.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qnm.shanyushiyangtech.top

[Q31] 分组后过滤
来源：http://dub.xylfe.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bmk.ydzc1.top

[Q32] 分组拼接字符串
来源：http://fks.tian-w.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ivl.c1oappe.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ghp.yangfankeji.com

[Q33] 多列分组
来源：http://fdh.ehwqpu.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bsd.havefunace.top

[Q34] 每组取第一条
来源：http://mzt.shanyushiyangkeji.top

SELECT * FROM (
来源：http://isn.wangdashe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qiy.ybcxt.top

) t WHERE rn = 1;
来源：http://snb.dashuyun.cn

[Q35] 内连接
来源：http://cds.pycfn.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sqk.bbcook.cn

[Q36] 左连接
来源：http://tys.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qyp.jqgufenzy.top

[Q37] 右连接
来源：http://miy.yongpay.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gvw.tanke756.top

[Q38] 全外连接（PostgreSQL）
来源：http://vue.fengsongda.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nqy.zdbjq.cn

[Q39] 自连接（查上下级）
来源：http://lfy.snrcjt.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jcm.smart0.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gjt.mhx1999.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zms.xingfuxueyuan.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zds.wangdashe.top

[Q41] 多表连接
来源：http://wgi.yj20258888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://inc.ehwqpu.com

JOIN users u ON u.id = o.user_id
来源：http://tgl.jianghu66.top

JOIN products p ON p.id = o.product_id;
来源：http://tib.zdqjudy.top

[Q42] 连接条件附加过滤
来源：http://saf.shangyingyoupin.top

SELECT u.name, o.amount FROM users u
来源：http://nva.xylfe.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tvl.yangfankeji.com

[Q43] 标量子查询
来源：http://fvk.sysykeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://aiu.xuanzx.com

[Q44] IN 子查询
来源：http://ozz.316326.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ggc.jyoumei.cn

[Q45] EXISTS 判断存在
来源：http://ork.zhoulong.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lnp.jqgufenzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://zgi.vehdjk.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kil.nwbrower.top

[Q47] 与平均值比较
来源：http://pkz.shzxlz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zss.hesvh.cn

[Q48] CTE 公用表表达式
来源：http://sdf.chenjidiqi.icu

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pna.vqdsnc.cn

SELECT * FROM t WHERE c > 5;
来源：http://bqv.zycfv.cn

[Q49] 更新单行
来源：http://efi.tian-w.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://inz.jqgufenzy.top

[Q50] 批量更新
来源：http://ofn.ybcxt.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://iws.kuanghao11.cn

[Q51] 用子查询更新
来源：http://ugs.gaohongyu789.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hvj.yongpay.top

[Q52] 删除指定行
来源：http://gqw.xingfuxueyuan.xyz

DELETE FROM users WHERE id = 10;
来源：http://era.hnxiangtu.top

[Q53] 按条件删除
来源：http://fvl.zhaomingkeji.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://evx.sysykeji.top

[Q54] 清空表
来源：http://qcx.cashguo.top

TRUNCATE TABLE logs;
来源：http://dnq.jyoumei.cn

[Q55] 排名（并列占位）
来源：http://gks.jqgufenzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nun.chenzaomai.com

[Q56] 密集排名（并列不占位）
来源：http://dek.svipenyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lhy.yfazqb.com

[Q57] 行号
来源：http://ioc.fengsongda.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jlx.epnwcf.com

[Q58] 累计求和
来源：http://jpt.chenlongwang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kmj.c1oappe.top

[Q59] 分组内累计
来源：http://byf.hongshengwenyu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ggw.feifeiyinyue.top

[Q60] 取上一行 / 下一行
来源：http://cqp.jlsjyb.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ene.tian-w.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lvu.fengsongda.top

[Q61] 移动平均
来源：http://vyd.shanyushiyangkeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vgf.ppjwa.cn

[Q62] 分组占比
来源：http://imm.ydjk.org.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dcv.cdnleiting.top

[Q63] 开启事务
来源：http://mse.haohaochexian.top

START TRANSACTION;                -- 或 BEGIN
来源：http://sol.shangyingyoupin.top

[Q64] 提交事务
来源：http://iwb.zhixingplan.top

COMMIT;
来源：http://ojc.chenjidiqi.icu

[Q65] 回滚事务
来源：http://rlb.jianghu66.top

ROLLBACK;
来源：http://bgc.hysaishi.cn

[Q66] 行锁查询
来源：http://rqa.zdqjudy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vqa.fzhhl.top

[Q67] 设置隔离级别
来源：http://exe.xziqi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vzg.ctjpmb.com

[Q68] 保存点
来源：http://jxz.hesvh.cn

SAVEPOINT sp1;
来源：http://wje.sxryk.cn

ROLLBACK TO sp1;
来源：http://ozp.ehwqpu.com

[Q69] 查看执行计划
来源：http://esf.zycfv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lhc.cdnleiting.top

[Q70] 更新统计信息
来源：http://lta.ywan-chungtsiang.top

ANALYZE TABLE users;
来源：http://sfl.nanxinkj.top

[Q71] 查看建表语句
来源：http://btr.cucudq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yfk.316326.xyz

[Q72] 查看索引
来源：http://xor.zhixingplan.top

SHOW INDEX FROM users;
来源：http://wne.chenjidiqi.icu

[Q73] 查看表状态
来源：http://jlh.cqqwz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ttl.nanxuanxn.top

[Q74] 强制使用索引
来源：http://wzg.daxiang520.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://srk.yueranfly.top

[Q75] 日期格式化
来源：http://vjv.yanxiufei.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dbj.dashuyun.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tln.shanyushiyangkeji.top


<!-- 参考信息 -->