代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wyk.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nxl.yj202588.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jcm.zhijiandao.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nye.aizwys.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ubi.yj202588.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kcr.hongshengwenyu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wvo.jqgfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jcw.yvedp.cn

================================================================================
来源：http://ulp.shuidangran.top

O. 并发与异步
来源：http://wzk.zhijiandao.cn

================================================================================
来源：http://gqq.epnwcf.com

[O01] 启动一个线程
来源：http://bsw.mhx1999.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mvi.jyoumei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zva.chenzaomai.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://waz.0kj1m.cn

TS:   // 同 JS
来源：http://gez.tarul.cn

Java: new Thread(() -> f()).start()
来源：http://ejw.epnwcf.com

Go:   go f()
来源：http://hsj.chenzaomai.com

Ruby: Thread.new { f }
来源：http://gfc.zycfv.cn

C#:   Task.Run(() => F());
来源：http://rsi.fktsv.cn

[O02] 使用线程池
来源：http://qxl.shanyushiyangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xsz.wangshuangyany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bfr.gotoacloud.top

JS:   // worker_threads 线程池
来源：http://fqg.nanxinkj.top

TS:   // worker_threads 线程池
来源：http://mof.quarkkingdee.top

Java: Executors.newFixedThreadPool(4)
来源：http://sno.zhongyouzk.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qbu.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wlt.gzhubu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://izk.pengpengdd.cyou

[O03] 加锁保护共享数据
来源：http://uyc.vqdsnc.cn

Py:   with lock: shared += 1
来源：http://ugv.mhx1999.top

PHP:  // 用 flock() 做文件锁
来源：http://tkv.tarul.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nwo.ydzc1.top

TS:   // 同 JS
来源：http://qjb.epnwcf.com

Java: synchronized (this) { shared++; }
来源：http://ygg.hongshengwenyu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dnk.hfpthk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nsl.zhaomingkeji.xyz

C#:   lock (gate) { shared++; }
来源：http://pix.zhaomingkeji.xyz

[O04] 定义异步函数并等待
来源：http://cff.fzhhl.top

Py:   async def f():⏎    await g()
来源：http://erg.jinghuilouyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://alo.ppjwa.cn

JS:   async function f() { await g(); }
来源：http://huj.yj20258888.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rjc.ydjk.org.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yag.jinqigfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xwh.cdnleiting.top

Ruby: # 用 Fiber 或 async gem
来源：http://rcd.svipenyu.cn

C#:   async Task F() { await G(); }
来源：http://hhx.yj202588.top

[O05] 并发执行并等待全部完成
来源：http://tbh.sxryk.cn

Py:   asyncio.gather(*tasks)
来源：http://xwv.havefunace.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://aar.mhx1999.top

JS:   await Promise.all(tasks)
来源：http://kyr.xinyue.icu

TS:   await Promise.all(tasks)
来源：http://nqk.vqdsnc.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://reb.hcnkem.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cru.jianghu66.top

Ruby: threads.map(&:join)
来源：http://xrq.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tgr.jqgufenzy.top

[O06] 使用进程池
来源：http://igr.sufxvd.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://alk.shuidangran.top

PHP:  // pcntl_fork 或多进程队列
来源：http://trl.tianlin.xyz

JS:   // child_process / cluster 模块
来源：http://hxq.zycfv.cn

TS:   // child_process / cluster 模块
来源：http://lsl.tianlin.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ufa.xinyue.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fra.cqqwz.cn

Ruby: // fork 块
来源：http://rfj.hcnkem.com

C#:   Parallel.For
来源：http://xgi.hcnkem.com

================================================================================
来源：http://stm.cdnleiting.top

P. 常用工具函数
来源：http://izz.cashguo.top

================================================================================
来源：http://xcq.xylfe.cn

[P01] 生成 UUID
来源：http://nxv.tanke756.top

Py:   str(uuid.uuid4())
来源：http://sdw.yj202588.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hmf.yangfankeji.com

JS:   crypto.randomUUID()
来源：http://mgc.wangdashe.top

TS:   crypto.randomUUID()
来源：http://lgj.zhengqikj.top

Java: UUID.randomUUID().toString()
来源：http://pce.cqqwz.cn

Go:   // 用 github.com/google/uuid
来源：http://eaj.shangyingyoupin.top

Ruby: SecureRandom.uuid
来源：http://oyl.nanxuanxn.top

C#:   Guid.NewGuid().ToString()
来源：http://zda.xinyue.icu

[P02] MD5 / SHA256 摘要
来源：http://pik.fzhhl.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cgm.sufxvd.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ewe.cheryme.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sdy.gzhubu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tbp.fengsongda.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xrv.hnxiangtu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ecg.vqdsnc.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blr.mhx1999.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vwa.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://xkn.iojbl.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xhx.hcnkem.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qpz.shangyingyoupin.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gpm.zdbjq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ecw.zhixingplan.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hko.tianlin.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oqo.jiagoushi.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://acx.sysykeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cli.9152youxi.cn

[P04] 求长度
来源：http://yfz.chenzaomai.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hld.yuxming.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vyz.shuidangran.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gxb.ywan-chungtsiang.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jjx.ybcxt.top

Java: list.size();  map.size();  s.length()
来源：http://hwh.wangdashe.top

Go:   len(arr);  len(m)
来源：http://mxa.andypj.xyz

Ruby: x.length;  x.size
来源：http://dzo.xuetiantiany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ogz.vehdjk.com

[P05] 判断两个对象内容是否相等
来源：http://yhl.xziqi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sav.havefunace.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yoh.zhongyouzk.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xax.zhaomingkeji.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pbb.redwolf501.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://snw.guowangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://uft.c1oappe.top

Ruby: a == b
来源：http://yfc.yj20258888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zba.hnqzz.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sjr.shuidangran.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lmm.jinyuanbaomall.cn

PHP:  if (empty($x)) {}
来源：http://qrx.zdbjq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uvl.redwolf501.top

TS:   if (x == null) {}
来源：http://yxb.ybcxt.top

Java: if (x == null || x.isEmpty()) {}
来源：http://bky.guannengcc.top

Go:   if x == nil {}
来源：http://rov.nwbrower.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ije.hysaishi.cn

C#:   if (x is null) {}
来源：http://xup.yuxming.cn

[P07] 防抖与节流
来源：http://tdh.chenlongwang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lzp.smart0.xyz

PHP:  // 手写时间戳比较
来源：http://ffq.birdmap.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wwf.zhaomingkeji.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nna.hesvh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qbs.hnxiangtu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dga.hfpthk.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gaz.sufxvd.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yfa.guannengcc.top

[P08] 处理浮点精度问题
来源：http://zjn.nanxinkj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ldz.ctjpmb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yys.ydzc1.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://olr.sysykeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kew.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xzk.aizwys.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zzv.xinyue.icu

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dpg.dianchejie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nel.bbcook.cn

================================================================================
来源：http://kvi.ehwqpu.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kok.9152youxi.cn

================================================================================
来源：http://ehc.aizwys.cn

[Q01] 创建表
来源：http://fog.shuidangran.top

CREATE TABLE users (
来源：http://egw.ivvv.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tqw.ywan-chungtsiang.top

name VARCHAR(50) NOT NULL,
来源：http://kvg.tanke756.top

email VARCHAR(100) UNIQUE,
来源：http://jee.jyoumei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://reh.shangyingyoupin.top

);
来源：http://mll.daria6918.cn

[Q02] 创建带外键的表
来源：http://mft.feifeiyinyue.top

CREATE TABLE orders (
来源：http://jti.redwolf501.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://itu.gzhubu.top

user_id INT NOT NULL,
来源：http://inz.yueranfly.top

amount DECIMAL(10, 2),
来源：http://kik.uphjek.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mzb.daxiang520.top

);
来源：http://axx.yueranfly.top

[Q03] 增加列
来源：http://gzc.yj20258.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ddk.vehdjk.com

[Q04] 修改列类型
来源：http://xif.ybcxt.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://csz.quarkkingdee.top

[Q05] 重命名列
来源：http://pjf.52xcode.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xri.jqgfzy.top

[Q06] 删除列
来源：http://uxo.cheryme.top

ALTER TABLE users DROP COLUMN age;
来源：http://yfx.nanxinkj.top

[Q07] 删除表
来源：http://zgq.jinqigfzy.top

DROP TABLE IF EXISTS orders;
来源：http://apw.uphjek.com

[Q08] 创建普通索引
来源：http://ryt.zhengqikj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nop.sysykeji.top

[Q09] 创建唯一索引
来源：http://jru.sjlbkw.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vil.sufxvd.cn

[Q10] 插入单行
来源：http://pvh.xinyue.icu

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://frp.316326.xyz

[Q11] 一次插入多行
来源：http://mix.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gud.hcnkem.com

[Q12] 插入后取自增 ID
来源：http://zkv.sjlbkw.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bhy.yvedp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://irf.tarul.cn

[Q13] 忽略重复插入
来源：http://nsg.jqgfzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iha.yvedp.cn

[Q14] 存在则更新（upsert）
来源：http://wfg.shangyingyoupin.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xaf.zhengqikj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hux.ehwqpu.com

[Q15] 查询全部
来源：http://yyc.pycfn.com

SELECT * FROM users;
来源：http://zah.yonumen.top

[Q16] 查询指定列
来源：http://xzv.fehbvm.com

SELECT id, name FROM users;
来源：http://ehi.jinghuilouyu.cn

[Q17] 条件查询
来源：http://zrb.gzhubu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uwr.snrcjt.cn

[Q18] 模糊匹配
来源：http://gtl.ybcxt.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ucc.jiagoushi.top

[Q19] 范围查询
来源：http://uif.cheryme.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xbr.xuetiantiany.cn

[Q20] IN 列表
来源：http://yyu.xziqi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fyd.fktsv.cn

[Q21] 空值判断
来源：http://wgj.kuanghao11.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kwn.zhongyouzk.top

[Q22] 排序
来源：http://red.quarkkingdee.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sgq.jinyuanbaomall.cn

[Q23] 分页
来源：http://zqf.sweek.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://apo.haohaochexian.top

[Q24] 去重
来源：http://snc.zhixingplan.top

SELECT DISTINCT city FROM users;
来源：http://sek.guannengcc.top

[Q25] 只取前 N 条
来源：http://xbd.cheryme.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ipk.hcnkem.com

[Q26] 计数
来源：http://mit.fzhhl.top

SELECT COUNT(*) FROM users;
来源：http://mcc.zycfv.cn

[Q27] 条件计数
来源：http://hpv.vqdsnc.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pgr.meibo888.top

[Q28] 求和与平均
来源：http://hgz.aizwys.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nen.mhx1999.top

[Q29] 最大最小值
来源：http://yqx.quarkkingdee.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://uzh.fzhhl.top

[Q30] 分组统计
来源：http://bgz.yuxming.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://onu.aizwys.cn

[Q31] 分组后过滤
来源：http://hmu.gzhubu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cce.havefunace.top

[Q32] 分组拼接字符串
来源：http://krq.yvedp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rjo.cucudq.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xzd.52xcode.cn

[Q33] 多列分组
来源：http://zes.hnqzz.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qzq.hesvh.cn

[Q34] 每组取第一条
来源：http://gaw.hammf.cn

SELECT * FROM (
来源：http://vgq.jinqigufen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://spe.vqdsnc.cn

) t WHERE rn = 1;
来源：http://grx.daria6918.cn

[Q35] 内连接
来源：http://bdo.tanke756.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ocm.ydjk.org.cn

[Q36] 左连接
来源：http://llb.jlsjyb.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://efb.zdbjq.cn

[Q37] 右连接
来源：http://anx.jiagoushi.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pxk.zhaomingkeji.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://ulo.smart0.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zda.shanyushiyangkeji.top

[Q39] 自连接（查上下级）
来源：http://hoh.yfazqb.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://hmr.hnqzz.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://emi.hongshengwenyu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pha.daria6918.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jmm.jlsjyb.cn

[Q41] 多表连接
来源：http://ocw.epnwcf.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://zrx.smart0.xyz

JOIN users u ON u.id = o.user_id
来源：http://gyu.pycfn.com

JOIN products p ON p.id = o.product_id;
来源：http://gog.gogol.net.cn

[Q42] 连接条件附加过滤
来源：http://nop.zhiwuduotai.top

SELECT u.name, o.amount FROM users u
来源：http://cej.xingfuxueyuan.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kon.fzhhl.top

[Q43] 标量子查询
来源：http://ilm.zycfv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wsu.cqqwz.cn

[Q44] IN 子查询
来源：http://yww.epnwcf.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wew.svipenyu.cn

[Q45] EXISTS 判断存在
来源：http://ozg.hcnkem.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tiz.yuanzhike.top

[Q46] NOT EXISTS 判断不存在
来源：http://sar.nwbrower.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ucy.fanxiaobao.xyz

[Q47] 与平均值比较
来源：http://hak.0kj1m.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ukn.xuanzx.com

[Q48] CTE 公用表表达式
来源：http://rpy.yongpay.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ned.havefunace.top

SELECT * FROM t WHERE c > 5;
来源：http://cbv.ivvv.top

[Q49] 更新单行
来源：http://yna.shangyingyoupin.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yyj.shuidangran.top

[Q50] 批量更新
来源：http://gnu.nwbrower.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sxv.zdqjudy.top

[Q51] 用子查询更新
来源：http://imn.havefunace.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gtk.yongpay.top

[Q52] 删除指定行
来源：http://bmj.yj20258888.top

DELETE FROM users WHERE id = 10;
来源：http://pvg.zhongyouzk.top

[Q53] 按条件删除
来源：http://pnt.vehdjk.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iac.wangdashe.top

[Q54] 清空表
来源：http://efo.jqgfzy.top

TRUNCATE TABLE logs;
来源：http://rcz.chenlongwang.top

[Q55] 排名（并列占位）
来源：http://unv.yfazqb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cdz.wangshuangyany.cn

[Q56] 密集排名（并列不占位）
来源：http://qmg.zhiwuduotai.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mqx.yj20258.top

[Q57] 行号
来源：http://ekf.pycfn.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bnn.aibaodan.cn

[Q58] 累计求和
来源：http://dds.yj20258.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hqp.chenzaomai.com

[Q59] 分组内累计
来源：http://dpm.ywan-chungtsiang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://npw.gogol.net.cn

[Q60] 取上一行 / 下一行
来源：http://tha.xinyue.icu

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pny.dashuyun.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ewr.xylfe.cn

[Q61] 移动平均
来源：http://qkf.bjfxy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dus.shzxlz.cn

[Q62] 分组占比
来源：http://ysv.bjfxy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xsu.vqdsnc.cn

[Q63] 开启事务
来源：http://ihj.hfpthk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hjt.ehwqpu.com

[Q64] 提交事务
来源：http://zrl.hnqzz.top

COMMIT;
来源：http://seo.quarkkingdee.top

[Q65] 回滚事务
来源：http://knt.zycfv.cn

ROLLBACK;
来源：http://nim.yj20258888.top

[Q66] 行锁查询
来源：http://kca.hnqzz.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ynd.birdmap.top

[Q67] 设置隔离级别
来源：http://ehm.bjfxy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fuf.fanxiaobao.xyz

[Q68] 保存点
来源：http://oax.zycfv.cn

SAVEPOINT sp1;
来源：http://unn.hnxiangtu.top


<!-- 参考信息 -->