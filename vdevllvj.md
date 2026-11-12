代发 wailian999

================================================================================
来源：http://wqa.redwolf501.top

O. 并发与异步
来源：http://yat.ydjk.org.cn

================================================================================
来源：http://dsg.xingfuxueyuan.xyz

[O01] 启动一个线程
来源：http://grj.xuetiantiany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jsl.yj20258888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hjf.xziqi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wwv.epnwcf.com

TS:   // 同 JS
来源：http://gyi.hysaishi.cn

Java: new Thread(() -> f()).start()
来源：http://skj.yfazqb.com

Go:   go f()
来源：http://ftw.ydzc1.top

Ruby: Thread.new { f }
来源：http://eeq.sjlbkw.cn

C#:   Task.Run(() => F());
来源：http://dpl.fanxiaobao.xyz

[O02] 使用线程池
来源：http://ugy.pycfn.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://osu.hywenlv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ogt.xylfe.cn

JS:   // worker_threads 线程池
来源：http://uth.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://zpd.jinyuanbaomall.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rho.hywenlv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://duq.kuanghao11.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sbj.sweek.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hli.chenjidiqi.icu

[O03] 加锁保护共享数据
来源：http://saw.yvedp.cn

Py:   with lock: shared += 1
来源：http://xei.epnwcf.com

PHP:  // 用 flock() 做文件锁
来源：http://rzc.bbcook.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://khc.vehdjk.com

TS:   // 同 JS
来源：http://jeb.yueranfly.top

Java: synchronized (this) { shared++; }
来源：http://jtt.shzxlz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sjd.hfpthk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ifw.yj202588.top

C#:   lock (gate) { shared++; }
来源：http://cwq.yfazqb.com

[O04] 定义异步函数并等待
来源：http://ixy.dianchejie.cn

Py:   async def f():⏎    await g()
来源：http://dqa.chenjidiqi.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lsy.yfazqb.com

JS:   async function f() { await g(); }
来源：http://ciy.ywan-chungtsiang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zxf.pengpengdd.cyou

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tlv.yvedp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nli.jinghuilouyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://oib.gotoacloud.top

C#:   async Task F() { await G(); }
来源：http://oiv.ydzc1.top

[O05] 并发执行并等待全部完成
来源：http://ikh.tanke756.top

Py:   asyncio.gather(*tasks)
来源：http://vox.jinghuilouyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eyj.snrcjt.cn

JS:   await Promise.all(tasks)
来源：http://zbq.aibaodan.cn

TS:   await Promise.all(tasks)
来源：http://tcr.jinqigfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uig.hysaishi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ffn.jinghuilouyu.cn

Ruby: threads.map(&:join)
来源：http://ezb.yuanzhike.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nwy.pycfn.com

[O06] 使用进程池
来源：http://cco.yfazqb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wgj.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zyn.shangyingyoupin.top

JS:   // child_process / cluster 模块
来源：http://cql.sxryk.cn

TS:   // child_process / cluster 模块
来源：http://nhj.hywenlv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xao.xziqi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://paq.yj20258888.top

Ruby: // fork 块
来源：http://pzf.yj20258888.top

C#:   Parallel.For
来源：http://zot.shangyingyoupin.top

================================================================================
来源：http://kka.zhiwuduotai.top

P. 常用工具函数
来源：http://equ.jinqigfzy.top

================================================================================
来源：http://xlm.cqqwz.cn

[P01] 生成 UUID
来源：http://qiq.andypj.xyz

Py:   str(uuid.uuid4())
来源：http://kmj.ehwqpu.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://thu.hesvh.cn

JS:   crypto.randomUUID()
来源：http://her.birdmap.top

TS:   crypto.randomUUID()
来源：http://dkj.jyoumei.cn

Java: UUID.randomUUID().toString()
来源：http://bes.cheryme.top

Go:   // 用 github.com/google/uuid
来源：http://qsi.yj202588.top

Ruby: SecureRandom.uuid
来源：http://hfh.shangyingyoupin.top

C#:   Guid.NewGuid().ToString()
来源：http://rap.sysykeji.top

[P02] MD5 / SHA256 摘要
来源：http://wih.hammf.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pts.cucudq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fzu.c1oappe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gwi.jlsjyb.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://igu.xingfuxueyuan.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nbt.bbcook.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oco.yanxiufei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kup.jqgufenzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gdc.gogol.net.cn

[P03] 生成短随机字符串
来源：http://xrb.sxryk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://knh.0kj1m.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xhl.ydzc1.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ofi.jyoumei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iaa.fengsongda.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ksp.xingfuxueyuan.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zdw.ybcxt.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mus.snrcjt.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lnv.xingfuxueyuan.xyz

[P04] 求长度
来源：http://bov.zhijiandao.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yyo.cdnleiting.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://awz.52xcode.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://leh.mhx1999.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hvg.zdbjq.cn

Java: list.size();  map.size();  s.length()
来源：http://oct.nanxinkj.top

Go:   len(arr);  len(m)
来源：http://ivv.jinqigufen.top

Ruby: x.length;  x.size
来源：http://ulo.cucudq.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fcr.cqqwz.cn

[P05] 判断两个对象内容是否相等
来源：http://wxp.fanxiaobao.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://ogn.iojbl.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xey.epnwcf.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ygd.yuxming.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wbz.iojbl.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rxq.guowangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://ccf.bbcook.cn

Ruby: a == b
来源：http://rkd.ydjk.org.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ocz.ydjk.org.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yuz.zhixingplan.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kps.yueranfly.top

PHP:  if (empty($x)) {}
来源：http://pjr.chenzaomai.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://veu.wangdashe.top

TS:   if (x == null) {}
来源：http://wqu.shzxlz.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wsj.cheryme.top

Go:   if x == nil {}
来源：http://hxl.haohaochexian.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wao.sysykeji.top

C#:   if (x is null) {}
来源：http://xcc.zdbjq.cn

[P07] 防抖与节流
来源：http://ptx.guowangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qze.cucudq.cn

PHP:  // 手写时间戳比较
来源：http://czf.svipenyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fso.iojbl.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://isl.yuxming.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cuy.cdnleiting.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ydh.pengpengdd.cyou

Ruby: // 手写闭包 + Time.now 判断
来源：http://vqh.xuanzx.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://okf.chenjidiqi.icu

[P08] 处理浮点精度问题
来源：http://pwp.ydjk.org.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ofr.tanke756.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kfi.yvedp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fvs.ydjk.org.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://afz.tian-w.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uvw.xuanzx.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hdp.zhongyouzk.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bek.cucudq.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mxg.ybcxt.top

================================================================================
来源：http://zul.hammf.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://svz.nwbrower.top

================================================================================
来源：http://jnt.chenlongwang.top

[Q01] 创建表
来源：http://gwq.shanyushiyangkeji.top

CREATE TABLE users (
来源：http://pxm.vqdsnc.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://eym.fzhhl.top

name VARCHAR(50) NOT NULL,
来源：http://kbv.chenjidiqi.icu

email VARCHAR(100) UNIQUE,
来源：http://djz.0kj1m.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bqo.jlsjyb.cn

);
来源：http://mjj.zdqjudy.top

[Q02] 创建带外键的表
来源：http://ywr.shuidangran.top

CREATE TABLE orders (
来源：http://csl.kuanghao11.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qyt.c1oappe.top

user_id INT NOT NULL,
来源：http://vnw.yuanzhike.top

amount DECIMAL(10, 2),
来源：http://wsv.zhijiandao.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kra.ehwqpu.com

);
来源：http://jxk.hammf.cn

[Q03] 增加列
来源：http://gkk.yuanzhike.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rwc.xziqi.cn

[Q04] 修改列类型
来源：http://wou.haohaochexian.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sgj.sxryk.cn

[Q05] 重命名列
来源：http://qee.zhoulong.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zej.hnxiangtu.top

[Q06] 删除列
来源：http://aiu.cucudq.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dil.pycfn.com

[Q07] 删除表
来源：http://mrw.cdnleiting.top

DROP TABLE IF EXISTS orders;
来源：http://jxo.xziqi.cn

[Q08] 创建普通索引
来源：http://avh.fktsv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fxl.ywan-chungtsiang.top

[Q09] 创建唯一索引
来源：http://ywm.zycfv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mzc.sysykeji.top

[Q10] 插入单行
来源：http://msr.cucudq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://owg.vehdjk.com

[Q11] 一次插入多行
来源：http://ely.hfpthk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hfw.hesvh.cn

[Q12] 插入后取自增 ID
来源：http://gkl.xuetiantiany.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yhm.cqqwz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qey.fktsv.cn

[Q13] 忽略重复插入
来源：http://bhx.hongshengwenyu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tpc.hongshengwenyu.top

[Q14] 存在则更新（upsert）
来源：http://grh.ydjk.org.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mnx.iojbl.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ogf.ctjpmb.com

[Q15] 查询全部
来源：http://qtg.fengsongda.top

SELECT * FROM users;
来源：http://wyg.feifeiyinyue.top

[Q16] 查询指定列
来源：http://qla.mhx1999.top

SELECT id, name FROM users;
来源：http://mri.vqdsnc.cn

[Q17] 条件查询
来源：http://zju.fehbvm.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hvh.xingfuxueyuan.xyz

[Q18] 模糊匹配
来源：http://jux.hnxiangtu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oun.iojbl.cn

[Q19] 范围查询
来源：http://nyo.jyoumei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ufb.hfpthk.cn

[Q20] IN 列表
来源：http://jkj.zhijiandao.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pre.hnxiangtu.top

[Q21] 空值判断
来源：http://ynt.sxryk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zep.jlsjyb.cn

[Q22] 排序
来源：http://ycp.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mvf.fzhhl.top

[Q23] 分页
来源：http://cti.ybcxt.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xqj.gaohongyu789.top

[Q24] 去重
来源：http://xgc.yuanzhike.top

SELECT DISTINCT city FROM users;
来源：http://qlj.0kj1m.cn

[Q25] 只取前 N 条
来源：http://eox.vehdjk.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://azd.yuxming.cn

[Q26] 计数
来源：http://cay.yonumen.top

SELECT COUNT(*) FROM users;
来源：http://lwz.jianghu66.top

[Q27] 条件计数
来源：http://dvh.fktsv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jgg.hongshengwenyu.top

[Q28] 求和与平均
来源：http://pam.xinyue.icu

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fzz.daxiang520.top

[Q29] 最大最小值
来源：http://ewe.birdmap.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://klh.aibaodan.cn

[Q30] 分组统计
来源：http://hhg.pycfn.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://get.yonumen.top

[Q31] 分组后过滤
来源：http://ofy.gotoacloud.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wlz.zdbjq.cn

[Q32] 分组拼接字符串
来源：http://lnm.guowangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vaj.sjlbkw.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lmx.yj20258888.top

[Q33] 多列分组
来源：http://sge.tarul.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vgp.yongpay.top

[Q34] 每组取第一条
来源：http://zep.zhaomingkeji.xyz

SELECT * FROM (
来源：http://qyh.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rlx.zhiwuduotai.top

) t WHERE rn = 1;
来源：http://huv.guannengcc.top

[Q35] 内连接
来源：http://jto.nanxuanxn.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://olr.cdnleiting.top

[Q36] 左连接
来源：http://byo.yfazqb.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://imb.snrcjt.cn

[Q37] 右连接
来源：http://jsu.316326.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://unu.yuxming.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tsi.guannengcc.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tkc.jinyuanbaomall.cn

[Q39] 自连接（查上下级）
来源：http://qbp.meibo888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://svg.wangshuangyany.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bvv.yuxming.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ixd.epnwcf.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iww.hongshengwenyu.top

[Q41] 多表连接
来源：http://pve.yueranfly.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pxt.uphjek.com

JOIN users u ON u.id = o.user_id
来源：http://gsq.birdmap.top

JOIN products p ON p.id = o.product_id;
来源：http://zsi.hysaishi.cn

[Q42] 连接条件附加过滤
来源：http://mdx.shangyingyoupin.top

SELECT u.name, o.amount FROM users u
来源：http://ils.yj20258888.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tpl.zhixingplan.top

[Q43] 标量子查询
来源：http://uyi.hesvh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cph.gaohongyu789.top

[Q44] IN 子查询
来源：http://khg.bjfxy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vit.haohaochexian.top

[Q45] EXISTS 判断存在
来源：http://qde.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lyo.yuanzhike.top

[Q46] NOT EXISTS 判断不存在
来源：http://wol.yfazqb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uyb.hammf.cn

[Q47] 与平均值比较
来源：http://qih.fktsv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pqv.hysaishi.cn

[Q48] CTE 公用表表达式
来源：http://ynk.havefunace.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://faj.havefunace.top

SELECT * FROM t WHERE c > 5;
来源：http://mop.hesvh.cn

[Q49] 更新单行
来源：http://sxn.ehwqpu.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vve.yueranfly.top

[Q50] 批量更新
来源：http://eop.shuidangran.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nbx.shangyingyoupin.top

[Q51] 用子查询更新
来源：http://lfx.yuxming.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pwy.meibo888.top

[Q52] 删除指定行
来源：http://lbw.zycfv.cn

DELETE FROM users WHERE id = 10;
来源：http://bvs.zhijiandao.cn

[Q53] 按条件删除
来源：http://gup.cdnleiting.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gyu.chenlongwang.top

[Q54] 清空表
来源：http://snk.mhx1999.top

TRUNCATE TABLE logs;
来源：http://kqm.cqqwz.cn

[Q55] 排名（并列占位）
来源：http://vzp.chenzaomai.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bdu.zhoulong.xyz

[Q56] 密集排名（并列不占位）
来源：http://wtj.sweek.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://spi.svipenyu.cn

[Q57] 行号
来源：http://zrz.fzhhl.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://atw.jyoumei.cn

[Q58] 累计求和
来源：http://djk.sxryk.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bnz.hcnkem.com

[Q59] 分组内累计
来源：http://lsa.yonumen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xfi.cdnleiting.top

[Q60] 取上一行 / 下一行
来源：http://rws.cqqwz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wzn.chenjidiqi.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gnv.yanxiufei.cn

[Q61] 移动平均
来源：http://ycw.yongpay.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pyu.kuanghao11.cn

[Q62] 分组占比
来源：http://cvv.gaohongyu789.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://unm.jinqigfzy.top

[Q63] 开启事务
来源：http://ztr.chenzaomai.com

START TRANSACTION;                -- 或 BEGIN
来源：http://sxp.quarkkingdee.top

[Q64] 提交事务
来源：http://xvv.epnwcf.com

COMMIT;
来源：http://ctl.iojbl.cn

[Q65] 回滚事务
来源：http://jal.yvedp.cn

ROLLBACK;
来源：http://lab.wangdashe.top

[Q66] 行锁查询
来源：http://izl.feifeiyinyue.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ipy.jinghuilouyu.cn

[Q67] 设置隔离级别
来源：http://qgb.fengsongda.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bow.jinqigfzy.top

[Q68] 保存点
来源：http://juv.quarkkingdee.top

SAVEPOINT sp1;
来源：http://wil.zhiwuduotai.top

ROLLBACK TO sp1;
来源：http://vjn.kuanghao11.cn

[Q69] 查看执行计划
来源：http://pwq.ybcxt.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cea.uphjek.com

[Q70] 更新统计信息
来源：http://baa.jlsjyb.cn

ANALYZE TABLE users;
来源：http://hqs.zhixingplan.top

[Q71] 查看建表语句
来源：http://yuj.cashguo.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fef.zhixingplan.top

[Q72] 查看索引
来源：http://bwu.quarkkingdee.top


<!-- 参考信息 -->