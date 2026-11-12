代发 wailian999

================================================================================
来源：http://smu.hywenlv.cn

O. 并发与异步
来源：http://asw.kuanghao11.cn

================================================================================
来源：http://prk.jinghuilouyu.cn

[O01] 启动一个线程
来源：http://pvs.gogol.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mqk.ydzc1.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hoa.cheryme.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tbz.zycfv.cn

TS:   // 同 JS
来源：http://lyc.tian-w.cn

Java: new Thread(() -> f()).start()
来源：http://rco.zhixingplan.top

Go:   go f()
来源：http://atl.redwolf501.top

Ruby: Thread.new { f }
来源：http://xnd.yfazqb.com

C#:   Task.Run(() => F());
来源：http://amf.xylfe.cn

[O02] 使用线程池
来源：http://tzb.yuxming.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lta.cqqwz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kqp.gogol.net.cn

JS:   // worker_threads 线程池
来源：http://zkv.hnqzz.top

TS:   // worker_threads 线程池
来源：http://bve.aizwys.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vsy.jinqigfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ujm.yangfankeji.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sdh.ydzc1.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tzh.feifeiyinyue.top

[O03] 加锁保护共享数据
来源：http://aev.aibaodan.cn

Py:   with lock: shared += 1
来源：http://cob.cheryme.top

PHP:  // 用 flock() 做文件锁
来源：http://lql.jinqigfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xnx.xylfe.cn

TS:   // 同 JS
来源：http://fwo.gotoacloud.top

Java: synchronized (this) { shared++; }
来源：http://nnm.andypj.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://urc.svipenyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fii.shangyingyoupin.top

C#:   lock (gate) { shared++; }
来源：http://nhi.fzhhl.top

[O04] 定义异步函数并等待
来源：http://hvx.fengsongda.top

Py:   async def f():⏎    await g()
来源：http://ipj.uphjek.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ebc.hammf.cn

JS:   async function f() { await g(); }
来源：http://eyt.shzxlz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xej.yuxming.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bnr.yangfankeji.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://myv.quarkkingdee.top

Ruby: # 用 Fiber 或 async gem
来源：http://kjv.svipenyu.cn

C#:   async Task F() { await G(); }
来源：http://kbp.sjlbkw.cn

[O05] 并发执行并等待全部完成
来源：http://gtn.birdmap.top

Py:   asyncio.gather(*tasks)
来源：http://aim.shzxlz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nog.hysaishi.cn

JS:   await Promise.all(tasks)
来源：http://uji.xuanzx.com

TS:   await Promise.all(tasks)
来源：http://vnh.jyoumei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fyc.ydjk.org.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zui.jlsjyb.cn

Ruby: threads.map(&:join)
来源：http://mpb.hnxiangtu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://klt.bbcook.cn

[O06] 使用进程池
来源：http://djg.xuetiantiany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qza.ctjpmb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://asr.nanxinkj.top

JS:   // child_process / cluster 模块
来源：http://xgl.yonumen.top

TS:   // child_process / cluster 模块
来源：http://owx.xylfe.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zhh.jqgfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zuq.vehdjk.com

Ruby: // fork 块
来源：http://lfl.9152youxi.cn

C#:   Parallel.For
来源：http://jqr.zhijiandao.cn

================================================================================
来源：http://zyn.pycfn.com

P. 常用工具函数
来源：http://bni.yanxiufei.cn

================================================================================
来源：http://prs.epnwcf.com

[P01] 生成 UUID
来源：http://fjc.hywenlv.cn

Py:   str(uuid.uuid4())
来源：http://eyd.jqgufenzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hwz.daria6918.cn

JS:   crypto.randomUUID()
来源：http://zmi.wangdashe.top

TS:   crypto.randomUUID()
来源：http://zxq.sxryk.cn

Java: UUID.randomUUID().toString()
来源：http://kpq.xuanzx.com

Go:   // 用 github.com/google/uuid
来源：http://tpe.iojbl.cn

Ruby: SecureRandom.uuid
来源：http://pki.iojbl.cn

C#:   Guid.NewGuid().ToString()
来源：http://est.gaohongyu789.top

[P02] MD5 / SHA256 摘要
来源：http://ubt.hnqzz.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wdq.hnxiangtu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zha.shanyushiyangkeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ful.bbcook.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dlb.chenzaomai.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://neb.chenzaomai.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://aax.gogol.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yup.zhijiandao.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lez.jiagoushi.top

[P03] 生成短随机字符串
来源：http://ewk.redwolf501.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fsj.jinyuanbaomall.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bsz.52xcode.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qdo.yueranfly.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tam.chenzaomai.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gzu.zdbjq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zoe.chenlongwang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ycx.sjlbkw.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xbt.dashuyun.cn

[P04] 求长度
来源：http://czd.shanyushiyangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ifs.cheryme.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gzk.ydjk.org.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dnr.vehdjk.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uui.fehbvm.com

Java: list.size();  map.size();  s.length()
来源：http://aui.haohaochexian.top

Go:   len(arr);  len(m)
来源：http://jxk.quarkkingdee.top

Ruby: x.length;  x.size
来源：http://cdk.ywan-chungtsiang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bjw.jqgfzy.top

[P05] 判断两个对象内容是否相等
来源：http://irc.fanxiaobao.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://ejo.fzhhl.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dcc.epnwcf.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://axh.snrcjt.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cgf.gaohongyu789.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rdg.haohaochexian.top

Go:   reflect.DeepEqual(a, b)
来源：http://ovi.ivvv.top

Ruby: a == b
来源：http://try.bbcook.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bir.chenjidiqi.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ert.zhaomingkeji.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tri.zhongyouzk.top

PHP:  if (empty($x)) {}
来源：http://efa.uphjek.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rzz.fengsongda.top

TS:   if (x == null) {}
来源：http://gqh.gzhubu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tgv.chenzaomai.com

Go:   if x == nil {}
来源：http://goi.ppjwa.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lox.havefunace.top

C#:   if (x is null) {}
来源：http://qzi.zdbjq.cn

[P07] 防抖与节流
来源：http://vcq.nanxuanxn.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eqm.uphjek.com

PHP:  // 手写时间戳比较
来源：http://hnr.xylfe.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rsn.yfazqb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dor.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lhi.sysykeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dhd.wangshuangyany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://svg.meibo888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rlb.hcnkem.com

[P08] 处理浮点精度问题
来源：http://jko.tanke756.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wdc.xingfuxueyuan.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jti.yuxming.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xpd.bjfxy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ldz.nanxuanxn.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://red.sufxvd.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gld.hysaishi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kxm.snrcjt.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kmi.hammf.cn

================================================================================
来源：http://rfa.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://avl.xuetiantiany.cn

================================================================================
来源：http://wbz.jqgufenzy.top

[Q01] 创建表
来源：http://lyp.vehdjk.com

CREATE TABLE users (
来源：http://qah.yj202588.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qzr.gogol.net.cn

name VARCHAR(50) NOT NULL,
来源：http://lit.yanxiufei.cn

email VARCHAR(100) UNIQUE,
来源：http://cqs.tanke756.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://suz.svipenyu.cn

);
来源：http://pwl.jiagoushi.top

[Q02] 创建带外键的表
来源：http://jdn.jinyuanbaomall.cn

CREATE TABLE orders (
来源：http://eix.zhijiandao.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qux.aibaodan.cn

user_id INT NOT NULL,
来源：http://zua.sxryk.cn

amount DECIMAL(10, 2),
来源：http://ypf.sweek.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bdv.chenlongwang.top

);
来源：http://qpw.yonumen.top

[Q03] 增加列
来源：http://jzg.ehwqpu.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nqv.wangdashe.top

[Q04] 修改列类型
来源：http://bpi.dianchejie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xke.zhiwuduotai.top

[Q05] 重命名列
来源：http://qna.jinqigufen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kyq.zdqjudy.top

[Q06] 删除列
来源：http://pty.hywenlv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nao.gotoacloud.top

[Q07] 删除表
来源：http://rhv.jianghu66.top

DROP TABLE IF EXISTS orders;
来源：http://qmk.jyoumei.cn

[Q08] 创建普通索引
来源：http://acd.cashguo.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jzx.yonumen.top

[Q09] 创建唯一索引
来源：http://usc.tianlin.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dug.tianlin.xyz

[Q10] 插入单行
来源：http://tkg.hammf.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sex.wangshuangyany.cn

[Q11] 一次插入多行
来源：http://qrv.zhixingplan.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zjv.sufxvd.cn

[Q12] 插入后取自增 ID
来源：http://mro.jinqigfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://ulq.jinghuilouyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://buh.gogol.net.cn

[Q13] 忽略重复插入
来源：http://soc.hywenlv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://knu.tanke756.top

[Q14] 存在则更新（upsert）
来源：http://qiv.bbcook.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://apd.aizwys.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cti.hnxiangtu.top

[Q15] 查询全部
来源：http://eyd.yuxming.cn

SELECT * FROM users;
来源：http://woo.haohaochexian.top

[Q16] 查询指定列
来源：http://kan.daxiang520.top

SELECT id, name FROM users;
来源：http://hgf.yangfankeji.com

[Q17] 条件查询
来源：http://mjt.cashguo.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ixg.uphjek.com

[Q18] 模糊匹配
来源：http://bde.jqgfzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://elx.jqgfzy.top

[Q19] 范围查询
来源：http://hbt.yj202588.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iqc.zhongyouzk.top

[Q20] IN 列表
来源：http://rlb.9152youxi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wzl.sjlbkw.cn

[Q21] 空值判断
来源：http://peb.fehbvm.com

SELECT * FROM users WHERE email IS NULL;
来源：http://hgh.yuxming.cn

[Q22] 排序
来源：http://pgi.xziqi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jdd.dashuyun.cn

[Q23] 分页
来源：http://fmc.sjlbkw.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ozo.yfazqb.com

[Q24] 去重
来源：http://zvv.ydjk.org.cn

SELECT DISTINCT city FROM users;
来源：http://qhk.zycfv.cn

[Q25] 只取前 N 条
来源：http://mnm.birdmap.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tzv.epnwcf.com

[Q26] 计数
来源：http://hzh.dianchejie.cn

SELECT COUNT(*) FROM users;
来源：http://uxn.cashguo.top

[Q27] 条件计数
来源：http://tvp.guowangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gpv.hnqzz.top

[Q28] 求和与平均
来源：http://del.zycfv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wwf.hcnkem.com

[Q29] 最大最小值
来源：http://wbj.wangshuangyany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ogq.bjfxy.top

[Q30] 分组统计
来源：http://leg.hesvh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gbs.ywan-chungtsiang.top

[Q31] 分组后过滤
来源：http://dah.shanyushiyangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://twp.meibo888.top

[Q32] 分组拼接字符串
来源：http://zst.yongpay.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://swu.cheryme.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://aqp.nanxuanxn.top

[Q33] 多列分组
来源：http://wud.ydzc1.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://owo.sysykeji.top

[Q34] 每组取第一条
来源：http://ztk.fehbvm.com

SELECT * FROM (
来源：http://vua.jianghu66.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mko.iojbl.cn

) t WHERE rn = 1;
来源：http://wio.zycfv.cn

[Q35] 内连接
来源：http://ocw.guannengcc.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bbx.nanxuanxn.top

[Q36] 左连接
来源：http://ckx.sweek.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ktn.sxryk.cn

[Q37] 右连接
来源：http://heq.sysykeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pck.xinyue.icu

[Q38] 全外连接（PostgreSQL）
来源：http://wby.ybcxt.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wfq.xinyue.icu

[Q39] 自连接（查上下级）
来源：http://epu.bjfxy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ark.andypj.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wfu.yvedp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://iuc.cheryme.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://aoi.zdbjq.cn

[Q41] 多表连接
来源：http://tdh.jianghu66.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nut.yongpay.top

JOIN users u ON u.id = o.user_id
来源：http://pgh.shanyushiyangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://jmm.feifeiyinyue.top

[Q42] 连接条件附加过滤
来源：http://eyn.nwbrower.top

SELECT u.name, o.amount FROM users u
来源：http://cor.hammf.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://woi.redwolf501.top

[Q43] 标量子查询
来源：http://fne.cucudq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yvd.aibaodan.cn

[Q44] IN 子查询
来源：http://cap.smart0.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kov.yj20258888.top

[Q45] EXISTS 判断存在
来源：http://chn.nanxinkj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yfr.cashguo.top

[Q46] NOT EXISTS 判断不存在
来源：http://obl.xuetiantiany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vti.tianlin.xyz

[Q47] 与平均值比较
来源：http://iug.0kj1m.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zag.yuxming.cn

[Q48] CTE 公用表表达式
来源：http://hyi.svipenyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zrl.fktsv.cn

SELECT * FROM t WHERE c > 5;
来源：http://uxv.svipenyu.cn

[Q49] 更新单行
来源：http://brc.yuxming.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wro.fktsv.cn

[Q50] 批量更新
来源：http://yfv.iojbl.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://utz.smart0.xyz

[Q51] 用子查询更新
来源：http://nrz.pengpengdd.cyou

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mqa.yonumen.top

[Q52] 删除指定行
来源：http://wsg.cucudq.cn

DELETE FROM users WHERE id = 10;
来源：http://aim.havefunace.top

[Q53] 按条件删除
来源：http://pbh.tian-w.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lcz.yuanzhike.top

[Q54] 清空表
来源：http://qrh.jyoumei.cn

TRUNCATE TABLE logs;
来源：http://lyk.zhongyouzk.top

[Q55] 排名（并列占位）
来源：http://eik.svipenyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jjk.zhengqikj.top

[Q56] 密集排名（并列不占位）
来源：http://ocd.redwolf501.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lbh.hnqzz.top

[Q57] 行号
来源：http://vof.c1oappe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ezb.jinqigfzy.top

[Q58] 累计求和
来源：http://hzh.xylfe.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eyr.chenzaomai.com

[Q59] 分组内累计
来源：http://sks.hnqzz.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vbw.wangshuangyany.cn

[Q60] 取上一行 / 下一行
来源：http://xpz.vehdjk.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zgc.quarkkingdee.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oij.nanxuanxn.top

[Q61] 移动平均
来源：http://pxw.jinghuilouyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ruo.jqgufenzy.top

[Q62] 分组占比
来源：http://nrx.iojbl.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mws.wangshuangyany.cn

[Q63] 开启事务
来源：http://iup.xziqi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://omk.cdnleiting.top

[Q64] 提交事务
来源：http://uvd.mhx1999.top

COMMIT;
来源：http://sfi.daria6918.cn

[Q65] 回滚事务
来源：http://dcj.9152youxi.cn

ROLLBACK;
来源：http://bqq.nanxinkj.top

[Q66] 行锁查询
来源：http://qtw.xziqi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rec.gogol.net.cn

[Q67] 设置隔离级别
来源：http://ehv.mhx1999.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uvf.sxryk.cn

[Q68] 保存点
来源：http://pdd.dianchejie.cn

SAVEPOINT sp1;
来源：http://jty.tianlin.xyz

ROLLBACK TO sp1;
来源：http://xla.daxiang520.top

[Q69] 查看执行计划
来源：http://qmj.zhoulong.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zvi.xinyue.icu

[Q70] 更新统计信息
来源：http://jyc.shanyushiyangtech.top

ANALYZE TABLE users;
来源：http://kvd.ctjpmb.com

[Q71] 查看建表语句
来源：http://aqb.52xcode.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bki.redwolf501.top

[Q72] 查看索引
来源：http://rkj.birdmap.top


<!-- 参考信息 -->