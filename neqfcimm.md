代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://apy.vehdjk.com

Go:   go f()
来源：http://ghv.fanxiaobao.xyz

Ruby: Thread.new { f }
来源：http://nhc.tanke756.top

C#:   Task.Run(() => F());
来源：http://xcf.zhijiandao.cn

[O02] 使用线程池
来源：http://rfw.yj202588.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://azp.shangyingyoupin.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xpv.fehbvm.com

JS:   // worker_threads 线程池
来源：http://sec.cucudq.cn

TS:   // worker_threads 线程池
来源：http://xlh.sxryk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kzb.smart0.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lin.nwbrower.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://snq.nanxinkj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cpt.zhongyouzk.top

[O03] 加锁保护共享数据
来源：http://jie.c1oappe.top

Py:   with lock: shared += 1
来源：http://vpn.cucudq.cn

PHP:  // 用 flock() 做文件锁
来源：http://nak.xingfuxueyuan.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ful.birdmap.top

TS:   // 同 JS
来源：http://fkl.sufxvd.cn

Java: synchronized (this) { shared++; }
来源：http://kju.ivvv.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fjw.cqqwz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cgn.yj202588.top

C#:   lock (gate) { shared++; }
来源：http://nus.jinqigfzy.top

[O04] 定义异步函数并等待
来源：http://ubc.jyoumei.cn

Py:   async def f():⏎    await g()
来源：http://ytx.sxryk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dmp.jiagoushi.top

JS:   async function f() { await g(); }
来源：http://tgu.chenzaomai.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://psq.0kj1m.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eka.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xnv.shanyushiyangkeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://ueo.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://lep.cashguo.top

[O05] 并发执行并等待全部完成
来源：http://daz.pengpengdd.cyou

Py:   asyncio.gather(*tasks)
来源：http://pah.xuetiantiany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tmo.jinqigfzy.top

JS:   await Promise.all(tasks)
来源：http://izx.yonumen.top

TS:   await Promise.all(tasks)
来源：http://ppq.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zuo.fktsv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zgm.cdnleiting.top

Ruby: threads.map(&:join)
来源：http://fyn.chenjidiqi.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://sap.guowangkeji.top

[O06] 使用进程池
来源：http://apo.sysykeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gnx.haohaochexian.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mje.tanke756.top

JS:   // child_process / cluster 模块
来源：http://xry.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://flq.zhoulong.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://raz.bbcook.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://etf.redwolf501.top

Ruby: // fork 块
来源：http://isj.dianchejie.cn

C#:   Parallel.For
来源：http://rsk.epnwcf.com

================================================================================
来源：http://hgf.sjlbkw.cn

P. 常用工具函数
来源：http://bpd.tarul.cn

================================================================================
来源：http://wnx.9152youxi.cn

[P01] 生成 UUID
来源：http://nyy.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://nhh.zdbjq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pcy.xuetiantiany.cn

JS:   crypto.randomUUID()
来源：http://uhk.aizwys.cn

TS:   crypto.randomUUID()
来源：http://nuw.sjlbkw.cn

Java: UUID.randomUUID().toString()
来源：http://qav.cdnleiting.top

Go:   // 用 github.com/google/uuid
来源：http://yfr.fengsongda.top

Ruby: SecureRandom.uuid
来源：http://wqz.ppjwa.cn

C#:   Guid.NewGuid().ToString()
来源：http://qun.jqgfzy.top

[P02] MD5 / SHA256 摘要
来源：http://ypo.c1oappe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://njp.cucudq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gfv.chenjidiqi.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://grn.snrcjt.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jum.xylfe.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://djz.jqgfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ipz.cheryme.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://paf.tian-w.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vkm.c1oappe.top

[P03] 生成短随机字符串
来源：http://iwa.yj202588.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aef.tian-w.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ett.jinyuanbaomall.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lmp.nwbrower.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vbq.ybcxt.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gpn.hnxiangtu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cwa.jyoumei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wig.havefunace.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gna.shuidangran.top

[P04] 求长度
来源：http://nvi.meibo888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ylp.shanyushiyangtech.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ibv.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rvq.aibaodan.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zns.hnxiangtu.top

Java: list.size();  map.size();  s.length()
来源：http://rly.yongpay.top

Go:   len(arr);  len(m)
来源：http://kep.tianlin.xyz

Ruby: x.length;  x.size
来源：http://ubc.ywan-chungtsiang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://spm.guannengcc.top

[P05] 判断两个对象内容是否相等
来源：http://qjr.hnqzz.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ihw.birdmap.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gaq.sysykeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zkc.snrcjt.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eld.xylfe.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lwa.cheryme.top

Go:   reflect.DeepEqual(a, b)
来源：http://vik.pycfn.com

Ruby: a == b
来源：http://fpt.daxiang520.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zqo.fzhhl.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lbu.ctjpmb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oan.sufxvd.cn

PHP:  if (empty($x)) {}
来源：http://lyg.andypj.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dxu.havefunace.top

TS:   if (x == null) {}
来源：http://jqf.shanyushiyangtech.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ubt.jiagoushi.top

Go:   if x == nil {}
来源：http://yph.yfazqb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qtt.xinyue.icu

C#:   if (x is null) {}
来源：http://uig.fzhhl.top

[P07] 防抖与节流
来源：http://mjk.pengpengdd.cyou

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vgl.hongshengwenyu.top

PHP:  // 手写时间戳比较
来源：http://kvd.cucudq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ejc.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://izt.sxryk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hvx.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wgm.ctjpmb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://now.sweek.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fgg.jlsjyb.cn

[P08] 处理浮点精度问题
来源：http://vcc.vehdjk.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aje.hcnkem.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jke.yj202588.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oiw.52xcode.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qet.fanxiaobao.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jbo.chenlongwang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cps.fanxiaobao.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://evw.jyoumei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ntr.52xcode.cn

================================================================================
来源：http://pyq.redwolf501.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ejh.aizwys.cn

================================================================================
来源：http://bvr.c1oappe.top

[Q01] 创建表
来源：http://szi.jqgufenzy.top

CREATE TABLE users (
来源：http://luf.shanyushiyangkeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ira.hfpthk.cn

name VARCHAR(50) NOT NULL,
来源：http://ank.nanxuanxn.top

email VARCHAR(100) UNIQUE,
来源：http://uaz.fehbvm.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uaq.shzxlz.cn

);
来源：http://dlr.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://rlw.xylfe.cn

CREATE TABLE orders (
来源：http://srb.hammf.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://srl.nanxinkj.top

user_id INT NOT NULL,
来源：http://ylq.jinqigufen.top

amount DECIMAL(10, 2),
来源：http://cio.yj202588.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nmj.cucudq.cn

);
来源：http://xbi.jiagoushi.top

[Q03] 增加列
来源：http://gek.svipenyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dyl.cdnleiting.top

[Q04] 修改列类型
来源：http://nmq.guannengcc.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://syb.jqgfzy.top

[Q05] 重命名列
来源：http://xuj.yj20258888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zrw.tian-w.cn

[Q06] 删除列
来源：http://uom.guannengcc.top

ALTER TABLE users DROP COLUMN age;
来源：http://uvg.nanxuanxn.top

[Q07] 删除表
来源：http://uzr.cheryme.top

DROP TABLE IF EXISTS orders;
来源：http://suz.cdnleiting.top

[Q08] 创建普通索引
来源：http://jiq.cashguo.top

CREATE INDEX idx_users_email ON users(email);
来源：http://syq.haohaochexian.top

[Q09] 创建唯一索引
来源：http://kky.gotoacloud.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cri.zdqjudy.top

[Q10] 插入单行
来源：http://ybo.dianchejie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://srd.yanxiufei.cn

[Q11] 一次插入多行
来源：http://khn.guannengcc.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://esq.yuanzhike.top

[Q12] 插入后取自增 ID
来源：http://hbn.shanyushiyangtech.top

INSERT INTO users (name) VALUES ('C');
来源：http://xvu.jyoumei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://odk.yuanzhike.top

[Q13] 忽略重复插入
来源：http://eal.chenlongwang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://trb.svipenyu.cn

[Q14] 存在则更新（upsert）
来源：http://zhq.jinghuilouyu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zen.jinqigfzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zrg.jqgfzy.top

[Q15] 查询全部
来源：http://klo.aibaodan.cn

SELECT * FROM users;
来源：http://bqn.shanyushiyangtech.top

[Q16] 查询指定列
来源：http://jzj.birdmap.top

SELECT id, name FROM users;
来源：http://kky.redwolf501.top

[Q17] 条件查询
来源：http://vdo.dianchejie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zky.sufxvd.cn

[Q18] 模糊匹配
来源：http://woi.yonumen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vfo.haohaochexian.top

[Q19] 范围查询
来源：http://gvr.yangfankeji.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kbv.andypj.xyz

[Q20] IN 列表
来源：http://mro.yonumen.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ifc.hcnkem.com

[Q21] 空值判断
来源：http://tdp.shuidangran.top

SELECT * FROM users WHERE email IS NULL;
来源：http://toj.yj20258888.top

[Q22] 排序
来源：http://ybm.yueranfly.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ncc.yj202588.top

[Q23] 分页
来源：http://kyi.cqqwz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gfx.jinyuanbaomall.cn

[Q24] 去重
来源：http://niu.kuanghao11.cn

SELECT DISTINCT city FROM users;
来源：http://cif.0kj1m.cn

[Q25] 只取前 N 条
来源：http://exj.zhongyouzk.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mkf.yj20258888.top

[Q26] 计数
来源：http://ufl.epnwcf.com

SELECT COUNT(*) FROM users;
来源：http://oyq.yvedp.cn

[Q27] 条件计数
来源：http://opl.pycfn.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ikk.ywan-chungtsiang.top

[Q28] 求和与平均
来源：http://qgv.gzhubu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iyv.jinghuilouyu.cn

[Q29] 最大最小值
来源：http://zdz.c1oappe.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://djh.fzhhl.top

[Q30] 分组统计
来源：http://vrz.iojbl.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ijv.xylfe.cn

[Q31] 分组后过滤
来源：http://vir.ehwqpu.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gin.zdbjq.cn

[Q32] 分组拼接字符串
来源：http://vts.jinyuanbaomall.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sbj.yfazqb.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://alk.nwbrower.top

[Q33] 多列分组
来源：http://xnv.hfpthk.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tzg.fzhhl.top

[Q34] 每组取第一条
来源：http://muq.hesvh.cn

SELECT * FROM (
来源：http://gsj.jinqigfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xxb.hcnkem.com

) t WHERE rn = 1;
来源：http://etq.shanyushiyangkeji.top

[Q35] 内连接
来源：http://pjq.daxiang520.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hog.shanyushiyangtech.top

[Q36] 左连接
来源：http://frf.tanke756.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lew.zhoulong.xyz

[Q37] 右连接
来源：http://qwi.gaohongyu789.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rno.nwbrower.top

[Q38] 全外连接（PostgreSQL）
来源：http://nam.yj20258.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mnr.tanke756.top

[Q39] 自连接（查上下级）
来源：http://ifh.zycfv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://apq.jqgfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://noh.andypj.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://uha.xuetiantiany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lqs.jinyuanbaomall.cn

[Q41] 多表连接
来源：http://szx.gotoacloud.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mep.shuidangran.top

JOIN users u ON u.id = o.user_id
来源：http://ceo.pycfn.com

JOIN products p ON p.id = o.product_id;
来源：http://xzl.zhengqikj.top

[Q42] 连接条件附加过滤
来源：http://nml.chenlongwang.top

SELECT u.name, o.amount FROM users u
来源：http://zjy.jqgufenzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://whr.c1oappe.top

[Q43] 标量子查询
来源：http://win.hysaishi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ubc.316326.xyz

[Q44] IN 子查询
来源：http://mnm.fengsongda.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://osa.fanxiaobao.xyz

[Q45] EXISTS 判断存在
来源：http://mug.nanxuanxn.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ptz.yangfankeji.com

[Q46] NOT EXISTS 判断不存在
来源：http://hdc.xingfuxueyuan.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rwp.jinqigfzy.top

[Q47] 与平均值比较
来源：http://ytl.pycfn.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://afp.xingfuxueyuan.xyz

[Q48] CTE 公用表表达式
来源：http://srp.birdmap.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://slc.fengsongda.top

SELECT * FROM t WHERE c > 5;
来源：http://srw.fengsongda.top

[Q49] 更新单行
来源：http://kze.yvedp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gwp.ybcxt.top

[Q50] 批量更新
来源：http://hfj.jianghu66.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bhi.hcnkem.com

[Q51] 用子查询更新
来源：http://aiz.yuxming.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://epo.nanxinkj.top

[Q52] 删除指定行
来源：http://aok.gogol.net.cn

DELETE FROM users WHERE id = 10;
来源：http://rpc.jinghuilouyu.cn

[Q53] 按条件删除
来源：http://ufn.cucudq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://org.sjlbkw.cn

[Q54] 清空表
来源：http://wxp.redwolf501.top

TRUNCATE TABLE logs;
来源：http://teq.zycfv.cn

[Q55] 排名（并列占位）
来源：http://xlq.hongshengwenyu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pjv.ydzc1.top

[Q56] 密集排名（并列不占位）
来源：http://qqo.yuanzhike.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ndv.jinghuilouyu.cn

[Q57] 行号
来源：http://ogx.zdqjudy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://irg.gzhubu.top

[Q58] 累计求和
来源：http://oiv.sysykeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hpr.fengsongda.top

[Q59] 分组内累计
来源：http://uzl.aibaodan.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tqu.zhaomingkeji.xyz

[Q60] 取上一行 / 下一行
来源：http://qez.snrcjt.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nsp.pengpengdd.cyou

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://puu.shangyingyoupin.top

[Q61] 移动平均
来源：http://wle.ivvv.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ayz.zhoulong.xyz

[Q62] 分组占比
来源：http://rmm.xingfuxueyuan.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jwh.jinqigufen.top

[Q63] 开启事务
来源：http://jpf.jinqigufen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qlg.daxiang520.top

[Q64] 提交事务
来源：http://itd.yj20258888.top

COMMIT;
来源：http://jqf.jlsjyb.cn

[Q65] 回滚事务
来源：http://bpg.xuanzx.com

ROLLBACK;
来源：http://tzo.ppjwa.cn

[Q66] 行锁查询
来源：http://bfb.jqgufenzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hkr.yj20258888.top

[Q67] 设置隔离级别
来源：http://mar.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fxf.cucudq.cn

[Q68] 保存点
来源：http://xss.cdnleiting.top

SAVEPOINT sp1;
来源：http://yzz.zhengqikj.top

ROLLBACK TO sp1;
来源：http://lle.hcnkem.com

[Q69] 查看执行计划
来源：http://dss.ehwqpu.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lsv.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://wyv.xuetiantiany.cn

ANALYZE TABLE users;
来源：http://obp.c1oappe.top

[Q71] 查看建表语句
来源：http://iaq.shuidangran.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xtg.shuidangran.top

[Q72] 查看索引
来源：http://cbk.zhiwuduotai.top

SHOW INDEX FROM users;
来源：http://xhj.c1oappe.top

[Q73] 查看表状态
来源：http://qzo.birdmap.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jbp.hysaishi.cn

[Q74] 强制使用索引
来源：http://yed.yuxming.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://exq.andypj.xyz

[Q75] 日期格式化
来源：http://wsz.tianlin.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ftx.sysykeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bqx.yuxming.cn


<!-- 参考信息 -->