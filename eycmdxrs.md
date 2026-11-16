代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://opa.fehbvm.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nyd.yuxming.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lfo.jyoumei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qgb.aibaodan.cn

================================================================================
来源：http://odq.tanke756.top

O. 并发与异步
来源：http://yzu.mhx1999.top

================================================================================
来源：http://xpx.tanke756.top

[O01] 启动一个线程
来源：http://hxv.uphjek.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://izs.wangdashe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ymq.shuidangran.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mis.bbcook.cn

TS:   // 同 JS
来源：http://pyg.ydzc1.top

Java: new Thread(() -> f()).start()
来源：http://mml.vehdjk.com

Go:   go f()
来源：http://lai.xylfe.cn

Ruby: Thread.new { f }
来源：http://fqu.jiagoushi.top

C#:   Task.Run(() => F());
来源：http://wuz.shangyingyoupin.top

[O02] 使用线程池
来源：http://tcp.ybcxt.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sce.yanxiufei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mdk.yueranfly.top

JS:   // worker_threads 线程池
来源：http://dbr.cashguo.top

TS:   // worker_threads 线程池
来源：http://pxw.yangfankeji.com

Java: Executors.newFixedThreadPool(4)
来源：http://kqp.316326.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://swo.ehwqpu.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://usw.xuanzx.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vxh.wangdashe.top

[O03] 加锁保护共享数据
来源：http://axo.jinqigfzy.top

Py:   with lock: shared += 1
来源：http://nwj.fehbvm.com

PHP:  // 用 flock() 做文件锁
来源：http://qqp.quarkkingdee.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://max.cucudq.cn

TS:   // 同 JS
来源：http://hyv.hesvh.cn

Java: synchronized (this) { shared++; }
来源：http://nra.shanyushiyangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://itg.yj20258.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://fku.nanxuanxn.top

C#:   lock (gate) { shared++; }
来源：http://kzg.hammf.cn

[O04] 定义异步函数并等待
来源：http://wgo.ydzc1.top

Py:   async def f():⏎    await g()
来源：http://ngn.gaohongyu789.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tts.fengsongda.top

JS:   async function f() { await g(); }
来源：http://hwm.hammf.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rof.fzhhl.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xjh.hfpthk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qzy.dashuyun.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ihf.vqdsnc.cn

C#:   async Task F() { await G(); }
来源：http://nmj.haohaochexian.top

[O05] 并发执行并等待全部完成
来源：http://cnz.hongshengwenyu.top

Py:   asyncio.gather(*tasks)
来源：http://lte.hywenlv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zvu.yj20258.top

JS:   await Promise.all(tasks)
来源：http://awx.zhengqikj.top

TS:   await Promise.all(tasks)
来源：http://rqj.havefunace.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sxr.guannengcc.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cxz.sweek.top

Ruby: threads.map(&:join)
来源：http://uid.zhengqikj.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nhz.fzhhl.top

[O06] 使用进程池
来源：http://kly.jinqigufen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yyj.shanyushiyangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://lvr.snrcjt.cn

JS:   // child_process / cluster 模块
来源：http://lnn.quarkkingdee.top

TS:   // child_process / cluster 模块
来源：http://iso.aibaodan.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rug.jlsjyb.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yfm.yangfankeji.com

Ruby: // fork 块
来源：http://dqm.hammf.cn

C#:   Parallel.For
来源：http://zxv.guannengcc.top

================================================================================
来源：http://xmr.jlsjyb.cn

P. 常用工具函数
来源：http://epq.shanyushiyangkeji.top

================================================================================
来源：http://ned.andypj.xyz

[P01] 生成 UUID
来源：http://fzf.sjlbkw.cn

Py:   str(uuid.uuid4())
来源：http://cyg.shzxlz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gjv.meibo888.top

JS:   crypto.randomUUID()
来源：http://rce.haohaochexian.top

TS:   crypto.randomUUID()
来源：http://zsu.meibo888.top

Java: UUID.randomUUID().toString()
来源：http://xst.cucudq.cn

Go:   // 用 github.com/google/uuid
来源：http://trx.smart0.xyz

Ruby: SecureRandom.uuid
来源：http://nrr.zhaomingkeji.xyz

C#:   Guid.NewGuid().ToString()
来源：http://dnx.bbcook.cn

[P02] MD5 / SHA256 摘要
来源：http://mjq.yuanzhike.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kja.daria6918.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wvz.cheryme.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xhh.shanyushiyangtech.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://und.jyoumei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mls.0kj1m.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cgs.wangshuangyany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://whg.9152youxi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mim.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://dtg.zycfv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zsn.daria6918.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kzy.svipenyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xgw.pengpengdd.cyou

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rrr.zhengqikj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vpz.jianghu66.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qos.xziqi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://din.ehwqpu.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qrm.feifeiyinyue.top

[P04] 求长度
来源：http://sgt.jqgufenzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nht.hysaishi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hwn.ppjwa.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://upi.bjfxy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oin.sweek.top

Java: list.size();  map.size();  s.length()
来源：http://xqi.9152youxi.cn

Go:   len(arr);  len(m)
来源：http://rvo.jqgufenzy.top

Ruby: x.length;  x.size
来源：http://exr.jqgfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gvv.xziqi.cn

[P05] 判断两个对象内容是否相等
来源：http://llf.xylfe.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tbn.zhaomingkeji.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gyz.nanxuanxn.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fxj.nwbrower.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tug.tanke756.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lbt.fzhhl.top

Go:   reflect.DeepEqual(a, b)
来源：http://qzh.yanxiufei.cn

Ruby: a == b
来源：http://hgn.jianghu66.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wvm.andypj.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zmr.jqgufenzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lyn.sysykeji.top

PHP:  if (empty($x)) {}
来源：http://cbv.wangshuangyany.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xpz.hongshengwenyu.top

TS:   if (x == null) {}
来源：http://era.gaohongyu789.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fsz.hcnkem.com

Go:   if x == nil {}
来源：http://xwy.nanxuanxn.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://avr.pycfn.com

C#:   if (x is null) {}
来源：http://vdg.dianchejie.cn

[P07] 防抖与节流
来源：http://per.hcnkem.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fig.quarkkingdee.top

PHP:  // 手写时间戳比较
来源：http://laq.kuanghao11.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ens.shanyushiyangtech.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gqj.yongpay.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xja.0kj1m.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cqj.pycfn.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://hkn.fehbvm.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dqo.jinqigfzy.top

[P08] 处理浮点精度问题
来源：http://ykr.tarul.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vym.feifeiyinyue.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://etq.quarkkingdee.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fjc.jlsjyb.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://grv.bbcook.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ikd.meibo888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kmf.pengpengdd.cyou

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jcb.fktsv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lvh.guannengcc.top

================================================================================
来源：http://eze.52xcode.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xgp.zhiwuduotai.top

================================================================================
来源：http://sto.yuanzhike.top

[Q01] 创建表
来源：http://thl.shanyushiyangkeji.top

CREATE TABLE users (
来源：http://hco.daria6918.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://chu.xingfuxueyuan.xyz

name VARCHAR(50) NOT NULL,
来源：http://wma.yj202588.top

email VARCHAR(100) UNIQUE,
来源：http://bno.chenlongwang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wsn.hesvh.cn

);
来源：http://hsw.sysykeji.top

[Q02] 创建带外键的表
来源：http://een.jiagoushi.top

CREATE TABLE orders (
来源：http://kkm.feifeiyinyue.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zlf.316326.xyz

user_id INT NOT NULL,
来源：http://vrh.havefunace.top

amount DECIMAL(10, 2),
来源：http://pvs.svipenyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sne.9152youxi.cn

);
来源：http://lps.hysaishi.cn

[Q03] 增加列
来源：http://twp.sweek.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zqf.xuetiantiany.cn

[Q04] 修改列类型
来源：http://hrl.svipenyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lwv.xuetiantiany.cn

[Q05] 重命名列
来源：http://ohl.hesvh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qcg.pycfn.com

[Q06] 删除列
来源：http://dod.sjlbkw.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rfn.yj202588.top

[Q07] 删除表
来源：http://zii.ywan-chungtsiang.top

DROP TABLE IF EXISTS orders;
来源：http://wof.hongshengwenyu.top

[Q08] 创建普通索引
来源：http://vmv.yj20258888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ehm.zhongyouzk.top

[Q09] 创建唯一索引
来源：http://ifr.jiagoushi.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jqw.zhixingplan.top

[Q10] 插入单行
来源：http://egj.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iaj.zycfv.cn

[Q11] 一次插入多行
来源：http://rsb.jianghu66.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dlx.snrcjt.cn

[Q12] 插入后取自增 ID
来源：http://abm.tianlin.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://gxe.mhx1999.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bul.gaohongyu789.top

[Q13] 忽略重复插入
来源：http://phi.daxiang520.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://umj.cdnleiting.top

[Q14] 存在则更新（upsert）
来源：http://qaz.xuanzx.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ins.dashuyun.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zhs.wangdashe.top

[Q15] 查询全部
来源：http://yua.birdmap.top

SELECT * FROM users;
来源：http://xlz.hnqzz.top

[Q16] 查询指定列
来源：http://jok.gotoacloud.top

SELECT id, name FROM users;
来源：http://ojj.chenzaomai.com

[Q17] 条件查询
来源：http://dln.pycfn.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xkh.gaohongyu789.top

[Q18] 模糊匹配
来源：http://nhj.gzhubu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wwq.fanxiaobao.xyz

[Q19] 范围查询
来源：http://fvp.fengsongda.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://peq.ywan-chungtsiang.top

[Q20] IN 列表
来源：http://fes.nwbrower.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cgz.zhoulong.xyz

[Q21] 空值判断
来源：http://rgc.cqqwz.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mni.jinghuilouyu.cn

[Q22] 排序
来源：http://wvy.pengpengdd.cyou

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lfw.yuanzhike.top

[Q23] 分页
来源：http://iac.hesvh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://atr.gotoacloud.top

[Q24] 去重
来源：http://pih.ctjpmb.com

SELECT DISTINCT city FROM users;
来源：http://xms.52xcode.cn

[Q25] 只取前 N 条
来源：http://ylp.zdqjudy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uxt.chenlongwang.top

[Q26] 计数
来源：http://pot.aibaodan.cn

SELECT COUNT(*) FROM users;
来源：http://tqn.zhongyouzk.top

[Q27] 条件计数
来源：http://gdt.bjfxy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ofo.ehwqpu.com

[Q28] 求和与平均
来源：http://hnn.sysykeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rgy.aizwys.cn

[Q29] 最大最小值
来源：http://hpl.epnwcf.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://piy.tarul.cn

[Q30] 分组统计
来源：http://tll.jqgufenzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hdt.nwbrower.top

[Q31] 分组后过滤
来源：http://qnv.vehdjk.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mxj.jinqigfzy.top

[Q32] 分组拼接字符串
来源：http://rbr.iojbl.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://aav.aibaodan.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rxv.jinghuilouyu.cn

[Q33] 多列分组
来源：http://rjr.aizwys.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sof.tanke756.top

[Q34] 每组取第一条
来源：http://ovt.c1oappe.top

SELECT * FROM (
来源：http://xyo.haohaochexian.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vsl.smart0.xyz

) t WHERE rn = 1;
来源：http://ilx.zhijiandao.cn

[Q35] 内连接
来源：http://tif.fzhhl.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://las.iojbl.cn

[Q36] 左连接
来源：http://ouj.daria6918.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://oyy.xinyue.icu

[Q37] 右连接
来源：http://ijj.zhixingplan.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kfz.haohaochexian.top

[Q38] 全外连接（PostgreSQL）
来源：http://sbd.hesvh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wic.fengsongda.top

[Q39] 自连接（查上下级）
来源：http://mtp.wangdashe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://enq.gzhubu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bqn.yangfankeji.com

[Q40] 交叉连接（笛卡尔积）
来源：http://gjw.jinqigufen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gtn.yanxiufei.cn

[Q41] 多表连接
来源：http://llt.tian-w.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hnr.316326.xyz

JOIN users u ON u.id = o.user_id
来源：http://zux.52xcode.cn

JOIN products p ON p.id = o.product_id;
来源：http://tke.zhixingplan.top

[Q42] 连接条件附加过滤
来源：http://sys.shzxlz.cn

SELECT u.name, o.amount FROM users u
来源：http://lqg.jinqigufen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oei.havefunace.top

[Q43] 标量子查询
来源：http://ixc.hywenlv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rgo.yj20258.top

[Q44] IN 子查询
来源：http://bls.xziqi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://loa.daria6918.cn

[Q45] EXISTS 判断存在
来源：http://jxx.hfpthk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qdj.jiagoushi.top

[Q46] NOT EXISTS 判断不存在
来源：http://qvh.daxiang520.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://onz.shuidangran.top

[Q47] 与平均值比较
来源：http://iay.vehdjk.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kjc.havefunace.top

[Q48] CTE 公用表表达式
来源：http://rnu.shanyushiyangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dhg.yj20258888.top

SELECT * FROM t WHERE c > 5;
来源：http://nto.sufxvd.cn

[Q49] 更新单行
来源：http://vta.redwolf501.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mnl.gaohongyu789.top

[Q50] 批量更新
来源：http://mgo.hesvh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tgz.zhijiandao.cn

[Q51] 用子查询更新
来源：http://acc.nanxuanxn.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dvx.havefunace.top

[Q52] 删除指定行
来源：http://pej.cdnleiting.top

DELETE FROM users WHERE id = 10;
来源：http://yfj.pengpengdd.cyou

[Q53] 按条件删除
来源：http://zcx.52xcode.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ubq.yongpay.top

[Q54] 清空表
来源：http://ooi.bjfxy.top

TRUNCATE TABLE logs;
来源：http://iej.jiagoushi.top

[Q55] 排名（并列占位）
来源：http://kna.yangfankeji.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mis.fengsongda.top

[Q56] 密集排名（并列不占位）
来源：http://mtk.haohaochexian.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rfa.epnwcf.com

[Q57] 行号
来源：http://cwx.yanxiufei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zrm.yanxiufei.cn

[Q58] 累计求和
来源：http://ayj.tanke756.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://poy.fktsv.cn

[Q59] 分组内累计
来源：http://nxi.316326.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hvi.kuanghao11.cn

[Q60] 取上一行 / 下一行
来源：http://pzd.bjfxy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xhh.yuanzhike.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rpg.jlsjyb.cn

[Q61] 移动平均
来源：http://pfc.guowangkeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rkq.yuxming.cn

[Q62] 分组占比
来源：http://wwn.gogol.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nzb.aibaodan.cn

[Q63] 开启事务
来源：http://lgg.fehbvm.com

START TRANSACTION;                -- 或 BEGIN
来源：http://hzk.aizwys.cn

[Q64] 提交事务
来源：http://vre.zdqjudy.top

COMMIT;
来源：http://lly.ppjwa.cn

[Q65] 回滚事务
来源：http://nyj.cashguo.top

ROLLBACK;
来源：http://dbo.yj202588.top

[Q66] 行锁查询
来源：http://lqt.gaohongyu789.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pxl.yuanzhike.top

[Q67] 设置隔离级别
来源：http://tqk.daxiang520.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qqt.chenlongwang.top

[Q68] 保存点
来源：http://rxs.zhoulong.xyz

SAVEPOINT sp1;
来源：http://qvs.redwolf501.top

ROLLBACK TO sp1;
来源：http://idq.hammf.cn

[Q69] 查看执行计划
来源：http://elf.ehwqpu.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://aos.yj20258888.top

[Q70] 更新统计信息
来源：http://nai.nanxinkj.top


<!-- 参考信息 -->