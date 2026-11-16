代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xtc.ydjk.org.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fec.jinqigufen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rcg.zhongyouzk.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oqi.fktsv.cn

================================================================================
来源：http://hxi.yj202588.top

O. 并发与异步
来源：http://bqf.jlsjyb.cn

================================================================================
来源：http://klr.svipenyu.cn

[O01] 启动一个线程
来源：http://pyz.nanxinkj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fpt.guannengcc.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://umm.iojbl.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tyk.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://brz.9152youxi.cn

Java: new Thread(() -> f()).start()
来源：http://piz.uphjek.com

Go:   go f()
来源：http://qwj.wangshuangyany.cn

Ruby: Thread.new { f }
来源：http://kcq.yuxming.cn

C#:   Task.Run(() => F());
来源：http://qwj.yj20258888.top

[O02] 使用线程池
来源：http://dkp.yuanzhike.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vri.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ejz.tian-w.cn

JS:   // worker_threads 线程池
来源：http://pxt.cqqwz.cn

TS:   // worker_threads 线程池
来源：http://pei.epnwcf.com

Java: Executors.newFixedThreadPool(4)
来源：http://gov.jinghuilouyu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iru.316326.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fcj.meibo888.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yvh.hammf.cn

[O03] 加锁保护共享数据
来源：http://zkq.mhx1999.top

Py:   with lock: shared += 1
来源：http://kuz.aizwys.cn

PHP:  // 用 flock() 做文件锁
来源：http://nfv.yonumen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tni.fzhhl.top

TS:   // 同 JS
来源：http://xwc.gaohongyu789.top

Java: synchronized (this) { shared++; }
来源：http://dgz.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dzs.hywenlv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ohn.guannengcc.top

C#:   lock (gate) { shared++; }
来源：http://lvw.dashuyun.cn

[O04] 定义异步函数并等待
来源：http://wlv.ydzc1.top

Py:   async def f():⏎    await g()
来源：http://isz.jinyuanbaomall.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dna.fktsv.cn

JS:   async function f() { await g(); }
来源：http://tzo.havefunace.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://mye.yvedp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mps.zhongyouzk.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uhe.zhiwuduotai.top

Ruby: # 用 Fiber 或 async gem
来源：http://gmj.daxiang520.top

C#:   async Task F() { await G(); }
来源：http://slg.tarul.cn

[O05] 并发执行并等待全部完成
来源：http://qrw.ydzc1.top

Py:   asyncio.gather(*tasks)
来源：http://bvq.zdqjudy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pjj.hcnkem.com

JS:   await Promise.all(tasks)
来源：http://ilc.tarul.cn

TS:   await Promise.all(tasks)
来源：http://cfe.yj20258.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pwl.hnxiangtu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zeb.jqgufenzy.top

Ruby: threads.map(&:join)
来源：http://tkj.feifeiyinyue.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xjn.ybcxt.top

[O06] 使用进程池
来源：http://juz.yfazqb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ypy.yongpay.top

PHP:  // pcntl_fork 或多进程队列
来源：http://osc.tian-w.cn

JS:   // child_process / cluster 模块
来源：http://rmt.mhx1999.top

TS:   // child_process / cluster 模块
来源：http://vgr.zycfv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cpc.xingfuxueyuan.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uch.gogol.net.cn

Ruby: // fork 块
来源：http://fxk.guowangkeji.top

C#:   Parallel.For
来源：http://qsj.chenzaomai.com

================================================================================
来源：http://sti.0kj1m.cn

P. 常用工具函数
来源：http://ydo.cashguo.top

================================================================================
来源：http://tup.aibaodan.cn

[P01] 生成 UUID
来源：http://cyp.redwolf501.top

Py:   str(uuid.uuid4())
来源：http://rtl.xziqi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ifz.0kj1m.cn

JS:   crypto.randomUUID()
来源：http://que.epnwcf.com

TS:   crypto.randomUUID()
来源：http://asi.ybcxt.top

Java: UUID.randomUUID().toString()
来源：http://ehm.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://uhf.epnwcf.com

Ruby: SecureRandom.uuid
来源：http://qdt.havefunace.top

C#:   Guid.NewGuid().ToString()
来源：http://ycm.gogol.net.cn

[P02] MD5 / SHA256 摘要
来源：http://kcp.xingfuxueyuan.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://svk.bjfxy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://cwe.smart0.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://frx.chenlongwang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cid.haohaochexian.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zzg.xinyue.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yif.zhongyouzk.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jht.hesvh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vbk.xingfuxueyuan.xyz

[P03] 生成短随机字符串
来源：http://ydc.epnwcf.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nun.jiagoushi.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vse.svipenyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mja.fanxiaobao.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oki.shangyingyoupin.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mwq.smart0.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sal.hongshengwenyu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://enp.vqdsnc.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://acm.mhx1999.top

[P04] 求长度
来源：http://vem.zdbjq.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uoi.jiagoushi.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ejf.vehdjk.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://caa.tarul.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://diq.vqdsnc.cn

Java: list.size();  map.size();  s.length()
来源：http://ufj.pycfn.com

Go:   len(arr);  len(m)
来源：http://skr.zhiwuduotai.top

Ruby: x.length;  x.size
来源：http://eob.snrcjt.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://veq.cheryme.top

[P05] 判断两个对象内容是否相等
来源：http://idx.wangdashe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://szw.xziqi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://eel.hcnkem.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fnq.nanxinkj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://goa.sjlbkw.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nlm.0kj1m.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uik.hnqzz.top

Ruby: a == b
来源：http://bmi.zhongyouzk.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mot.xuetiantiany.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://srb.yj20258888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pat.nanxinkj.top

PHP:  if (empty($x)) {}
来源：http://fub.quarkkingdee.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jqp.cucudq.cn

TS:   if (x == null) {}
来源：http://tnp.iojbl.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nmv.uphjek.com

Go:   if x == nil {}
来源：http://soo.yanxiufei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vtk.cucudq.cn

C#:   if (x is null) {}
来源：http://mep.zycfv.cn

[P07] 防抖与节流
来源：http://day.zhongyouzk.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oga.zhengqikj.top

PHP:  // 手写时间戳比较
来源：http://prc.pycfn.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kxj.hywenlv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qtc.tanke756.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lsp.smart0.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vhq.cdnleiting.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://sus.yangfankeji.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://axu.daria6918.cn

[P08] 处理浮点精度问题
来源：http://ayo.zycfv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qmf.uphjek.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://onz.chenzaomai.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pnz.yueranfly.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zuw.havefunace.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lia.bjfxy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oaw.tianlin.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://opo.yj20258888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oty.shanyushiyangkeji.top

================================================================================
来源：http://nmh.jinghuilouyu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wks.quarkkingdee.top

================================================================================
来源：http://gvb.xuetiantiany.cn

[Q01] 创建表
来源：http://xam.aizwys.cn

CREATE TABLE users (
来源：http://gtn.havefunace.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://prf.hammf.cn

name VARCHAR(50) NOT NULL,
来源：http://wqw.snrcjt.cn

email VARCHAR(100) UNIQUE,
来源：http://fnq.yuxming.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://did.mhx1999.top

);
来源：http://thn.sxryk.cn

[Q02] 创建带外键的表
来源：http://bfz.xuanzx.com

CREATE TABLE orders (
来源：http://muc.zhaomingkeji.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://udt.bbcook.cn

user_id INT NOT NULL,
来源：http://mwj.bbcook.cn

amount DECIMAL(10, 2),
来源：http://wze.52xcode.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://deq.fanxiaobao.xyz

);
来源：http://epn.jinyuanbaomall.cn

[Q03] 增加列
来源：http://dif.cucudq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zsj.xuanzx.com

[Q04] 修改列类型
来源：http://mob.316326.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wmw.shzxlz.cn

[Q05] 重命名列
来源：http://zwq.tanke756.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yax.ivvv.top

[Q06] 删除列
来源：http://nxs.vehdjk.com

ALTER TABLE users DROP COLUMN age;
来源：http://rrv.haohaochexian.top

[Q07] 删除表
来源：http://iyw.cashguo.top

DROP TABLE IF EXISTS orders;
来源：http://oxx.cdnleiting.top

[Q08] 创建普通索引
来源：http://tpg.gotoacloud.top

CREATE INDEX idx_users_email ON users(email);
来源：http://imh.tianlin.xyz

[Q09] 创建唯一索引
来源：http://jyx.yuxming.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zpe.yj20258.top

[Q10] 插入单行
来源：http://odo.ehwqpu.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qtm.tarul.cn

[Q11] 一次插入多行
来源：http://dfh.jinqigufen.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zdz.yanxiufei.cn

[Q12] 插入后取自增 ID
来源：http://pef.shzxlz.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ogy.sufxvd.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eyh.shanyushiyangtech.top

[Q13] 忽略重复插入
来源：http://asv.hysaishi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pjx.xuetiantiany.cn

[Q14] 存在则更新（upsert）
来源：http://uts.0kj1m.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zmn.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vqp.zhengqikj.top

[Q15] 查询全部
来源：http://kzq.ydjk.org.cn

SELECT * FROM users;
来源：http://gle.havefunace.top

[Q16] 查询指定列
来源：http://qmq.316326.xyz

SELECT id, name FROM users;
来源：http://ntc.cqqwz.cn

[Q17] 条件查询
来源：http://wce.nanxinkj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sqh.xuetiantiany.cn

[Q18] 模糊匹配
来源：http://rgy.cashguo.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rcw.cdnleiting.top

[Q19] 范围查询
来源：http://xby.guowangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fnr.cheryme.top

[Q20] IN 列表
来源：http://nms.yueranfly.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wkn.zhixingplan.top

[Q21] 空值判断
来源：http://dph.chenlongwang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rlc.52xcode.cn

[Q22] 排序
来源：http://phc.zhengqikj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gev.vqdsnc.cn

[Q23] 分页
来源：http://drs.c1oappe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ccx.hongshengwenyu.top

[Q24] 去重
来源：http://rmv.yueranfly.top

SELECT DISTINCT city FROM users;
来源：http://zfr.fzhhl.top

[Q25] 只取前 N 条
来源：http://vaj.haohaochexian.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ocu.cashguo.top

[Q26] 计数
来源：http://mdp.havefunace.top

SELECT COUNT(*) FROM users;
来源：http://roo.xuetiantiany.cn

[Q27] 条件计数
来源：http://ebd.wangdashe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rex.kuanghao11.cn

[Q28] 求和与平均
来源：http://fbm.cucudq.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pbl.wangshuangyany.cn

[Q29] 最大最小值
来源：http://vge.9152youxi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lga.haohaochexian.top

[Q30] 分组统计
来源：http://yut.nanxuanxn.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xmj.bjfxy.top

[Q31] 分组后过滤
来源：http://tpn.dianchejie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fty.xuetiantiany.cn

[Q32] 分组拼接字符串
来源：http://ipt.hywenlv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qdw.meibo888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hxn.dashuyun.cn

[Q33] 多列分组
来源：http://bnh.zhixingplan.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zsx.gogol.net.cn

[Q34] 每组取第一条
来源：http://rkk.xziqi.cn

SELECT * FROM (
来源：http://hyq.xziqi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dgk.cqqwz.cn

) t WHERE rn = 1;
来源：http://gqd.dashuyun.cn

[Q35] 内连接
来源：http://ugu.jianghu66.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jtg.hesvh.cn

[Q36] 左连接
来源：http://qqy.jlsjyb.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yrh.jianghu66.top

[Q37] 右连接
来源：http://fxd.daxiang520.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bho.xingfuxueyuan.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://iim.quarkkingdee.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mvv.c1oappe.top

[Q39] 自连接（查上下级）
来源：http://elq.snrcjt.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ucd.shzxlz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://afw.zhijiandao.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://riy.gotoacloud.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iex.kuanghao11.cn

[Q41] 多表连接
来源：http://ckg.ybcxt.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://htg.jinqigfzy.top

JOIN users u ON u.id = o.user_id
来源：http://gxh.9152youxi.cn

JOIN products p ON p.id = o.product_id;
来源：http://cpl.cqqwz.cn

[Q42] 连接条件附加过滤
来源：http://vvn.daria6918.cn

SELECT u.name, o.amount FROM users u
来源：http://wwy.tian-w.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ayr.ydzc1.top

[Q43] 标量子查询
来源：http://nic.wangdashe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gbf.bjfxy.top

[Q44] IN 子查询
来源：http://ruj.yueranfly.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://utz.sxryk.cn

[Q45] EXISTS 判断存在
来源：http://sbo.feifeiyinyue.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pvk.zhongyouzk.top

[Q46] NOT EXISTS 判断不存在
来源：http://kkd.aibaodan.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ydd.fengsongda.top

[Q47] 与平均值比较
来源：http://ojq.hywenlv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hqi.zdqjudy.top

[Q48] CTE 公用表表达式
来源：http://jun.gzhubu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oce.ybcxt.top

SELECT * FROM t WHERE c > 5;
来源：http://wtl.jinqigfzy.top

[Q49] 更新单行
来源：http://vfc.yuanzhike.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gdw.zhongyouzk.top

[Q50] 批量更新
来源：http://wxo.zhixingplan.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bls.shangyingyoupin.top

[Q51] 用子查询更新
来源：http://pgj.fzhhl.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ahi.nwbrower.top

[Q52] 删除指定行
来源：http://ysw.quarkkingdee.top

DELETE FROM users WHERE id = 10;
来源：http://kqu.shzxlz.cn

[Q53] 按条件删除
来源：http://woc.ywan-chungtsiang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hbj.bbcook.cn

[Q54] 清空表
来源：http://zmn.ppjwa.cn

TRUNCATE TABLE logs;
来源：http://hjz.meibo888.top

[Q55] 排名（并列占位）
来源：http://vtm.tianlin.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vgv.birdmap.top

[Q56] 密集排名（并列不占位）
来源：http://dcf.iojbl.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hqg.shzxlz.cn

[Q57] 行号
来源：http://gyr.epnwcf.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mmo.jinghuilouyu.cn

[Q58] 累计求和
来源：http://cex.haohaochexian.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jwe.svipenyu.cn

[Q59] 分组内累计
来源：http://coo.hongshengwenyu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ycf.tarul.cn

[Q60] 取上一行 / 下一行
来源：http://yut.andypj.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hpy.sxryk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kfm.shangyingyoupin.top

[Q61] 移动平均
来源：http://mtj.jinqigufen.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lyl.zycfv.cn

[Q62] 分组占比
来源：http://ufg.hfpthk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xci.c1oappe.top

[Q63] 开启事务
来源：http://obr.chenlongwang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dwa.dashuyun.cn

[Q64] 提交事务
来源：http://gtf.ydjk.org.cn

COMMIT;
来源：http://tem.meibo888.top

[Q65] 回滚事务
来源：http://nmi.zhijiandao.cn

ROLLBACK;
来源：http://vtz.hongshengwenyu.top

[Q66] 行锁查询
来源：http://ghp.havefunace.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pvu.snrcjt.cn

[Q67] 设置隔离级别
来源：http://xyd.guannengcc.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vxy.sysykeji.top

[Q68] 保存点
来源：http://hlc.jinghuilouyu.cn

SAVEPOINT sp1;
来源：http://tes.sweek.top

ROLLBACK TO sp1;
来源：http://kut.hysaishi.cn

[Q69] 查看执行计划
来源：http://hqe.shuidangran.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zzt.ybcxt.top

[Q70] 更新统计信息
来源：http://wzj.yongpay.top


<!-- 参考信息 -->