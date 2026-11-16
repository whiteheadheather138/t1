代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aze.sjlbkw.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fys.wangdashe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hli.meibo888.top

TS:   // 同 JS
来源：http://iux.jinghuilouyu.cn

Java: new Thread(() -> f()).start()
来源：http://iwz.chenjidiqi.icu

Go:   go f()
来源：http://umm.chenzaomai.com

Ruby: Thread.new { f }
来源：http://vwi.zhiwuduotai.top

C#:   Task.Run(() => F());
来源：http://hqb.yj20258.top

[O02] 使用线程池
来源：http://nso.jlsjyb.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ecv.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://olk.fehbvm.com

JS:   // worker_threads 线程池
来源：http://weq.yanxiufei.cn

TS:   // worker_threads 线程池
来源：http://ddc.hfpthk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://orx.yj20258888.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yeu.meibo888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://neh.jianghu66.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xef.zhengqikj.top

[O03] 加锁保护共享数据
来源：http://xls.fzhhl.top

Py:   with lock: shared += 1
来源：http://vju.yj20258.top

PHP:  // 用 flock() 做文件锁
来源：http://uvb.smart0.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fdn.wangdashe.top

TS:   // 同 JS
来源：http://rwc.guannengcc.top

Java: synchronized (this) { shared++; }
来源：http://nxt.sweek.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gxg.zhongyouzk.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wmo.yj20258888.top

C#:   lock (gate) { shared++; }
来源：http://usi.shuidangran.top

[O04] 定义异步函数并等待
来源：http://joo.epnwcf.com

Py:   async def f():⏎    await g()
来源：http://rhv.chenlongwang.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pwx.jinqigufen.top

JS:   async function f() { await g(); }
来源：http://jfw.kuanghao11.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gai.yonumen.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zsz.yvedp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ijx.fehbvm.com

Ruby: # 用 Fiber 或 async gem
来源：http://kmx.jianghu66.top

C#:   async Task F() { await G(); }
来源：http://ocd.uphjek.com

[O05] 并发执行并等待全部完成
来源：http://sww.yuxming.cn

Py:   asyncio.gather(*tasks)
来源：http://wkt.yueranfly.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bxm.vqdsnc.cn

JS:   await Promise.all(tasks)
来源：http://pad.yj202588.top

TS:   await Promise.all(tasks)
来源：http://ans.jlsjyb.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bdp.hnqzz.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fns.fzhhl.top

Ruby: threads.map(&:join)
来源：http://tos.feifeiyinyue.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lls.yj20258888.top

[O06] 使用进程池
来源：http://rkn.jinqigfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wzu.hnqzz.top

PHP:  // pcntl_fork 或多进程队列
来源：http://arf.chenlongwang.top

JS:   // child_process / cluster 模块
来源：http://zsf.sysykeji.top

TS:   // child_process / cluster 模块
来源：http://nru.sjlbkw.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zty.daria6918.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fdt.meibo888.top

Ruby: // fork 块
来源：http://eoy.zhongyouzk.top

C#:   Parallel.For
来源：http://opd.fanxiaobao.xyz

================================================================================
来源：http://uvx.9152youxi.cn

P. 常用工具函数
来源：http://boc.cdnleiting.top

================================================================================
来源：http://azv.tarul.cn

[P01] 生成 UUID
来源：http://ecm.jinqigfzy.top

Py:   str(uuid.uuid4())
来源：http://xwj.ppjwa.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pyk.gzhubu.top

JS:   crypto.randomUUID()
来源：http://qmf.aibaodan.cn

TS:   crypto.randomUUID()
来源：http://mzk.andypj.xyz

Java: UUID.randomUUID().toString()
来源：http://iuk.chenjidiqi.icu

Go:   // 用 github.com/google/uuid
来源：http://auc.ybcxt.top

Ruby: SecureRandom.uuid
来源：http://wdu.yvedp.cn

C#:   Guid.NewGuid().ToString()
来源：http://ahw.hnxiangtu.top

[P02] MD5 / SHA256 摘要
来源：http://cpv.gzhubu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jik.jyoumei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yzb.yuanzhike.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dcl.quarkkingdee.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tiv.xinyue.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://syn.gogol.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cpz.jianghu66.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xsx.fktsv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tak.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://bpy.316326.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dkw.hcnkem.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jrz.uphjek.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bhg.yj202588.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dva.chenlongwang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wmc.tianlin.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hqr.yanxiufei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zek.xingfuxueyuan.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mqd.kuanghao11.cn

[P04] 求长度
来源：http://ksj.tarul.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qwg.mhx1999.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sqe.guowangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://imu.sufxvd.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rdd.ivvv.top

Java: list.size();  map.size();  s.length()
来源：http://ypx.jianghu66.top

Go:   len(arr);  len(m)
来源：http://ixs.sjlbkw.cn

Ruby: x.length;  x.size
来源：http://tdh.daxiang520.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zkz.dashuyun.cn

[P05] 判断两个对象内容是否相等
来源：http://tqb.zhijiandao.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hne.andypj.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://avn.epnwcf.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mgh.hcnkem.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kqg.ehwqpu.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nxs.nanxuanxn.top

Go:   reflect.DeepEqual(a, b)
来源：http://zqf.ctjpmb.com

Ruby: a == b
来源：http://stp.ydzc1.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xus.yvedp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vhf.hywenlv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pcu.aizwys.cn

PHP:  if (empty($x)) {}
来源：http://yud.sufxvd.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pco.andypj.xyz

TS:   if (x == null) {}
来源：http://ppx.fzhhl.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ptw.hongshengwenyu.top

Go:   if x == nil {}
来源：http://bjc.zhengqikj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oae.xuanzx.com

C#:   if (x is null) {}
来源：http://kxa.hnxiangtu.top

[P07] 防抖与节流
来源：http://smz.cashguo.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bgy.yongpay.top

PHP:  // 手写时间戳比较
来源：http://bgb.chenzaomai.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uql.xylfe.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gln.fanxiaobao.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jad.hnxiangtu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qkj.jinqigufen.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://bcw.nwbrower.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kax.sweek.top

[P08] 处理浮点精度问题
来源：http://vbb.yuanzhike.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ynf.zhoulong.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mdq.quarkkingdee.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dcs.mhx1999.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jky.nwbrower.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oxq.zhaomingkeji.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qlj.tanke756.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ynf.bbcook.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tyi.epnwcf.com

================================================================================
来源：http://nqb.guowangkeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ogl.andypj.xyz

================================================================================
来源：http://cgs.vehdjk.com

[Q01] 创建表
来源：http://qae.chenjidiqi.icu

CREATE TABLE users (
来源：http://gpn.zdbjq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://aav.meibo888.top

name VARCHAR(50) NOT NULL,
来源：http://ocu.fanxiaobao.xyz

email VARCHAR(100) UNIQUE,
来源：http://czp.dianchejie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://elg.9152youxi.cn

);
来源：http://fdw.uphjek.com

[Q02] 创建带外键的表
来源：http://qdb.ybcxt.top

CREATE TABLE orders (
来源：http://kox.ydjk.org.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://glu.andypj.xyz

user_id INT NOT NULL,
来源：http://qhj.nwbrower.top

amount DECIMAL(10, 2),
来源：http://rpt.fzhhl.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wqv.tianlin.xyz

);
来源：http://ifn.zhongyouzk.top

[Q03] 增加列
来源：http://ihp.jinghuilouyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wam.kuanghao11.cn

[Q04] 修改列类型
来源：http://puh.zhixingplan.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qss.ehwqpu.com

[Q05] 重命名列
来源：http://inx.fengsongda.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://iwe.chenjidiqi.icu

[Q06] 删除列
来源：http://lny.nwbrower.top

ALTER TABLE users DROP COLUMN age;
来源：http://roy.jinqigufen.top

[Q07] 删除表
来源：http://waz.cdnleiting.top

DROP TABLE IF EXISTS orders;
来源：http://upl.zhengqikj.top

[Q08] 创建普通索引
来源：http://cdb.zhijiandao.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pcm.ivvv.top

[Q09] 创建唯一索引
来源：http://bjr.xinyue.icu

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ent.nanxuanxn.top

[Q10] 插入单行
来源：http://joh.epnwcf.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xax.shzxlz.cn

[Q11] 一次插入多行
来源：http://zyr.tanke756.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ese.ywan-chungtsiang.top

[Q12] 插入后取自增 ID
来源：http://vvf.yueranfly.top

INSERT INTO users (name) VALUES ('C');
来源：http://rfb.guowangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://txf.andypj.xyz

[Q13] 忽略重复插入
来源：http://pqw.yongpay.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gxb.hfpthk.cn

[Q14] 存在则更新（upsert）
来源：http://wgn.shuidangran.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kye.nanxuanxn.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jaf.guannengcc.top

[Q15] 查询全部
来源：http://buh.gotoacloud.top

SELECT * FROM users;
来源：http://lsw.ydjk.org.cn

[Q16] 查询指定列
来源：http://oit.fanxiaobao.xyz

SELECT id, name FROM users;
来源：http://qbh.pengpengdd.cyou

[Q17] 条件查询
来源：http://thn.zhongyouzk.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vse.shanyushiyangkeji.top

[Q18] 模糊匹配
来源：http://jpa.wangdashe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jgb.zhengqikj.top

[Q19] 范围查询
来源：http://jet.jlsjyb.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mys.yj20258888.top

[Q20] IN 列表
来源：http://dlt.sjlbkw.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fva.smart0.xyz

[Q21] 空值判断
来源：http://cos.zhongyouzk.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vct.zhiwuduotai.top

[Q22] 排序
来源：http://rwd.xuetiantiany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://soy.fzhhl.top

[Q23] 分页
来源：http://kua.redwolf501.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://naz.smart0.xyz

[Q24] 去重
来源：http://iya.meibo888.top

SELECT DISTINCT city FROM users;
来源：http://lxe.hammf.cn

[Q25] 只取前 N 条
来源：http://qbt.zycfv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://edh.hfpthk.cn

[Q26] 计数
来源：http://qsx.nanxuanxn.top

SELECT COUNT(*) FROM users;
来源：http://ntb.yonumen.top

[Q27] 条件计数
来源：http://zuu.mhx1999.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nem.hesvh.cn

[Q28] 求和与平均
来源：http://ejg.daria6918.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zit.birdmap.top

[Q29] 最大最小值
来源：http://aaj.gotoacloud.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ygh.cashguo.top

[Q30] 分组统计
来源：http://lwb.iojbl.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://llq.c1oappe.top

[Q31] 分组后过滤
来源：http://lpa.smart0.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xyp.ybcxt.top

[Q32] 分组拼接字符串
来源：http://nnp.shzxlz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ygf.xingfuxueyuan.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jzu.haohaochexian.top

[Q33] 多列分组
来源：http://jdg.cashguo.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hpr.yj202588.top

[Q34] 每组取第一条
来源：http://tzl.smart0.xyz

SELECT * FROM (
来源：http://zja.bbcook.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sxi.redwolf501.top

) t WHERE rn = 1;
来源：http://bej.hammf.cn

[Q35] 内连接
来源：http://pri.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rag.ydjk.org.cn

[Q36] 左连接
来源：http://vqn.xinyue.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mbz.daxiang520.top

[Q37] 右连接
来源：http://xbc.xuetiantiany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fpx.guowangkeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://oka.pengpengdd.cyou

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://odq.kuanghao11.cn

[Q39] 自连接（查上下级）
来源：http://mpu.jinghuilouyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://roa.52xcode.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qxn.cdnleiting.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ywq.shangyingyoupin.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dih.guowangkeji.top

[Q41] 多表连接
来源：http://naz.jinyuanbaomall.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xug.sjlbkw.cn

JOIN users u ON u.id = o.user_id
来源：http://enz.bjfxy.top

JOIN products p ON p.id = o.product_id;
来源：http://lyf.mhx1999.top

[Q42] 连接条件附加过滤
来源：http://ljl.yj20258888.top

SELECT u.name, o.amount FROM users u
来源：http://pqy.yongpay.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bnf.yueranfly.top

[Q43] 标量子查询
来源：http://zry.kuanghao11.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://krm.hysaishi.cn

[Q44] IN 子查询
来源：http://onb.316326.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://eav.wangdashe.top

[Q45] EXISTS 判断存在
来源：http://hdo.gaohongyu789.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://njf.hnqzz.top

[Q46] NOT EXISTS 判断不存在
来源：http://xmt.jlsjyb.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ana.xylfe.cn

[Q47] 与平均值比较
来源：http://fuh.52xcode.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dfo.epnwcf.com

[Q48] CTE 公用表表达式
来源：http://yan.guannengcc.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mlr.jqgufenzy.top

SELECT * FROM t WHERE c > 5;
来源：http://vjc.ydzc1.top

[Q49] 更新单行
来源：http://yzt.snrcjt.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vba.tianlin.xyz

[Q50] 批量更新
来源：http://ftm.ydzc1.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rwo.yuxming.cn

[Q51] 用子查询更新
来源：http://iev.epnwcf.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dql.daria6918.cn

[Q52] 删除指定行
来源：http://ckb.yj202588.top

DELETE FROM users WHERE id = 10;
来源：http://ifs.zhixingplan.top

[Q53] 按条件删除
来源：http://nnl.gzhubu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bvy.daxiang520.top

[Q54] 清空表
来源：http://yip.yj202588.top

TRUNCATE TABLE logs;
来源：http://vom.hywenlv.cn

[Q55] 排名（并列占位）
来源：http://qyy.zhijiandao.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jmf.pengpengdd.cyou

[Q56] 密集排名（并列不占位）
来源：http://ulx.gotoacloud.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://izx.jiagoushi.top

[Q57] 行号
来源：http://nfo.pycfn.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hic.birdmap.top

[Q58] 累计求和
来源：http://tmm.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://joo.sysykeji.top

[Q59] 分组内累计
来源：http://pqa.hcnkem.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pxt.jinghuilouyu.cn

[Q60] 取上一行 / 下一行
来源：http://gwy.yfazqb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qqt.yj20258.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sqe.yueranfly.top

[Q61] 移动平均
来源：http://zfl.fktsv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kvd.52xcode.cn

[Q62] 分组占比
来源：http://qrq.aibaodan.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mko.zhaomingkeji.xyz

[Q63] 开启事务
来源：http://pvr.bbcook.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lsh.svipenyu.cn

[Q64] 提交事务
来源：http://vca.ywan-chungtsiang.top

COMMIT;
来源：http://wpr.cucudq.cn

[Q65] 回滚事务
来源：http://rtr.jlsjyb.cn

ROLLBACK;
来源：http://aah.zhoulong.xyz

[Q66] 行锁查询
来源：http://ayy.smart0.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://taz.jinyuanbaomall.cn

[Q67] 设置隔离级别
来源：http://jiz.chenjidiqi.icu

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kdt.zhengqikj.top

[Q68] 保存点
来源：http://zhn.iojbl.cn

SAVEPOINT sp1;
来源：http://zkr.jianghu66.top

ROLLBACK TO sp1;
来源：http://kwi.zycfv.cn

[Q69] 查看执行计划
来源：http://nus.quarkkingdee.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kqy.nanxuanxn.top

[Q70] 更新统计信息
来源：http://zjf.xylfe.cn

ANALYZE TABLE users;
来源：http://xvs.feifeiyinyue.top

[Q71] 查看建表语句
来源：http://rsv.tianlin.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fdf.jlsjyb.cn

[Q72] 查看索引
来源：http://bwv.xuanzx.com

SHOW INDEX FROM users;
来源：http://ldq.aibaodan.cn

[Q73] 查看表状态
来源：http://izd.tianlin.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://che.vqdsnc.cn

[Q74] 强制使用索引
来源：http://aps.wangshuangyany.cn


<!-- 参考信息 -->