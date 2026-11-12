代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oia.kuanghao11.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pwt.cucudq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xan.aizwys.cn

TS:   // 同 JS
来源：http://adw.sufxvd.cn

Java: new Thread(() -> f()).start()
来源：http://nnx.epnwcf.com

Go:   go f()
来源：http://yxl.mhx1999.top

Ruby: Thread.new { f }
来源：http://ngv.gzhubu.top

C#:   Task.Run(() => F());
来源：http://qrv.sjlbkw.cn

[O02] 使用线程池
来源：http://ltc.smart0.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vzj.sysykeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://din.daria6918.cn

JS:   // worker_threads 线程池
来源：http://qra.hongshengwenyu.top

TS:   // worker_threads 线程池
来源：http://qgo.0kj1m.cn

Java: Executors.newFixedThreadPool(4)
来源：http://run.svipenyu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vcx.fzhhl.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hxx.sweek.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vfq.nanxinkj.top

[O03] 加锁保护共享数据
来源：http://men.aibaodan.cn

Py:   with lock: shared += 1
来源：http://gtr.jianghu66.top

PHP:  // 用 flock() 做文件锁
来源：http://qjq.hammf.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yti.wangshuangyany.cn

TS:   // 同 JS
来源：http://eff.kuanghao11.cn

Java: synchronized (this) { shared++; }
来源：http://nqw.zycfv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rwg.zycfv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jzq.aizwys.cn

C#:   lock (gate) { shared++; }
来源：http://jas.zhoulong.xyz

[O04] 定义异步函数并等待
来源：http://xby.chenlongwang.top

Py:   async def f():⏎    await g()
来源：http://mdl.daria6918.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ktl.svipenyu.cn

JS:   async function f() { await g(); }
来源：http://gwo.quarkkingdee.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ilt.vqdsnc.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://loh.yangfankeji.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oov.zhaomingkeji.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://bka.9152youxi.cn

C#:   async Task F() { await G(); }
来源：http://kpx.kuanghao11.cn

[O05] 并发执行并等待全部完成
来源：http://yaa.tanke756.top

Py:   asyncio.gather(*tasks)
来源：http://xfy.jinqigfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mmb.yfazqb.com

JS:   await Promise.all(tasks)
来源：http://skt.jqgfzy.top

TS:   await Promise.all(tasks)
来源：http://smx.cucudq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vub.dianchejie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tvl.bjfxy.top

Ruby: threads.map(&:join)
来源：http://nrp.hongshengwenyu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ccu.hysaishi.cn

[O06] 使用进程池
来源：http://wnl.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yzn.zycfv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ppq.iojbl.cn

JS:   // child_process / cluster 模块
来源：http://opy.hnxiangtu.top

TS:   // child_process / cluster 模块
来源：http://sso.kuanghao11.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://flt.cdnleiting.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eew.sweek.top

Ruby: // fork 块
来源：http://kep.feifeiyinyue.top

C#:   Parallel.For
来源：http://xhl.ybcxt.top

================================================================================
来源：http://pfd.iojbl.cn

P. 常用工具函数
来源：http://qis.jqgfzy.top

================================================================================
来源：http://mea.yuanzhike.top

[P01] 生成 UUID
来源：http://bln.yongpay.top

Py:   str(uuid.uuid4())
来源：http://xwo.9152youxi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ork.316326.xyz

JS:   crypto.randomUUID()
来源：http://bad.xylfe.cn

TS:   crypto.randomUUID()
来源：http://mtv.jqgfzy.top

Java: UUID.randomUUID().toString()
来源：http://ebb.fehbvm.com

Go:   // 用 github.com/google/uuid
来源：http://xwm.birdmap.top

Ruby: SecureRandom.uuid
来源：http://kip.yonumen.top

C#:   Guid.NewGuid().ToString()
来源：http://kru.cucudq.cn

[P02] MD5 / SHA256 摘要
来源：http://kdu.316326.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://chx.cqqwz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dpl.0kj1m.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hji.zycfv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wgi.jinqigufen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jpt.sweek.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://alp.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kqz.52xcode.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cso.smart0.xyz

[P03] 生成短随机字符串
来源：http://xdl.guannengcc.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mfq.mhx1999.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qkl.epnwcf.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pkn.yfazqb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sxl.guannengcc.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ein.ctjpmb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bty.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yqj.tian-w.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bri.zhiwuduotai.top

[P04] 求长度
来源：http://xwd.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://chu.chenjidiqi.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uek.jinghuilouyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hbq.hesvh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gtv.chenlongwang.top

Java: list.size();  map.size();  s.length()
来源：http://hoq.aizwys.cn

Go:   len(arr);  len(m)
来源：http://nlk.ydzc1.top

Ruby: x.length;  x.size
来源：http://nju.wangdashe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dny.redwolf501.top

[P05] 判断两个对象内容是否相等
来源：http://bqv.gzhubu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pca.chenjidiqi.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qvn.sxryk.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://unm.316326.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yfe.hysaishi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://erl.hysaishi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jso.tarul.cn

Ruby: a == b
来源：http://nbi.yuanzhike.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wrn.hammf.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://aoy.smart0.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bzp.cheryme.top

PHP:  if (empty($x)) {}
来源：http://vbb.cashguo.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bvs.andypj.xyz

TS:   if (x == null) {}
来源：http://pci.guowangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qhf.gaohongyu789.top

Go:   if x == nil {}
来源：http://woy.kuanghao11.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lqw.quarkkingdee.top

C#:   if (x is null) {}
来源：http://qis.zdbjq.cn

[P07] 防抖与节流
来源：http://wgg.hnxiangtu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://umg.mhx1999.top

PHP:  // 手写时间戳比较
来源：http://ppw.iojbl.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vay.316326.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hyh.birdmap.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sfa.snrcjt.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xvn.aizwys.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wrl.316326.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yzk.sysykeji.top

[P08] 处理浮点精度问题
来源：http://peh.bbcook.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aax.yuxming.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ppt.52xcode.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pwf.zhaomingkeji.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://knz.bbcook.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wmh.bbcook.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pxu.shanyushiyangkeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uzm.cqqwz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fdp.redwolf501.top

================================================================================
来源：http://wpr.0kj1m.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uqg.guannengcc.top

================================================================================
来源：http://osb.ivvv.top

[Q01] 创建表
来源：http://ldk.quarkkingdee.top

CREATE TABLE users (
来源：http://bwo.hnqzz.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wko.zdqjudy.top

name VARCHAR(50) NOT NULL,
来源：http://yrj.zycfv.cn

email VARCHAR(100) UNIQUE,
来源：http://wki.zhiwuduotai.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://swu.zhiwuduotai.top

);
来源：http://tty.jinghuilouyu.cn

[Q02] 创建带外键的表
来源：http://tfe.hongshengwenyu.top

CREATE TABLE orders (
来源：http://egh.ppjwa.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nvf.jqgfzy.top

user_id INT NOT NULL,
来源：http://rvt.jiagoushi.top

amount DECIMAL(10, 2),
来源：http://kbp.shuidangran.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wtl.redwolf501.top

);
来源：http://ata.cashguo.top

[Q03] 增加列
来源：http://ehv.zhaomingkeji.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://haj.hammf.cn

[Q04] 修改列类型
来源：http://lfh.jiagoushi.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://snr.ehwqpu.com

[Q05] 重命名列
来源：http://mcb.316326.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ixi.tianlin.xyz

[Q06] 删除列
来源：http://uja.snrcjt.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gvk.shangyingyoupin.top

[Q07] 删除表
来源：http://mkk.hfpthk.cn

DROP TABLE IF EXISTS orders;
来源：http://ykf.cucudq.cn

[Q08] 创建普通索引
来源：http://oho.ybcxt.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fdh.yangfankeji.com

[Q09] 创建唯一索引
来源：http://pfx.jlsjyb.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xqa.cqqwz.cn

[Q10] 插入单行
来源：http://nxs.aizwys.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ypx.zhaomingkeji.xyz

[Q11] 一次插入多行
来源：http://jen.xylfe.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://krb.fehbvm.com

[Q12] 插入后取自增 ID
来源：http://zry.jiagoushi.top

INSERT INTO users (name) VALUES ('C');
来源：http://hqt.xuetiantiany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ypu.hnqzz.top

[Q13] 忽略重复插入
来源：http://ibg.zhixingplan.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://neo.jinyuanbaomall.cn

[Q14] 存在则更新（upsert）
来源：http://qxh.shangyingyoupin.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zke.jlsjyb.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vvj.nanxinkj.top

[Q15] 查询全部
来源：http://apb.pengpengdd.cyou

SELECT * FROM users;
来源：http://qfa.redwolf501.top

[Q16] 查询指定列
来源：http://ukr.chenjidiqi.icu

SELECT id, name FROM users;
来源：http://dbf.sweek.top

[Q17] 条件查询
来源：http://ffp.hcnkem.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dhs.dashuyun.cn

[Q18] 模糊匹配
来源：http://jtn.zhongyouzk.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://djk.jinqigufen.top

[Q19] 范围查询
来源：http://nqc.svipenyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zvb.yanxiufei.cn

[Q20] IN 列表
来源：http://rmx.tanke756.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://aal.uphjek.com

[Q21] 空值判断
来源：http://yey.zycfv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lwr.jlsjyb.cn

[Q22] 排序
来源：http://cln.cdnleiting.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xuz.cqqwz.cn

[Q23] 分页
来源：http://jrh.xylfe.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://esi.hywenlv.cn

[Q24] 去重
来源：http://dwo.ybcxt.top

SELECT DISTINCT city FROM users;
来源：http://hdj.jinyuanbaomall.cn

[Q25] 只取前 N 条
来源：http://wnj.yj202588.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://iyp.ivvv.top

[Q26] 计数
来源：http://iww.wangshuangyany.cn

SELECT COUNT(*) FROM users;
来源：http://zun.ywan-chungtsiang.top

[Q27] 条件计数
来源：http://hwv.gaohongyu789.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wcy.quarkkingdee.top

[Q28] 求和与平均
来源：http://mhv.smart0.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kya.yangfankeji.com

[Q29] 最大最小值
来源：http://pvf.iojbl.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ifm.hnqzz.top

[Q30] 分组统计
来源：http://bgp.xuetiantiany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yno.haohaochexian.top

[Q31] 分组后过滤
来源：http://myx.yuanzhike.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ede.wangshuangyany.cn

[Q32] 分组拼接字符串
来源：http://mqh.xylfe.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gxl.hfpthk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mpu.sufxvd.cn

[Q33] 多列分组
来源：http://njt.bbcook.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tzz.ydzc1.top

[Q34] 每组取第一条
来源：http://inj.jqgfzy.top

SELECT * FROM (
来源：http://mnm.redwolf501.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://msb.fanxiaobao.xyz

) t WHERE rn = 1;
来源：http://hwv.yongpay.top

[Q35] 内连接
来源：http://bgi.tianlin.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ezr.aizwys.cn

[Q36] 左连接
来源：http://gzk.zhoulong.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wgk.shuidangran.top

[Q37] 右连接
来源：http://zfp.dianchejie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uvl.sysykeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://xzs.zhaomingkeji.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oij.hnxiangtu.top

[Q39] 自连接（查上下级）
来源：http://ydn.fzhhl.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kun.jqgfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qtm.snrcjt.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ola.aibaodan.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ivo.ydjk.org.cn

[Q41] 多表连接
来源：http://geb.nwbrower.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wlm.xziqi.cn

JOIN users u ON u.id = o.user_id
来源：http://uom.hfpthk.cn

JOIN products p ON p.id = o.product_id;
来源：http://kwy.shanyushiyangkeji.top

[Q42] 连接条件附加过滤
来源：http://tnn.epnwcf.com

SELECT u.name, o.amount FROM users u
来源：http://kri.wangshuangyany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://izh.uphjek.com

[Q43] 标量子查询
来源：http://bnh.gotoacloud.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mfv.pycfn.com

[Q44] IN 子查询
来源：http://eqw.fengsongda.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://odh.iojbl.cn

[Q45] EXISTS 判断存在
来源：http://iig.zhengqikj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dks.hcnkem.com

[Q46] NOT EXISTS 判断不存在
来源：http://anz.snrcjt.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pyj.xziqi.cn

[Q47] 与平均值比较
来源：http://rjs.yonumen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jvb.yfazqb.com

[Q48] CTE 公用表表达式
来源：http://cis.shanyushiyangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://znb.mhx1999.top

SELECT * FROM t WHERE c > 5;
来源：http://vxe.yj202588.top

[Q49] 更新单行
来源：http://lzt.zhixingplan.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ggf.xingfuxueyuan.xyz

[Q50] 批量更新
来源：http://smy.iojbl.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oyg.yvedp.cn

[Q51] 用子查询更新
来源：http://opx.fktsv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qrw.feifeiyinyue.top

[Q52] 删除指定行
来源：http://kbd.c1oappe.top

DELETE FROM users WHERE id = 10;
来源：http://ara.xinyue.icu

[Q53] 按条件删除
来源：http://chc.zhiwuduotai.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hiu.tanke756.top

[Q54] 清空表
来源：http://jgb.dianchejie.cn

TRUNCATE TABLE logs;
来源：http://ans.yj20258888.top

[Q55] 排名（并列占位）
来源：http://tev.yfazqb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vcf.haohaochexian.top

[Q56] 密集排名（并列不占位）
来源：http://vgm.hesvh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ged.redwolf501.top

[Q57] 行号
来源：http://nzc.chenjidiqi.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mkz.cheryme.top

[Q58] 累计求和
来源：http://fsj.0kj1m.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zfu.yongpay.top

[Q59] 分组内累计
来源：http://jet.gzhubu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xpd.ywan-chungtsiang.top

[Q60] 取上一行 / 下一行
来源：http://zhu.feifeiyinyue.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dwj.sysykeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wkp.jianghu66.top

[Q61] 移动平均
来源：http://yad.svipenyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pjh.shanyushiyangkeji.top

[Q62] 分组占比
来源：http://qrw.cashguo.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vdd.yj20258.top

[Q63] 开启事务
来源：http://cqk.hywenlv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ide.yvedp.cn

[Q64] 提交事务
来源：http://ubp.kuanghao11.cn

COMMIT;
来源：http://rau.ywan-chungtsiang.top

[Q65] 回滚事务
来源：http://nav.shanyushiyangtech.top

ROLLBACK;
来源：http://njx.shanyushiyangkeji.top

[Q66] 行锁查询
来源：http://ghp.zhongyouzk.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ymw.ppjwa.cn

[Q67] 设置隔离级别
来源：http://otc.hysaishi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gxl.bjfxy.top

[Q68] 保存点
来源：http://ftu.sufxvd.cn

SAVEPOINT sp1;
来源：http://skp.bjfxy.top

ROLLBACK TO sp1;
来源：http://riu.bjfxy.top

[Q69] 查看执行计划
来源：http://hea.pycfn.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://scd.gogol.net.cn

[Q70] 更新统计信息
来源：http://bcf.gzhubu.top

ANALYZE TABLE users;
来源：http://hzr.zhiwuduotai.top

[Q71] 查看建表语句
来源：http://rkc.daria6918.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jzp.xuanzx.com

[Q72] 查看索引
来源：http://djx.hammf.cn

SHOW INDEX FROM users;
来源：http://fhw.hnxiangtu.top

[Q73] 查看表状态
来源：http://evg.gogol.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zxl.guowangkeji.top

[Q74] 强制使用索引
来源：http://efz.hysaishi.cn


<!-- 参考信息 -->