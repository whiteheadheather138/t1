代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rbl.yj20258888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aak.fehbvm.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hgs.hnqzz.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qnp.ehwqpu.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ymm.9152youxi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tgf.daxiang520.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://shm.shzxlz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fpr.yangfankeji.com

================================================================================
来源：http://muw.redwolf501.top

O. 并发与异步
来源：http://gxn.zdqjudy.top

================================================================================
来源：http://nje.daxiang520.top

[O01] 启动一个线程
来源：http://xxf.aizwys.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://myj.chenlongwang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://emc.feifeiyinyue.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://use.shanyushiyangtech.top

TS:   // 同 JS
来源：http://scw.fanxiaobao.xyz

Java: new Thread(() -> f()).start()
来源：http://hlk.jianghu66.top

Go:   go f()
来源：http://wxv.yuxming.cn

Ruby: Thread.new { f }
来源：http://vyj.aizwys.cn

C#:   Task.Run(() => F());
来源：http://mht.zhaomingkeji.xyz

[O02] 使用线程池
来源：http://aux.jianghu66.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sam.yj202588.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ddh.ctjpmb.com

JS:   // worker_threads 线程池
来源：http://nmg.xingfuxueyuan.xyz

TS:   // worker_threads 线程池
来源：http://byn.hammf.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sam.zhaomingkeji.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fdj.yanxiufei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vor.316326.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tid.zhiwuduotai.top

[O03] 加锁保护共享数据
来源：http://rlx.xinyue.icu

Py:   with lock: shared += 1
来源：http://ycz.cheryme.top

PHP:  // 用 flock() 做文件锁
来源：http://lth.zdqjudy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cnz.hcnkem.com

TS:   // 同 JS
来源：http://hua.tianlin.xyz

Java: synchronized (this) { shared++; }
来源：http://qea.xziqi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qxs.gzhubu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dqw.jiagoushi.top

C#:   lock (gate) { shared++; }
来源：http://ypa.hnqzz.top

[O04] 定义异步函数并等待
来源：http://bni.316326.xyz

Py:   async def f():⏎    await g()
来源：http://bnt.9152youxi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pti.chenjidiqi.icu

JS:   async function f() { await g(); }
来源：http://gla.jyoumei.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://azs.tanke756.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gyn.c1oappe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gur.shzxlz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ufx.ydjk.org.cn

C#:   async Task F() { await G(); }
来源：http://miq.svipenyu.cn

[O05] 并发执行并等待全部完成
来源：http://sqr.tanke756.top

Py:   asyncio.gather(*tasks)
来源：http://uyc.feifeiyinyue.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ole.shuidangran.top

JS:   await Promise.all(tasks)
来源：http://aao.smart0.xyz

TS:   await Promise.all(tasks)
来源：http://igf.aizwys.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sdb.hesvh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zfh.zycfv.cn

Ruby: threads.map(&:join)
来源：http://yhx.316326.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://nfa.shanyushiyangtech.top

[O06] 使用进程池
来源：http://btt.c1oappe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tfs.xziqi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yvl.cucudq.cn

JS:   // child_process / cluster 模块
来源：http://olj.yfazqb.com

TS:   // child_process / cluster 模块
来源：http://anq.0kj1m.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://udp.yj202588.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hqf.fehbvm.com

Ruby: // fork 块
来源：http://bzv.xylfe.cn

C#:   Parallel.For
来源：http://hrh.havefunace.top

================================================================================
来源：http://yjc.hesvh.cn

P. 常用工具函数
来源：http://wgl.zhongyouzk.top

================================================================================
来源：http://fwd.zhixingplan.top

[P01] 生成 UUID
来源：http://vii.yongpay.top

Py:   str(uuid.uuid4())
来源：http://emw.yj20258888.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mxr.guannengcc.top

JS:   crypto.randomUUID()
来源：http://kva.ywan-chungtsiang.top

TS:   crypto.randomUUID()
来源：http://mlz.shzxlz.cn

Java: UUID.randomUUID().toString()
来源：http://amj.zycfv.cn

Go:   // 用 github.com/google/uuid
来源：http://qki.daria6918.cn

Ruby: SecureRandom.uuid
来源：http://yvt.yj20258.top

C#:   Guid.NewGuid().ToString()
来源：http://mri.yueranfly.top

[P02] MD5 / SHA256 摘要
来源：http://hsk.hongshengwenyu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://irn.xuetiantiany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://smg.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jxe.daria6918.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aih.sufxvd.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cek.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pxz.sxryk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ugx.jianghu66.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://chv.hywenlv.cn

[P03] 生成短随机字符串
来源：http://swf.birdmap.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://awr.gogol.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rdy.zhaomingkeji.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zar.fehbvm.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hoz.daria6918.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://duh.zhiwuduotai.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pkb.chenzaomai.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://nyy.svipenyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://soc.yj202588.top

[P04] 求长度
来源：http://bbn.zdbjq.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fta.shangyingyoupin.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gya.shanyushiyangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hqj.shanyushiyangtech.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jbc.bbcook.cn

Java: list.size();  map.size();  s.length()
来源：http://qkl.chenjidiqi.icu

Go:   len(arr);  len(m)
来源：http://ltu.zhengqikj.top

Ruby: x.length;  x.size
来源：http://mta.yonumen.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lbh.zhijiandao.cn

[P05] 判断两个对象内容是否相等
来源：http://oqw.yj20258.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://bko.yj20258888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://une.gzhubu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://klz.dianchejie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kly.jyoumei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fxb.nanxuanxn.top

Go:   reflect.DeepEqual(a, b)
来源：http://svb.cdnleiting.top

Ruby: a == b
来源：http://ubr.cdnleiting.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yqd.jinghuilouyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mhr.fehbvm.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mml.cheryme.top

PHP:  if (empty($x)) {}
来源：http://nzu.sysykeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jgf.andypj.xyz

TS:   if (x == null) {}
来源：http://mhv.aizwys.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nid.fehbvm.com

Go:   if x == nil {}
来源：http://gky.shzxlz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qjj.jlsjyb.cn

C#:   if (x is null) {}
来源：http://vin.havefunace.top

[P07] 防抖与节流
来源：http://tds.ywan-chungtsiang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zih.yvedp.cn

PHP:  // 手写时间戳比较
来源：http://txu.zdbjq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bih.yanxiufei.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xjx.9152youxi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://new.nanxinkj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cdd.cashguo.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://tpq.ivvv.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gdq.fzhhl.top

[P08] 处理浮点精度问题
来源：http://tzu.zhaomingkeji.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://voj.yuanzhike.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zrg.ppjwa.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rrq.jlsjyb.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gmt.vqdsnc.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bdm.meibo888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hdw.jinqigufen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yfj.jianghu66.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://atp.xuetiantiany.cn

================================================================================
来源：http://pik.0kj1m.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eml.yuxming.cn

================================================================================
来源：http://rgx.aibaodan.cn

[Q01] 创建表
来源：http://abj.pengpengdd.cyou

CREATE TABLE users (
来源：http://hzi.jiagoushi.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nyg.yvedp.cn

name VARCHAR(50) NOT NULL,
来源：http://yft.52xcode.cn

email VARCHAR(100) UNIQUE,
来源：http://kqt.wangdashe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ffe.sxryk.cn

);
来源：http://pch.ybcxt.top

[Q02] 创建带外键的表
来源：http://vqu.kuanghao11.cn

CREATE TABLE orders (
来源：http://ety.yongpay.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bbu.yj20258.top

user_id INT NOT NULL,
来源：http://ljr.bbcook.cn

amount DECIMAL(10, 2),
来源：http://xlk.jlsjyb.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://taa.tian-w.cn

);
来源：http://uxd.hywenlv.cn

[Q03] 增加列
来源：http://ldx.shanyushiyangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mga.haohaochexian.top

[Q04] 修改列类型
来源：http://cab.birdmap.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dzx.hywenlv.cn

[Q05] 重命名列
来源：http://hqf.hnxiangtu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tzx.tian-w.cn

[Q06] 删除列
来源：http://caa.sysykeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://rgz.hysaishi.cn

[Q07] 删除表
来源：http://mfr.chenjidiqi.icu

DROP TABLE IF EXISTS orders;
来源：http://upv.hongshengwenyu.top

[Q08] 创建普通索引
来源：http://kkv.jianghu66.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pdd.zhiwuduotai.top

[Q09] 创建唯一索引
来源：http://wwt.jqgfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://aid.zhongyouzk.top

[Q10] 插入单行
来源：http://wbs.tianlin.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ggu.daxiang520.top

[Q11] 一次插入多行
来源：http://ryw.52xcode.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yns.sxryk.cn

[Q12] 插入后取自增 ID
来源：http://ufc.snrcjt.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ntf.havefunace.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yje.dashuyun.cn

[Q13] 忽略重复插入
来源：http://pzj.andypj.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zfr.hongshengwenyu.top

[Q14] 存在则更新（upsert）
来源：http://jbf.hammf.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pfi.guowangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rlp.hongshengwenyu.top

[Q15] 查询全部
来源：http://jqq.snrcjt.cn

SELECT * FROM users;
来源：http://hgv.fanxiaobao.xyz

[Q16] 查询指定列
来源：http://ibh.zhoulong.xyz

SELECT id, name FROM users;
来源：http://kby.nanxinkj.top

[Q17] 条件查询
来源：http://bth.hysaishi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iat.yj20258888.top

[Q18] 模糊匹配
来源：http://ywx.hnqzz.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ppl.cqqwz.cn

[Q19] 范围查询
来源：http://kox.bjfxy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://are.fktsv.cn

[Q20] IN 列表
来源：http://elx.daria6918.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pas.ctjpmb.com

[Q21] 空值判断
来源：http://dxk.zycfv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://umn.gaohongyu789.top

[Q22] 排序
来源：http://fka.bjfxy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qcr.52xcode.cn

[Q23] 分页
来源：http://jtp.zhixingplan.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qqe.yfazqb.com

[Q24] 去重
来源：http://rvi.zdqjudy.top

SELECT DISTINCT city FROM users;
来源：http://sti.zycfv.cn

[Q25] 只取前 N 条
来源：http://pqf.hongshengwenyu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fax.jlsjyb.cn

[Q26] 计数
来源：http://rqt.guowangkeji.top

SELECT COUNT(*) FROM users;
来源：http://tmq.jianghu66.top

[Q27] 条件计数
来源：http://gtu.kuanghao11.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://twg.birdmap.top

[Q28] 求和与平均
来源：http://jfw.zhixingplan.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dme.yongpay.top

[Q29] 最大最小值
来源：http://age.tianlin.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://zaa.shanyushiyangtech.top

[Q30] 分组统计
来源：http://xuq.ppjwa.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rzn.shangyingyoupin.top

[Q31] 分组后过滤
来源：http://yyg.cucudq.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bvs.jianghu66.top

[Q32] 分组拼接字符串
来源：http://ary.hnxiangtu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nmk.sxryk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tto.vqdsnc.cn

[Q33] 多列分组
来源：http://phi.ehwqpu.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://orb.yangfankeji.com

[Q34] 每组取第一条
来源：http://nsc.sweek.top

SELECT * FROM (
来源：http://fce.nanxinkj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vtn.ywan-chungtsiang.top

) t WHERE rn = 1;
来源：http://adj.gaohongyu789.top

[Q35] 内连接
来源：http://tpr.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qeb.jiagoushi.top

[Q36] 左连接
来源：http://ngo.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wfx.nwbrower.top

[Q37] 右连接
来源：http://xmv.yuanzhike.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wdz.yuxming.cn

[Q38] 全外连接（PostgreSQL）
来源：http://uhp.meibo888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iqv.sjlbkw.cn

[Q39] 自连接（查上下级）
来源：http://lhc.hnxiangtu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://vls.pycfn.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ush.smart0.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://cfg.9152youxi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oih.chenjidiqi.icu

[Q41] 多表连接
来源：http://klw.0kj1m.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://htf.ivvv.top

JOIN users u ON u.id = o.user_id
来源：http://wol.chenjidiqi.icu

JOIN products p ON p.id = o.product_id;
来源：http://wul.vqdsnc.cn

[Q42] 连接条件附加过滤
来源：http://glm.daxiang520.top

SELECT u.name, o.amount FROM users u
来源：http://oah.mhx1999.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jxc.zycfv.cn

[Q43] 标量子查询
来源：http://xng.smart0.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tft.zhengqikj.top

[Q44] IN 子查询
来源：http://pln.snrcjt.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://loo.mhx1999.top

[Q45] EXISTS 判断存在
来源：http://fzh.vqdsnc.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wmf.wangdashe.top

[Q46] NOT EXISTS 判断不存在
来源：http://bxc.zhaomingkeji.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ary.aibaodan.cn

[Q47] 与平均值比较
来源：http://otf.shzxlz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ebj.jianghu66.top

[Q48] CTE 公用表表达式
来源：http://gwh.cucudq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://juf.tianlin.xyz

SELECT * FROM t WHERE c > 5;
来源：http://frt.birdmap.top

[Q49] 更新单行
来源：http://teo.jinqigufen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hwg.tianlin.xyz

[Q50] 批量更新
来源：http://nvv.shanyushiyangtech.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fmo.nwbrower.top

[Q51] 用子查询更新
来源：http://knx.ydjk.org.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://krg.zhongyouzk.top

[Q52] 删除指定行
来源：http://ifo.jinqigufen.top

DELETE FROM users WHERE id = 10;
来源：http://pru.yj20258.top

[Q53] 按条件删除
来源：http://brp.tianlin.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kll.sjlbkw.cn

[Q54] 清空表
来源：http://csz.jinghuilouyu.cn

TRUNCATE TABLE logs;
来源：http://vzz.cheryme.top

[Q55] 排名（并列占位）
来源：http://ubx.gogol.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gfs.shanyushiyangtech.top

[Q56] 密集排名（并列不占位）
来源：http://ojr.vqdsnc.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://drd.jinqigfzy.top

[Q57] 行号
来源：http://fny.jianghu66.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xgx.yangfankeji.com

[Q58] 累计求和
来源：http://okr.fengsongda.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dgj.yonumen.top

[Q59] 分组内累计
来源：http://azh.fanxiaobao.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uhm.jinqigufen.top

[Q60] 取上一行 / 下一行
来源：http://das.yanxiufei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://adu.yj202588.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cav.bjfxy.top

[Q61] 移动平均
来源：http://arb.xylfe.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nho.yueranfly.top

[Q62] 分组占比
来源：http://kmz.bjfxy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dwb.pengpengdd.cyou

[Q63] 开启事务
来源：http://jwa.fehbvm.com

START TRANSACTION;                -- 或 BEGIN
来源：http://kui.cheryme.top

[Q64] 提交事务
来源：http://hex.snrcjt.cn

COMMIT;
来源：http://kes.wangshuangyany.cn

[Q65] 回滚事务
来源：http://jyb.chenlongwang.top

ROLLBACK;
来源：http://xii.dianchejie.cn

[Q66] 行锁查询
来源：http://hmj.jianghu66.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://abj.ydzc1.top

[Q67] 设置隔离级别
来源：http://fvp.gzhubu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hth.jinyuanbaomall.cn

[Q68] 保存点
来源：http://ibb.ywan-chungtsiang.top

SAVEPOINT sp1;
来源：http://rea.fengsongda.top


<!-- 参考信息 -->