代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://srm.vqdsnc.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lgm.zhoulong.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nvt.zhengqikj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jvi.yonumen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ymn.zhijiandao.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mao.quarkkingdee.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://myk.ivvv.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ijx.cheryme.top

================================================================================
来源：http://mgh.wangshuangyany.cn

O. 并发与异步
来源：http://qfe.yj202588.top

================================================================================
来源：http://gxb.ydzc1.top

[O01] 启动一个线程
来源：http://tpu.yfazqb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tco.ppjwa.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://obh.sysykeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ztg.zycfv.cn

TS:   // 同 JS
来源：http://ofp.shanyushiyangtech.top

Java: new Thread(() -> f()).start()
来源：http://uvc.hywenlv.cn

Go:   go f()
来源：http://zdw.zhongyouzk.top

Ruby: Thread.new { f }
来源：http://mff.hammf.cn

C#:   Task.Run(() => F());
来源：http://fml.shzxlz.cn

[O02] 使用线程池
来源：http://duc.nwbrower.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lrr.0kj1m.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jrz.fanxiaobao.xyz

JS:   // worker_threads 线程池
来源：http://jqa.hnxiangtu.top

TS:   // worker_threads 线程池
来源：http://lgj.bjfxy.top

Java: Executors.newFixedThreadPool(4)
来源：http://kpl.jinyuanbaomall.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qnm.gotoacloud.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zdu.yfazqb.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hpa.yj20258.top

[O03] 加锁保护共享数据
来源：http://cvn.zycfv.cn

Py:   with lock: shared += 1
来源：http://wbw.jinghuilouyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://vhq.jyoumei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fih.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://eem.sweek.top

Java: synchronized (this) { shared++; }
来源：http://zvc.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://etw.fengsongda.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ejz.iojbl.cn

C#:   lock (gate) { shared++; }
来源：http://cbm.meibo888.top

[O04] 定义异步函数并等待
来源：http://koq.svipenyu.cn

Py:   async def f():⏎    await g()
来源：http://olb.chenzaomai.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lja.jianghu66.top

JS:   async function f() { await g(); }
来源：http://qco.cheryme.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://iqo.ppjwa.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dmh.yj20258.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yak.xingfuxueyuan.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://rtt.pycfn.com

C#:   async Task F() { await G(); }
来源：http://axt.yj20258.top

[O05] 并发执行并等待全部完成
来源：http://miz.haohaochexian.top

Py:   asyncio.gather(*tasks)
来源：http://kvk.chenzaomai.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kkb.tarul.cn

JS:   await Promise.all(tasks)
来源：http://pze.wangshuangyany.cn

TS:   await Promise.all(tasks)
来源：http://pkm.sweek.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tbr.cashguo.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zmp.zhoulong.xyz

Ruby: threads.map(&:join)
来源：http://qyj.tarul.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://anr.ywan-chungtsiang.top

[O06] 使用进程池
来源：http://nzn.yanxiufei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qfm.aizwys.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fox.yuanzhike.top

JS:   // child_process / cluster 模块
来源：http://mwl.aibaodan.cn

TS:   // child_process / cluster 模块
来源：http://yxd.0kj1m.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qox.yj20258888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ufn.cucudq.cn

Ruby: // fork 块
来源：http://ynl.yj202588.top

C#:   Parallel.For
来源：http://zcg.zdqjudy.top

================================================================================
来源：http://rqe.hnxiangtu.top

P. 常用工具函数
来源：http://xoj.fzhhl.top

================================================================================
来源：http://lsf.jinghuilouyu.cn

[P01] 生成 UUID
来源：http://ffu.haohaochexian.top

Py:   str(uuid.uuid4())
来源：http://ymt.fehbvm.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rzc.sweek.top

JS:   crypto.randomUUID()
来源：http://qox.jqgfzy.top

TS:   crypto.randomUUID()
来源：http://edd.haohaochexian.top

Java: UUID.randomUUID().toString()
来源：http://cew.xuetiantiany.cn

Go:   // 用 github.com/google/uuid
来源：http://qnh.hnqzz.top

Ruby: SecureRandom.uuid
来源：http://exj.yongpay.top

C#:   Guid.NewGuid().ToString()
来源：http://hfa.yj20258888.top

[P02] MD5 / SHA256 摘要
来源：http://umd.iojbl.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pge.yj20258888.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://eut.fengsongda.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pwy.hcnkem.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://neu.xuetiantiany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ogw.bjfxy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qzo.gzhubu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ebn.zycfv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://voy.tanke756.top

[P03] 生成短随机字符串
来源：http://egx.hongshengwenyu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jla.cucudq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jbx.kuanghao11.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wgb.xingfuxueyuan.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xie.sysykeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dbd.jinyuanbaomall.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aad.smart0.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://jvi.fzhhl.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hkl.yanxiufei.cn

[P04] 求长度
来源：http://ofj.pengpengdd.cyou

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xhj.bbcook.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tip.jlsjyb.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://efj.tanke756.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://myw.yanxiufei.cn

Java: list.size();  map.size();  s.length()
来源：http://mlr.sysykeji.top

Go:   len(arr);  len(m)
来源：http://hcz.meibo888.top

Ruby: x.length;  x.size
来源：http://bul.hnxiangtu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://stx.aizwys.cn

[P05] 判断两个对象内容是否相等
来源：http://jvs.zhaomingkeji.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://udo.zhijiandao.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qzj.hammf.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wuz.daxiang520.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yax.bjfxy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://edh.smart0.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://gnp.gogol.net.cn

Ruby: a == b
来源：http://iuh.birdmap.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mgp.ehwqpu.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jog.ppjwa.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sve.fzhhl.top

PHP:  if (empty($x)) {}
来源：http://edg.ctjpmb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rxn.fanxiaobao.xyz

TS:   if (x == null) {}
来源：http://ywr.hcnkem.com

Java: if (x == null || x.isEmpty()) {}
来源：http://wpv.snrcjt.cn

Go:   if x == nil {}
来源：http://fnf.jqgufenzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ewn.hcnkem.com

C#:   if (x is null) {}
来源：http://ayz.aizwys.cn

[P07] 防抖与节流
来源：http://ylx.chenlongwang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sqk.uphjek.com

PHP:  // 手写时间戳比较
来源：http://npb.dianchejie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ant.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lye.jinqigufen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cie.sxryk.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://skv.yvedp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lwk.aibaodan.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://itm.gotoacloud.top

[P08] 处理浮点精度问题
来源：http://lnn.xuanzx.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ndq.sysykeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sjw.ivvv.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yoj.hammf.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qne.fengsongda.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aau.vqdsnc.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uwt.daxiang520.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dsv.sxryk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zxr.yuanzhike.top

================================================================================
来源：http://sjf.hysaishi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://txq.pengpengdd.cyou

================================================================================
来源：http://ewr.zhengqikj.top

[Q01] 创建表
来源：http://nar.jqgufenzy.top

CREATE TABLE users (
来源：http://sjx.haohaochexian.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pwy.wangshuangyany.cn

name VARCHAR(50) NOT NULL,
来源：http://crp.cqqwz.cn

email VARCHAR(100) UNIQUE,
来源：http://egc.sysykeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://red.fanxiaobao.xyz

);
来源：http://wok.zdqjudy.top

[Q02] 创建带外键的表
来源：http://yfw.hammf.cn

CREATE TABLE orders (
来源：http://nem.zdqjudy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xxl.9152youxi.cn

user_id INT NOT NULL,
来源：http://vot.cdnleiting.top

amount DECIMAL(10, 2),
来源：http://eky.kuanghao11.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ved.snrcjt.cn

);
来源：http://hpv.tarul.cn

[Q03] 增加列
来源：http://hzd.dianchejie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hmg.yonumen.top

[Q04] 修改列类型
来源：http://erf.fengsongda.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rqr.shanyushiyangtech.top

[Q05] 重命名列
来源：http://xui.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tgx.birdmap.top

[Q06] 删除列
来源：http://fhl.zhengqikj.top

ALTER TABLE users DROP COLUMN age;
来源：http://jkp.hesvh.cn

[Q07] 删除表
来源：http://qil.gaohongyu789.top

DROP TABLE IF EXISTS orders;
来源：http://vvw.vqdsnc.cn

[Q08] 创建普通索引
来源：http://fjf.cdnleiting.top

CREATE INDEX idx_users_email ON users(email);
来源：http://yky.cqqwz.cn

[Q09] 创建唯一索引
来源：http://erk.kuanghao11.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cdt.cdnleiting.top

[Q10] 插入单行
来源：http://ien.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lbr.yj20258888.top

[Q11] 一次插入多行
来源：http://num.zhixingplan.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kpt.mhx1999.top

[Q12] 插入后取自增 ID
来源：http://oko.zdqjudy.top

INSERT INTO users (name) VALUES ('C');
来源：http://anf.0kj1m.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yyj.zhixingplan.top

[Q13] 忽略重复插入
来源：http://gbt.dianchejie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vid.sufxvd.cn

[Q14] 存在则更新（upsert）
来源：http://rhx.zhongyouzk.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dcb.quarkkingdee.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jdk.xingfuxueyuan.xyz

[Q15] 查询全部
来源：http://zsy.9152youxi.cn

SELECT * FROM users;
来源：http://wes.zhoulong.xyz

[Q16] 查询指定列
来源：http://zzd.sysykeji.top

SELECT id, name FROM users;
来源：http://tsd.52xcode.cn

[Q17] 条件查询
来源：http://zgz.tarul.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ptv.chenzaomai.com

[Q18] 模糊匹配
来源：http://vii.zdbjq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ojt.ctjpmb.com

[Q19] 范围查询
来源：http://grg.meibo888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dfb.sxryk.cn

[Q20] IN 列表
来源：http://mcv.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kuw.hcnkem.com

[Q21] 空值判断
来源：http://jlv.yj20258888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://cfk.gaohongyu789.top

[Q22] 排序
来源：http://gcw.hnqzz.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://thh.hcnkem.com

[Q23] 分页
来源：http://izx.jiagoushi.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ewk.dashuyun.cn

[Q24] 去重
来源：http://bcb.52xcode.cn

SELECT DISTINCT city FROM users;
来源：http://uqi.ywan-chungtsiang.top

[Q25] 只取前 N 条
来源：http://pgj.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nph.jinghuilouyu.cn

[Q26] 计数
来源：http://eqf.smart0.xyz

SELECT COUNT(*) FROM users;
来源：http://ice.ivvv.top

[Q27] 条件计数
来源：http://foi.cqqwz.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ust.yonumen.top

[Q28] 求和与平均
来源：http://mxp.yuxming.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eiv.c1oappe.top

[Q29] 最大最小值
来源：http://dfr.uphjek.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://dqk.cheryme.top

[Q30] 分组统计
来源：http://eup.smart0.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mjo.bjfxy.top

[Q31] 分组后过滤
来源：http://qao.fengsongda.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ggi.0kj1m.cn

[Q32] 分组拼接字符串
来源：http://stp.meibo888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yux.sjlbkw.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://aum.cucudq.cn

[Q33] 多列分组
来源：http://kqm.xinyue.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://byb.xingfuxueyuan.xyz

[Q34] 每组取第一条
来源：http://zhg.kuanghao11.cn

SELECT * FROM (
来源：http://exv.shanyushiyangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lzi.xuetiantiany.cn

) t WHERE rn = 1;
来源：http://hun.xingfuxueyuan.xyz

[Q35] 内连接
来源：http://ktm.ybcxt.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ccf.ydjk.org.cn

[Q36] 左连接
来源：http://itw.zhongyouzk.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xbn.vqdsnc.cn

[Q37] 右连接
来源：http://brk.jinyuanbaomall.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mik.nwbrower.top

[Q38] 全外连接（PostgreSQL）
来源：http://ovm.xziqi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fbd.cdnleiting.top

[Q39] 自连接（查上下级）
来源：http://ceu.xylfe.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xbb.hywenlv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fyb.zhixingplan.top

[Q40] 交叉连接（笛卡尔积）
来源：http://kad.guowangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://aps.sxryk.cn

[Q41] 多表连接
来源：http://ogn.zdqjudy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ddq.cdnleiting.top

JOIN users u ON u.id = o.user_id
来源：http://ilj.shangyingyoupin.top

JOIN products p ON p.id = o.product_id;
来源：http://cwd.jqgfzy.top

[Q42] 连接条件附加过滤
来源：http://szp.sjlbkw.cn

SELECT u.name, o.amount FROM users u
来源：http://qiw.hywenlv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bol.nwbrower.top

[Q43] 标量子查询
来源：http://eqq.hfpthk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hck.yj202588.top

[Q44] IN 子查询
来源：http://dph.gaohongyu789.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tty.zdbjq.cn

[Q45] EXISTS 判断存在
来源：http://kyy.nwbrower.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tlc.jianghu66.top

[Q46] NOT EXISTS 判断不存在
来源：http://zpz.0kj1m.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://epv.dianchejie.cn

[Q47] 与平均值比较
来源：http://tnj.52xcode.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ayh.yj202588.top

[Q48] CTE 公用表表达式
来源：http://ruc.sxryk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qeb.cashguo.top

SELECT * FROM t WHERE c > 5;
来源：http://cfa.jqgfzy.top

[Q49] 更新单行
来源：http://wxv.xylfe.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jyk.yfazqb.com

[Q50] 批量更新
来源：http://lvo.xziqi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zwl.shanyushiyangtech.top

[Q51] 用子查询更新
来源：http://gkw.pengpengdd.cyou

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pwv.yueranfly.top

[Q52] 删除指定行
来源：http://nhg.pycfn.com

DELETE FROM users WHERE id = 10;
来源：http://tfu.zhixingplan.top

[Q53] 按条件删除
来源：http://jhw.hcnkem.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ivb.yvedp.cn

[Q54] 清空表
来源：http://gvr.chenlongwang.top

TRUNCATE TABLE logs;
来源：http://uwv.chenzaomai.com

[Q55] 排名（并列占位）
来源：http://vtw.zycfv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fvq.shanyushiyangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://mbc.jinqigfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://itf.nwbrower.top

[Q57] 行号
来源：http://ncd.9152youxi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://one.havefunace.top

[Q58] 累计求和
来源：http://tev.tianlin.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zye.birdmap.top

[Q59] 分组内累计
来源：http://wdo.yfazqb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://seh.nwbrower.top

[Q60] 取上一行 / 下一行
来源：http://scc.xuanzx.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://clo.yvedp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://shd.xylfe.cn

[Q61] 移动平均
来源：http://nxg.xziqi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jwo.jqgfzy.top

[Q62] 分组占比
来源：http://zet.andypj.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hju.ybcxt.top

[Q63] 开启事务
来源：http://wbk.tanke756.top

START TRANSACTION;                -- 或 BEGIN
来源：http://lrw.chenzaomai.com

[Q64] 提交事务
来源：http://odb.guannengcc.top

COMMIT;
来源：http://iak.zhiwuduotai.top

[Q65] 回滚事务
来源：http://ujy.nanxinkj.top

ROLLBACK;
来源：http://mar.yueranfly.top

[Q66] 行锁查询
来源：http://buv.aibaodan.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qjz.xziqi.cn

[Q67] 设置隔离级别
来源：http://hda.yueranfly.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pty.yanxiufei.cn

[Q68] 保存点
来源：http://cui.hammf.cn

SAVEPOINT sp1;
来源：http://vcv.zdqjudy.top


<!-- 参考信息 -->