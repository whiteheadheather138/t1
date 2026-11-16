代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://peb.yj20258888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wpl.yonumen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fuo.9152youxi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gtm.jianghu66.top

================================================================================
来源：http://gif.cucudq.cn

O. 并发与异步
来源：http://old.xylfe.cn

================================================================================
来源：http://mnf.daria6918.cn

[O01] 启动一个线程
来源：http://wbh.iojbl.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kwa.gzhubu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wpr.redwolf501.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bsv.yuanzhike.top

TS:   // 同 JS
来源：http://qee.sysykeji.top

Java: new Thread(() -> f()).start()
来源：http://ern.shangyingyoupin.top

Go:   go f()
来源：http://wrq.birdmap.top

Ruby: Thread.new { f }
来源：http://bkx.yuanzhike.top

C#:   Task.Run(() => F());
来源：http://dlt.chenjidiqi.icu

[O02] 使用线程池
来源：http://pnm.aizwys.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wya.hysaishi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rst.0kj1m.cn

JS:   // worker_threads 线程池
来源：http://wut.316326.xyz

TS:   // worker_threads 线程池
来源：http://jel.ctjpmb.com

Java: Executors.newFixedThreadPool(4)
来源：http://mlx.ywan-chungtsiang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gti.hywenlv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hpz.c1oappe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lho.fanxiaobao.xyz

[O03] 加锁保护共享数据
来源：http://hwj.bbcook.cn

Py:   with lock: shared += 1
来源：http://csh.yuxming.cn

PHP:  // 用 flock() 做文件锁
来源：http://gwm.epnwcf.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://prk.yuxming.cn

TS:   // 同 JS
来源：http://syo.feifeiyinyue.top

Java: synchronized (this) { shared++; }
来源：http://gmw.jyoumei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://brd.aizwys.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://was.shuidangran.top

C#:   lock (gate) { shared++; }
来源：http://lmd.mhx1999.top

[O04] 定义异步函数并等待
来源：http://hau.ppjwa.cn

Py:   async def f():⏎    await g()
来源：http://guh.shanyushiyangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xgr.fanxiaobao.xyz

JS:   async function f() { await g(); }
来源：http://mhk.cqqwz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hnc.cqqwz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://psj.xinyue.icu

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wdu.zycfv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://aqp.vehdjk.com

C#:   async Task F() { await G(); }
来源：http://dcv.nanxinkj.top

[O05] 并发执行并等待全部完成
来源：http://rlm.ehwqpu.com

Py:   asyncio.gather(*tasks)
来源：http://fxa.haohaochexian.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yiz.hammf.cn

JS:   await Promise.all(tasks)
来源：http://xuq.ctjpmb.com

TS:   await Promise.all(tasks)
来源：http://gge.zhongyouzk.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qrk.pengpengdd.cyou

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vbo.shanyushiyangkeji.top

Ruby: threads.map(&:join)
来源：http://dzm.feifeiyinyue.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ufc.sysykeji.top

[O06] 使用进程池
来源：http://kid.shangyingyoupin.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://csy.xinyue.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://nro.fengsongda.top

JS:   // child_process / cluster 模块
来源：http://hhx.ivvv.top

TS:   // child_process / cluster 模块
来源：http://vuz.zdbjq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uhp.fehbvm.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eab.fanxiaobao.xyz

Ruby: // fork 块
来源：http://cge.ydjk.org.cn

C#:   Parallel.For
来源：http://xce.zhoulong.xyz

================================================================================
来源：http://nga.vehdjk.com

P. 常用工具函数
来源：http://pdn.epnwcf.com

================================================================================
来源：http://vbt.jinqigufen.top

[P01] 生成 UUID
来源：http://eqt.tian-w.cn

Py:   str(uuid.uuid4())
来源：http://seq.zycfv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rhv.ywan-chungtsiang.top

JS:   crypto.randomUUID()
来源：http://nke.ctjpmb.com

TS:   crypto.randomUUID()
来源：http://dzy.pycfn.com

Java: UUID.randomUUID().toString()
来源：http://fnf.yonumen.top

Go:   // 用 github.com/google/uuid
来源：http://qol.andypj.xyz

Ruby: SecureRandom.uuid
来源：http://cao.yueranfly.top

C#:   Guid.NewGuid().ToString()
来源：http://wbh.shangyingyoupin.top

[P02] MD5 / SHA256 摘要
来源：http://qwu.fehbvm.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fzw.jianghu66.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://rqn.hammf.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yfo.tanke756.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tsc.feifeiyinyue.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uhm.chenlongwang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rsc.sweek.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yrb.yj20258888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qyx.ppjwa.cn

[P03] 生成短随机字符串
来源：http://qet.xuetiantiany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lmj.chenjidiqi.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wnm.yuanzhike.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ses.zdqjudy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://svx.ctjpmb.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://boz.tanke756.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sty.pengpengdd.cyou

Ruby: SecureRandom.alphanumeric(16)
来源：http://rnf.andypj.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fhc.hnqzz.top

[P04] 求长度
来源：http://xjk.bjfxy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://htk.hammf.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xvv.shanyushiyangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fcx.yj20258.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fut.316326.xyz

Java: list.size();  map.size();  s.length()
来源：http://gma.gogol.net.cn

Go:   len(arr);  len(m)
来源：http://ytz.gotoacloud.top

Ruby: x.length;  x.size
来源：http://euv.pengpengdd.cyou

C#:   list.Count;  dict.Count;  s.Length
来源：http://xyc.hcnkem.com

[P05] 判断两个对象内容是否相等
来源：http://zwx.cheryme.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nph.yuanzhike.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gys.hnxiangtu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yed.nanxinkj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dhf.andypj.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kvo.ydjk.org.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fop.yongpay.top

Ruby: a == b
来源：http://cot.sweek.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bsu.fanxiaobao.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jgc.316326.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cuf.hnxiangtu.top

PHP:  if (empty($x)) {}
来源：http://vmi.daria6918.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ecs.shzxlz.cn

TS:   if (x == null) {}
来源：http://hfg.pengpengdd.cyou

Java: if (x == null || x.isEmpty()) {}
来源：http://bpo.tarul.cn

Go:   if x == nil {}
来源：http://qah.ivvv.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jvw.hcnkem.com

C#:   if (x is null) {}
来源：http://ldq.shanyushiyangtech.top

[P07] 防抖与节流
来源：http://cuw.jinqigufen.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kay.zhongyouzk.top

PHP:  // 手写时间戳比较
来源：http://boq.ybcxt.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kyh.chenlongwang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://svx.iojbl.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://meu.pycfn.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hrd.epnwcf.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://zua.smart0.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gwt.guowangkeji.top

[P08] 处理浮点精度问题
来源：http://cef.ywan-chungtsiang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gjk.shuidangran.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yvm.gotoacloud.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wlh.andypj.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://anl.fktsv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://phl.guowangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ltk.pengpengdd.cyou

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://erg.9152youxi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uev.ppjwa.cn

================================================================================
来源：http://jzn.ivvv.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fnq.zhixingplan.top

================================================================================
来源：http://skh.cucudq.cn

[Q01] 创建表
来源：http://kds.yj20258.top

CREATE TABLE users (
来源：http://rjy.shanyushiyangkeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wmb.gzhubu.top

name VARCHAR(50) NOT NULL,
来源：http://hkf.sweek.top

email VARCHAR(100) UNIQUE,
来源：http://dxh.iojbl.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ezk.ybcxt.top

);
来源：http://lsx.xinyue.icu

[Q02] 创建带外键的表
来源：http://kug.zhaomingkeji.xyz

CREATE TABLE orders (
来源：http://sqw.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://icb.316326.xyz

user_id INT NOT NULL,
来源：http://yrg.jiagoushi.top

amount DECIMAL(10, 2),
来源：http://xox.feifeiyinyue.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jnp.shangyingyoupin.top

);
来源：http://jdh.mhx1999.top

[Q03] 增加列
来源：http://wwi.daria6918.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lac.cheryme.top

[Q04] 修改列类型
来源：http://hmo.pycfn.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hhn.haohaochexian.top

[Q05] 重命名列
来源：http://icn.fzhhl.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qga.gaohongyu789.top

[Q06] 删除列
来源：http://zvf.bjfxy.top

ALTER TABLE users DROP COLUMN age;
来源：http://guz.guowangkeji.top

[Q07] 删除表
来源：http://egp.jinqigfzy.top

DROP TABLE IF EXISTS orders;
来源：http://dif.zhengqikj.top

[Q08] 创建普通索引
来源：http://npm.svipenyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ovc.jinqigfzy.top

[Q09] 创建唯一索引
来源：http://vfo.vqdsnc.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cyp.hongshengwenyu.top

[Q10] 插入单行
来源：http://laf.ctjpmb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mas.chenzaomai.com

[Q11] 一次插入多行
来源：http://ali.xziqi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ayi.yvedp.cn

[Q12] 插入后取自增 ID
来源：http://baz.andypj.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://iyx.wangdashe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vgz.chenjidiqi.icu

[Q13] 忽略重复插入
来源：http://pmb.yj20258888.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nmr.chenzaomai.com

[Q14] 存在则更新（upsert）
来源：http://vng.chenzaomai.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cla.jianghu66.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fqx.0kj1m.cn

[Q15] 查询全部
来源：http://zyx.redwolf501.top

SELECT * FROM users;
来源：http://rwd.redwolf501.top

[Q16] 查询指定列
来源：http://wvx.tanke756.top

SELECT id, name FROM users;
来源：http://tkw.jinqigufen.top

[Q17] 条件查询
来源：http://gsg.yueranfly.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ouc.svipenyu.cn

[Q18] 模糊匹配
来源：http://jwo.shanyushiyangtech.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zjz.snrcjt.cn

[Q19] 范围查询
来源：http://fok.pycfn.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://aew.xylfe.cn

[Q20] IN 列表
来源：http://amr.chenjidiqi.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kyq.sweek.top

[Q21] 空值判断
来源：http://hlp.zycfv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ilq.zdqjudy.top

[Q22] 排序
来源：http://dbc.chenlongwang.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gzd.feifeiyinyue.top

[Q23] 分页
来源：http://jcg.gogol.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://erh.jlsjyb.cn

[Q24] 去重
来源：http://oel.c1oappe.top

SELECT DISTINCT city FROM users;
来源：http://jln.bjfxy.top

[Q25] 只取前 N 条
来源：http://kee.sjlbkw.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jpx.yuanzhike.top

[Q26] 计数
来源：http://xlh.jinqigfzy.top

SELECT COUNT(*) FROM users;
来源：http://wpp.birdmap.top

[Q27] 条件计数
来源：http://yzq.kuanghao11.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oox.xingfuxueyuan.xyz

[Q28] 求和与平均
来源：http://rfx.xziqi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nnc.nwbrower.top

[Q29] 最大最小值
来源：http://vlq.yj20258.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://frs.fehbvm.com

[Q30] 分组统计
来源：http://ccm.9152youxi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://onv.zhaomingkeji.xyz

[Q31] 分组后过滤
来源：http://cse.wangshuangyany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bjx.redwolf501.top

[Q32] 分组拼接字符串
来源：http://eyt.xylfe.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oot.yj20258888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://iul.xuanzx.com

[Q33] 多列分组
来源：http://zpm.fengsongda.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://syu.hywenlv.cn

[Q34] 每组取第一条
来源：http://kfs.shangyingyoupin.top

SELECT * FROM (
来源：http://bmu.chenlongwang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fui.shuidangran.top

) t WHERE rn = 1;
来源：http://opq.gotoacloud.top

[Q35] 内连接
来源：http://lat.tarul.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://smn.zycfv.cn

[Q36] 左连接
来源：http://xqs.jianghu66.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pit.zycfv.cn

[Q37] 右连接
来源：http://nms.0kj1m.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://aos.yvedp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lfs.daxiang520.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://han.xuetiantiany.cn

[Q39] 自连接（查上下级）
来源：http://kzm.shzxlz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lbi.xuanzx.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bja.vehdjk.com

[Q40] 交叉连接（笛卡尔积）
来源：http://tin.havefunace.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://amg.guannengcc.top

[Q41] 多表连接
来源：http://glq.daxiang520.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wsv.fengsongda.top

JOIN users u ON u.id = o.user_id
来源：http://vzt.shuidangran.top

JOIN products p ON p.id = o.product_id;
来源：http://ohc.jyoumei.cn

[Q42] 连接条件附加过滤
来源：http://yji.aizwys.cn

SELECT u.name, o.amount FROM users u
来源：http://juy.jqgfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://soa.zhoulong.xyz

[Q43] 标量子查询
来源：http://lfo.yj202588.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://imz.pycfn.com

[Q44] IN 子查询
来源：http://ift.vehdjk.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ypq.nwbrower.top

[Q45] EXISTS 判断存在
来源：http://ajc.wangshuangyany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uvv.ybcxt.top

[Q46] NOT EXISTS 判断不存在
来源：http://ges.jinyuanbaomall.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xum.wangshuangyany.cn

[Q47] 与平均值比较
来源：http://srj.sjlbkw.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://afj.fzhhl.top

[Q48] CTE 公用表表达式
来源：http://lll.zhongyouzk.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tim.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://xqg.fengsongda.top

[Q49] 更新单行
来源：http://sqn.yonumen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fwr.zhixingplan.top

[Q50] 批量更新
来源：http://myo.meibo888.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zkq.zhijiandao.cn

[Q51] 用子查询更新
来源：http://pzt.feifeiyinyue.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jdv.jianghu66.top

[Q52] 删除指定行
来源：http://kqm.jiagoushi.top

DELETE FROM users WHERE id = 10;
来源：http://uhq.daria6918.cn

[Q53] 按条件删除
来源：http://lxg.sweek.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ywu.feifeiyinyue.top

[Q54] 清空表
来源：http://ydx.zhiwuduotai.top

TRUNCATE TABLE logs;
来源：http://viu.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://huj.xingfuxueyuan.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xgq.zdqjudy.top

[Q56] 密集排名（并列不占位）
来源：http://gzg.gzhubu.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ddd.xuanzx.com

[Q57] 行号
来源：http://efx.dashuyun.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eid.yj20258.top

[Q58] 累计求和
来源：http://pvo.ctjpmb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://axs.jianghu66.top

[Q59] 分组内累计
来源：http://iah.9152youxi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hyu.sxryk.cn

[Q60] 取上一行 / 下一行
来源：http://moe.gotoacloud.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bqq.jinqigufen.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bld.quarkkingdee.top

[Q61] 移动平均
来源：http://bxs.zdbjq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ggu.kuanghao11.cn

[Q62] 分组占比
来源：http://xzv.xinyue.icu

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hua.iojbl.cn

[Q63] 开启事务
来源：http://ioq.hysaishi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cjf.xuanzx.com

[Q64] 提交事务
来源：http://iqa.cucudq.cn

COMMIT;
来源：http://mpr.tarul.cn

[Q65] 回滚事务
来源：http://hql.jyoumei.cn

ROLLBACK;
来源：http://txw.uphjek.com

[Q66] 行锁查询
来源：http://sxv.yj20258888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rtz.zdbjq.cn

[Q67] 设置隔离级别
来源：http://mif.hammf.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ovj.yuxming.cn

[Q68] 保存点
来源：http://ucq.pycfn.com

SAVEPOINT sp1;
来源：http://zqk.zhaomingkeji.xyz

ROLLBACK TO sp1;
来源：http://qja.ctjpmb.com

[Q69] 查看执行计划
来源：http://ryi.ctjpmb.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eyq.havefunace.top

[Q70] 更新统计信息
来源：http://vcg.kuanghao11.cn


<!-- 参考信息 -->