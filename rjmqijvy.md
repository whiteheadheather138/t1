代发 wailian999

================================================================================
来源：http://stx.bbcook.cn

O. 并发与异步
来源：http://zqr.chenjidiqi.icu

================================================================================
来源：http://ndj.0kj1m.cn

[O01] 启动一个线程
来源：http://uva.gogol.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jno.haohaochexian.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yhj.chenjidiqi.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lup.xuetiantiany.cn

TS:   // 同 JS
来源：http://iqe.ywan-chungtsiang.top

Java: new Thread(() -> f()).start()
来源：http://jdg.shanyushiyangkeji.top

Go:   go f()
来源：http://whu.jinghuilouyu.cn

Ruby: Thread.new { f }
来源：http://zrq.chenzaomai.com

C#:   Task.Run(() => F());
来源：http://ltb.0kj1m.cn

[O02] 使用线程池
来源：http://jfn.yj20258888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lqi.xinyue.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ycs.316326.xyz

JS:   // worker_threads 线程池
来源：http://rks.ivvv.top

TS:   // worker_threads 线程池
来源：http://iet.sufxvd.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ish.xziqi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zei.pengpengdd.cyou

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sno.meibo888.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ajr.yanxiufei.cn

[O03] 加锁保护共享数据
来源：http://gkq.tianlin.xyz

Py:   with lock: shared += 1
来源：http://mkx.ybcxt.top

PHP:  // 用 flock() 做文件锁
来源：http://gmm.hysaishi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lqe.hesvh.cn

TS:   // 同 JS
来源：http://fdu.fehbvm.com

Java: synchronized (this) { shared++; }
来源：http://bhc.gogol.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vzs.cashguo.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://aqo.hnxiangtu.top

C#:   lock (gate) { shared++; }
来源：http://hks.fktsv.cn

[O04] 定义异步函数并等待
来源：http://zuw.shangyingyoupin.top

Py:   async def f():⏎    await g()
来源：http://bly.vehdjk.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zwy.zycfv.cn

JS:   async function f() { await g(); }
来源：http://cak.sxryk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vuh.ctjpmb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sfy.52xcode.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zrk.yj20258.top

Ruby: # 用 Fiber 或 async gem
来源：http://hff.xylfe.cn

C#:   async Task F() { await G(); }
来源：http://spg.ppjwa.cn

[O05] 并发执行并等待全部完成
来源：http://zke.haohaochexian.top

Py:   asyncio.gather(*tasks)
来源：http://azl.mhx1999.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fmu.tarul.cn

JS:   await Promise.all(tasks)
来源：http://dki.zhoulong.xyz

TS:   await Promise.all(tasks)
来源：http://tul.cdnleiting.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rfq.shzxlz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ddb.yueranfly.top

Ruby: threads.map(&:join)
来源：http://yql.gaohongyu789.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pfv.zhoulong.xyz

[O06] 使用进程池
来源：http://wxb.xziqi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cey.chenlongwang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jwd.epnwcf.com

JS:   // child_process / cluster 模块
来源：http://mbk.hcnkem.com

TS:   // child_process / cluster 模块
来源：http://wdv.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kwh.fehbvm.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uqz.zhoulong.xyz

Ruby: // fork 块
来源：http://rmc.fzhhl.top

C#:   Parallel.For
来源：http://sin.hfpthk.cn

================================================================================
来源：http://wpf.zhixingplan.top

P. 常用工具函数
来源：http://ycf.xuanzx.com

================================================================================
来源：http://oig.iojbl.cn

[P01] 生成 UUID
来源：http://szm.fengsongda.top

Py:   str(uuid.uuid4())
来源：http://zco.nwbrower.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kpa.daria6918.cn

JS:   crypto.randomUUID()
来源：http://mnh.hesvh.cn

TS:   crypto.randomUUID()
来源：http://ltg.316326.xyz

Java: UUID.randomUUID().toString()
来源：http://zvm.yj20258888.top

Go:   // 用 github.com/google/uuid
来源：http://msj.sxryk.cn

Ruby: SecureRandom.uuid
来源：http://mbz.0kj1m.cn

C#:   Guid.NewGuid().ToString()
来源：http://phr.smart0.xyz

[P02] MD5 / SHA256 摘要
来源：http://shc.sufxvd.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lab.xingfuxueyuan.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://eup.jqgufenzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lvq.hcnkem.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vsr.gotoacloud.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://eho.guannengcc.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sst.0kj1m.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cfy.smart0.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jyh.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://ukv.hysaishi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pjq.52xcode.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hgj.ivvv.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yrb.jinghuilouyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hco.birdmap.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lnq.tanke756.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://syr.quarkkingdee.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://nqv.ctjpmb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://seg.gogol.net.cn

[P04] 求长度
来源：http://wsw.meibo888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ese.jinyuanbaomall.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://inb.ybcxt.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://muf.tarul.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gcx.aizwys.cn

Java: list.size();  map.size();  s.length()
来源：http://jaf.cqqwz.cn

Go:   len(arr);  len(m)
来源：http://hdv.hnqzz.top

Ruby: x.length;  x.size
来源：http://ppa.jinqigufen.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xtq.daxiang520.top

[P05] 判断两个对象内容是否相等
来源：http://tbh.fengsongda.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://laz.shanyushiyangtech.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dog.smart0.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://axk.nanxuanxn.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://byq.feifeiyinyue.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tvu.fzhhl.top

Go:   reflect.DeepEqual(a, b)
来源：http://igk.mhx1999.top

Ruby: a == b
来源：http://mwk.jinyuanbaomall.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://izi.jlsjyb.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vfe.aibaodan.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dru.xylfe.cn

PHP:  if (empty($x)) {}
来源：http://wwi.zhiwuduotai.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iot.yj20258.top

TS:   if (x == null) {}
来源：http://gqq.nanxuanxn.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hps.jqgfzy.top

Go:   if x == nil {}
来源：http://emd.cucudq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blu.svipenyu.cn

C#:   if (x is null) {}
来源：http://upm.jqgufenzy.top

[P07] 防抖与节流
来源：http://vxn.daria6918.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://taj.haohaochexian.top

PHP:  // 手写时间戳比较
来源：http://zcg.bbcook.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xaa.mhx1999.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sct.jiagoushi.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ycn.cqqwz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xad.feifeiyinyue.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qda.zycfv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fre.ybcxt.top

[P08] 处理浮点精度问题
来源：http://jgf.cqqwz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mdr.shzxlz.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jnd.yanxiufei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://asp.aizwys.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jrw.yongpay.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kkv.zdbjq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ikb.ppjwa.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://esw.shanyushiyangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mqw.cucudq.cn

================================================================================
来源：http://dbv.cheryme.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lsd.smart0.xyz

================================================================================
来源：http://vlp.hongshengwenyu.top

[Q01] 创建表
来源：http://hpo.jinyuanbaomall.cn

CREATE TABLE users (
来源：http://gcd.yueranfly.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tdk.hnxiangtu.top

name VARCHAR(50) NOT NULL,
来源：http://sem.zhijiandao.cn

email VARCHAR(100) UNIQUE,
来源：http://lri.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qgf.hnxiangtu.top

);
来源：http://fif.hcnkem.com

[Q02] 创建带外键的表
来源：http://luf.cheryme.top

CREATE TABLE orders (
来源：http://rtx.xziqi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://goc.hongshengwenyu.top

user_id INT NOT NULL,
来源：http://xio.jyoumei.cn

amount DECIMAL(10, 2),
来源：http://toy.nanxinkj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bjh.yongpay.top

);
来源：http://uaf.hnxiangtu.top

[Q03] 增加列
来源：http://wte.jlsjyb.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rka.svipenyu.cn

[Q04] 修改列类型
来源：http://nus.pengpengdd.cyou

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ohq.zdbjq.cn

[Q05] 重命名列
来源：http://chy.jqgufenzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dhv.xuanzx.com

[Q06] 删除列
来源：http://tqu.haohaochexian.top

ALTER TABLE users DROP COLUMN age;
来源：http://isq.kuanghao11.cn

[Q07] 删除表
来源：http://atc.zhixingplan.top

DROP TABLE IF EXISTS orders;
来源：http://ifl.sxryk.cn

[Q08] 创建普通索引
来源：http://xsa.zhixingplan.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gar.hnqzz.top

[Q09] 创建唯一索引
来源：http://wir.bbcook.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lcd.zhongyouzk.top

[Q10] 插入单行
来源：http://ykg.tianlin.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lun.pycfn.com

[Q11] 一次插入多行
来源：http://oxj.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fkm.epnwcf.com

[Q12] 插入后取自增 ID
来源：http://gul.jinqigfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://qqx.havefunace.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fph.shanyushiyangtech.top

[Q13] 忽略重复插入
来源：http://qru.hnxiangtu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://txo.zhengqikj.top

[Q14] 存在则更新（upsert）
来源：http://xgs.yfazqb.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nia.yanxiufei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qcy.fzhhl.top

[Q15] 查询全部
来源：http://qzh.cucudq.cn

SELECT * FROM users;
来源：http://tjr.shanyushiyangtech.top

[Q16] 查询指定列
来源：http://zgg.epnwcf.com

SELECT id, name FROM users;
来源：http://mij.gzhubu.top

[Q17] 条件查询
来源：http://pio.vqdsnc.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://anu.jinghuilouyu.cn

[Q18] 模糊匹配
来源：http://pnp.fzhhl.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pgm.andypj.xyz

[Q19] 范围查询
来源：http://bci.xziqi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qum.gotoacloud.top

[Q20] IN 列表
来源：http://dyk.xylfe.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jby.nanxuanxn.top

[Q21] 空值判断
来源：http://ppx.nanxuanxn.top

SELECT * FROM users WHERE email IS NULL;
来源：http://cib.aizwys.cn

[Q22] 排序
来源：http://vdm.tian-w.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pyk.xuanzx.com

[Q23] 分页
来源：http://mks.haohaochexian.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tzo.ywan-chungtsiang.top

[Q24] 去重
来源：http://fuk.wangdashe.top

SELECT DISTINCT city FROM users;
来源：http://msy.hongshengwenyu.top

[Q25] 只取前 N 条
来源：http://cqn.mhx1999.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cwl.yongpay.top

[Q26] 计数
来源：http://jkz.316326.xyz

SELECT COUNT(*) FROM users;
来源：http://bof.sweek.top

[Q27] 条件计数
来源：http://gai.wangdashe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hvw.fengsongda.top

[Q28] 求和与平均
来源：http://kri.0kj1m.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yme.gogol.net.cn

[Q29] 最大最小值
来源：http://viv.sufxvd.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ycz.wangshuangyany.cn

[Q30] 分组统计
来源：http://wtj.yanxiufei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iea.hnqzz.top

[Q31] 分组后过滤
来源：http://rmb.yj20258.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dke.sjlbkw.cn

[Q32] 分组拼接字符串
来源：http://crs.tarul.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zre.sufxvd.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zms.hysaishi.cn

[Q33] 多列分组
来源：http://odk.zdbjq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wii.xuetiantiany.cn

[Q34] 每组取第一条
来源：http://mog.birdmap.top

SELECT * FROM (
来源：http://cdz.zdbjq.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dhs.jiagoushi.top

) t WHERE rn = 1;
来源：http://lnl.zhongyouzk.top

[Q35] 内连接
来源：http://ude.wangdashe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oty.shanyushiyangkeji.top

[Q36] 左连接
来源：http://xtg.meibo888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zfq.hysaishi.cn

[Q37] 右连接
来源：http://uqf.vqdsnc.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xsv.jianghu66.top

[Q38] 全外连接（PostgreSQL）
来源：http://vwp.quarkkingdee.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zdk.tanke756.top

[Q39] 自连接（查上下级）
来源：http://xku.kuanghao11.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fjq.xziqi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fgp.nwbrower.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hri.meibo888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gzr.zhijiandao.cn

[Q41] 多表连接
来源：http://lrq.hammf.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dhl.yangfankeji.com

JOIN users u ON u.id = o.user_id
来源：http://nnv.tarul.cn

JOIN products p ON p.id = o.product_id;
来源：http://glz.yangfankeji.com

[Q42] 连接条件附加过滤
来源：http://zmo.chenjidiqi.icu

SELECT u.name, o.amount FROM users u
来源：http://ecy.yonumen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://amx.chenzaomai.com

[Q43] 标量子查询
来源：http://qsm.shzxlz.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yio.jinqigufen.top

[Q44] IN 子查询
来源：http://yvc.jyoumei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://azq.feifeiyinyue.top

[Q45] EXISTS 判断存在
来源：http://cao.nwbrower.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wnx.daxiang520.top

[Q46] NOT EXISTS 判断不存在
来源：http://uop.yueranfly.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qzn.tian-w.cn

[Q47] 与平均值比较
来源：http://mjw.jinghuilouyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://owm.tianlin.xyz

[Q48] CTE 公用表表达式
来源：http://zdc.zhijiandao.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://elu.cheryme.top

SELECT * FROM t WHERE c > 5;
来源：http://mkj.wangshuangyany.cn

[Q49] 更新单行
来源：http://epe.yj202588.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://muu.sufxvd.cn

[Q50] 批量更新
来源：http://ffs.cashguo.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://czd.ehwqpu.com

[Q51] 用子查询更新
来源：http://kse.jianghu66.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dly.yfazqb.com

[Q52] 删除指定行
来源：http://khy.gogol.net.cn

DELETE FROM users WHERE id = 10;
来源：http://lxj.kuanghao11.cn

[Q53] 按条件删除
来源：http://dcv.jqgfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rdp.cucudq.cn

[Q54] 清空表
来源：http://mle.nwbrower.top

TRUNCATE TABLE logs;
来源：http://ivu.cheryme.top

[Q55] 排名（并列占位）
来源：http://zus.tarul.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qow.gaohongyu789.top

[Q56] 密集排名（并列不占位）
来源：http://lya.ydzc1.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pbq.zhoulong.xyz

[Q57] 行号
来源：http://agk.bbcook.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sar.nwbrower.top

[Q58] 累计求和
来源：http://avx.havefunace.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bow.ctjpmb.com

[Q59] 分组内累计
来源：http://qju.cashguo.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gms.gaohongyu789.top

[Q60] 取上一行 / 下一行
来源：http://ygz.yonumen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://whp.feifeiyinyue.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://udb.smart0.xyz

[Q61] 移动平均
来源：http://wxq.iojbl.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fdy.smart0.xyz

[Q62] 分组占比
来源：http://uqj.yuxming.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sze.chenjidiqi.icu

[Q63] 开启事务
来源：http://yuv.shangyingyoupin.top

START TRANSACTION;                -- 或 BEGIN
来源：http://uhs.ppjwa.cn

[Q64] 提交事务
来源：http://syc.shuidangran.top

COMMIT;
来源：http://ivj.chenlongwang.top

[Q65] 回滚事务
来源：http://rfk.yueranfly.top

ROLLBACK;
来源：http://qsr.shangyingyoupin.top

[Q66] 行锁查询
来源：http://sgj.zhaomingkeji.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://awc.cucudq.cn

[Q67] 设置隔离级别
来源：http://rwa.yuanzhike.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lur.xylfe.cn

[Q68] 保存点
来源：http://cgm.ivvv.top

SAVEPOINT sp1;
来源：http://tha.zhixingplan.top

ROLLBACK TO sp1;
来源：http://sqx.zhengqikj.top

[Q69] 查看执行计划
来源：http://izz.cheryme.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zdy.sxryk.cn

[Q70] 更新统计信息
来源：http://tdu.bjfxy.top

ANALYZE TABLE users;
来源：http://yhf.daxiang520.top

[Q71] 查看建表语句
来源：http://byo.yongpay.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ipl.meibo888.top

[Q72] 查看索引
来源：http://pih.tianlin.xyz


<!-- 参考信息 -->