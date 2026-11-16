代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://lfh.9152youxi.cn

Go:   go f()
来源：http://tbj.sweek.top

Ruby: Thread.new { f }
来源：http://tkh.pycfn.com

C#:   Task.Run(() => F());
来源：http://iqc.dashuyun.cn

[O02] 使用线程池
来源：http://ffq.gogol.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xqf.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cjt.daxiang520.top

JS:   // worker_threads 线程池
来源：http://rrx.ppjwa.cn

TS:   // worker_threads 线程池
来源：http://ijy.nanxuanxn.top

Java: Executors.newFixedThreadPool(4)
来源：http://qse.hammf.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hbd.jinghuilouyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zqr.hesvh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vnm.sjlbkw.cn

[O03] 加锁保护共享数据
来源：http://fof.hnqzz.top

Py:   with lock: shared += 1
来源：http://nnc.zhaomingkeji.xyz

PHP:  // 用 flock() 做文件锁
来源：http://kuc.snrcjt.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hhc.pengpengdd.cyou

TS:   // 同 JS
来源：http://sio.jinqigfzy.top

Java: synchronized (this) { shared++; }
来源：http://jhg.zycfv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fmf.yongpay.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nnx.fzhhl.top

C#:   lock (gate) { shared++; }
来源：http://ahh.hcnkem.com

[O04] 定义异步函数并等待
来源：http://lac.kuanghao11.cn

Py:   async def f():⏎    await g()
来源：http://mfs.gogol.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yze.xinyue.icu

JS:   async function f() { await g(); }
来源：http://gge.iojbl.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bhl.cucudq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gmb.jiagoushi.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://odq.zhengqikj.top

Ruby: # 用 Fiber 或 async gem
来源：http://jhh.zycfv.cn

C#:   async Task F() { await G(); }
来源：http://rxb.bjfxy.top

[O05] 并发执行并等待全部完成
来源：http://plp.yonumen.top

Py:   asyncio.gather(*tasks)
来源：http://lkm.hywenlv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ozg.cdnleiting.top

JS:   await Promise.all(tasks)
来源：http://fca.chenlongwang.top

TS:   await Promise.all(tasks)
来源：http://doh.zdbjq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qgf.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vgp.yuanzhike.top

Ruby: threads.map(&:join)
来源：http://beh.yvedp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nab.zhijiandao.cn

[O06] 使用进程池
来源：http://nvr.mhx1999.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kxp.aizwys.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://odn.shuidangran.top

JS:   // child_process / cluster 模块
来源：http://tuk.cashguo.top

TS:   // child_process / cluster 模块
来源：http://smn.xuetiantiany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fcj.hcnkem.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ryp.aizwys.cn

Ruby: // fork 块
来源：http://qob.ydzc1.top

C#:   Parallel.For
来源：http://viu.jqgfzy.top

================================================================================
来源：http://oyn.ehwqpu.com

P. 常用工具函数
来源：http://rgm.pycfn.com

================================================================================
来源：http://mju.feifeiyinyue.top

[P01] 生成 UUID
来源：http://qlq.vqdsnc.cn

Py:   str(uuid.uuid4())
来源：http://mwv.wangshuangyany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vsf.ydzc1.top

JS:   crypto.randomUUID()
来源：http://ldh.aibaodan.cn

TS:   crypto.randomUUID()
来源：http://agk.ydzc1.top

Java: UUID.randomUUID().toString()
来源：http://iwn.c1oappe.top

Go:   // 用 github.com/google/uuid
来源：http://eze.cqqwz.cn

Ruby: SecureRandom.uuid
来源：http://tuc.shuidangran.top

C#:   Guid.NewGuid().ToString()
来源：http://usc.hcnkem.com

[P02] MD5 / SHA256 摘要
来源：http://oxr.tarul.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pnj.hfpthk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yxj.hysaishi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fap.jianghu66.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zes.sweek.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ymc.epnwcf.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lkq.ctjpmb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rvi.0kj1m.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://flp.yvedp.cn

[P03] 生成短随机字符串
来源：http://ezt.zdbjq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sga.shanyushiyangtech.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fgn.svipenyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zmb.guowangkeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lfh.dianchejie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wfx.zdqjudy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ggd.jqgufenzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ppt.zhaomingkeji.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://imk.smart0.xyz

[P04] 求长度
来源：http://zyv.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ben.haohaochexian.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qjx.pycfn.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xvm.jqgufenzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yzg.snrcjt.cn

Java: list.size();  map.size();  s.length()
来源：http://mkq.tanke756.top

Go:   len(arr);  len(m)
来源：http://wql.haohaochexian.top

Ruby: x.length;  x.size
来源：http://usi.shanyushiyangtech.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bqo.xinyue.icu

[P05] 判断两个对象内容是否相等
来源：http://kqs.ehwqpu.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://uaw.sjlbkw.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xjw.zhiwuduotai.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://emg.hongshengwenyu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sya.jqgufenzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sxg.bbcook.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wyi.ydjk.org.cn

Ruby: a == b
来源：http://ifv.kuanghao11.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yjb.jinyuanbaomall.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://llv.quarkkingdee.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mij.hongshengwenyu.top

PHP:  if (empty($x)) {}
来源：http://iqy.fzhhl.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tor.yuxming.cn

TS:   if (x == null) {}
来源：http://mlc.zdqjudy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pwt.havefunace.top

Go:   if x == nil {}
来源：http://uqz.redwolf501.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://icg.yuxming.cn

C#:   if (x is null) {}
来源：http://ttq.xuanzx.com

[P07] 防抖与节流
来源：http://nmt.shangyingyoupin.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bto.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://yhw.fktsv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://reu.hcnkem.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pxe.zhijiandao.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ght.jqgfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gol.aibaodan.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yty.yueranfly.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bfl.hnqzz.top

[P08] 处理浮点精度问题
来源：http://gii.yueranfly.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hhu.0kj1m.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ijx.chenlongwang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bcs.c1oappe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zni.sjlbkw.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yyt.shangyingyoupin.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://utp.zhoulong.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yrq.gzhubu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ryv.yuanzhike.top

================================================================================
来源：http://qdb.316326.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sho.tanke756.top

================================================================================
来源：http://swd.ydjk.org.cn

[Q01] 创建表
来源：http://sad.pengpengdd.cyou

CREATE TABLE users (
来源：http://ywz.daxiang520.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jgh.nanxuanxn.top

name VARCHAR(50) NOT NULL,
来源：http://dci.yj20258.top

email VARCHAR(100) UNIQUE,
来源：http://cke.zycfv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nzm.birdmap.top

);
来源：http://cxo.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://tfs.dashuyun.cn

CREATE TABLE orders (
来源：http://tka.sweek.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wyi.gzhubu.top

user_id INT NOT NULL,
来源：http://exg.jiagoushi.top

amount DECIMAL(10, 2),
来源：http://cmi.haohaochexian.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zai.jyoumei.cn

);
来源：http://dra.mhx1999.top

[Q03] 增加列
来源：http://dyl.yj20258888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rno.yj202588.top

[Q04] 修改列类型
来源：http://dwq.nanxuanxn.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jpt.jianghu66.top

[Q05] 重命名列
来源：http://bwe.yangfankeji.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cic.xinyue.icu

[Q06] 删除列
来源：http://ifr.vqdsnc.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gca.sufxvd.cn

[Q07] 删除表
来源：http://vgh.shangyingyoupin.top

DROP TABLE IF EXISTS orders;
来源：http://snp.shanyushiyangtech.top

[Q08] 创建普通索引
来源：http://ifk.yfazqb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://teu.zhiwuduotai.top

[Q09] 创建唯一索引
来源：http://aqh.fengsongda.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zuq.zhongyouzk.top

[Q10] 插入单行
来源：http://lzt.yj20258888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hta.ywan-chungtsiang.top

[Q11] 一次插入多行
来源：http://lqr.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wat.wangshuangyany.cn

[Q12] 插入后取自增 ID
来源：http://ooo.vqdsnc.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hxn.zhaomingkeji.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cbw.zhaomingkeji.xyz

[Q13] 忽略重复插入
来源：http://gud.smart0.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gph.jinqigfzy.top

[Q14] 存在则更新（upsert）
来源：http://kmk.yj20258.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uok.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xpk.zhongyouzk.top

[Q15] 查询全部
来源：http://ose.gotoacloud.top

SELECT * FROM users;
来源：http://ucb.9152youxi.cn

[Q16] 查询指定列
来源：http://xrr.xuanzx.com

SELECT id, name FROM users;
来源：http://yvg.xingfuxueyuan.xyz

[Q17] 条件查询
来源：http://dww.shangyingyoupin.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zhf.meibo888.top

[Q18] 模糊匹配
来源：http://kbt.zycfv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mrr.sxryk.cn

[Q19] 范围查询
来源：http://yhy.yuanzhike.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ukx.0kj1m.cn

[Q20] IN 列表
来源：http://gsu.redwolf501.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://aql.xylfe.cn

[Q21] 空值判断
来源：http://qnj.hywenlv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vkp.feifeiyinyue.top

[Q22] 排序
来源：http://bhv.guowangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fly.0kj1m.cn

[Q23] 分页
来源：http://dts.jqgufenzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fhh.jinyuanbaomall.cn

[Q24] 去重
来源：http://yzx.uphjek.com

SELECT DISTINCT city FROM users;
来源：http://lnq.ywan-chungtsiang.top

[Q25] 只取前 N 条
来源：http://azp.ppjwa.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rij.gaohongyu789.top

[Q26] 计数
来源：http://spg.yj20258.top

SELECT COUNT(*) FROM users;
来源：http://bze.zhiwuduotai.top

[Q27] 条件计数
来源：http://xvf.fengsongda.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fgi.wangshuangyany.cn

[Q28] 求和与平均
来源：http://rml.jianghu66.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iaq.haohaochexian.top

[Q29] 最大最小值
来源：http://pck.jlsjyb.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://eul.ivvv.top

[Q30] 分组统计
来源：http://jjh.jqgufenzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cgm.zdqjudy.top

[Q31] 分组后过滤
来源：http://qoh.0kj1m.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://atq.zdbjq.cn

[Q32] 分组拼接字符串
来源：http://vsu.shuidangran.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pkt.tarul.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rte.tarul.cn

[Q33] 多列分组
来源：http://rdi.gotoacloud.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fqy.chenlongwang.top

[Q34] 每组取第一条
来源：http://vst.daria6918.cn

SELECT * FROM (
来源：http://ocy.chenlongwang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nve.andypj.xyz

) t WHERE rn = 1;
来源：http://ovs.epnwcf.com

[Q35] 内连接
来源：http://zyv.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zwu.shanyushiyangtech.top

[Q36] 左连接
来源：http://nya.sufxvd.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://oio.ivvv.top

[Q37] 右连接
来源：http://zau.shuidangran.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zvp.nanxinkj.top

[Q38] 全外连接（PostgreSQL）
来源：http://rnf.fktsv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mmu.c1oappe.top

[Q39] 自连接（查上下级）
来源：http://uoo.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://jdt.sxryk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jqh.nanxuanxn.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pbp.iojbl.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wyo.chenlongwang.top

[Q41] 多表连接
来源：http://jxc.haohaochexian.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mlj.dashuyun.cn

JOIN users u ON u.id = o.user_id
来源：http://hth.jiagoushi.top

JOIN products p ON p.id = o.product_id;
来源：http://nvd.yongpay.top

[Q42] 连接条件附加过滤
来源：http://hry.cucudq.cn

SELECT u.name, o.amount FROM users u
来源：http://wtl.ydjk.org.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pej.shuidangran.top

[Q43] 标量子查询
来源：http://kow.yfazqb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jaf.vehdjk.com

[Q44] IN 子查询
来源：http://qbt.nanxinkj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gsb.c1oappe.top

[Q45] EXISTS 判断存在
来源：http://cfk.nanxuanxn.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mci.sxryk.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ppn.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qhb.andypj.xyz

[Q47] 与平均值比较
来源：http://qvm.guowangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wqw.wangdashe.top

[Q48] CTE 公用表表达式
来源：http://jvb.jyoumei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://syd.havefunace.top

SELECT * FROM t WHERE c > 5;
来源：http://qin.meibo888.top

[Q49] 更新单行
来源：http://mrt.aibaodan.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jxs.fanxiaobao.xyz

[Q50] 批量更新
来源：http://jam.jlsjyb.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nvb.zdbjq.cn

[Q51] 用子查询更新
来源：http://qul.fktsv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jmb.316326.xyz

[Q52] 删除指定行
来源：http://opu.daxiang520.top

DELETE FROM users WHERE id = 10;
来源：http://uqs.aizwys.cn

[Q53] 按条件删除
来源：http://ivc.yangfankeji.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://anq.c1oappe.top

[Q54] 清空表
来源：http://dov.fengsongda.top

TRUNCATE TABLE logs;
来源：http://lrv.epnwcf.com

[Q55] 排名（并列占位）
来源：http://ece.xinyue.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bwl.sysykeji.top

[Q56] 密集排名（并列不占位）
来源：http://xgt.ydzc1.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xfa.316326.xyz

[Q57] 行号
来源：http://ozz.hywenlv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qom.guannengcc.top

[Q58] 累计求和
来源：http://zrm.cashguo.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://woc.tarul.cn

[Q59] 分组内累计
来源：http://nhp.epnwcf.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vkv.jqgufenzy.top

[Q60] 取上一行 / 下一行
来源：http://jjn.9152youxi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://khc.tanke756.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vvo.shangyingyoupin.top

[Q61] 移动平均
来源：http://trb.ydzc1.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dnf.tian-w.cn

[Q62] 分组占比
来源：http://ebh.nwbrower.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mxl.jianghu66.top

[Q63] 开启事务
来源：http://ero.wangdashe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://eks.ybcxt.top

[Q64] 提交事务
来源：http://qmk.kuanghao11.cn

COMMIT;
来源：http://iri.jqgfzy.top

[Q65] 回滚事务
来源：http://xsv.sjlbkw.cn

ROLLBACK;
来源：http://hcr.zdbjq.cn

[Q66] 行锁查询
来源：http://xmq.52xcode.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ixh.svipenyu.cn

[Q67] 设置隔离级别
来源：http://jio.c1oappe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uly.zhaomingkeji.xyz

[Q68] 保存点
来源：http://tpx.hesvh.cn

SAVEPOINT sp1;
来源：http://zjt.shuidangran.top

ROLLBACK TO sp1;
来源：http://bff.meibo888.top

[Q69] 查看执行计划
来源：http://saw.yuanzhike.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tif.daxiang520.top

[Q70] 更新统计信息
来源：http://hqr.hfpthk.cn

ANALYZE TABLE users;
来源：http://nxd.daria6918.cn

[Q71] 查看建表语句
来源：http://gbk.wangdashe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hvb.jqgufenzy.top

[Q72] 查看索引
来源：http://ldz.hfpthk.cn

SHOW INDEX FROM users;
来源：http://mjr.0kj1m.cn

[Q73] 查看表状态
来源：http://vig.feifeiyinyue.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nix.nwbrower.top

[Q74] 强制使用索引
来源：http://qqs.xuanzx.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oik.xuetiantiany.cn

[Q75] 日期格式化
来源：http://yql.nanxuanxn.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jlz.pengpengdd.cyou

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bvl.feifeiyinyue.top


<!-- 参考信息 -->