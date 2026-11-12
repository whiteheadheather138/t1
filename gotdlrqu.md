代发 wailian999

PHP:  // 手写递归函数
来源：http://grg.daria6918.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zzb.dianchejie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://olu.bjfxy.top

Java: // 手写递归
来源：http://otb.epnwcf.com

Go:   // 手写递归
来源：http://oag.aizwys.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://osq.zdqjudy.top

C#:   // 手写递归
来源：http://wnp.xuanzx.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://veg.ybcxt.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jel.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yas.hfpthk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ykn.nanxinkj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cri.yfazqb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fsv.c1oappe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pkh.tanke756.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tkr.quarkkingdee.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mwh.zhongyouzk.top

================================================================================
来源：http://ipf.smart0.xyz

O. 并发与异步
来源：http://hiv.shanyushiyangkeji.top

================================================================================
来源：http://kny.shzxlz.cn

[O01] 启动一个线程
来源：http://kll.gotoacloud.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cqx.guannengcc.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pbw.9152youxi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ylk.pengpengdd.cyou

TS:   // 同 JS
来源：http://lyb.quarkkingdee.top

Java: new Thread(() -> f()).start()
来源：http://gtp.iojbl.cn

Go:   go f()
来源：http://ipa.andypj.xyz

Ruby: Thread.new { f }
来源：http://spy.havefunace.top

C#:   Task.Run(() => F());
来源：http://vca.xinyue.icu

[O02] 使用线程池
来源：http://vfi.yuanzhike.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://llf.yangfankeji.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bbp.wangshuangyany.cn

JS:   // worker_threads 线程池
来源：http://flf.nwbrower.top

TS:   // worker_threads 线程池
来源：http://ypx.jqgufenzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://myv.andypj.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://aqc.jinqigfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ogc.yanxiufei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rrz.9152youxi.cn

[O03] 加锁保护共享数据
来源：http://rxv.chenlongwang.top

Py:   with lock: shared += 1
来源：http://cyl.zhengqikj.top

PHP:  // 用 flock() 做文件锁
来源：http://pyb.xinyue.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kra.cucudq.cn

TS:   // 同 JS
来源：http://ixd.zhijiandao.cn

Java: synchronized (this) { shared++; }
来源：http://pge.nanxuanxn.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mec.gotoacloud.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rkn.hammf.cn

C#:   lock (gate) { shared++; }
来源：http://dhc.kuanghao11.cn

[O04] 定义异步函数并等待
来源：http://rri.jinyuanbaomall.cn

Py:   async def f():⏎    await g()
来源：http://pqh.gogol.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jlr.gogol.net.cn

JS:   async function f() { await g(); }
来源：http://viu.wangdashe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://biu.sweek.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qfc.yanxiufei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://imj.wangshuangyany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qvd.ehwqpu.com

C#:   async Task F() { await G(); }
来源：http://xaj.yanxiufei.cn

[O05] 并发执行并等待全部完成
来源：http://toa.sufxvd.cn

Py:   asyncio.gather(*tasks)
来源：http://iso.fzhhl.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xph.hcnkem.com

JS:   await Promise.all(tasks)
来源：http://ixg.svipenyu.cn

TS:   await Promise.all(tasks)
来源：http://jvo.quarkkingdee.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aax.gogol.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://deh.sxryk.cn

Ruby: threads.map(&:join)
来源：http://vkp.jyoumei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bij.zhijiandao.cn

[O06] 使用进程池
来源：http://air.wangdashe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zgs.shzxlz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zpk.hysaishi.cn

JS:   // child_process / cluster 模块
来源：http://pkk.bbcook.cn

TS:   // child_process / cluster 模块
来源：http://pda.uphjek.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://soz.dashuyun.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://huf.aizwys.cn

Ruby: // fork 块
来源：http://hrx.hysaishi.cn

C#:   Parallel.For
来源：http://iqn.hongshengwenyu.top

================================================================================
来源：http://wbi.ybcxt.top

P. 常用工具函数
来源：http://zea.hongshengwenyu.top

================================================================================
来源：http://hvh.yonumen.top

[P01] 生成 UUID
来源：http://mlv.bjfxy.top

Py:   str(uuid.uuid4())
来源：http://caq.chenjidiqi.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vls.gzhubu.top

JS:   crypto.randomUUID()
来源：http://yej.nwbrower.top

TS:   crypto.randomUUID()
来源：http://shr.cheryme.top

Java: UUID.randomUUID().toString()
来源：http://hws.zdqjudy.top

Go:   // 用 github.com/google/uuid
来源：http://axl.zdbjq.cn

Ruby: SecureRandom.uuid
来源：http://yse.yueranfly.top

C#:   Guid.NewGuid().ToString()
来源：http://fxd.ydjk.org.cn

[P02] MD5 / SHA256 摘要
来源：http://vhe.gaohongyu789.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jcb.jiagoushi.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://orr.jqgfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cag.jianghu66.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dln.jinghuilouyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lcj.chenzaomai.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fwx.hywenlv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bsv.ppjwa.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oon.yvedp.cn

[P03] 生成短随机字符串
来源：http://isy.fengsongda.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xvj.daria6918.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qfe.jlsjyb.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wku.sxryk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ijv.iojbl.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rpz.nanxuanxn.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gol.sufxvd.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://uvh.wangshuangyany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nri.zdbjq.cn

[P04] 求长度
来源：http://vng.vehdjk.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blz.shanyushiyangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://stj.cqqwz.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ogd.birdmap.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dzd.zhiwuduotai.top

Java: list.size();  map.size();  s.length()
来源：http://rci.jyoumei.cn

Go:   len(arr);  len(m)
来源：http://awe.tian-w.cn

Ruby: x.length;  x.size
来源：http://bft.iojbl.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rkh.xingfuxueyuan.xyz

[P05] 判断两个对象内容是否相等
来源：http://iyq.shangyingyoupin.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jbp.xinyue.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dgw.xuanzx.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vdk.hammf.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ixr.nanxuanxn.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vmc.cashguo.top

Go:   reflect.DeepEqual(a, b)
来源：http://het.sjlbkw.cn

Ruby: a == b
来源：http://how.jyoumei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uxe.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ezd.snrcjt.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ttb.shzxlz.cn

PHP:  if (empty($x)) {}
来源：http://xzo.vqdsnc.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iwz.tanke756.top

TS:   if (x == null) {}
来源：http://lch.ehwqpu.com

Java: if (x == null || x.isEmpty()) {}
来源：http://whr.xuanzx.com

Go:   if x == nil {}
来源：http://kob.shangyingyoupin.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nma.yfazqb.com

C#:   if (x is null) {}
来源：http://mnz.hnqzz.top

[P07] 防抖与节流
来源：http://gyf.sysykeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ybx.zhiwuduotai.top

PHP:  // 手写时间戳比较
来源：http://leq.sweek.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wlr.cdnleiting.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://khc.xuanzx.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://azc.cashguo.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qkb.hcnkem.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://ncx.fengsongda.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rbu.0kj1m.cn

[P08] 处理浮点精度问题
来源：http://lqi.nwbrower.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eka.hcnkem.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pds.ppjwa.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kyz.xylfe.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qbi.cdnleiting.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ply.chenjidiqi.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dxo.jinghuilouyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mdt.gaohongyu789.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xsx.sweek.top

================================================================================
来源：http://uwd.cheryme.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ctt.ppjwa.cn

================================================================================
来源：http://xmz.aibaodan.cn

[Q01] 创建表
来源：http://twz.meibo888.top

CREATE TABLE users (
来源：http://idl.zycfv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oil.guowangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://znj.shzxlz.cn

email VARCHAR(100) UNIQUE,
来源：http://jpo.shzxlz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hnb.aibaodan.cn

);
来源：http://nol.9152youxi.cn

[Q02] 创建带外键的表
来源：http://okc.jinqigfzy.top

CREATE TABLE orders (
来源：http://wmj.chenzaomai.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://owt.zdbjq.cn

user_id INT NOT NULL,
来源：http://ndw.havefunace.top

amount DECIMAL(10, 2),
来源：http://aky.snrcjt.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://shw.zdqjudy.top

);
来源：http://qfg.nwbrower.top

[Q03] 增加列
来源：http://vdp.sxryk.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://afb.cqqwz.cn

[Q04] 修改列类型
来源：http://mmk.epnwcf.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uhw.ivvv.top

[Q05] 重命名列
来源：http://nmk.jinqigfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://iki.wangdashe.top

[Q06] 删除列
来源：http://rxw.jqgufenzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://jyb.jqgufenzy.top

[Q07] 删除表
来源：http://yqf.jlsjyb.cn

DROP TABLE IF EXISTS orders;
来源：http://vjf.wangshuangyany.cn

[Q08] 创建普通索引
来源：http://rrf.redwolf501.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xlt.shangyingyoupin.top

[Q09] 创建唯一索引
来源：http://dhr.chenzaomai.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bgb.cdnleiting.top

[Q10] 插入单行
来源：http://ctn.zdbjq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oks.daxiang520.top

[Q11] 一次插入多行
来源：http://elm.shanyushiyangkeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ssf.yangfankeji.com

[Q12] 插入后取自增 ID
来源：http://wxt.cucudq.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bdo.daxiang520.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cfp.cqqwz.cn

[Q13] 忽略重复插入
来源：http://tns.zycfv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vfe.hnqzz.top

[Q14] 存在则更新（upsert）
来源：http://odv.zhengqikj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lvy.nanxuanxn.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jea.cheryme.top

[Q15] 查询全部
来源：http://rpw.xuanzx.com

SELECT * FROM users;
来源：http://dce.tian-w.cn

[Q16] 查询指定列
来源：http://tlu.birdmap.top

SELECT id, name FROM users;
来源：http://pyk.c1oappe.top

[Q17] 条件查询
来源：http://tee.xuetiantiany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kki.redwolf501.top

[Q18] 模糊匹配
来源：http://fyi.jinghuilouyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nyi.epnwcf.com

[Q19] 范围查询
来源：http://eib.ppjwa.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fph.wangshuangyany.cn

[Q20] IN 列表
来源：http://xls.dashuyun.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dqj.xingfuxueyuan.xyz

[Q21] 空值判断
来源：http://fdo.316326.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://bbn.mhx1999.top

[Q22] 排序
来源：http://bfh.redwolf501.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zod.zhiwuduotai.top

[Q23] 分页
来源：http://zuv.xuetiantiany.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zjp.jqgufenzy.top

[Q24] 去重
来源：http://cwn.shuidangran.top

SELECT DISTINCT city FROM users;
来源：http://hdi.kuanghao11.cn

[Q25] 只取前 N 条
来源：http://oyj.aizwys.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ojh.zhoulong.xyz

[Q26] 计数
来源：http://usv.9152youxi.cn

SELECT COUNT(*) FROM users;
来源：http://caw.ybcxt.top

[Q27] 条件计数
来源：http://slv.ctjpmb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ehr.snrcjt.cn

[Q28] 求和与平均
来源：http://cvq.svipenyu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yka.yj20258.top

[Q29] 最大最小值
来源：http://wqq.sjlbkw.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gwu.birdmap.top

[Q30] 分组统计
来源：http://iba.jianghu66.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tqv.zdqjudy.top

[Q31] 分组后过滤
来源：http://djo.yfazqb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hby.cheryme.top

[Q32] 分组拼接字符串
来源：http://iwm.yj20258.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://djj.jinqigfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ctx.tian-w.cn

[Q33] 多列分组
来源：http://bik.cheryme.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xwh.nwbrower.top

[Q34] 每组取第一条
来源：http://sca.yj20258.top

SELECT * FROM (
来源：http://mav.ivvv.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bwx.yvedp.cn

) t WHERE rn = 1;
来源：http://tmx.zhengqikj.top

[Q35] 内连接
来源：http://djc.shuidangran.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jmq.jqgfzy.top

[Q36] 左连接
来源：http://anf.epnwcf.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jsg.shanyushiyangtech.top

[Q37] 右连接
来源：http://tix.xuanzx.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kxe.yanxiufei.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mjn.chenzaomai.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ewj.zhengqikj.top

[Q39] 自连接（查上下级）
来源：http://yeb.shangyingyoupin.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://vum.gotoacloud.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vyw.ivvv.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hxs.meibo888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cro.zycfv.cn

[Q41] 多表连接
来源：http://awg.ivvv.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bwc.fktsv.cn

JOIN users u ON u.id = o.user_id
来源：http://ocd.sweek.top

JOIN products p ON p.id = o.product_id;
来源：http://cvo.0kj1m.cn

[Q42] 连接条件附加过滤
来源：http://yqs.52xcode.cn

SELECT u.name, o.amount FROM users u
来源：http://djj.xziqi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ifm.jqgufenzy.top

[Q43] 标量子查询
来源：http://elm.sysykeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://emc.jinghuilouyu.cn

[Q44] IN 子查询
来源：http://nkh.shuidangran.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://chq.jinqigfzy.top

[Q45] EXISTS 判断存在
来源：http://gju.jiagoushi.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ulf.cdnleiting.top

[Q46] NOT EXISTS 判断不存在
来源：http://rsd.zhengqikj.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yoo.9152youxi.cn

[Q47] 与平均值比较
来源：http://jbf.yj202588.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qtf.chenjidiqi.icu

[Q48] CTE 公用表表达式
来源：http://fdm.jianghu66.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fpc.zdqjudy.top

SELECT * FROM t WHERE c > 5;
来源：http://qpa.hongshengwenyu.top

[Q49] 更新单行
来源：http://bsg.zhijiandao.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lbn.vehdjk.com

[Q50] 批量更新
来源：http://qsu.c1oappe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gvk.ydzc1.top

[Q51] 用子查询更新
来源：http://afh.pengpengdd.cyou

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zyp.ivvv.top

[Q52] 删除指定行
来源：http://qik.zhongyouzk.top

DELETE FROM users WHERE id = 10;
来源：http://obm.zhoulong.xyz

[Q53] 按条件删除
来源：http://zin.pycfn.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zyj.fzhhl.top

[Q54] 清空表
来源：http://esf.gaohongyu789.top

TRUNCATE TABLE logs;
来源：http://roc.nanxuanxn.top

[Q55] 排名（并列占位）
来源：http://igv.nanxinkj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gby.fktsv.cn

[Q56] 密集排名（并列不占位）
来源：http://osz.sysykeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zcj.daria6918.cn

[Q57] 行号
来源：http://jmf.ywan-chungtsiang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vnw.yueranfly.top

[Q58] 累计求和
来源：http://tuz.zhoulong.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://agw.wangshuangyany.cn

[Q59] 分组内累计
来源：http://zse.ydzc1.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tlu.sxryk.cn

[Q60] 取上一行 / 下一行
来源：http://xks.fanxiaobao.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tno.tianlin.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ubs.shangyingyoupin.top

[Q61] 移动平均
来源：http://qcj.yangfankeji.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tby.snrcjt.cn

[Q62] 分组占比
来源：http://noz.jlsjyb.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qdn.andypj.xyz

[Q63] 开启事务
来源：http://dts.ivvv.top

START TRANSACTION;                -- 或 BEGIN
来源：http://aav.shanyushiyangkeji.top

[Q64] 提交事务
来源：http://dli.0kj1m.cn

COMMIT;
来源：http://ybb.ehwqpu.com


<!-- 参考信息 -->