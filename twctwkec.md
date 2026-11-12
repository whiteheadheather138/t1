代发 wailian999

PHP:  // 手写递归函数
来源：http://zkn.hnqzz.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tbz.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vgb.xuetiantiany.cn

Java: // 手写递归
来源：http://nfz.sysykeji.top

Go:   // 手写递归
来源：http://rcm.kuanghao11.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wdr.jqgfzy.top

C#:   // 手写递归
来源：http://ydy.shanyushiyangkeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ctn.fehbvm.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mwh.gaohongyu789.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://eir.hnqzz.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://why.hcnkem.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wpn.daxiang520.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rdw.kuanghao11.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yhn.ppjwa.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sso.yanxiufei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yjm.chenjidiqi.icu

================================================================================
来源：http://vxo.guannengcc.top

O. 并发与异步
来源：http://uey.meibo888.top

================================================================================
来源：http://vjo.shangyingyoupin.top

[O01] 启动一个线程
来源：http://knu.tianlin.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://emv.jianghu66.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cvd.cdnleiting.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kmr.sufxvd.cn

TS:   // 同 JS
来源：http://jlz.zhaomingkeji.xyz

Java: new Thread(() -> f()).start()
来源：http://hxq.xuetiantiany.cn

Go:   go f()
来源：http://dhz.hywenlv.cn

Ruby: Thread.new { f }
来源：http://mkx.chenzaomai.com

C#:   Task.Run(() => F());
来源：http://iph.bbcook.cn

[O02] 使用线程池
来源：http://hyp.redwolf501.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ybg.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mze.vehdjk.com

JS:   // worker_threads 线程池
来源：http://nma.wangdashe.top

TS:   // worker_threads 线程池
来源：http://nvk.ywan-chungtsiang.top

Java: Executors.newFixedThreadPool(4)
来源：http://bfp.hcnkem.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mum.hammf.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wcy.hywenlv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ajr.shanyushiyangkeji.top

[O03] 加锁保护共享数据
来源：http://odw.yj202588.top

Py:   with lock: shared += 1
来源：http://haj.nanxinkj.top

PHP:  // 用 flock() 做文件锁
来源：http://qgw.zdbjq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lcb.jlsjyb.cn

TS:   // 同 JS
来源：http://yzg.smart0.xyz

Java: synchronized (this) { shared++; }
来源：http://eye.dianchejie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ydi.sjlbkw.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xjd.yuxming.cn

C#:   lock (gate) { shared++; }
来源：http://kjc.jinqigufen.top

[O04] 定义异步函数并等待
来源：http://gxn.9152youxi.cn

Py:   async def f():⏎    await g()
来源：http://fel.tianlin.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ycw.xingfuxueyuan.xyz

JS:   async function f() { await g(); }
来源：http://smi.ybcxt.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gte.hywenlv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fsr.quarkkingdee.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rnb.yangfankeji.com

Ruby: # 用 Fiber 或 async gem
来源：http://yfk.jinqigufen.top

C#:   async Task F() { await G(); }
来源：http://zcr.zhoulong.xyz

[O05] 并发执行并等待全部完成
来源：http://ucz.ywan-chungtsiang.top

Py:   asyncio.gather(*tasks)
来源：http://ckk.fanxiaobao.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vjn.jqgufenzy.top

JS:   await Promise.all(tasks)
来源：http://hvw.ywan-chungtsiang.top

TS:   await Promise.all(tasks)
来源：http://biy.ivvv.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://seg.gzhubu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sac.havefunace.top

Ruby: threads.map(&:join)
来源：http://nla.tanke756.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fei.gotoacloud.top

[O06] 使用进程池
来源：http://kwh.xuetiantiany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gss.tarul.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ycb.hysaishi.cn

JS:   // child_process / cluster 模块
来源：http://jzi.yueranfly.top

TS:   // child_process / cluster 模块
来源：http://ivg.jlsjyb.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pro.daxiang520.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ahy.wangdashe.top

Ruby: // fork 块
来源：http://mon.fanxiaobao.xyz

C#:   Parallel.For
来源：http://hvg.hysaishi.cn

================================================================================
来源：http://nip.sufxvd.cn

P. 常用工具函数
来源：http://ysy.yonumen.top

================================================================================
来源：http://ith.xylfe.cn

[P01] 生成 UUID
来源：http://ntr.sweek.top

Py:   str(uuid.uuid4())
来源：http://gaf.hcnkem.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pns.yj202588.top

JS:   crypto.randomUUID()
来源：http://xdh.cucudq.cn

TS:   crypto.randomUUID()
来源：http://atw.fehbvm.com

Java: UUID.randomUUID().toString()
来源：http://dhq.hammf.cn

Go:   // 用 github.com/google/uuid
来源：http://ekl.316326.xyz

Ruby: SecureRandom.uuid
来源：http://prt.yanxiufei.cn

C#:   Guid.NewGuid().ToString()
来源：http://rvd.cucudq.cn

[P02] MD5 / SHA256 摘要
来源：http://aak.zhaomingkeji.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dbh.redwolf501.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://iwo.gotoacloud.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zpu.zycfv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pvp.yj202588.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bvq.smart0.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eii.jiagoushi.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ngt.chenlongwang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kws.chenzaomai.com

[P03] 生成短随机字符串
来源：http://kcj.meibo888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mys.uphjek.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fim.zhijiandao.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://acg.jinqigufen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bfq.nanxinkj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tvx.sweek.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ddg.cqqwz.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yxu.nanxinkj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wen.hysaishi.cn

[P04] 求长度
来源：http://hjo.ywan-chungtsiang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dir.jinghuilouyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://elc.jqgufenzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xcs.yangfankeji.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vgz.xingfuxueyuan.xyz

Java: list.size();  map.size();  s.length()
来源：http://jbj.fzhhl.top

Go:   len(arr);  len(m)
来源：http://krr.zhijiandao.cn

Ruby: x.length;  x.size
来源：http://yrf.shanyushiyangtech.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://hjk.yj20258.top

[P05] 判断两个对象内容是否相等
来源：http://xru.ppjwa.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://evb.c1oappe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ndi.xylfe.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://for.jinqigufen.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dns.guannengcc.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nav.xingfuxueyuan.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://ich.feifeiyinyue.top

Ruby: a == b
来源：http://gwg.c1oappe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://znv.fengsongda.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lyr.hcnkem.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tmv.ctjpmb.com

PHP:  if (empty($x)) {}
来源：http://cno.yj20258.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qwh.yanxiufei.cn

TS:   if (x == null) {}
来源：http://njn.zhaomingkeji.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://gwa.zhengqikj.top

Go:   if x == nil {}
来源：http://ido.shzxlz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gae.zhoulong.xyz

C#:   if (x is null) {}
来源：http://ixv.yj20258888.top

[P07] 防抖与节流
来源：http://wtz.dianchejie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zbv.snrcjt.cn

PHP:  // 手写时间戳比较
来源：http://ofg.jyoumei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kpc.xuanzx.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lan.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yoe.gaohongyu789.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ipo.dashuyun.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zow.shanyushiyangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zkm.xuanzx.com

[P08] 处理浮点精度问题
来源：http://riw.wangdashe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hpk.tanke756.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gmo.gzhubu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vka.zhijiandao.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sto.shanyushiyangtech.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uax.wangshuangyany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zyu.hnqzz.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vin.chenzaomai.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qzz.sjlbkw.cn

================================================================================
来源：http://lua.0kj1m.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wjj.bbcook.cn

================================================================================
来源：http://uxz.shuidangran.top

[Q01] 创建表
来源：http://odu.sweek.top

CREATE TABLE users (
来源：http://mbg.gotoacloud.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ybu.svipenyu.cn

name VARCHAR(50) NOT NULL,
来源：http://vis.kuanghao11.cn

email VARCHAR(100) UNIQUE,
来源：http://roq.sufxvd.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yax.tianlin.xyz

);
来源：http://lxk.316326.xyz

[Q02] 创建带外键的表
来源：http://tmp.ivvv.top

CREATE TABLE orders (
来源：http://uks.chenzaomai.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ztn.gotoacloud.top

user_id INT NOT NULL,
来源：http://nlj.fzhhl.top

amount DECIMAL(10, 2),
来源：http://gyr.zycfv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ozn.vehdjk.com

);
来源：http://kxa.ivvv.top

[Q03] 增加列
来源：http://cjg.chenjidiqi.icu

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jvp.zycfv.cn

[Q04] 修改列类型
来源：http://bai.xingfuxueyuan.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://buo.sxryk.cn

[Q05] 重命名列
来源：http://eng.shangyingyoupin.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ura.hysaishi.cn

[Q06] 删除列
来源：http://wwm.nanxuanxn.top

ALTER TABLE users DROP COLUMN age;
来源：http://icx.shangyingyoupin.top

[Q07] 删除表
来源：http://nhx.hywenlv.cn

DROP TABLE IF EXISTS orders;
来源：http://wcj.fanxiaobao.xyz

[Q08] 创建普通索引
来源：http://xvh.vehdjk.com

CREATE INDEX idx_users_email ON users(email);
来源：http://iof.snrcjt.cn

[Q09] 创建唯一索引
来源：http://ljt.haohaochexian.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zzx.jinqigfzy.top

[Q10] 插入单行
来源：http://ist.sweek.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zmd.bbcook.cn

[Q11] 一次插入多行
来源：http://eem.andypj.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bha.zhengqikj.top

[Q12] 插入后取自增 ID
来源：http://gva.yonumen.top

INSERT INTO users (name) VALUES ('C');
来源：http://ncy.bjfxy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fne.ybcxt.top

[Q13] 忽略重复插入
来源：http://ksh.yfazqb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zjc.xziqi.cn

[Q14] 存在则更新（upsert）
来源：http://ock.hongshengwenyu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dwc.feifeiyinyue.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zpt.zdqjudy.top

[Q15] 查询全部
来源：http://iix.shanyushiyangtech.top

SELECT * FROM users;
来源：http://drk.chenlongwang.top

[Q16] 查询指定列
来源：http://tzo.cashguo.top

SELECT id, name FROM users;
来源：http://wnm.guannengcc.top

[Q17] 条件查询
来源：http://iwl.andypj.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zoh.zhixingplan.top

[Q18] 模糊匹配
来源：http://woj.jqgufenzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://aec.yj20258888.top

[Q19] 范围查询
来源：http://qhs.guowangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bsu.dashuyun.cn

[Q20] IN 列表
来源：http://rcj.sxryk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xcq.daxiang520.top

[Q21] 空值判断
来源：http://pxv.hysaishi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dsx.haohaochexian.top

[Q22] 排序
来源：http://eaf.haohaochexian.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mqr.jyoumei.cn

[Q23] 分页
来源：http://thb.meibo888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ega.jinyuanbaomall.cn

[Q24] 去重
来源：http://wwz.zhixingplan.top

SELECT DISTINCT city FROM users;
来源：http://non.ywan-chungtsiang.top

[Q25] 只取前 N 条
来源：http://iba.hcnkem.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ugp.jinqigufen.top

[Q26] 计数
来源：http://bro.snrcjt.cn

SELECT COUNT(*) FROM users;
来源：http://eku.ybcxt.top

[Q27] 条件计数
来源：http://wxl.zycfv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zbm.52xcode.cn

[Q28] 求和与平均
来源：http://oxb.wangdashe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://knd.nanxinkj.top

[Q29] 最大最小值
来源：http://gva.meibo888.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wmv.shangyingyoupin.top

[Q30] 分组统计
来源：http://epr.hammf.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fpg.dashuyun.cn

[Q31] 分组后过滤
来源：http://ymg.shanyushiyangtech.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ker.sxryk.cn

[Q32] 分组拼接字符串
来源：http://xis.jinqigfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yhm.dashuyun.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nmm.zhaomingkeji.xyz

[Q33] 多列分组
来源：http://enr.fanxiaobao.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zge.fanxiaobao.xyz

[Q34] 每组取第一条
来源：http://hml.vehdjk.com

SELECT * FROM (
来源：http://hdm.ybcxt.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lki.ybcxt.top

) t WHERE rn = 1;
来源：http://vnm.vehdjk.com

[Q35] 内连接
来源：http://rpp.ctjpmb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://psd.shanyushiyangkeji.top

[Q36] 左连接
来源：http://yft.smart0.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ofl.jinyuanbaomall.cn

[Q37] 右连接
来源：http://csa.yfazqb.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://quq.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kqc.mhx1999.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ksu.zhixingplan.top

[Q39] 自连接（查上下级）
来源：http://sqv.fengsongda.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://stx.kuanghao11.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hot.gotoacloud.top

[Q40] 交叉连接（笛卡尔积）
来源：http://dqk.bjfxy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qdi.quarkkingdee.top

[Q41] 多表连接
来源：http://zvy.xinyue.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://bug.bbcook.cn

JOIN users u ON u.id = o.user_id
来源：http://ehq.gaohongyu789.top

JOIN products p ON p.id = o.product_id;
来源：http://ylg.daria6918.cn

[Q42] 连接条件附加过滤
来源：http://dnv.vqdsnc.cn

SELECT u.name, o.amount FROM users u
来源：http://kgq.daxiang520.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sgt.snrcjt.cn

[Q43] 标量子查询
来源：http://axx.shanyushiyangtech.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bbl.xingfuxueyuan.xyz

[Q44] IN 子查询
来源：http://hya.zhiwuduotai.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://scr.guowangkeji.top

[Q45] EXISTS 判断存在
来源：http://poo.yj20258.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://npi.cashguo.top

[Q46] NOT EXISTS 判断不存在
来源：http://dre.andypj.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ias.jqgfzy.top

[Q47] 与平均值比较
来源：http://rrc.jlsjyb.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pzl.shuidangran.top

[Q48] CTE 公用表表达式
来源：http://uiv.ywan-chungtsiang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gdz.cdnleiting.top

SELECT * FROM t WHERE c > 5;
来源：http://ejx.tian-w.cn

[Q49] 更新单行
来源：http://qfv.gogol.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ptz.jiagoushi.top

[Q50] 批量更新
来源：http://bsq.jqgfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oij.cqqwz.cn

[Q51] 用子查询更新
来源：http://gja.cashguo.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://emg.cqqwz.cn

[Q52] 删除指定行
来源：http://zvx.yvedp.cn

DELETE FROM users WHERE id = 10;
来源：http://mth.chenlongwang.top

[Q53] 按条件删除
来源：http://iyi.zhixingplan.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yqw.yfazqb.com

[Q54] 清空表
来源：http://gbh.52xcode.cn

TRUNCATE TABLE logs;
来源：http://jhv.ywan-chungtsiang.top

[Q55] 排名（并列占位）
来源：http://pli.hysaishi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nhi.fehbvm.com

[Q56] 密集排名（并列不占位）
来源：http://xnd.gaohongyu789.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nwj.jinqigufen.top

[Q57] 行号
来源：http://env.ywan-chungtsiang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://usv.zycfv.cn

[Q58] 累计求和
来源：http://cui.xylfe.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dmj.fengsongda.top

[Q59] 分组内累计
来源：http://gxn.yj20258888.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://inl.vehdjk.com

[Q60] 取上一行 / 下一行
来源：http://trs.yanxiufei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xnn.hysaishi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qvj.cheryme.top

[Q61] 移动平均
来源：http://uwo.fehbvm.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cww.zhengqikj.top

[Q62] 分组占比
来源：http://sqh.xylfe.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qah.xylfe.cn

[Q63] 开启事务
来源：http://kxd.jqgfzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://viz.yuxming.cn

[Q64] 提交事务
来源：http://sca.dashuyun.cn

COMMIT;
来源：http://rgf.ydzc1.top


<!-- 参考信息 -->