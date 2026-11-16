代发 wailian999

TS:   // worker_threads 线程池
来源：http://ouo.hongshengwenyu.top

Java: Executors.newFixedThreadPool(4)
来源：http://fqe.hcnkem.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fwp.sufxvd.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://whp.zhijiandao.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rnb.zhengqikj.top

[O03] 加锁保护共享数据
来源：http://rjl.zdqjudy.top

Py:   with lock: shared += 1
来源：http://yxj.nwbrower.top

PHP:  // 用 flock() 做文件锁
来源：http://mis.xziqi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mlm.jqgufenzy.top

TS:   // 同 JS
来源：http://iej.cheryme.top

Java: synchronized (this) { shared++; }
来源：http://wdd.aizwys.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mgz.yfazqb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://cru.ywan-chungtsiang.top

C#:   lock (gate) { shared++; }
来源：http://moo.fanxiaobao.xyz

[O04] 定义异步函数并等待
来源：http://zbn.shangyingyoupin.top

Py:   async def f():⏎    await g()
来源：http://hmi.zhijiandao.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tif.daxiang520.top

JS:   async function f() { await g(); }
来源：http://cty.xingfuxueyuan.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://unl.zycfv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lhu.vehdjk.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://doe.hesvh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xto.ydjk.org.cn

C#:   async Task F() { await G(); }
来源：http://wfe.jianghu66.top

[O05] 并发执行并等待全部完成
来源：http://ppy.guannengcc.top

Py:   asyncio.gather(*tasks)
来源：http://cos.kuanghao11.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kzh.zhijiandao.cn

JS:   await Promise.all(tasks)
来源：http://hha.sufxvd.cn

TS:   await Promise.all(tasks)
来源：http://gqv.chenjidiqi.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hbu.fzhhl.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kls.yuanzhike.top

Ruby: threads.map(&:join)
来源：http://dqk.jinqigufen.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qzl.chenzaomai.com

[O06] 使用进程池
来源：http://rpq.xuanzx.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wiv.zhongyouzk.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vwv.birdmap.top

JS:   // child_process / cluster 模块
来源：http://vsq.ehwqpu.com

TS:   // child_process / cluster 模块
来源：http://jmx.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mzb.sjlbkw.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://csy.jqgfzy.top

Ruby: // fork 块
来源：http://sty.yuxming.cn

C#:   Parallel.For
来源：http://cwc.c1oappe.top

================================================================================
来源：http://vph.yonumen.top

P. 常用工具函数
来源：http://wsw.hywenlv.cn

================================================================================
来源：http://hbe.daria6918.cn

[P01] 生成 UUID
来源：http://tkx.yanxiufei.cn

Py:   str(uuid.uuid4())
来源：http://qkz.birdmap.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ihc.sweek.top

JS:   crypto.randomUUID()
来源：http://myq.shanyushiyangtech.top

TS:   crypto.randomUUID()
来源：http://qhc.zhiwuduotai.top

Java: UUID.randomUUID().toString()
来源：http://utq.fanxiaobao.xyz

Go:   // 用 github.com/google/uuid
来源：http://hih.fktsv.cn

Ruby: SecureRandom.uuid
来源：http://olh.shanyushiyangtech.top

C#:   Guid.NewGuid().ToString()
来源：http://knv.aibaodan.cn

[P02] MD5 / SHA256 摘要
来源：http://itu.chenjidiqi.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bya.yfazqb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://bet.sysykeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bej.cheryme.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hfm.gzhubu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://txf.gaohongyu789.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ujy.nanxinkj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dsm.sjlbkw.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jba.tian-w.cn

[P03] 生成短随机字符串
来源：http://wkp.yj20258888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://upq.zhengqikj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://alv.yj20258888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zrd.jqgufenzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ewu.fktsv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gir.sxryk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sxy.aibaodan.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kkn.vqdsnc.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yck.zhaomingkeji.xyz

[P04] 求长度
来源：http://yad.cqqwz.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hoa.daria6918.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hfk.zycfv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://emj.shanyushiyangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uta.vehdjk.com

Java: list.size();  map.size();  s.length()
来源：http://wze.nanxuanxn.top

Go:   len(arr);  len(m)
来源：http://dfp.mhx1999.top

Ruby: x.length;  x.size
来源：http://yjk.zycfv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hks.yanxiufei.cn

[P05] 判断两个对象内容是否相等
来源：http://ojw.tanke756.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://asq.redwolf501.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yvj.yj20258.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://svc.yj202588.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jdb.andypj.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zzo.zhijiandao.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gks.bbcook.cn

Ruby: a == b
来源：http://uqx.fktsv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cne.sjlbkw.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jvw.quarkkingdee.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://njt.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://mpw.zhiwuduotai.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xhv.ydjk.org.cn

TS:   if (x == null) {}
来源：http://isx.redwolf501.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wtl.ybcxt.top

Go:   if x == nil {}
来源：http://xpw.yfazqb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hvc.nanxuanxn.top

C#:   if (x is null) {}
来源：http://pli.xylfe.cn

[P07] 防抖与节流
来源：http://wpy.jianghu66.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ndg.ivvv.top

PHP:  // 手写时间戳比较
来源：http://dvj.smart0.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jdr.zhengqikj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://moy.havefunace.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nuw.nanxuanxn.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mld.ppjwa.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fev.xylfe.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://trc.zhengqikj.top

[P08] 处理浮点精度问题
来源：http://sos.ivvv.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mmu.sjlbkw.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gtm.shangyingyoupin.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oci.yangfankeji.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yhr.tianlin.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wdj.hcnkem.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tzd.shanyushiyangkeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kqf.jqgfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://auv.xylfe.cn

================================================================================
来源：http://isn.ydjk.org.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xnj.iojbl.cn

================================================================================
来源：http://mxl.316326.xyz

[Q01] 创建表
来源：http://vlv.gotoacloud.top

CREATE TABLE users (
来源：http://yer.feifeiyinyue.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zuz.yanxiufei.cn

name VARCHAR(50) NOT NULL,
来源：http://dvs.haohaochexian.top

email VARCHAR(100) UNIQUE,
来源：http://qcj.cucudq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bxz.haohaochexian.top

);
来源：http://tmn.zhaomingkeji.xyz

[Q02] 创建带外键的表
来源：http://rxf.smart0.xyz

CREATE TABLE orders (
来源：http://kkr.guannengcc.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qsy.fehbvm.com

user_id INT NOT NULL,
来源：http://pdf.jinyuanbaomall.cn

amount DECIMAL(10, 2),
来源：http://ydl.chenjidiqi.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://oyu.pycfn.com

);
来源：http://czi.gotoacloud.top

[Q03] 增加列
来源：http://vgm.jinqigfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bwg.9152youxi.cn

[Q04] 修改列类型
来源：http://eyy.yueranfly.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pux.meibo888.top

[Q05] 重命名列
来源：http://usj.ybcxt.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yip.zhongyouzk.top

[Q06] 删除列
来源：http://rxj.yvedp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rjk.shzxlz.cn

[Q07] 删除表
来源：http://lmb.yueranfly.top

DROP TABLE IF EXISTS orders;
来源：http://xuu.shanyushiyangtech.top

[Q08] 创建普通索引
来源：http://xvw.uphjek.com

CREATE INDEX idx_users_email ON users(email);
来源：http://uej.9152youxi.cn

[Q09] 创建唯一索引
来源：http://ofb.smart0.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dae.52xcode.cn

[Q10] 插入单行
来源：http://bqu.fktsv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ikx.cqqwz.cn

[Q11] 一次插入多行
来源：http://qnf.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://suz.zdqjudy.top

[Q12] 插入后取自增 ID
来源：http://fve.kuanghao11.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ihb.jinyuanbaomall.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kga.yangfankeji.com

[Q13] 忽略重复插入
来源：http://jtj.xziqi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ixd.xuetiantiany.cn

[Q14] 存在则更新（upsert）
来源：http://auw.zhongyouzk.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ibs.nwbrower.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lqp.xylfe.cn

[Q15] 查询全部
来源：http://zqj.ivvv.top

SELECT * FROM users;
来源：http://duz.yangfankeji.com

[Q16] 查询指定列
来源：http://quy.haohaochexian.top

SELECT id, name FROM users;
来源：http://dyq.pengpengdd.cyou

[Q17] 条件查询
来源：http://bgg.yangfankeji.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://psm.andypj.xyz

[Q18] 模糊匹配
来源：http://upm.zhijiandao.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://brk.fehbvm.com

[Q19] 范围查询
来源：http://ejh.redwolf501.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mak.dianchejie.cn

[Q20] IN 列表
来源：http://lxz.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gkt.hcnkem.com

[Q21] 空值判断
来源：http://kez.316326.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://hjl.hongshengwenyu.top

[Q22] 排序
来源：http://nwy.sjlbkw.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://acu.epnwcf.com

[Q23] 分页
来源：http://eao.ywan-chungtsiang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sqx.hywenlv.cn

[Q24] 去重
来源：http://kth.yuxming.cn

SELECT DISTINCT city FROM users;
来源：http://imk.ctjpmb.com

[Q25] 只取前 N 条
来源：http://efz.uphjek.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rng.dianchejie.cn

[Q26] 计数
来源：http://coe.xingfuxueyuan.xyz

SELECT COUNT(*) FROM users;
来源：http://ocf.sjlbkw.cn

[Q27] 条件计数
来源：http://ivt.bjfxy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sem.ydzc1.top

[Q28] 求和与平均
来源：http://gkv.0kj1m.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ell.zhixingplan.top

[Q29] 最大最小值
来源：http://lwx.yj202588.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ulo.smart0.xyz

[Q30] 分组统计
来源：http://xke.chenlongwang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nxr.jinyuanbaomall.cn

[Q31] 分组后过滤
来源：http://kwu.sufxvd.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dcd.xingfuxueyuan.xyz

[Q32] 分组拼接字符串
来源：http://mud.meibo888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gqx.bjfxy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qqe.cdnleiting.top

[Q33] 多列分组
来源：http://wkb.chenzaomai.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gqf.fanxiaobao.xyz

[Q34] 每组取第一条
来源：http://mdb.zhiwuduotai.top

SELECT * FROM (
来源：http://nfa.cqqwz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cpt.yongpay.top

) t WHERE rn = 1;
来源：http://sar.shangyingyoupin.top

[Q35] 内连接
来源：http://bnq.chenlongwang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tvo.hammf.cn

[Q36] 左连接
来源：http://zpb.zycfv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dbe.zhiwuduotai.top

[Q37] 右连接
来源：http://swc.fzhhl.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://niv.xingfuxueyuan.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://lvt.xingfuxueyuan.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xxk.zhoulong.xyz

[Q39] 自连接（查上下级）
来源：http://vsg.jinghuilouyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zrl.ydjk.org.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zsp.guowangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://khe.ivvv.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bgh.yj202588.top

[Q41] 多表连接
来源：http://jwi.daxiang520.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rwe.zdqjudy.top

JOIN users u ON u.id = o.user_id
来源：http://kmf.jinghuilouyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://kqw.jlsjyb.cn

[Q42] 连接条件附加过滤
来源：http://cmo.daxiang520.top

SELECT u.name, o.amount FROM users u
来源：http://kju.ydjk.org.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bre.nanxuanxn.top

[Q43] 标量子查询
来源：http://owe.tianlin.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hab.ivvv.top

[Q44] IN 子查询
来源：http://sip.hnxiangtu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rtv.hysaishi.cn

[Q45] EXISTS 判断存在
来源：http://ief.ydzc1.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wsl.birdmap.top

[Q46] NOT EXISTS 判断不存在
来源：http://aoe.sysykeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rtp.jqgfzy.top

[Q47] 与平均值比较
来源：http://xkh.chenlongwang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zus.nanxuanxn.top

[Q48] CTE 公用表表达式
来源：http://mgx.52xcode.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pwu.hnxiangtu.top

SELECT * FROM t WHERE c > 5;
来源：http://fnq.zdqjudy.top

[Q49] 更新单行
来源：http://ryp.sufxvd.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://utz.vehdjk.com

[Q50] 批量更新
来源：http://kns.andypj.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kgx.vehdjk.com

[Q51] 用子查询更新
来源：http://czc.jinghuilouyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nwu.wangdashe.top

[Q52] 删除指定行
来源：http://hjv.cqqwz.cn

DELETE FROM users WHERE id = 10;
来源：http://eqx.ywan-chungtsiang.top

[Q53] 按条件删除
来源：http://psv.yanxiufei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qco.shzxlz.cn

[Q54] 清空表
来源：http://cgc.uphjek.com

TRUNCATE TABLE logs;
来源：http://erp.vqdsnc.cn

[Q55] 排名（并列占位）
来源：http://xmi.sysykeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://era.tian-w.cn

[Q56] 密集排名（并列不占位）
来源：http://ama.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rlh.ydjk.org.cn

[Q57] 行号
来源：http://sqv.316326.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oxp.zhengqikj.top

[Q58] 累计求和
来源：http://kuj.cqqwz.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://btl.tianlin.xyz

[Q59] 分组内累计
来源：http://mry.shuidangran.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mel.pycfn.com

[Q60] 取上一行 / 下一行
来源：http://fge.yuxming.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hjj.chenjidiqi.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mxk.cqqwz.cn

[Q61] 移动平均
来源：http://cxk.yanxiufei.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zts.fktsv.cn

[Q62] 分组占比
来源：http://rmk.ctjpmb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mou.hcnkem.com

[Q63] 开启事务
来源：http://dqm.ppjwa.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fyi.cashguo.top

[Q64] 提交事务
来源：http://ioy.yj20258888.top

COMMIT;
来源：http://avy.svipenyu.cn

[Q65] 回滚事务
来源：http://zbw.andypj.xyz

ROLLBACK;
来源：http://kgq.fehbvm.com

[Q66] 行锁查询
来源：http://pwv.ydzc1.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hna.feifeiyinyue.top

[Q67] 设置隔离级别
来源：http://zmb.zdqjudy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uam.yonumen.top

[Q68] 保存点
来源：http://cgj.vqdsnc.cn

SAVEPOINT sp1;
来源：http://wco.316326.xyz

ROLLBACK TO sp1;
来源：http://ygx.hywenlv.cn

[Q69] 查看执行计划
来源：http://oqe.guannengcc.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vmc.yonumen.top

[Q70] 更新统计信息
来源：http://mre.zhaomingkeji.xyz

ANALYZE TABLE users;
来源：http://psh.c1oappe.top

[Q71] 查看建表语句
来源：http://dnr.tian-w.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hjp.vqdsnc.cn

[Q72] 查看索引
来源：http://lie.zhijiandao.cn

SHOW INDEX FROM users;
来源：http://zea.redwolf501.top

[Q73] 查看表状态
来源：http://jql.jianghu66.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xcs.jinqigufen.top

[Q74] 强制使用索引
来源：http://vcq.zdbjq.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://azo.zhixingplan.top

[Q75] 日期格式化
来源：http://mhj.sxryk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ejl.yonumen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uva.sysykeji.top

[Q76] 按天统计
来源：http://mnf.hnqzz.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bru.vehdjk.com

[Q77] 时间加减
来源：http://rmo.smart0.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jkd.ppjwa.cn

[Q78] 当前时间
来源：http://iad.jlsjyb.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://omr.hcnkem.com

[Q79] 字符串拼接
来源：http://eci.svipenyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ufq.nwbrower.top


<!-- 参考信息 -->