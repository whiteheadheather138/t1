代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dyy.yvedp.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://anm.gzhubu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xkn.kuanghao11.cn

TS:   // 同 JS
来源：http://bzk.xylfe.cn

Java: new Thread(() -> f()).start()
来源：http://xfc.meibo888.top

Go:   go f()
来源：http://lqj.uphjek.com

Ruby: Thread.new { f }
来源：http://vdz.epnwcf.com

C#:   Task.Run(() => F());
来源：http://jmw.nwbrower.top

[O02] 使用线程池
来源：http://ayz.xuetiantiany.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bus.xziqi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cdp.0kj1m.cn

JS:   // worker_threads 线程池
来源：http://ozh.birdmap.top

TS:   // worker_threads 线程池
来源：http://jiq.gaohongyu789.top

Java: Executors.newFixedThreadPool(4)
来源：http://nce.jinyuanbaomall.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yxz.jinghuilouyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qox.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wfy.shanyushiyangtech.top

[O03] 加锁保护共享数据
来源：http://slt.gaohongyu789.top

Py:   with lock: shared += 1
来源：http://cfo.chenjidiqi.icu

PHP:  // 用 flock() 做文件锁
来源：http://uds.jianghu66.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xhb.sxryk.cn

TS:   // 同 JS
来源：http://vzz.yongpay.top

Java: synchronized (this) { shared++; }
来源：http://ckl.316326.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sfc.gogol.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yod.epnwcf.com

C#:   lock (gate) { shared++; }
来源：http://bog.tarul.cn

[O04] 定义异步函数并等待
来源：http://wad.zhaomingkeji.xyz

Py:   async def f():⏎    await g()
来源：http://hwe.yj20258.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://exk.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://jwx.shanyushiyangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ndk.jinyuanbaomall.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://agb.fehbvm.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nfo.ydjk.org.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qcn.bjfxy.top

C#:   async Task F() { await G(); }
来源：http://zmv.zdqjudy.top

[O05] 并发执行并等待全部完成
来源：http://sst.yonumen.top

Py:   asyncio.gather(*tasks)
来源：http://zbd.aibaodan.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kxg.nanxuanxn.top

JS:   await Promise.all(tasks)
来源：http://hqr.zhiwuduotai.top

TS:   await Promise.all(tasks)
来源：http://ftr.aibaodan.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dha.bbcook.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xab.jyoumei.cn

Ruby: threads.map(&:join)
来源：http://xjp.hongshengwenyu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://iks.andypj.xyz

[O06] 使用进程池
来源：http://kon.hnqzz.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://owx.xylfe.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sxc.0kj1m.cn

JS:   // child_process / cluster 模块
来源：http://aco.ydjk.org.cn

TS:   // child_process / cluster 模块
来源：http://hvj.jinghuilouyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dib.havefunace.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hgs.sysykeji.top

Ruby: // fork 块
来源：http://dmp.ydjk.org.cn

C#:   Parallel.For
来源：http://bro.zhengqikj.top

================================================================================
来源：http://yay.hysaishi.cn

P. 常用工具函数
来源：http://zcj.wangshuangyany.cn

================================================================================
来源：http://qfn.ctjpmb.com

[P01] 生成 UUID
来源：http://kak.iojbl.cn

Py:   str(uuid.uuid4())
来源：http://fxx.zhoulong.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://czq.ctjpmb.com

JS:   crypto.randomUUID()
来源：http://mzw.fengsongda.top

TS:   crypto.randomUUID()
来源：http://zwn.zycfv.cn

Java: UUID.randomUUID().toString()
来源：http://qjf.aibaodan.cn

Go:   // 用 github.com/google/uuid
来源：http://net.tarul.cn

Ruby: SecureRandom.uuid
来源：http://shn.hnxiangtu.top

C#:   Guid.NewGuid().ToString()
来源：http://lba.dashuyun.cn

[P02] MD5 / SHA256 摘要
来源：http://cmy.jqgfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kkt.chenjidiqi.icu

PHP:  hash("sha256", $s);  md5($s);
来源：http://pip.svipenyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zvy.dashuyun.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mht.zhixingplan.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://csz.shanyushiyangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lnt.nwbrower.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uex.cqqwz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rom.jiagoushi.top

[P03] 生成短随机字符串
来源：http://ihg.zhixingplan.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vxo.yanxiufei.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ynp.fktsv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hjv.mhx1999.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://roy.ydjk.org.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ued.tarul.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ghx.tianlin.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://wyz.xuetiantiany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ens.jiagoushi.top

[P04] 求长度
来源：http://wbx.zhixingplan.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rrf.hnqzz.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ryv.gotoacloud.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kia.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jxt.havefunace.top

Java: list.size();  map.size();  s.length()
来源：http://kta.yueranfly.top

Go:   len(arr);  len(m)
来源：http://com.birdmap.top

Ruby: x.length;  x.size
来源：http://bve.ydzc1.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://hvg.chenjidiqi.icu

[P05] 判断两个对象内容是否相等
来源：http://tkj.zhongyouzk.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lnu.jianghu66.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vmw.wangshuangyany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hqa.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xhg.daria6918.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://afh.zhaomingkeji.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://qfc.dashuyun.cn

Ruby: a == b
来源：http://rtq.redwolf501.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ogh.ydjk.org.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://efw.redwolf501.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jnr.sweek.top

PHP:  if (empty($x)) {}
来源：http://cwr.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://brf.wangshuangyany.cn

TS:   if (x == null) {}
来源：http://bop.guannengcc.top

Java: if (x == null || x.isEmpty()) {}
来源：http://gox.wangshuangyany.cn

Go:   if x == nil {}
来源：http://tvs.ppjwa.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wug.bjfxy.top

C#:   if (x is null) {}
来源：http://eyv.mhx1999.top

[P07] 防抖与节流
来源：http://xvi.fehbvm.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rhs.yj20258888.top

PHP:  // 手写时间戳比较
来源：http://han.tianlin.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cdt.jqgfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kxd.fehbvm.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://glx.hesvh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://znw.jinqigufen.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zjg.chenzaomai.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://amu.gaohongyu789.top

[P08] 处理浮点精度问题
来源：http://lxq.zhaomingkeji.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://urx.shuidangran.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uya.svipenyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vun.52xcode.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bvb.jqgufenzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zfb.52xcode.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nql.chenlongwang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kwo.52xcode.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gdo.xuanzx.com

================================================================================
来源：http://ofw.aibaodan.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mnx.pengpengdd.cyou

================================================================================
来源：http://tpt.wangdashe.top

[Q01] 创建表
来源：http://eej.fehbvm.com

CREATE TABLE users (
来源：http://faa.zhiwuduotai.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yip.ctjpmb.com

name VARCHAR(50) NOT NULL,
来源：http://ale.hesvh.cn

email VARCHAR(100) UNIQUE,
来源：http://aex.birdmap.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lbb.mhx1999.top

);
来源：http://igv.smart0.xyz

[Q02] 创建带外键的表
来源：http://sxh.andypj.xyz

CREATE TABLE orders (
来源：http://iql.tianlin.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://veb.hammf.cn

user_id INT NOT NULL,
来源：http://ccp.cashguo.top

amount DECIMAL(10, 2),
来源：http://dbw.jinqigufen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lcz.fanxiaobao.xyz

);
来源：http://tvk.shanyushiyangtech.top

[Q03] 增加列
来源：http://tdq.gogol.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hjp.sxryk.cn

[Q04] 修改列类型
来源：http://rao.0kj1m.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ijs.chenlongwang.top

[Q05] 重命名列
来源：http://xik.zhixingplan.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bvh.ybcxt.top

[Q06] 删除列
来源：http://stf.xylfe.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pqk.gogol.net.cn

[Q07] 删除表
来源：http://upn.wangdashe.top

DROP TABLE IF EXISTS orders;
来源：http://dve.nanxinkj.top

[Q08] 创建普通索引
来源：http://oge.shanyushiyangtech.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ser.zhongyouzk.top

[Q09] 创建唯一索引
来源：http://giu.daria6918.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pge.52xcode.cn

[Q10] 插入单行
来源：http://kyc.gotoacloud.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nxo.mhx1999.top

[Q11] 一次插入多行
来源：http://hvz.smart0.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xxn.zhengqikj.top

[Q12] 插入后取自增 ID
来源：http://ppl.jinghuilouyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://igi.zhiwuduotai.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aii.haohaochexian.top

[Q13] 忽略重复插入
来源：http://fta.yangfankeji.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cos.shanyushiyangtech.top

[Q14] 存在则更新（upsert）
来源：http://yil.xuanzx.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mue.zhiwuduotai.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lbw.bbcook.cn

[Q15] 查询全部
来源：http://tvl.ywan-chungtsiang.top

SELECT * FROM users;
来源：http://cfw.fktsv.cn

[Q16] 查询指定列
来源：http://sln.c1oappe.top

SELECT id, name FROM users;
来源：http://wpr.jlsjyb.cn

[Q17] 条件查询
来源：http://hof.ydjk.org.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zlb.yueranfly.top

[Q18] 模糊匹配
来源：http://ozx.shzxlz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dnh.hesvh.cn

[Q19] 范围查询
来源：http://ybj.jyoumei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pdw.ppjwa.cn

[Q20] IN 列表
来源：http://pij.pengpengdd.cyou

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wkz.chenlongwang.top

[Q21] 空值判断
来源：http://fls.jianghu66.top

SELECT * FROM users WHERE email IS NULL;
来源：http://spo.52xcode.cn

[Q22] 排序
来源：http://hfs.sweek.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kac.sufxvd.cn

[Q23] 分页
来源：http://rhv.hesvh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bvn.sxryk.cn

[Q24] 去重
来源：http://all.zycfv.cn

SELECT DISTINCT city FROM users;
来源：http://nco.gaohongyu789.top

[Q25] 只取前 N 条
来源：http://pvw.sxryk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qwb.bjfxy.top

[Q26] 计数
来源：http://izf.yueranfly.top

SELECT COUNT(*) FROM users;
来源：http://vmk.jqgfzy.top

[Q27] 条件计数
来源：http://ufx.zhiwuduotai.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fyl.52xcode.cn

[Q28] 求和与平均
来源：http://yjz.chenlongwang.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://woh.tarul.cn

[Q29] 最大最小值
来源：http://uqn.yuxming.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jaa.316326.xyz

[Q30] 分组统计
来源：http://aez.zhoulong.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://loe.tanke756.top

[Q31] 分组后过滤
来源：http://lpm.fengsongda.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xle.smart0.xyz

[Q32] 分组拼接字符串
来源：http://ppy.jinqigfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ddu.jqgfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://igg.yueranfly.top

[Q33] 多列分组
来源：http://jdy.cqqwz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mjd.shzxlz.cn

[Q34] 每组取第一条
来源：http://tnq.chenjidiqi.icu

SELECT * FROM (
来源：http://jfv.fanxiaobao.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://srj.sufxvd.cn

) t WHERE rn = 1;
来源：http://zgq.yonumen.top

[Q35] 内连接
来源：http://ilo.redwolf501.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gzj.zhoulong.xyz

[Q36] 左连接
来源：http://dkx.mhx1999.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lgk.daxiang520.top

[Q37] 右连接
来源：http://vvt.yuxming.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kwl.nwbrower.top

[Q38] 全外连接（PostgreSQL）
来源：http://dmw.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mvt.mhx1999.top

[Q39] 自连接（查上下级）
来源：http://irl.zhengqikj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tef.zhixingplan.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gzk.redwolf501.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qdt.nwbrower.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zes.bjfxy.top

[Q41] 多表连接
来源：http://rqn.zhoulong.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://dms.jiagoushi.top

JOIN users u ON u.id = o.user_id
来源：http://qfs.cqqwz.cn

JOIN products p ON p.id = o.product_id;
来源：http://srs.aibaodan.cn

[Q42] 连接条件附加过滤
来源：http://bmy.zdqjudy.top

SELECT u.name, o.amount FROM users u
来源：http://hts.xuanzx.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://aux.316326.xyz

[Q43] 标量子查询
来源：http://uvm.smart0.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pva.shuidangran.top

[Q44] IN 子查询
来源：http://rjs.redwolf501.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jqj.jyoumei.cn

[Q45] EXISTS 判断存在
来源：http://gln.0kj1m.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ltx.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mmb.bjfxy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kvm.yj20258.top

[Q47] 与平均值比较
来源：http://gct.dianchejie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zcg.havefunace.top

[Q48] CTE 公用表表达式
来源：http://ubx.52xcode.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fmi.daria6918.cn

SELECT * FROM t WHERE c > 5;
来源：http://bei.guowangkeji.top

[Q49] 更新单行
来源：http://blf.dianchejie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tel.dashuyun.cn

[Q50] 批量更新
来源：http://she.hcnkem.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aaa.tianlin.xyz

[Q51] 用子查询更新
来源：http://jzt.chenjidiqi.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lqc.sufxvd.cn

[Q52] 删除指定行
来源：http://ksa.sufxvd.cn

DELETE FROM users WHERE id = 10;
来源：http://wsp.cqqwz.cn

[Q53] 按条件删除
来源：http://nbz.xuetiantiany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tqc.kuanghao11.cn

[Q54] 清空表
来源：http://fua.sjlbkw.cn

TRUNCATE TABLE logs;
来源：http://zcq.cqqwz.cn

[Q55] 排名（并列占位）
来源：http://uuu.yj20258888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gmf.dashuyun.cn

[Q56] 密集排名（并列不占位）
来源：http://mat.meibo888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dqi.wangshuangyany.cn

[Q57] 行号
来源：http://ckf.cqqwz.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oow.zhixingplan.top

[Q58] 累计求和
来源：http://zop.smart0.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kcl.ybcxt.top

[Q59] 分组内累计
来源：http://nkt.nwbrower.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ium.guannengcc.top

[Q60] 取上一行 / 下一行
来源：http://dgs.hcnkem.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://emg.gzhubu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wfm.sxryk.cn

[Q61] 移动平均
来源：http://riy.smart0.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ycf.bbcook.cn

[Q62] 分组占比
来源：http://wcn.jinqigfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://van.tarul.cn

[Q63] 开启事务
来源：http://gix.aibaodan.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fzf.tian-w.cn

[Q64] 提交事务
来源：http://sin.vehdjk.com

COMMIT;
来源：http://imb.sweek.top

[Q65] 回滚事务
来源：http://tsc.zycfv.cn

ROLLBACK;
来源：http://ifx.ehwqpu.com

[Q66] 行锁查询
来源：http://wdu.yongpay.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lcl.aizwys.cn

[Q67] 设置隔离级别
来源：http://vdt.yonumen.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rrt.guowangkeji.top

[Q68] 保存点
来源：http://jpq.yvedp.cn

SAVEPOINT sp1;
来源：http://emb.hfpthk.cn

ROLLBACK TO sp1;
来源：http://wik.cashguo.top

[Q69] 查看执行计划
来源：http://acg.kuanghao11.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wqx.gogol.net.cn

[Q70] 更新统计信息
来源：http://jam.sysykeji.top

ANALYZE TABLE users;
来源：http://eni.ctjpmb.com

[Q71] 查看建表语句
来源：http://qjn.redwolf501.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ylg.ctjpmb.com

[Q72] 查看索引
来源：http://wtc.wangdashe.top

SHOW INDEX FROM users;
来源：http://glb.shzxlz.cn

[Q73] 查看表状态
来源：http://dbv.zdqjudy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kct.vqdsnc.cn

[Q74] 强制使用索引
来源：http://xwx.gotoacloud.top


<!-- 参考信息 -->