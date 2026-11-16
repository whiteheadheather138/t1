代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wcv.zhengqikj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://meg.sysykeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zgf.tarul.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xbw.zhongyouzk.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lfo.tanke756.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://omw.hywenlv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://asc.snrcjt.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jjp.tian-w.cn

================================================================================
来源：http://jge.vqdsnc.cn

O. 并发与异步
来源：http://saa.wangshuangyany.cn

================================================================================
来源：http://bgw.gaohongyu789.top

[O01] 启动一个线程
来源：http://oyi.xylfe.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zve.tianlin.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sya.yonumen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dww.bbcook.cn

TS:   // 同 JS
来源：http://ysi.meibo888.top

Java: new Thread(() -> f()).start()
来源：http://zua.tianlin.xyz

Go:   go f()
来源：http://zkm.gaohongyu789.top

Ruby: Thread.new { f }
来源：http://tue.yvedp.cn

C#:   Task.Run(() => F());
来源：http://vsx.sweek.top

[O02] 使用线程池
来源：http://byn.smart0.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pry.cheryme.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zyf.daria6918.cn

JS:   // worker_threads 线程池
来源：http://nbp.fengsongda.top

TS:   // worker_threads 线程池
来源：http://jzf.zhaomingkeji.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://daz.hammf.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vgc.sufxvd.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xng.tianlin.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://phf.52xcode.cn

[O03] 加锁保护共享数据
来源：http://qzo.chenzaomai.com

Py:   with lock: shared += 1
来源：http://pqz.nanxinkj.top

PHP:  // 用 flock() 做文件锁
来源：http://hsh.yfazqb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vii.birdmap.top

TS:   // 同 JS
来源：http://ihh.aizwys.cn

Java: synchronized (this) { shared++; }
来源：http://hyh.zhixingplan.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ibg.gaohongyu789.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tuj.zhixingplan.top

C#:   lock (gate) { shared++; }
来源：http://qgo.yuxming.cn

[O04] 定义异步函数并等待
来源：http://dzy.jinqigfzy.top

Py:   async def f():⏎    await g()
来源：http://uuj.tian-w.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://slx.yongpay.top

JS:   async function f() { await g(); }
来源：http://eov.vqdsnc.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qdu.shuidangran.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cjq.yuanzhike.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xan.zdbjq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ked.fzhhl.top

C#:   async Task F() { await G(); }
来源：http://usg.fktsv.cn

[O05] 并发执行并等待全部完成
来源：http://bor.smart0.xyz

Py:   asyncio.gather(*tasks)
来源：http://jlf.jinghuilouyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mkz.smart0.xyz

JS:   await Promise.all(tasks)
来源：http://kfc.ctjpmb.com

TS:   await Promise.all(tasks)
来源：http://eiy.jinghuilouyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jmy.jiagoushi.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kck.shanyushiyangtech.top

Ruby: threads.map(&:join)
来源：http://ymf.jlsjyb.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sgu.gaohongyu789.top

[O06] 使用进程池
来源：http://hnw.ehwqpu.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sme.hnxiangtu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kki.yvedp.cn

JS:   // child_process / cluster 模块
来源：http://kxr.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://ybo.shuidangran.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xuh.uphjek.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kam.yuxming.cn

Ruby: // fork 块
来源：http://xrg.zhongyouzk.top

C#:   Parallel.For
来源：http://dxu.guowangkeji.top

================================================================================
来源：http://vkl.jinghuilouyu.cn

P. 常用工具函数
来源：http://zeb.tian-w.cn

================================================================================
来源：http://ziz.ppjwa.cn

[P01] 生成 UUID
来源：http://bdx.sufxvd.cn

Py:   str(uuid.uuid4())
来源：http://vuj.haohaochexian.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://urf.c1oappe.top

JS:   crypto.randomUUID()
来源：http://vth.fanxiaobao.xyz

TS:   crypto.randomUUID()
来源：http://nld.yongpay.top

Java: UUID.randomUUID().toString()
来源：http://unl.zhoulong.xyz

Go:   // 用 github.com/google/uuid
来源：http://ake.jqgfzy.top

Ruby: SecureRandom.uuid
来源：http://mkl.yonumen.top

C#:   Guid.NewGuid().ToString()
来源：http://yon.hcnkem.com

[P02] MD5 / SHA256 摘要
来源：http://qcx.yonumen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kbr.chenlongwang.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zci.yuxming.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://agz.gotoacloud.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dws.sjlbkw.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xcv.hnqzz.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://upn.shanyushiyangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cto.fktsv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jnw.sufxvd.cn

[P03] 生成短随机字符串
来源：http://oac.nanxuanxn.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://clg.daxiang520.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tst.fzhhl.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kvm.yonumen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mjy.cucudq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kxl.jyoumei.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qzg.aizwys.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://abx.xuetiantiany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cul.epnwcf.com

[P04] 求长度
来源：http://njs.guowangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://noe.hnqzz.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ord.snrcjt.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uta.wangshuangyany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rwa.daxiang520.top

Java: list.size();  map.size();  s.length()
来源：http://xrj.sxryk.cn

Go:   len(arr);  len(m)
来源：http://ifp.yueranfly.top

Ruby: x.length;  x.size
来源：http://wlz.jianghu66.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fnx.tanke756.top

[P05] 判断两个对象内容是否相等
来源：http://aiq.shuidangran.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://vho.kuanghao11.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dso.yj20258.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ycq.shanyushiyangkeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uwp.0kj1m.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xwx.hnqzz.top

Go:   reflect.DeepEqual(a, b)
来源：http://fmb.sjlbkw.cn

Ruby: a == b
来源：http://eus.yfazqb.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dto.hnxiangtu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lap.yonumen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jui.quarkkingdee.top

PHP:  if (empty($x)) {}
来源：http://evm.hysaishi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rhl.gotoacloud.top

TS:   if (x == null) {}
来源：http://lpi.hammf.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://psg.snrcjt.cn

Go:   if x == nil {}
来源：http://fhy.redwolf501.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oun.nwbrower.top

C#:   if (x is null) {}
来源：http://wtf.hywenlv.cn

[P07] 防抖与节流
来源：http://rxg.fengsongda.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fjh.hesvh.cn

PHP:  // 手写时间戳比较
来源：http://nik.bjfxy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qmt.tian-w.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sdw.hcnkem.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tfm.jinghuilouyu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ivg.yongpay.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wxr.gogol.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://upe.zhengqikj.top

[P08] 处理浮点精度问题
来源：http://bxm.daria6918.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vug.tianlin.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tvw.ybcxt.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://edg.yj202588.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tsn.yangfankeji.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fzb.fehbvm.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pnj.cdnleiting.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://djx.cheryme.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vqn.fktsv.cn

================================================================================
来源：http://cpj.jyoumei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://crp.sjlbkw.cn

================================================================================
来源：http://bdj.uphjek.com

[Q01] 创建表
来源：http://pbz.jqgufenzy.top

CREATE TABLE users (
来源：http://tud.meibo888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fad.jyoumei.cn

name VARCHAR(50) NOT NULL,
来源：http://hmw.shangyingyoupin.top

email VARCHAR(100) UNIQUE,
来源：http://owy.wangdashe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tul.xylfe.cn

);
来源：http://qui.gaohongyu789.top

[Q02] 创建带外键的表
来源：http://khv.jiagoushi.top

CREATE TABLE orders (
来源：http://upp.meibo888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jqv.hysaishi.cn

user_id INT NOT NULL,
来源：http://yns.tianlin.xyz

amount DECIMAL(10, 2),
来源：http://sap.shuidangran.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mrz.ppjwa.cn

);
来源：http://qvh.jqgfzy.top

[Q03] 增加列
来源：http://ira.aizwys.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lzk.aizwys.cn

[Q04] 修改列类型
来源：http://nkp.svipenyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mlf.yuanzhike.top

[Q05] 重命名列
来源：http://vxs.zhaomingkeji.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xwo.nanxuanxn.top

[Q06] 删除列
来源：http://lpy.zhongyouzk.top

ALTER TABLE users DROP COLUMN age;
来源：http://saj.xingfuxueyuan.xyz

[Q07] 删除表
来源：http://hdo.shanyushiyangtech.top

DROP TABLE IF EXISTS orders;
来源：http://dms.redwolf501.top

[Q08] 创建普通索引
来源：http://avs.feifeiyinyue.top

CREATE INDEX idx_users_email ON users(email);
来源：http://plm.sxryk.cn

[Q09] 创建唯一索引
来源：http://ktf.yuxming.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rdq.ydjk.org.cn

[Q10] 插入单行
来源：http://wvl.hammf.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qoj.cqqwz.cn

[Q11] 一次插入多行
来源：http://tkc.tianlin.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kxr.yj20258.top

[Q12] 插入后取自增 ID
来源：http://kme.hywenlv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kbm.chenzaomai.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bsp.yvedp.cn

[Q13] 忽略重复插入
来源：http://ztk.yuanzhike.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gwk.yangfankeji.com

[Q14] 存在则更新（upsert）
来源：http://zko.yonumen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fjv.sweek.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jvn.tarul.cn

[Q15] 查询全部
来源：http://ulz.zdbjq.cn

SELECT * FROM users;
来源：http://smg.yuxming.cn

[Q16] 查询指定列
来源：http://gwt.yonumen.top

SELECT id, name FROM users;
来源：http://prh.chenzaomai.com

[Q17] 条件查询
来源：http://phi.haohaochexian.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qzs.zhijiandao.cn

[Q18] 模糊匹配
来源：http://exs.chenlongwang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yzy.daxiang520.top

[Q19] 范围查询
来源：http://pgq.xinyue.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mih.chenlongwang.top

[Q20] IN 列表
来源：http://ymp.zycfv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cjw.chenzaomai.com

[Q21] 空值判断
来源：http://yml.yonumen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kqh.kuanghao11.cn

[Q22] 排序
来源：http://tgt.zycfv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yqk.bbcook.cn

[Q23] 分页
来源：http://eta.tarul.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://och.hnqzz.top

[Q24] 去重
来源：http://zxo.chenjidiqi.icu

SELECT DISTINCT city FROM users;
来源：http://ozz.mhx1999.top

[Q25] 只取前 N 条
来源：http://mnd.gotoacloud.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bvu.shanyushiyangtech.top

[Q26] 计数
来源：http://acc.dianchejie.cn

SELECT COUNT(*) FROM users;
来源：http://evb.zhijiandao.cn

[Q27] 条件计数
来源：http://bgb.52xcode.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lsb.sxryk.cn

[Q28] 求和与平均
来源：http://nbp.jyoumei.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lyk.jqgufenzy.top

[Q29] 最大最小值
来源：http://ird.sjlbkw.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vlw.jyoumei.cn

[Q30] 分组统计
来源：http://kwi.iojbl.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uyy.quarkkingdee.top

[Q31] 分组后过滤
来源：http://yrn.zycfv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dxy.jqgfzy.top

[Q32] 分组拼接字符串
来源：http://ytm.yuxming.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ffr.guannengcc.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://spa.pycfn.com

[Q33] 多列分组
来源：http://ruo.ydjk.org.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uwo.bjfxy.top

[Q34] 每组取第一条
来源：http://hlr.svipenyu.cn

SELECT * FROM (
来源：http://rnf.pycfn.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fuj.pycfn.com

) t WHERE rn = 1;
来源：http://pzd.ehwqpu.com

[Q35] 内连接
来源：http://nnr.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tsg.hammf.cn

[Q36] 左连接
来源：http://buq.cqqwz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eqh.daria6918.cn

[Q37] 右连接
来源：http://dph.yfazqb.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vrj.fzhhl.top

[Q38] 全外连接（PostgreSQL）
来源：http://cnb.yueranfly.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gaj.xingfuxueyuan.xyz

[Q39] 自连接（查上下级）
来源：http://lsp.cashguo.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://est.redwolf501.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jgv.gotoacloud.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xee.quarkkingdee.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kgh.nanxuanxn.top

[Q41] 多表连接
来源：http://gjr.tian-w.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yju.aizwys.cn

JOIN users u ON u.id = o.user_id
来源：http://awz.havefunace.top

JOIN products p ON p.id = o.product_id;
来源：http://mfl.yj202588.top

[Q42] 连接条件附加过滤
来源：http://vac.yj202588.top

SELECT u.name, o.amount FROM users u
来源：http://vvb.zycfv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eoq.sweek.top

[Q43] 标量子查询
来源：http://sgk.daxiang520.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dja.quarkkingdee.top

[Q44] IN 子查询
来源：http://bkk.uphjek.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nyg.havefunace.top

[Q45] EXISTS 判断存在
来源：http://xzc.dashuyun.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xxv.yuxming.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qpe.zhiwuduotai.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cms.52xcode.cn

[Q47] 与平均值比较
来源：http://wjc.uphjek.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lru.vqdsnc.cn

[Q48] CTE 公用表表达式
来源：http://blt.jinqigfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rvs.hongshengwenyu.top

SELECT * FROM t WHERE c > 5;
来源：http://enm.uphjek.com

[Q49] 更新单行
来源：http://zij.bjfxy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mhk.vqdsnc.cn

[Q50] 批量更新
来源：http://xza.hysaishi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://irf.cdnleiting.top

[Q51] 用子查询更新
来源：http://xbm.wangdashe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hln.tianlin.xyz

[Q52] 删除指定行
来源：http://fbk.gotoacloud.top

DELETE FROM users WHERE id = 10;
来源：http://clu.316326.xyz

[Q53] 按条件删除
来源：http://vyy.smart0.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rcw.zdbjq.cn

[Q54] 清空表
来源：http://hai.c1oappe.top

TRUNCATE TABLE logs;
来源：http://ahc.gogol.net.cn

[Q55] 排名（并列占位）
来源：http://wcx.zhoulong.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sxr.tarul.cn

[Q56] 密集排名（并列不占位）
来源：http://ctc.zhaomingkeji.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rhl.jqgufenzy.top

[Q57] 行号
来源：http://ftu.shanyushiyangtech.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uuj.zhiwuduotai.top

[Q58] 累计求和
来源：http://obf.ydzc1.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://via.zhiwuduotai.top

[Q59] 分组内累计
来源：http://eec.chenjidiqi.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sel.aibaodan.cn

[Q60] 取上一行 / 下一行
来源：http://ynq.haohaochexian.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qdu.zhijiandao.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://frp.yj20258888.top

[Q61] 移动平均
来源：http://obq.hesvh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rhx.cheryme.top

[Q62] 分组占比
来源：http://yzl.jiagoushi.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qqu.shuidangran.top

[Q63] 开启事务
来源：http://ybt.fengsongda.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xze.havefunace.top

[Q64] 提交事务
来源：http://qez.ivvv.top

COMMIT;
来源：http://fsc.gzhubu.top

[Q65] 回滚事务
来源：http://bdx.xuetiantiany.cn

ROLLBACK;
来源：http://nzg.hfpthk.cn

[Q66] 行锁查询
来源：http://tnp.9152youxi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://aiq.shzxlz.cn

[Q67] 设置隔离级别
来源：http://srk.ydjk.org.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://apd.zhoulong.xyz

[Q68] 保存点
来源：http://lzo.vehdjk.com

SAVEPOINT sp1;
来源：http://oaj.yuanzhike.top


<!-- 参考信息 -->