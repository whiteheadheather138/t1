代发 wailian999

Go:   // 手写递归
来源：http://bpw.yuxming.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oyb.zdbjq.cn

C#:   // 手写递归
来源：http://hdp.chenjidiqi.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nab.yj20258.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://chq.yj202588.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wev.kuanghao11.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kpq.fengsongda.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rug.hfpthk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rqq.ivvv.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vhy.yuanzhike.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ghh.cqqwz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qdt.xuanzx.com

================================================================================
来源：http://jgu.smart0.xyz

O. 并发与异步
来源：http://yzz.bjfxy.top

================================================================================
来源：http://sdb.zdbjq.cn

[O01] 启动一个线程
来源：http://lzg.nanxinkj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://eja.haohaochexian.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://foc.ydjk.org.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ozb.zdqjudy.top

TS:   // 同 JS
来源：http://hjj.quarkkingdee.top

Java: new Thread(() -> f()).start()
来源：http://veh.xuetiantiany.cn

Go:   go f()
来源：http://vhz.jqgfzy.top

Ruby: Thread.new { f }
来源：http://kpl.yanxiufei.cn

C#:   Task.Run(() => F());
来源：http://vtt.zhiwuduotai.top

[O02] 使用线程池
来源：http://snh.nwbrower.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gog.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xjh.aizwys.cn

JS:   // worker_threads 线程池
来源：http://cxh.jqgufenzy.top

TS:   // worker_threads 线程池
来源：http://qcj.havefunace.top

Java: Executors.newFixedThreadPool(4)
来源：http://rfl.vqdsnc.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ixk.ivvv.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wjs.tarul.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ddt.nwbrower.top

[O03] 加锁保护共享数据
来源：http://jcb.xinyue.icu

Py:   with lock: shared += 1
来源：http://jjw.sufxvd.cn

PHP:  // 用 flock() 做文件锁
来源：http://svx.quarkkingdee.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tuo.yanxiufei.cn

TS:   // 同 JS
来源：http://owo.daria6918.cn

Java: synchronized (this) { shared++; }
来源：http://icf.epnwcf.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dzl.jiagoushi.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tjz.tianlin.xyz

C#:   lock (gate) { shared++; }
来源：http://grk.zhongyouzk.top

[O04] 定义异步函数并等待
来源：http://daf.jqgfzy.top

Py:   async def f():⏎    await g()
来源：http://gpm.yj20258.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://psb.shuidangran.top

JS:   async function f() { await g(); }
来源：http://feq.shangyingyoupin.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qqx.snrcjt.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vfd.xinyue.icu

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zlp.hesvh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zbu.fehbvm.com

C#:   async Task F() { await G(); }
来源：http://iid.ydjk.org.cn

[O05] 并发执行并等待全部完成
来源：http://bsb.jinqigufen.top

Py:   asyncio.gather(*tasks)
来源：http://xtg.hywenlv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vea.wangshuangyany.cn

JS:   await Promise.all(tasks)
来源：http://xlx.9152youxi.cn

TS:   await Promise.all(tasks)
来源：http://dvh.zdqjudy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pim.aibaodan.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wpg.shangyingyoupin.top

Ruby: threads.map(&:join)
来源：http://yav.jinyuanbaomall.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wlp.jlsjyb.cn

[O06] 使用进程池
来源：http://gqk.cashguo.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zhp.cucudq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rja.hysaishi.cn

JS:   // child_process / cluster 模块
来源：http://kdm.tian-w.cn

TS:   // child_process / cluster 模块
来源：http://coo.hcnkem.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nqm.vehdjk.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://myy.xylfe.cn

Ruby: // fork 块
来源：http://smy.gogol.net.cn

C#:   Parallel.For
来源：http://dxe.havefunace.top

================================================================================
来源：http://fqe.pengpengdd.cyou

P. 常用工具函数
来源：http://nvy.cdnleiting.top

================================================================================
来源：http://olb.wangshuangyany.cn

[P01] 生成 UUID
来源：http://tqd.ywan-chungtsiang.top

Py:   str(uuid.uuid4())
来源：http://zwx.zhiwuduotai.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fdk.sufxvd.cn

JS:   crypto.randomUUID()
来源：http://bil.hywenlv.cn

TS:   crypto.randomUUID()
来源：http://ueg.ywan-chungtsiang.top

Java: UUID.randomUUID().toString()
来源：http://ouc.hfpthk.cn

Go:   // 用 github.com/google/uuid
来源：http://iut.sufxvd.cn

Ruby: SecureRandom.uuid
来源：http://tin.iojbl.cn

C#:   Guid.NewGuid().ToString()
来源：http://pah.shangyingyoupin.top

[P02] MD5 / SHA256 摘要
来源：http://xab.guowangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gaa.shanyushiyangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://pde.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hwj.xinyue.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xcr.xuetiantiany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rlw.cashguo.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dki.gotoacloud.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ejt.fanxiaobao.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iay.gzhubu.top

[P03] 生成短随机字符串
来源：http://ust.yuxming.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ctm.guannengcc.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://maf.daxiang520.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://smg.jlsjyb.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kfl.epnwcf.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://clw.jinyuanbaomall.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jsy.shuidangran.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zwk.redwolf501.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hqd.c1oappe.top

[P04] 求长度
来源：http://llg.zhengqikj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ajw.hnxiangtu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ecz.shanyushiyangtech.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jgv.fanxiaobao.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://awl.ydzc1.top

Java: list.size();  map.size();  s.length()
来源：http://wkx.hammf.cn

Go:   len(arr);  len(m)
来源：http://nrh.hammf.cn

Ruby: x.length;  x.size
来源：http://evf.shuidangran.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://iou.ydzc1.top

[P05] 判断两个对象内容是否相等
来源：http://rew.sxryk.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dem.jiagoushi.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jsb.epnwcf.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bds.ehwqpu.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fyc.jqgufenzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kpy.yvedp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://stx.daria6918.cn

Ruby: a == b
来源：http://kyr.chenjidiqi.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rlf.chenjidiqi.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://drj.yueranfly.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uru.nwbrower.top

PHP:  if (empty($x)) {}
来源：http://jjr.quarkkingdee.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://seu.andypj.xyz

TS:   if (x == null) {}
来源：http://jla.gaohongyu789.top

Java: if (x == null || x.isEmpty()) {}
来源：http://nbr.jinqigufen.top

Go:   if x == nil {}
来源：http://vbx.yanxiufei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://htl.andypj.xyz

C#:   if (x is null) {}
来源：http://nml.hcnkem.com

[P07] 防抖与节流
来源：http://aes.andypj.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://txp.yuxming.cn

PHP:  // 手写时间戳比较
来源：http://cfr.dianchejie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sji.dashuyun.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kbv.tarul.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zib.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mcg.hnqzz.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nif.haohaochexian.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xjt.xylfe.cn

[P08] 处理浮点精度问题
来源：http://mzz.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zmn.gotoacloud.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ilh.feifeiyinyue.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kff.iojbl.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ifg.cqqwz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mby.yj20258888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yyn.gotoacloud.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jyk.ydjk.org.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rhs.sufxvd.cn

================================================================================
来源：http://hrn.cashguo.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oyf.guowangkeji.top

================================================================================
来源：http://zki.0kj1m.cn

[Q01] 创建表
来源：http://opo.nanxinkj.top

CREATE TABLE users (
来源：http://boj.nwbrower.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://evd.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://xmg.jianghu66.top

email VARCHAR(100) UNIQUE,
来源：http://vqw.xingfuxueyuan.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://orp.shanyushiyangtech.top

);
来源：http://oxn.jinyuanbaomall.cn

[Q02] 创建带外键的表
来源：http://uih.hammf.cn

CREATE TABLE orders (
来源：http://dkc.cashguo.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ekw.ydjk.org.cn

user_id INT NOT NULL,
来源：http://jjm.jiagoushi.top

amount DECIMAL(10, 2),
来源：http://cmq.ywan-chungtsiang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rgl.yuanzhike.top

);
来源：http://fdj.xuanzx.com

[Q03] 增加列
来源：http://xmz.yongpay.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hps.nanxuanxn.top

[Q04] 修改列类型
来源：http://pdp.gaohongyu789.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rsc.yangfankeji.com

[Q05] 重命名列
来源：http://vvi.tanke756.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jph.chenjidiqi.icu

[Q06] 删除列
来源：http://llo.birdmap.top

ALTER TABLE users DROP COLUMN age;
来源：http://xjj.zhiwuduotai.top

[Q07] 删除表
来源：http://erj.ppjwa.cn

DROP TABLE IF EXISTS orders;
来源：http://kfm.tarul.cn

[Q08] 创建普通索引
来源：http://pqo.feifeiyinyue.top

CREATE INDEX idx_users_email ON users(email);
来源：http://zvh.tianlin.xyz

[Q09] 创建唯一索引
来源：http://gtd.ybcxt.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pfl.zdbjq.cn

[Q10] 插入单行
来源：http://uxn.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sbo.svipenyu.cn

[Q11] 一次插入多行
来源：http://cik.cheryme.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gpd.sxryk.cn

[Q12] 插入后取自增 ID
来源：http://ohd.pycfn.com

INSERT INTO users (name) VALUES ('C');
来源：http://rzv.zhixingplan.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hde.316326.xyz

[Q13] 忽略重复插入
来源：http://rnb.smart0.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jeq.cashguo.top

[Q14] 存在则更新（upsert）
来源：http://zut.ehwqpu.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://udi.kuanghao11.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vku.feifeiyinyue.top

[Q15] 查询全部
来源：http://vbp.xuanzx.com

SELECT * FROM users;
来源：http://zqg.yongpay.top

[Q16] 查询指定列
来源：http://bjw.zycfv.cn

SELECT id, name FROM users;
来源：http://kla.haohaochexian.top

[Q17] 条件查询
来源：http://qac.zhoulong.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ppp.yonumen.top

[Q18] 模糊匹配
来源：http://gtf.pengpengdd.cyou

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fpu.hysaishi.cn

[Q19] 范围查询
来源：http://tkc.quarkkingdee.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ccf.tanke756.top

[Q20] IN 列表
来源：http://qpo.dianchejie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wav.xuetiantiany.cn

[Q21] 空值判断
来源：http://uql.yonumen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://eaj.yuanzhike.top

[Q22] 排序
来源：http://mci.tanke756.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://guz.hongshengwenyu.top

[Q23] 分页
来源：http://zuk.ydzc1.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://aqn.shzxlz.cn

[Q24] 去重
来源：http://cki.vehdjk.com

SELECT DISTINCT city FROM users;
来源：http://qrz.yvedp.cn

[Q25] 只取前 N 条
来源：http://aov.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fuz.hesvh.cn

[Q26] 计数
来源：http://ezd.sxryk.cn

SELECT COUNT(*) FROM users;
来源：http://xiw.chenlongwang.top

[Q27] 条件计数
来源：http://fzq.andypj.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mwt.wangshuangyany.cn

[Q28] 求和与平均
来源：http://nfk.redwolf501.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zvn.yj20258.top

[Q29] 最大最小值
来源：http://ktd.guannengcc.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://otd.fanxiaobao.xyz

[Q30] 分组统计
来源：http://csp.sysykeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yrz.wangdashe.top

[Q31] 分组后过滤
来源：http://dqp.xuetiantiany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vus.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://lhk.daxiang520.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mdd.bjfxy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lhq.dianchejie.cn

[Q33] 多列分组
来源：http://tja.zhoulong.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pss.quarkkingdee.top

[Q34] 每组取第一条
来源：http://iez.jianghu66.top

SELECT * FROM (
来源：http://nut.vqdsnc.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oco.shuidangran.top

) t WHERE rn = 1;
来源：http://bvr.zhengqikj.top

[Q35] 内连接
来源：http://vfc.svipenyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://crm.ybcxt.top

[Q36] 左连接
来源：http://qyk.yangfankeji.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ajc.xuetiantiany.cn

[Q37] 右连接
来源：http://lgg.xylfe.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://btj.yuanzhike.top

[Q38] 全外连接（PostgreSQL）
来源：http://rco.vehdjk.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cyr.nanxinkj.top

[Q39] 自连接（查上下级）
来源：http://riy.52xcode.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qki.hongshengwenyu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oao.svipenyu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://oum.vqdsnc.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jzf.cashguo.top

[Q41] 多表连接
来源：http://ebg.zhixingplan.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cox.zhongyouzk.top

JOIN users u ON u.id = o.user_id
来源：http://ytv.c1oappe.top

JOIN products p ON p.id = o.product_id;
来源：http://ufp.sjlbkw.cn

[Q42] 连接条件附加过滤
来源：http://mje.cqqwz.cn

SELECT u.name, o.amount FROM users u
来源：http://gif.sufxvd.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ncl.hammf.cn

[Q43] 标量子查询
来源：http://eop.redwolf501.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ufl.yangfankeji.com

[Q44] IN 子查询
来源：http://ivf.bbcook.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mcx.xuanzx.com

[Q45] EXISTS 判断存在
来源：http://qrl.birdmap.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://juk.yueranfly.top

[Q46] NOT EXISTS 判断不存在
来源：http://sga.jinqigfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oge.yvedp.cn

[Q47] 与平均值比较
来源：http://gxy.fehbvm.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://plm.hfpthk.cn

[Q48] CTE 公用表表达式
来源：http://vno.yj20258888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ged.tarul.cn

SELECT * FROM t WHERE c > 5;
来源：http://xip.wangdashe.top

[Q49] 更新单行
来源：http://nre.fengsongda.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zex.uphjek.com

[Q50] 批量更新
来源：http://lua.52xcode.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cyj.jianghu66.top

[Q51] 用子查询更新
来源：http://mnl.yongpay.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pqj.wangdashe.top

[Q52] 删除指定行
来源：http://xry.yj20258888.top

DELETE FROM users WHERE id = 10;
来源：http://vto.epnwcf.com

[Q53] 按条件删除
来源：http://mep.pycfn.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tdf.yuanzhike.top

[Q54] 清空表
来源：http://bjd.birdmap.top

TRUNCATE TABLE logs;
来源：http://urk.shanyushiyangtech.top

[Q55] 排名（并列占位）
来源：http://yfe.fktsv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kax.shuidangran.top

[Q56] 密集排名（并列不占位）
来源：http://xhm.dashuyun.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dnz.xylfe.cn

[Q57] 行号
来源：http://qkb.zycfv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gny.hammf.cn

[Q58] 累计求和
来源：http://dtk.xuetiantiany.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wri.hesvh.cn

[Q59] 分组内累计
来源：http://gzv.316326.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://shy.aibaodan.cn

[Q60] 取上一行 / 下一行
来源：http://ftz.yj20258.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wth.9152youxi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qyj.uphjek.com

[Q61] 移动平均
来源：http://vnq.bbcook.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gzq.yanxiufei.cn

[Q62] 分组占比
来源：http://xnj.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ztb.xuetiantiany.cn

[Q63] 开启事务
来源：http://fxg.xylfe.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lgv.jinqigufen.top

[Q64] 提交事务
来源：http://slx.c1oappe.top

COMMIT;
来源：http://tvo.chenjidiqi.icu

[Q65] 回滚事务
来源：http://kua.ybcxt.top

ROLLBACK;
来源：http://vyv.uphjek.com

[Q66] 行锁查询
来源：http://fuz.c1oappe.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nlk.sufxvd.cn


<!-- 参考信息 -->