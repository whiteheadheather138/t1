代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dta.yj20258.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fbk.guannengcc.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yvu.xylfe.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kzj.jqgfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cuz.wangdashe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yxf.xinyue.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bih.316326.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fuf.epnwcf.com

================================================================================
来源：http://xbp.chenzaomai.com

O. 并发与异步
来源：http://dfd.zhaomingkeji.xyz

================================================================================
来源：http://apb.shangyingyoupin.top

[O01] 启动一个线程
来源：http://lom.jyoumei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://khl.fehbvm.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wwm.pycfn.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://isq.cqqwz.cn

TS:   // 同 JS
来源：http://igf.haohaochexian.top

Java: new Thread(() -> f()).start()
来源：http://csu.zhaomingkeji.xyz

Go:   go f()
来源：http://mix.yanxiufei.cn

Ruby: Thread.new { f }
来源：http://dmy.yj202588.top

C#:   Task.Run(() => F());
来源：http://ijr.aibaodan.cn

[O02] 使用线程池
来源：http://hig.tanke756.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uqb.yfazqb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uca.gogol.net.cn

JS:   // worker_threads 线程池
来源：http://pqy.daxiang520.top

TS:   // worker_threads 线程池
来源：http://kip.smart0.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://vyw.sysykeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cyt.jinqigfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://udi.zhoulong.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qmu.0kj1m.cn

[O03] 加锁保护共享数据
来源：http://sit.jlsjyb.cn

Py:   with lock: shared += 1
来源：http://jjh.tarul.cn

PHP:  // 用 flock() 做文件锁
来源：http://tba.pengpengdd.cyou

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pix.gotoacloud.top

TS:   // 同 JS
来源：http://iqi.gaohongyu789.top

Java: synchronized (this) { shared++; }
来源：http://emo.yuanzhike.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qbo.yuanzhike.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vps.gaohongyu789.top

C#:   lock (gate) { shared++; }
来源：http://tfd.pengpengdd.cyou

[O04] 定义异步函数并等待
来源：http://igc.hywenlv.cn

Py:   async def f():⏎    await g()
来源：http://xll.zhaomingkeji.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mli.shanyushiyangkeji.top

JS:   async function f() { await g(); }
来源：http://zfh.ppjwa.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pwr.wangshuangyany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gbc.gzhubu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gwu.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://xpf.c1oappe.top

C#:   async Task F() { await G(); }
来源：http://mnt.hcnkem.com

[O05] 并发执行并等待全部完成
来源：http://idg.0kj1m.cn

Py:   asyncio.gather(*tasks)
来源：http://tnd.vqdsnc.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oly.cdnleiting.top

JS:   await Promise.all(tasks)
来源：http://ylx.daria6918.cn

TS:   await Promise.all(tasks)
来源：http://muc.birdmap.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hpf.uphjek.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://owk.hfpthk.cn

Ruby: threads.map(&:join)
来源：http://ujh.fanxiaobao.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://zbf.daxiang520.top

[O06] 使用进程池
来源：http://qez.sysykeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fov.vqdsnc.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ntx.hammf.cn

JS:   // child_process / cluster 模块
来源：http://gbn.sxryk.cn

TS:   // child_process / cluster 模块
来源：http://iqg.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gmr.cheryme.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bve.feifeiyinyue.top

Ruby: // fork 块
来源：http://obx.epnwcf.com

C#:   Parallel.For
来源：http://vhw.feifeiyinyue.top

================================================================================
来源：http://kma.yongpay.top

P. 常用工具函数
来源：http://uco.xingfuxueyuan.xyz

================================================================================
来源：http://ldq.guowangkeji.top

[P01] 生成 UUID
来源：http://hnw.52xcode.cn

Py:   str(uuid.uuid4())
来源：http://kxy.yj20258888.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gjz.hcnkem.com

JS:   crypto.randomUUID()
来源：http://pkq.ctjpmb.com

TS:   crypto.randomUUID()
来源：http://peu.nanxuanxn.top

Java: UUID.randomUUID().toString()
来源：http://fhk.9152youxi.cn

Go:   // 用 github.com/google/uuid
来源：http://tdn.hesvh.cn

Ruby: SecureRandom.uuid
来源：http://xeh.redwolf501.top

C#:   Guid.NewGuid().ToString()
来源：http://iqj.chenjidiqi.icu

[P02] MD5 / SHA256 摘要
来源：http://bpr.fktsv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blx.jinyuanbaomall.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://umt.zhixingplan.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vmx.vqdsnc.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oyx.fktsv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://euf.gogol.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zpe.jinghuilouyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bbu.xuetiantiany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yzp.snrcjt.cn

[P03] 生成短随机字符串
来源：http://dmc.fktsv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zxl.yongpay.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ufm.jyoumei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://huj.daria6918.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ors.yj202588.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pfc.sjlbkw.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dws.zhiwuduotai.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://auo.jlsjyb.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hoy.xuetiantiany.cn

[P04] 求长度
来源：http://lwv.xinyue.icu

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ssy.jiagoushi.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ckh.jqgfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gcs.316326.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kdr.xuanzx.com

Java: list.size();  map.size();  s.length()
来源：http://uvs.yonumen.top

Go:   len(arr);  len(m)
来源：http://vkg.nanxuanxn.top

Ruby: x.length;  x.size
来源：http://uly.meibo888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rdr.cucudq.cn

[P05] 判断两个对象内容是否相等
来源：http://fkh.jinyuanbaomall.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pbm.cashguo.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hyw.hfpthk.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ayz.guannengcc.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://igw.gzhubu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rrf.jyoumei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ofy.chenlongwang.top

Ruby: a == b
来源：http://kkz.jqgufenzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ugt.cheryme.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xwf.hesvh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mxz.jyoumei.cn

PHP:  if (empty($x)) {}
来源：http://bzs.redwolf501.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mhx.haohaochexian.top

TS:   if (x == null) {}
来源：http://sjo.jinqigfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mof.fanxiaobao.xyz

Go:   if x == nil {}
来源：http://nqf.shanyushiyangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wlp.hongshengwenyu.top

C#:   if (x is null) {}
来源：http://qly.xziqi.cn

[P07] 防抖与节流
来源：http://fmk.jyoumei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dfm.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://bdd.gogol.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nli.c1oappe.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://szw.redwolf501.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://stl.52xcode.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jcd.xziqi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zlu.meibo888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cts.havefunace.top

[P08] 处理浮点精度问题
来源：http://ett.cashguo.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aed.jinqigufen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://waf.zhaomingkeji.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://szg.tanke756.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gte.ybcxt.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://min.jqgfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bnf.zhiwuduotai.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vqv.jinyuanbaomall.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://win.fktsv.cn

================================================================================
来源：http://gzl.yj202588.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://adu.shanyushiyangkeji.top

================================================================================
来源：http://rrp.xuetiantiany.cn

[Q01] 创建表
来源：http://wjw.xylfe.cn

CREATE TABLE users (
来源：http://lfg.gotoacloud.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dyk.redwolf501.top

name VARCHAR(50) NOT NULL,
来源：http://ysw.yvedp.cn

email VARCHAR(100) UNIQUE,
来源：http://ivh.haohaochexian.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xdq.birdmap.top

);
来源：http://zrq.yueranfly.top

[Q02] 创建带外键的表
来源：http://voq.zhiwuduotai.top

CREATE TABLE orders (
来源：http://caj.hnqzz.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ntg.hcnkem.com

user_id INT NOT NULL,
来源：http://gmo.cdnleiting.top

amount DECIMAL(10, 2),
来源：http://ept.zhoulong.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xkg.xziqi.cn

);
来源：http://trz.shanyushiyangtech.top

[Q03] 增加列
来源：http://kuz.hysaishi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ten.ywan-chungtsiang.top

[Q04] 修改列类型
来源：http://tqq.yanxiufei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uys.chenlongwang.top

[Q05] 重命名列
来源：http://jrn.tanke756.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nma.chenzaomai.com

[Q06] 删除列
来源：http://exy.316326.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://gnh.chenzaomai.com

[Q07] 删除表
来源：http://qwh.zhiwuduotai.top

DROP TABLE IF EXISTS orders;
来源：http://ovu.chenzaomai.com

[Q08] 创建普通索引
来源：http://irw.fanxiaobao.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://gom.yuanzhike.top

[Q09] 创建唯一索引
来源：http://vzt.pengpengdd.cyou

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://udg.cashguo.top

[Q10] 插入单行
来源：http://adc.jyoumei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jzr.zhijiandao.cn

[Q11] 一次插入多行
来源：http://czv.yj20258.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vmx.nwbrower.top

[Q12] 插入后取自增 ID
来源：http://pib.guowangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://vua.feifeiyinyue.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fvb.jinyuanbaomall.cn

[Q13] 忽略重复插入
来源：http://cyz.snrcjt.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cgm.tanke756.top

[Q14] 存在则更新（upsert）
来源：http://nei.dashuyun.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://aii.shangyingyoupin.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://slo.yj202588.top

[Q15] 查询全部
来源：http://ecu.hnqzz.top

SELECT * FROM users;
来源：http://lpu.jianghu66.top

[Q16] 查询指定列
来源：http://obw.zhengqikj.top

SELECT id, name FROM users;
来源：http://hsf.yongpay.top

[Q17] 条件查询
来源：http://qem.xuetiantiany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lij.ybcxt.top

[Q18] 模糊匹配
来源：http://obv.cashguo.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ltd.jinqigfzy.top

[Q19] 范围查询
来源：http://tko.nanxinkj.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dne.fanxiaobao.xyz

[Q20] IN 列表
来源：http://pje.aizwys.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ues.svipenyu.cn

[Q21] 空值判断
来源：http://fds.smart0.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://ncj.iojbl.cn

[Q22] 排序
来源：http://gkp.uphjek.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zze.hesvh.cn

[Q23] 分页
来源：http://pgf.ybcxt.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://thj.quarkkingdee.top

[Q24] 去重
来源：http://jmv.zhixingplan.top

SELECT DISTINCT city FROM users;
来源：http://uhr.yj20258888.top

[Q25] 只取前 N 条
来源：http://yvh.sweek.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tvj.ydzc1.top

[Q26] 计数
来源：http://jtc.gotoacloud.top

SELECT COUNT(*) FROM users;
来源：http://don.chenzaomai.com

[Q27] 条件计数
来源：http://tzq.guannengcc.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sie.xinyue.icu

[Q28] 求和与平均
来源：http://zes.shanyushiyangtech.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://svw.meibo888.top

[Q29] 最大最小值
来源：http://tuh.ehwqpu.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://kus.wangdashe.top

[Q30] 分组统计
来源：http://vei.zhixingplan.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dqc.hcnkem.com

[Q31] 分组后过滤
来源：http://rzg.fktsv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://idd.cheryme.top

[Q32] 分组拼接字符串
来源：http://gdf.guowangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zvj.ydjk.org.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kmc.andypj.xyz

[Q33] 多列分组
来源：http://zyj.bbcook.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://suo.dashuyun.cn

[Q34] 每组取第一条
来源：http://skl.dashuyun.cn

SELECT * FROM (
来源：http://yle.ywan-chungtsiang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kna.cdnleiting.top

) t WHERE rn = 1;
来源：http://fop.redwolf501.top

[Q35] 内连接
来源：http://bpv.epnwcf.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qqt.hnqzz.top

[Q36] 左连接
来源：http://dgz.gogol.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://skt.zhoulong.xyz

[Q37] 右连接
来源：http://hwv.zhengqikj.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uuu.ctjpmb.com

[Q38] 全外连接（PostgreSQL）
来源：http://zlq.ydzc1.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yxt.jinyuanbaomall.cn

[Q39] 自连接（查上下级）
来源：http://vll.zhiwuduotai.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qnz.hywenlv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ejk.iojbl.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lmy.guowangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gic.yangfankeji.com

[Q41] 多表连接
来源：http://ynn.wangdashe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bzv.xinyue.icu

JOIN users u ON u.id = o.user_id
来源：http://mtg.jqgufenzy.top

JOIN products p ON p.id = o.product_id;
来源：http://nps.chenjidiqi.icu

[Q42] 连接条件附加过滤
来源：http://cdi.xuanzx.com

SELECT u.name, o.amount FROM users u
来源：http://jeb.hesvh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dbi.zhongyouzk.top

[Q43] 标量子查询
来源：http://vcd.zhoulong.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jwk.yanxiufei.cn

[Q44] IN 子查询
来源：http://ewi.xuetiantiany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dzf.hesvh.cn

[Q45] EXISTS 判断存在
来源：http://quy.vehdjk.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qxn.zhiwuduotai.top

[Q46] NOT EXISTS 判断不存在
来源：http://rcy.aibaodan.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vnq.gzhubu.top

[Q47] 与平均值比较
来源：http://edo.tarul.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://arp.shzxlz.cn

[Q48] CTE 公用表表达式
来源：http://quy.sufxvd.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gqq.sweek.top

SELECT * FROM t WHERE c > 5;
来源：http://aln.redwolf501.top

[Q49] 更新单行
来源：http://hpw.shzxlz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zef.fehbvm.com

[Q50] 批量更新
来源：http://hrh.jianghu66.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jkq.wangshuangyany.cn

[Q51] 用子查询更新
来源：http://iiz.0kj1m.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oap.yonumen.top

[Q52] 删除指定行
来源：http://khz.chenzaomai.com

DELETE FROM users WHERE id = 10;
来源：http://wtk.cucudq.cn

[Q53] 按条件删除
来源：http://frm.xuanzx.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hxr.hnxiangtu.top

[Q54] 清空表
来源：http://gyc.wangdashe.top

TRUNCATE TABLE logs;
来源：http://kap.52xcode.cn

[Q55] 排名（并列占位）
来源：http://zsv.jqgufenzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://clb.tarul.cn

[Q56] 密集排名（并列不占位）
来源：http://prh.yj202588.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xfd.shuidangran.top

[Q57] 行号
来源：http://eba.yj20258.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mxg.shzxlz.cn

[Q58] 累计求和
来源：http://efo.vqdsnc.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://slk.daxiang520.top

[Q59] 分组内累计
来源：http://hwo.zhiwuduotai.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qjn.hysaishi.cn

[Q60] 取上一行 / 下一行
来源：http://ekh.ywan-chungtsiang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nwv.aizwys.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zdc.aizwys.cn

[Q61] 移动平均
来源：http://rjc.tianlin.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://obk.gogol.net.cn

[Q62] 分组占比
来源：http://sci.zhaomingkeji.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yvd.gogol.net.cn

[Q63] 开启事务
来源：http://gib.tianlin.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://rcd.dashuyun.cn

[Q64] 提交事务
来源：http://gnl.cashguo.top

COMMIT;
来源：http://vet.jinyuanbaomall.cn

[Q65] 回滚事务
来源：http://bcw.cdnleiting.top

ROLLBACK;
来源：http://fkk.nanxinkj.top

[Q66] 行锁查询
来源：http://pli.ivvv.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://weo.yueranfly.top

[Q67] 设置隔离级别
来源：http://ylb.hammf.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gfh.chenlongwang.top

[Q68] 保存点
来源：http://mcz.zhongyouzk.top

SAVEPOINT sp1;
来源：http://sac.gotoacloud.top


<!-- 参考信息 -->