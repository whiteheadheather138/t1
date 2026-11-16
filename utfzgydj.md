代发 wailian999

================================================================================
来源：http://lmm.fktsv.cn

O. 并发与异步
来源：http://rvp.316326.xyz

================================================================================
来源：http://wgc.hesvh.cn

[O01] 启动一个线程
来源：http://aje.hnqzz.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rxy.316326.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nkr.yanxiufei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tko.jinqigufen.top

TS:   // 同 JS
来源：http://xns.haohaochexian.top

Java: new Thread(() -> f()).start()
来源：http://hzg.yfazqb.com

Go:   go f()
来源：http://njc.shanyushiyangkeji.top

Ruby: Thread.new { f }
来源：http://pwc.52xcode.cn

C#:   Task.Run(() => F());
来源：http://bqr.uphjek.com

[O02] 使用线程池
来源：http://ltx.zhixingplan.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zwr.nanxuanxn.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rce.uphjek.com

JS:   // worker_threads 线程池
来源：http://hrt.nwbrower.top

TS:   // worker_threads 线程池
来源：http://lff.yj20258888.top

Java: Executors.newFixedThreadPool(4)
来源：http://psu.zhoulong.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rzb.ehwqpu.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wkq.aibaodan.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cub.fehbvm.com

[O03] 加锁保护共享数据
来源：http://ahc.ppjwa.cn

Py:   with lock: shared += 1
来源：http://vef.hnxiangtu.top

PHP:  // 用 flock() 做文件锁
来源：http://nsu.hesvh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://esp.nwbrower.top

TS:   // 同 JS
来源：http://doc.ivvv.top

Java: synchronized (this) { shared++; }
来源：http://qjr.chenzaomai.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ebc.chenlongwang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wow.aizwys.cn

C#:   lock (gate) { shared++; }
来源：http://jhk.fengsongda.top

[O04] 定义异步函数并等待
来源：http://dim.ybcxt.top

Py:   async def f():⏎    await g()
来源：http://ref.vehdjk.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://foc.hongshengwenyu.top

JS:   async function f() { await g(); }
来源：http://wor.dashuyun.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tae.fktsv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hxo.yanxiufei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://djq.xziqi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tyg.ydjk.org.cn

C#:   async Task F() { await G(); }
来源：http://ytg.fanxiaobao.xyz

[O05] 并发执行并等待全部完成
来源：http://yey.ppjwa.cn

Py:   asyncio.gather(*tasks)
来源：http://tpn.fehbvm.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hpr.zhengqikj.top

JS:   await Promise.all(tasks)
来源：http://hfx.xinyue.icu

TS:   await Promise.all(tasks)
来源：http://fgf.iojbl.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cbz.snrcjt.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rpv.hywenlv.cn

Ruby: threads.map(&:join)
来源：http://zzf.gaohongyu789.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mtu.jinqigfzy.top

[O06] 使用进程池
来源：http://iua.sufxvd.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qlz.0kj1m.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ygz.yueranfly.top

JS:   // child_process / cluster 模块
来源：http://fid.gogol.net.cn

TS:   // child_process / cluster 模块
来源：http://bjv.wangdashe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cyr.meibo888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hux.zhongyouzk.top

Ruby: // fork 块
来源：http://ykx.sxryk.cn

C#:   Parallel.For
来源：http://raq.zhixingplan.top

================================================================================
来源：http://uvo.wangshuangyany.cn

P. 常用工具函数
来源：http://zze.hfpthk.cn

================================================================================
来源：http://yzs.bjfxy.top

[P01] 生成 UUID
来源：http://zmg.hammf.cn

Py:   str(uuid.uuid4())
来源：http://qyq.yfazqb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nfu.gzhubu.top

JS:   crypto.randomUUID()
来源：http://fws.vqdsnc.cn

TS:   crypto.randomUUID()
来源：http://cwx.0kj1m.cn

Java: UUID.randomUUID().toString()
来源：http://mpd.guowangkeji.top

Go:   // 用 github.com/google/uuid
来源：http://jsb.quarkkingdee.top

Ruby: SecureRandom.uuid
来源：http://wms.guannengcc.top

C#:   Guid.NewGuid().ToString()
来源：http://qve.hywenlv.cn

[P02] MD5 / SHA256 摘要
来源：http://xwo.jinyuanbaomall.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bfq.zdbjq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rhx.yj20258.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://esq.nanxinkj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://roz.zhiwuduotai.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lev.epnwcf.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fsm.zhaomingkeji.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kcg.jinghuilouyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mdb.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://avy.fengsongda.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lfh.yj20258.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rbr.hcnkem.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://plp.sufxvd.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dex.bbcook.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hhd.vqdsnc.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tqn.smart0.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://ilc.shzxlz.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hbx.yj202588.top

[P04] 求长度
来源：http://bgm.daria6918.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nkd.bjfxy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vjx.ywan-chungtsiang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://leu.vqdsnc.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aqi.xingfuxueyuan.xyz

Java: list.size();  map.size();  s.length()
来源：http://vqq.hcnkem.com

Go:   len(arr);  len(m)
来源：http://rgm.chenlongwang.top

Ruby: x.length;  x.size
来源：http://ypq.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://mau.ppjwa.cn

[P05] 判断两个对象内容是否相等
来源：http://nqs.feifeiyinyue.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://tlt.cqqwz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cqx.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iex.zdqjudy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eoh.fzhhl.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jym.smart0.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://jxz.52xcode.cn

Ruby: a == b
来源：http://dbj.jinqigfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rqm.aizwys.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://usg.fehbvm.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fqq.daxiang520.top

PHP:  if (empty($x)) {}
来源：http://ngb.hongshengwenyu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wpm.wangshuangyany.cn

TS:   if (x == null) {}
来源：http://moj.hongshengwenyu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xjj.zhongyouzk.top

Go:   if x == nil {}
来源：http://gle.kuanghao11.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hlf.yj20258888.top

C#:   if (x is null) {}
来源：http://hfl.tanke756.top

[P07] 防抖与节流
来源：http://pnh.hammf.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bay.ywan-chungtsiang.top

PHP:  // 手写时间戳比较
来源：http://wot.haohaochexian.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ava.zdbjq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wkg.jinqigufen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://npr.vehdjk.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://goy.dashuyun.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gux.yongpay.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lki.zhoulong.xyz

[P08] 处理浮点精度问题
来源：http://xtk.ywan-chungtsiang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ebv.cucudq.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wvp.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pdb.shuidangran.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xpw.zdbjq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dxi.fengsongda.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ngo.yonumen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mum.hnxiangtu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rzj.jyoumei.cn

================================================================================
来源：http://dgs.bbcook.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kiu.tarul.cn

================================================================================
来源：http://bhf.shanyushiyangtech.top

[Q01] 创建表
来源：http://xdt.ivvv.top

CREATE TABLE users (
来源：http://skg.fktsv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qbs.feifeiyinyue.top

name VARCHAR(50) NOT NULL,
来源：http://xbn.cucudq.cn

email VARCHAR(100) UNIQUE,
来源：http://yuo.52xcode.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gmp.snrcjt.cn

);
来源：http://pig.hywenlv.cn

[Q02] 创建带外键的表
来源：http://wvr.zdbjq.cn

CREATE TABLE orders (
来源：http://xol.xuetiantiany.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gfz.ctjpmb.com

user_id INT NOT NULL,
来源：http://hhw.c1oappe.top

amount DECIMAL(10, 2),
来源：http://cqp.yanxiufei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nhk.zhiwuduotai.top

);
来源：http://sjo.sweek.top

[Q03] 增加列
来源：http://zpf.zhongyouzk.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://emz.yj202588.top

[Q04] 修改列类型
来源：http://mjp.tian-w.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cma.redwolf501.top

[Q05] 重命名列
来源：http://yqu.ehwqpu.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cam.shanyushiyangtech.top

[Q06] 删除列
来源：http://jfu.wangdashe.top

ALTER TABLE users DROP COLUMN age;
来源：http://bfw.jinqigufen.top

[Q07] 删除表
来源：http://hml.zycfv.cn

DROP TABLE IF EXISTS orders;
来源：http://dfn.hcnkem.com

[Q08] 创建普通索引
来源：http://fgi.kuanghao11.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dwl.bjfxy.top

[Q09] 创建唯一索引
来源：http://ezu.xingfuxueyuan.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sve.xylfe.cn

[Q10] 插入单行
来源：http://dbc.hammf.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kob.ppjwa.cn

[Q11] 一次插入多行
来源：http://gir.hammf.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://npv.andypj.xyz

[Q12] 插入后取自增 ID
来源：http://dnf.aibaodan.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jhh.zhongyouzk.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rro.birdmap.top

[Q13] 忽略重复插入
来源：http://dep.tianlin.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fez.haohaochexian.top

[Q14] 存在则更新（upsert）
来源：http://rli.cqqwz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cyp.cucudq.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bqg.0kj1m.cn

[Q15] 查询全部
来源：http://wsd.tian-w.cn

SELECT * FROM users;
来源：http://acn.jqgfzy.top

[Q16] 查询指定列
来源：http://cfc.yj202588.top

SELECT id, name FROM users;
来源：http://vkx.xziqi.cn

[Q17] 条件查询
来源：http://xgh.zhongyouzk.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nbs.dashuyun.cn

[Q18] 模糊匹配
来源：http://hji.wangdashe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ytr.52xcode.cn

[Q19] 范围查询
来源：http://jam.zhijiandao.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wir.haohaochexian.top

[Q20] IN 列表
来源：http://lpj.xziqi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cfu.ydzc1.top

[Q21] 空值判断
来源：http://ekd.redwolf501.top

SELECT * FROM users WHERE email IS NULL;
来源：http://abh.cqqwz.cn

[Q22] 排序
来源：http://tbx.ydzc1.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ktd.gaohongyu789.top

[Q23] 分页
来源：http://bri.shanyushiyangtech.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jui.jqgufenzy.top

[Q24] 去重
来源：http://xjn.zhiwuduotai.top

SELECT DISTINCT city FROM users;
来源：http://ufd.gaohongyu789.top

[Q25] 只取前 N 条
来源：http://igd.pengpengdd.cyou

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gtx.cheryme.top

[Q26] 计数
来源：http://hrn.cucudq.cn

SELECT COUNT(*) FROM users;
来源：http://mvv.zhaomingkeji.xyz

[Q27] 条件计数
来源：http://vyv.cdnleiting.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kgx.cdnleiting.top

[Q28] 求和与平均
来源：http://fbx.guannengcc.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tsx.fktsv.cn

[Q29] 最大最小值
来源：http://erw.bjfxy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bha.tarul.cn

[Q30] 分组统计
来源：http://tck.smart0.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pgr.c1oappe.top

[Q31] 分组后过滤
来源：http://gvg.316326.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jjv.ybcxt.top

[Q32] 分组拼接字符串
来源：http://orq.hammf.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xrb.andypj.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bqr.yonumen.top

[Q33] 多列分组
来源：http://ecm.dianchejie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ylz.yanxiufei.cn

[Q34] 每组取第一条
来源：http://idm.fzhhl.top

SELECT * FROM (
来源：http://owh.gzhubu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vsb.sufxvd.cn

) t WHERE rn = 1;
来源：http://jla.epnwcf.com

[Q35] 内连接
来源：http://pwi.jinqigfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rwa.shanyushiyangkeji.top

[Q36] 左连接
来源：http://vki.yuxming.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://iap.xziqi.cn

[Q37] 右连接
来源：http://zce.shzxlz.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iwe.ywan-chungtsiang.top

[Q38] 全外连接（PostgreSQL）
来源：http://mrt.wangdashe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ekf.jyoumei.cn

[Q39] 自连接（查上下级）
来源：http://mzh.fzhhl.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://uru.cucudq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bgw.dashuyun.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lxc.pengpengdd.cyou

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dan.xylfe.cn

[Q41] 多表连接
来源：http://obt.tarul.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rpv.pycfn.com

JOIN users u ON u.id = o.user_id
来源：http://okd.shuidangran.top

JOIN products p ON p.id = o.product_id;
来源：http://kxs.c1oappe.top

[Q42] 连接条件附加过滤
来源：http://oxo.vqdsnc.cn

SELECT u.name, o.amount FROM users u
来源：http://xoy.iojbl.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mhe.xuanzx.com

[Q43] 标量子查询
来源：http://zub.gogol.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rja.xingfuxueyuan.xyz

[Q44] IN 子查询
来源：http://ibg.ywan-chungtsiang.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fej.guannengcc.top

[Q45] EXISTS 判断存在
来源：http://tvj.jinqigufen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://woq.quarkkingdee.top

[Q46] NOT EXISTS 判断不存在
来源：http://zmp.fehbvm.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gbi.chenjidiqi.icu

[Q47] 与平均值比较
来源：http://jkh.chenjidiqi.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://swe.guowangkeji.top

[Q48] CTE 公用表表达式
来源：http://psg.fehbvm.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rne.tian-w.cn

SELECT * FROM t WHERE c > 5;
来源：http://cvx.yj20258888.top

[Q49] 更新单行
来源：http://jfg.cdnleiting.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dug.ppjwa.cn

[Q50] 批量更新
来源：http://xpk.zhixingplan.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vmz.vqdsnc.cn

[Q51] 用子查询更新
来源：http://wsi.chenjidiqi.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hck.uphjek.com

[Q52] 删除指定行
来源：http://jmu.iojbl.cn

DELETE FROM users WHERE id = 10;
来源：http://zpx.bjfxy.top

[Q53] 按条件删除
来源：http://xoi.yj202588.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://suf.nanxinkj.top

[Q54] 清空表
来源：http://gwv.sxryk.cn

TRUNCATE TABLE logs;
来源：http://pez.uphjek.com

[Q55] 排名（并列占位）
来源：http://zwk.cdnleiting.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://klm.zhaomingkeji.xyz

[Q56] 密集排名（并列不占位）
来源：http://stj.zhaomingkeji.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gsf.yuxming.cn

[Q57] 行号
来源：http://fhg.xuetiantiany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ypu.ivvv.top

[Q58] 累计求和
来源：http://qdl.jyoumei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vnk.uphjek.com

[Q59] 分组内累计
来源：http://mkf.yj20258.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vmg.ivvv.top

[Q60] 取上一行 / 下一行
来源：http://xfa.sysykeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://usl.sweek.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bta.chenzaomai.com

[Q61] 移动平均
来源：http://imf.yj20258888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jjx.gzhubu.top

[Q62] 分组占比
来源：http://cfy.yuxming.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vwk.fzhhl.top

[Q63] 开启事务
来源：http://znx.sxryk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ucp.fzhhl.top

[Q64] 提交事务
来源：http://roo.hammf.cn

COMMIT;
来源：http://psd.cheryme.top

[Q65] 回滚事务
来源：http://chc.bjfxy.top

ROLLBACK;
来源：http://rut.uphjek.com

[Q66] 行锁查询
来源：http://dcr.shzxlz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://aud.xziqi.cn

[Q67] 设置隔离级别
来源：http://vqs.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jfi.xylfe.cn

[Q68] 保存点
来源：http://bcs.yfazqb.com

SAVEPOINT sp1;
来源：http://oyw.vehdjk.com

ROLLBACK TO sp1;
来源：http://mnj.sysykeji.top

[Q69] 查看执行计划
来源：http://ggu.quarkkingdee.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://thg.ydzc1.top

[Q70] 更新统计信息
来源：http://xlf.jinghuilouyu.cn

ANALYZE TABLE users;
来源：http://qwd.fktsv.cn

[Q71] 查看建表语句
来源：http://ahc.vehdjk.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vus.xziqi.cn

[Q72] 查看索引
来源：http://wqs.daxiang520.top


<!-- 参考信息 -->