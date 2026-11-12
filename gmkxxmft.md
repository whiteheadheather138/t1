代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rfr.svipenyu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qzy.daria6918.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dhk.yanxiufei.cn

TS:   // 同 JS
来源：http://xph.smart0.xyz

Java: new Thread(() -> f()).start()
来源：http://bcc.yueranfly.top

Go:   go f()
来源：http://ykd.hfpthk.cn

Ruby: Thread.new { f }
来源：http://lsf.xuanzx.com

C#:   Task.Run(() => F());
来源：http://ekq.yj202588.top

[O02] 使用线程池
来源：http://enu.chenjidiqi.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tgv.jinqigfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://icb.xziqi.cn

JS:   // worker_threads 线程池
来源：http://tae.jyoumei.cn

TS:   // worker_threads 线程池
来源：http://itt.yj202588.top

Java: Executors.newFixedThreadPool(4)
来源：http://prs.ehwqpu.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ykd.0kj1m.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://khw.jinqigufen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oyj.sysykeji.top

[O03] 加锁保护共享数据
来源：http://eqv.svipenyu.cn

Py:   with lock: shared += 1
来源：http://uuo.quarkkingdee.top

PHP:  // 用 flock() 做文件锁
来源：http://pkz.zhongyouzk.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cns.wangdashe.top

TS:   // 同 JS
来源：http://zok.ivvv.top

Java: synchronized (this) { shared++; }
来源：http://lwc.zhengqikj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rsm.yj20258888.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://sho.sxryk.cn

C#:   lock (gate) { shared++; }
来源：http://dqm.ydjk.org.cn

[O04] 定义异步函数并等待
来源：http://xjg.zhongyouzk.top

Py:   async def f():⏎    await g()
来源：http://quf.hesvh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lcd.yanxiufei.cn

JS:   async function f() { await g(); }
来源：http://vrq.shangyingyoupin.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qjy.yfazqb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://khr.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hjb.hfpthk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kyx.xylfe.cn

C#:   async Task F() { await G(); }
来源：http://sta.zhixingplan.top

[O05] 并发执行并等待全部完成
来源：http://atz.zhiwuduotai.top

Py:   asyncio.gather(*tasks)
来源：http://udg.birdmap.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pjf.hesvh.cn

JS:   await Promise.all(tasks)
来源：http://nmr.gaohongyu789.top

TS:   await Promise.all(tasks)
来源：http://vbg.shzxlz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iur.ywan-chungtsiang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kij.epnwcf.com

Ruby: threads.map(&:join)
来源：http://rro.zhongyouzk.top

C#:   await Task.WhenAll(t1, t2)
来源：http://uaq.hysaishi.cn

[O06] 使用进程池
来源：http://ura.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://esy.pengpengdd.cyou

PHP:  // pcntl_fork 或多进程队列
来源：http://nva.gogol.net.cn

JS:   // child_process / cluster 模块
来源：http://oqm.nanxinkj.top

TS:   // child_process / cluster 模块
来源：http://zgh.gzhubu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dtd.yj202588.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://iqq.gaohongyu789.top

Ruby: // fork 块
来源：http://teo.tarul.cn

C#:   Parallel.For
来源：http://qiv.yfazqb.com

================================================================================
来源：http://vnv.cashguo.top

P. 常用工具函数
来源：http://sjr.yfazqb.com

================================================================================
来源：http://jst.dashuyun.cn

[P01] 生成 UUID
来源：http://mul.andypj.xyz

Py:   str(uuid.uuid4())
来源：http://uuh.jinqigfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rzg.vqdsnc.cn

JS:   crypto.randomUUID()
来源：http://wte.yj202588.top

TS:   crypto.randomUUID()
来源：http://axx.fzhhl.top

Java: UUID.randomUUID().toString()
来源：http://ttg.dashuyun.cn

Go:   // 用 github.com/google/uuid
来源：http://yri.ehwqpu.com

Ruby: SecureRandom.uuid
来源：http://drt.dashuyun.cn

C#:   Guid.NewGuid().ToString()
来源：http://oke.hnxiangtu.top

[P02] MD5 / SHA256 摘要
来源：http://dnq.yuxming.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://smn.zhongyouzk.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://kha.ydzc1.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uku.cqqwz.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aul.ydzc1.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jlz.quarkkingdee.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nqq.zhijiandao.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zkx.hammf.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://roo.chenjidiqi.icu

[P03] 生成短随机字符串
来源：http://fqj.andypj.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kxe.yj202588.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ese.guannengcc.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dxb.jianghu66.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pkh.nanxinkj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xll.andypj.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kfk.guannengcc.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://oeh.sjlbkw.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://amv.cdnleiting.top

[P04] 求长度
来源：http://mxu.fanxiaobao.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uud.gzhubu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lhj.yongpay.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aic.feifeiyinyue.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kme.316326.xyz

Java: list.size();  map.size();  s.length()
来源：http://viw.ybcxt.top

Go:   len(arr);  len(m)
来源：http://igm.snrcjt.cn

Ruby: x.length;  x.size
来源：http://glb.shuidangran.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fky.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://ypw.fehbvm.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://axr.gzhubu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ysw.zhengqikj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tnt.xuetiantiany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bhz.xziqi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://slg.zhaomingkeji.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://upv.yanxiufei.cn

Ruby: a == b
来源：http://ufo.yj202588.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://acr.aibaodan.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wio.sxryk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wbe.pengpengdd.cyou

PHP:  if (empty($x)) {}
来源：http://mzy.aizwys.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kfo.zdqjudy.top

TS:   if (x == null) {}
来源：http://qmm.meibo888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wku.jqgufenzy.top

Go:   if x == nil {}
来源：http://hat.tarul.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bjp.yvedp.cn

C#:   if (x is null) {}
来源：http://sma.dashuyun.cn

[P07] 防抖与节流
来源：http://trx.hnxiangtu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cfq.shanyushiyangkeji.top

PHP:  // 手写时间戳比较
来源：http://ebr.aizwys.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pmv.ywan-chungtsiang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xri.jinghuilouyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cpw.316326.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rch.ppjwa.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dzw.zhixingplan.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yjm.cqqwz.cn

[P08] 处理浮点精度问题
来源：http://zsi.uphjek.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mtz.dianchejie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rnz.hammf.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ylr.xingfuxueyuan.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vtz.cashguo.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mqx.ehwqpu.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hxs.zhijiandao.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zca.bjfxy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yto.vehdjk.com

================================================================================
来源：http://jiz.vqdsnc.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ulr.daxiang520.top

================================================================================
来源：http://hoc.zhixingplan.top

[Q01] 创建表
来源：http://ilf.shanyushiyangkeji.top

CREATE TABLE users (
来源：http://avr.haohaochexian.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zuu.shangyingyoupin.top

name VARCHAR(50) NOT NULL,
来源：http://ysc.wangdashe.top

email VARCHAR(100) UNIQUE,
来源：http://yqe.jyoumei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sqk.guannengcc.top

);
来源：http://ugv.nwbrower.top

[Q02] 创建带外键的表
来源：http://kpk.sxryk.cn

CREATE TABLE orders (
来源：http://wdl.fanxiaobao.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://abg.birdmap.top

user_id INT NOT NULL,
来源：http://gus.yonumen.top

amount DECIMAL(10, 2),
来源：http://nwe.svipenyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fuh.cdnleiting.top

);
来源：http://dvb.jqgufenzy.top

[Q03] 增加列
来源：http://hso.svipenyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://atu.cheryme.top

[Q04] 修改列类型
来源：http://tqq.ydzc1.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://owb.xinyue.icu

[Q05] 重命名列
来源：http://amm.epnwcf.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ckw.haohaochexian.top

[Q06] 删除列
来源：http://gck.daria6918.cn

ALTER TABLE users DROP COLUMN age;
来源：http://egi.iojbl.cn

[Q07] 删除表
来源：http://zqr.fktsv.cn

DROP TABLE IF EXISTS orders;
来源：http://ujw.zhaomingkeji.xyz

[Q08] 创建普通索引
来源：http://iom.xingfuxueyuan.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://crv.tarul.cn

[Q09] 创建唯一索引
来源：http://cxk.dianchejie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://imo.aibaodan.cn

[Q10] 插入单行
来源：http://rsi.epnwcf.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oeg.yuxming.cn

[Q11] 一次插入多行
来源：http://riw.yongpay.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cyn.shuidangran.top

[Q12] 插入后取自增 ID
来源：http://jrv.hywenlv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://efp.bbcook.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nzj.jinyuanbaomall.cn

[Q13] 忽略重复插入
来源：http://fdm.havefunace.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gci.uphjek.com

[Q14] 存在则更新（upsert）
来源：http://ibz.zhiwuduotai.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tvg.fzhhl.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://btw.hnqzz.top

[Q15] 查询全部
来源：http://vqb.zhijiandao.cn

SELECT * FROM users;
来源：http://xzz.cheryme.top

[Q16] 查询指定列
来源：http://nsx.shanyushiyangtech.top

SELECT id, name FROM users;
来源：http://evm.hfpthk.cn

[Q17] 条件查询
来源：http://jrj.vqdsnc.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kbt.wangdashe.top

[Q18] 模糊匹配
来源：http://zcv.52xcode.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wwg.0kj1m.cn

[Q19] 范围查询
来源：http://pmh.cashguo.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kzf.jlsjyb.cn

[Q20] IN 列表
来源：http://qma.hesvh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bja.daria6918.cn

[Q21] 空值判断
来源：http://dhc.sjlbkw.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hpi.9152youxi.cn

[Q22] 排序
来源：http://kov.hysaishi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zup.uphjek.com

[Q23] 分页
来源：http://fvo.hywenlv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dvr.fengsongda.top

[Q24] 去重
来源：http://esv.ydjk.org.cn

SELECT DISTINCT city FROM users;
来源：http://hud.daria6918.cn

[Q25] 只取前 N 条
来源：http://wca.c1oappe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hpj.shanyushiyangkeji.top

[Q26] 计数
来源：http://yqr.hnxiangtu.top

SELECT COUNT(*) FROM users;
来源：http://dtw.vqdsnc.cn

[Q27] 条件计数
来源：http://oeu.xinyue.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lfd.gotoacloud.top

[Q28] 求和与平均
来源：http://nsf.epnwcf.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wsu.yueranfly.top

[Q29] 最大最小值
来源：http://iwn.xuetiantiany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://par.fanxiaobao.xyz

[Q30] 分组统计
来源：http://xjk.chenzaomai.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://grm.fanxiaobao.xyz

[Q31] 分组后过滤
来源：http://ztx.yueranfly.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wke.bbcook.cn

[Q32] 分组拼接字符串
来源：http://kue.ivvv.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mwc.jinqigfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://foz.epnwcf.com

[Q33] 多列分组
来源：http://mxm.cqqwz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dzx.xylfe.cn

[Q34] 每组取第一条
来源：http://bpi.ivvv.top

SELECT * FROM (
来源：http://vgj.jinyuanbaomall.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vpv.zhiwuduotai.top

) t WHERE rn = 1;
来源：http://std.kuanghao11.cn

[Q35] 内连接
来源：http://tln.ivvv.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xof.shanyushiyangkeji.top

[Q36] 左连接
来源：http://uum.yuxming.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uoj.zhijiandao.cn

[Q37] 右连接
来源：http://kvt.kuanghao11.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iei.shzxlz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://swj.bjfxy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zmm.meibo888.top

[Q39] 自连接（查上下级）
来源：http://hch.jianghu66.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://iku.aizwys.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nob.wangdashe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://awy.dianchejie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mna.smart0.xyz

[Q41] 多表连接
来源：http://ovz.sjlbkw.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jfh.jyoumei.cn

JOIN users u ON u.id = o.user_id
来源：http://gzp.sufxvd.cn

JOIN products p ON p.id = o.product_id;
来源：http://zle.hfpthk.cn

[Q42] 连接条件附加过滤
来源：http://gge.cashguo.top

SELECT u.name, o.amount FROM users u
来源：http://udm.jlsjyb.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://onk.yanxiufei.cn

[Q43] 标量子查询
来源：http://ovx.jqgfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://aeb.epnwcf.com

[Q44] IN 子查询
来源：http://zye.yongpay.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ewt.uphjek.com

[Q45] EXISTS 判断存在
来源：http://rbd.chenzaomai.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jkt.feifeiyinyue.top

[Q46] NOT EXISTS 判断不存在
来源：http://yix.hongshengwenyu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hyq.yfazqb.com

[Q47] 与平均值比较
来源：http://jui.hysaishi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rwf.meibo888.top

[Q48] CTE 公用表表达式
来源：http://bux.sjlbkw.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zxr.hnqzz.top

SELECT * FROM t WHERE c > 5;
来源：http://dgi.c1oappe.top

[Q49] 更新单行
来源：http://fre.cqqwz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lwf.kuanghao11.cn

[Q50] 批量更新
来源：http://ddn.pengpengdd.cyou

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fmc.xuanzx.com

[Q51] 用子查询更新
来源：http://wtz.ehwqpu.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://epa.zdbjq.cn

[Q52] 删除指定行
来源：http://dfh.tianlin.xyz

DELETE FROM users WHERE id = 10;
来源：http://lnd.zdqjudy.top

[Q53] 按条件删除
来源：http://myo.yfazqb.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://urd.chenzaomai.com

[Q54] 清空表
来源：http://ivc.redwolf501.top

TRUNCATE TABLE logs;
来源：http://uym.cashguo.top

[Q55] 排名（并列占位）
来源：http://gjl.jlsjyb.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dnz.sysykeji.top

[Q56] 密集排名（并列不占位）
来源：http://csj.xingfuxueyuan.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kmi.zycfv.cn

[Q57] 行号
来源：http://tzh.yj20258888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://edh.zycfv.cn

[Q58] 累计求和
来源：http://sit.yuanzhike.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mqk.fzhhl.top

[Q59] 分组内累计
来源：http://wls.shanyushiyangtech.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fye.gaohongyu789.top

[Q60] 取上一行 / 下一行
来源：http://uzz.jinghuilouyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rlj.hcnkem.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sft.sweek.top

[Q61] 移动平均
来源：http://msp.zdbjq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qes.zhiwuduotai.top

[Q62] 分组占比
来源：http://sry.epnwcf.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jeb.kuanghao11.cn

[Q63] 开启事务
来源：http://cfx.feifeiyinyue.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qst.tarul.cn

[Q64] 提交事务
来源：http://npa.fehbvm.com

COMMIT;
来源：http://oto.yangfankeji.com

[Q65] 回滚事务
来源：http://tly.fehbvm.com

ROLLBACK;
来源：http://knr.smart0.xyz

[Q66] 行锁查询
来源：http://rag.ydjk.org.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kni.fengsongda.top

[Q67] 设置隔离级别
来源：http://pmo.guowangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wpp.jqgufenzy.top

[Q68] 保存点
来源：http://cvc.bjfxy.top

SAVEPOINT sp1;
来源：http://ozl.ydzc1.top

ROLLBACK TO sp1;
来源：http://fsh.xziqi.cn

[Q69] 查看执行计划
来源：http://osd.gotoacloud.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rtx.xylfe.cn

[Q70] 更新统计信息
来源：http://qvf.aibaodan.cn

ANALYZE TABLE users;
来源：http://fah.yongpay.top

[Q71] 查看建表语句
来源：http://etf.c1oappe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eyl.vqdsnc.cn

[Q72] 查看索引
来源：http://pig.kuanghao11.cn

SHOW INDEX FROM users;
来源：http://fgu.bbcook.cn

[Q73] 查看表状态
来源：http://erz.jinqigufen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tiz.zhongyouzk.top

[Q74] 强制使用索引
来源：http://ild.feifeiyinyue.top


<!-- 参考信息 -->