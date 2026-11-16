代发 wailian999

PHP:  // 手写递归函数
来源：http://ufj.hongshengwenyu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ngg.hywenlv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bjc.vehdjk.com

Java: // 手写递归
来源：http://cac.cqqwz.cn

Go:   // 手写递归
来源：http://kui.uphjek.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xvd.ydjk.org.cn

C#:   // 手写递归
来源：http://jvl.pengpengdd.cyou

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jwk.fktsv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lok.316326.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qrm.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rea.fzhhl.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yoa.daxiang520.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fmj.hammf.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ute.yfazqb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xkd.yuxming.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pwi.gaohongyu789.top

================================================================================
来源：http://ufk.tian-w.cn

O. 并发与异步
来源：http://zjz.hesvh.cn

================================================================================
来源：http://fan.cdnleiting.top

[O01] 启动一个线程
来源：http://cxt.dashuyun.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pff.wangshuangyany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ooz.havefunace.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hjx.wangdashe.top

TS:   // 同 JS
来源：http://yhl.gaohongyu789.top

Java: new Thread(() -> f()).start()
来源：http://rwv.vqdsnc.cn

Go:   go f()
来源：http://ghp.chenzaomai.com

Ruby: Thread.new { f }
来源：http://reo.hcnkem.com

C#:   Task.Run(() => F());
来源：http://jqg.tanke756.top

[O02] 使用线程池
来源：http://gzj.nwbrower.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://goe.svipenyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://upm.52xcode.cn

JS:   // worker_threads 线程池
来源：http://lhx.fanxiaobao.xyz

TS:   // worker_threads 线程池
来源：http://ndu.bjfxy.top

Java: Executors.newFixedThreadPool(4)
来源：http://mig.jinqigufen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dwk.feifeiyinyue.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rwx.zhengqikj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nlo.yuanzhike.top

[O03] 加锁保护共享数据
来源：http://btt.yfazqb.com

Py:   with lock: shared += 1
来源：http://hor.ybcxt.top

PHP:  // 用 flock() 做文件锁
来源：http://pag.xuetiantiany.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dir.shanyushiyangtech.top

TS:   // 同 JS
来源：http://jkk.hesvh.cn

Java: synchronized (this) { shared++; }
来源：http://xbs.sxryk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://afd.cashguo.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rrr.0kj1m.cn

C#:   lock (gate) { shared++; }
来源：http://wxu.redwolf501.top

[O04] 定义异步函数并等待
来源：http://ffd.wangdashe.top

Py:   async def f():⏎    await g()
来源：http://vlj.fzhhl.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fkg.smart0.xyz

JS:   async function f() { await g(); }
来源：http://jag.ydzc1.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gfv.andypj.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sjj.cqqwz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://opy.snrcjt.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lot.vqdsnc.cn

C#:   async Task F() { await G(); }
来源：http://wsf.uphjek.com

[O05] 并发执行并等待全部完成
来源：http://cdu.zhijiandao.cn

Py:   asyncio.gather(*tasks)
来源：http://zqt.c1oappe.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mwn.quarkkingdee.top

JS:   await Promise.all(tasks)
来源：http://doi.yanxiufei.cn

TS:   await Promise.all(tasks)
来源：http://fdw.hnqzz.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oha.zhijiandao.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hdh.jianghu66.top

Ruby: threads.map(&:join)
来源：http://biy.xinyue.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://mkj.bjfxy.top

[O06] 使用进程池
来源：http://uoo.jlsjyb.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hor.yvedp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://flf.svipenyu.cn

JS:   // child_process / cluster 模块
来源：http://dxt.xinyue.icu

TS:   // child_process / cluster 模块
来源：http://fac.ivvv.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vgb.zycfv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mgc.hnxiangtu.top

Ruby: // fork 块
来源：http://tsn.9152youxi.cn

C#:   Parallel.For
来源：http://ufr.jiagoushi.top

================================================================================
来源：http://qpz.cucudq.cn

P. 常用工具函数
来源：http://qvt.fzhhl.top

================================================================================
来源：http://nzb.zhaomingkeji.xyz

[P01] 生成 UUID
来源：http://ehd.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://cpc.cucudq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sbp.xinyue.icu

JS:   crypto.randomUUID()
来源：http://lfr.tarul.cn

TS:   crypto.randomUUID()
来源：http://jqj.gzhubu.top

Java: UUID.randomUUID().toString()
来源：http://fko.vqdsnc.cn

Go:   // 用 github.com/google/uuid
来源：http://snt.sjlbkw.cn

Ruby: SecureRandom.uuid
来源：http://ucq.iojbl.cn

C#:   Guid.NewGuid().ToString()
来源：http://flq.tian-w.cn

[P02] MD5 / SHA256 摘要
来源：http://hrd.snrcjt.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://syv.shanyushiyangtech.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bfl.ywan-chungtsiang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rff.fktsv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ftd.tanke756.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ykc.tanke756.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ulp.nanxuanxn.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uax.yonumen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kws.feifeiyinyue.top

[P03] 生成短随机字符串
来源：http://nfa.0kj1m.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hqy.zdqjudy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vnd.nanxinkj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fjt.xylfe.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xut.daxiang520.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lkn.daxiang520.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ldj.jyoumei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jov.chenjidiqi.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lmg.sjlbkw.cn

[P04] 求长度
来源：http://vko.quarkkingdee.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rmb.ybcxt.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qvm.tian-w.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ffa.shanyushiyangtech.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gdi.guowangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://rhw.ybcxt.top

Go:   len(arr);  len(m)
来源：http://jtj.xinyue.icu

Ruby: x.length;  x.size
来源：http://bhn.andypj.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://taj.nanxuanxn.top

[P05] 判断两个对象内容是否相等
来源：http://epk.xingfuxueyuan.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://png.xuetiantiany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vxx.xuetiantiany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xzr.52xcode.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kdr.sweek.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eqz.yj20258.top

Go:   reflect.DeepEqual(a, b)
来源：http://ghv.cdnleiting.top

Ruby: a == b
来源：http://scx.shanyushiyangtech.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dtj.yonumen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vvy.bbcook.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fji.nanxuanxn.top

PHP:  if (empty($x)) {}
来源：http://hgb.0kj1m.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iru.aibaodan.cn

TS:   if (x == null) {}
来源：http://hem.hcnkem.com

Java: if (x == null || x.isEmpty()) {}
来源：http://dtx.ydjk.org.cn

Go:   if x == nil {}
来源：http://jts.shanyushiyangtech.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zpy.uphjek.com

C#:   if (x is null) {}
来源：http://zyk.yvedp.cn

[P07] 防抖与节流
来源：http://axl.sjlbkw.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xhk.shangyingyoupin.top

PHP:  // 手写时间戳比较
来源：http://sao.pengpengdd.cyou

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mbr.52xcode.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zqo.zdbjq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://btn.hcnkem.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sgt.xuanzx.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://bnm.sweek.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xbg.iojbl.cn

[P08] 处理浮点精度问题
来源：http://oer.sjlbkw.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://txg.ywan-chungtsiang.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dvr.sweek.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uae.sweek.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mxf.birdmap.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rde.gzhubu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://had.cdnleiting.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wxd.cqqwz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gfx.havefunace.top

================================================================================
来源：http://ukl.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nnv.fanxiaobao.xyz

================================================================================
来源：http://skk.yuanzhike.top

[Q01] 创建表
来源：http://occ.svipenyu.cn

CREATE TABLE users (
来源：http://clv.zycfv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ihg.jianghu66.top

name VARCHAR(50) NOT NULL,
来源：http://auw.shanyushiyangtech.top

email VARCHAR(100) UNIQUE,
来源：http://yto.smart0.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xed.dashuyun.cn

);
来源：http://irl.zdqjudy.top

[Q02] 创建带外键的表
来源：http://aha.wangdashe.top

CREATE TABLE orders (
来源：http://yos.jqgufenzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pfo.daria6918.cn

user_id INT NOT NULL,
来源：http://mjb.mhx1999.top

amount DECIMAL(10, 2),
来源：http://wps.ppjwa.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ohn.jiagoushi.top

);
来源：http://cva.jqgfzy.top

[Q03] 增加列
来源：http://yuz.cqqwz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xap.iojbl.cn

[Q04] 修改列类型
来源：http://yfl.daxiang520.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://inb.gotoacloud.top

[Q05] 重命名列
来源：http://sek.chenzaomai.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mxq.ehwqpu.com

[Q06] 删除列
来源：http://akj.jianghu66.top

ALTER TABLE users DROP COLUMN age;
来源：http://cqr.fktsv.cn

[Q07] 删除表
来源：http://hlj.sufxvd.cn

DROP TABLE IF EXISTS orders;
来源：http://aoy.aibaodan.cn

[Q08] 创建普通索引
来源：http://cop.fzhhl.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hqr.mhx1999.top

[Q09] 创建唯一索引
来源：http://koc.birdmap.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cvd.yueranfly.top

[Q10] 插入单行
来源：http://prb.haohaochexian.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vmf.xuanzx.com

[Q11] 一次插入多行
来源：http://ket.xziqi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xke.xuanzx.com

[Q12] 插入后取自增 ID
来源：http://rwh.tianlin.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://wsf.guannengcc.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fxz.cdnleiting.top

[Q13] 忽略重复插入
来源：http://bqw.cdnleiting.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tdm.sweek.top

[Q14] 存在则更新（upsert）
来源：http://cxh.shanyushiyangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uwl.cdnleiting.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jpd.hnxiangtu.top

[Q15] 查询全部
来源：http://xwu.cdnleiting.top

SELECT * FROM users;
来源：http://qai.zhengqikj.top

[Q16] 查询指定列
来源：http://gra.yueranfly.top

SELECT id, name FROM users;
来源：http://qvz.cucudq.cn

[Q17] 条件查询
来源：http://mgk.snrcjt.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jxi.fehbvm.com

[Q18] 模糊匹配
来源：http://azu.iojbl.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://trw.xinyue.icu

[Q19] 范围查询
来源：http://ugm.yueranfly.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ldr.hywenlv.cn

[Q20] IN 列表
来源：http://enr.zhijiandao.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uvk.wangdashe.top

[Q21] 空值判断
来源：http://awc.ydjk.org.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://auk.snrcjt.cn

[Q22] 排序
来源：http://dnn.jinqigfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mmj.yvedp.cn

[Q23] 分页
来源：http://pqj.cheryme.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pla.ydzc1.top

[Q24] 去重
来源：http://keg.yongpay.top

SELECT DISTINCT city FROM users;
来源：http://dqc.fzhhl.top

[Q25] 只取前 N 条
来源：http://ozi.shanyushiyangtech.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gzh.zdbjq.cn

[Q26] 计数
来源：http://qoq.jianghu66.top

SELECT COUNT(*) FROM users;
来源：http://nzo.yj202588.top

[Q27] 条件计数
来源：http://qgo.aizwys.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xcq.meibo888.top

[Q28] 求和与平均
来源：http://szg.ywan-chungtsiang.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cij.fanxiaobao.xyz

[Q29] 最大最小值
来源：http://mbb.ppjwa.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://klw.jinyuanbaomall.cn

[Q30] 分组统计
来源：http://mae.zhongyouzk.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nzi.jqgfzy.top

[Q31] 分组后过滤
来源：http://sln.shzxlz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://czd.zdqjudy.top

[Q32] 分组拼接字符串
来源：http://hhj.xinyue.icu

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://atw.xuetiantiany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ylh.ctjpmb.com

[Q33] 多列分组
来源：http://npu.hnqzz.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gef.quarkkingdee.top

[Q34] 每组取第一条
来源：http://yse.gaohongyu789.top

SELECT * FROM (
来源：http://ssi.epnwcf.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://opo.ehwqpu.com

) t WHERE rn = 1;
来源：http://crh.daxiang520.top

[Q35] 内连接
来源：http://jpu.yj20258888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gzd.hnxiangtu.top

[Q36] 左连接
来源：http://hds.gotoacloud.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://taj.hongshengwenyu.top

[Q37] 右连接
来源：http://nyd.ybcxt.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cxw.fehbvm.com

[Q38] 全外连接（PostgreSQL）
来源：http://lks.cashguo.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iyt.yangfankeji.com

[Q39] 自连接（查上下级）
来源：http://whk.redwolf501.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qbk.havefunace.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xfr.jqgfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pqr.cheryme.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ewq.feifeiyinyue.top

[Q41] 多表连接
来源：http://spo.aizwys.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rgw.316326.xyz

JOIN users u ON u.id = o.user_id
来源：http://swf.dianchejie.cn

JOIN products p ON p.id = o.product_id;
来源：http://ugk.9152youxi.cn

[Q42] 连接条件附加过滤
来源：http://bgq.9152youxi.cn

SELECT u.name, o.amount FROM users u
来源：http://zsx.yonumen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uyn.yangfankeji.com

[Q43] 标量子查询
来源：http://qwb.9152youxi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ycg.ydzc1.top

[Q44] IN 子查询
来源：http://vzq.zdqjudy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qtw.yanxiufei.cn

[Q45] EXISTS 判断存在
来源：http://lll.chenlongwang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wsr.snrcjt.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dmt.jinghuilouyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cwi.shuidangran.top

[Q47] 与平均值比较
来源：http://vmn.fehbvm.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xmr.jyoumei.cn

[Q48] CTE 公用表表达式
来源：http://kme.fzhhl.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://opm.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://egh.pycfn.com

[Q49] 更新单行
来源：http://tdf.shanyushiyangtech.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wtc.tianlin.xyz

[Q50] 批量更新
来源：http://tnw.zhijiandao.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ggx.tianlin.xyz

[Q51] 用子查询更新
来源：http://ctc.zdbjq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ozn.yfazqb.com

[Q52] 删除指定行
来源：http://fty.chenjidiqi.icu

DELETE FROM users WHERE id = 10;
来源：http://fbe.pycfn.com

[Q53] 按条件删除
来源：http://exr.yfazqb.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tic.cheryme.top

[Q54] 清空表
来源：http://jyw.jinyuanbaomall.cn

TRUNCATE TABLE logs;
来源：http://pvx.iojbl.cn

[Q55] 排名（并列占位）
来源：http://mla.sweek.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ups.aibaodan.cn

[Q56] 密集排名（并列不占位）
来源：http://cxo.yj20258888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xex.ehwqpu.com

[Q57] 行号
来源：http://ajc.jiagoushi.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gxu.yfazqb.com

[Q58] 累计求和
来源：http://jkd.chenjidiqi.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kmh.yfazqb.com

[Q59] 分组内累计
来源：http://cga.wangdashe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zxs.yangfankeji.com

[Q60] 取上一行 / 下一行
来源：http://rhm.yanxiufei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wwk.zhiwuduotai.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rio.tarul.cn

[Q61] 移动平均
来源：http://qyb.cucudq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rwr.yuxming.cn

[Q62] 分组占比
来源：http://nry.guannengcc.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zvz.yangfankeji.com

[Q63] 开启事务
来源：http://xzf.yanxiufei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wsr.316326.xyz

[Q64] 提交事务
来源：http://ygq.hnqzz.top

COMMIT;
来源：http://ghg.zhengqikj.top


<!-- 参考信息 -->