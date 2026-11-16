代发 wailian999

PHP:  // 手写递归函数
来源：http://jas.havefunace.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xbl.sjlbkw.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://trw.ybcxt.top

Java: // 手写递归
来源：http://szt.jinghuilouyu.cn

Go:   // 手写递归
来源：http://ujf.yj202588.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cbb.hnxiangtu.top

C#:   // 手写递归
来源：http://anh.dianchejie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fao.bbcook.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mym.yuanzhike.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kbo.chenzaomai.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uew.tian-w.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tax.dianchejie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://smu.yj20258888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://svr.zhengqikj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qqy.yonumen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zby.cheryme.top

================================================================================
来源：http://ncs.nanxinkj.top

O. 并发与异步
来源：http://yzr.shzxlz.cn

================================================================================
来源：http://iup.gaohongyu789.top

[O01] 启动一个线程
来源：http://uon.xziqi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vwx.fanxiaobao.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hfw.ydjk.org.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://byx.cashguo.top

TS:   // 同 JS
来源：http://aht.fzhhl.top

Java: new Thread(() -> f()).start()
来源：http://dap.zycfv.cn

Go:   go f()
来源：http://qua.iojbl.cn

Ruby: Thread.new { f }
来源：http://jhf.daxiang520.top

C#:   Task.Run(() => F());
来源：http://cuy.nanxinkj.top

[O02] 使用线程池
来源：http://wux.fktsv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fci.yongpay.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bek.jyoumei.cn

JS:   // worker_threads 线程池
来源：http://xlz.yueranfly.top

TS:   // worker_threads 线程池
来源：http://zam.yfazqb.com

Java: Executors.newFixedThreadPool(4)
来源：http://gxa.andypj.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ezp.chenlongwang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ozz.birdmap.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xzo.vehdjk.com

[O03] 加锁保护共享数据
来源：http://pqr.shangyingyoupin.top

Py:   with lock: shared += 1
来源：http://urf.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://ubc.sufxvd.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sai.hysaishi.cn

TS:   // 同 JS
来源：http://qmh.jqgufenzy.top

Java: synchronized (this) { shared++; }
来源：http://yxs.chenzaomai.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yun.mhx1999.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ekj.mhx1999.top

C#:   lock (gate) { shared++; }
来源：http://ymo.andypj.xyz

[O04] 定义异步函数并等待
来源：http://yan.meibo888.top

Py:   async def f():⏎    await g()
来源：http://pcn.kuanghao11.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://osa.chenlongwang.top

JS:   async function f() { await g(); }
来源：http://xme.smart0.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://uax.zhoulong.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wrk.bjfxy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ead.tanke756.top

Ruby: # 用 Fiber 或 async gem
来源：http://yap.zdqjudy.top

C#:   async Task F() { await G(); }
来源：http://hzm.sweek.top

[O05] 并发执行并等待全部完成
来源：http://wgl.yuxming.cn

Py:   asyncio.gather(*tasks)
来源：http://mea.hcnkem.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sze.hongshengwenyu.top

JS:   await Promise.all(tasks)
来源：http://vqj.fengsongda.top

TS:   await Promise.all(tasks)
来源：http://azk.nwbrower.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kds.xinyue.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ycm.fzhhl.top

Ruby: threads.map(&:join)
来源：http://mop.fehbvm.com

C#:   await Task.WhenAll(t1, t2)
来源：http://exw.ydjk.org.cn

[O06] 使用进程池
来源：http://wsc.vqdsnc.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rlf.nwbrower.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uov.aibaodan.cn

JS:   // child_process / cluster 模块
来源：http://wti.vehdjk.com

TS:   // child_process / cluster 模块
来源：http://utk.daria6918.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vbb.fktsv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mil.fanxiaobao.xyz

Ruby: // fork 块
来源：http://pgm.fktsv.cn

C#:   Parallel.For
来源：http://fru.wangshuangyany.cn

================================================================================
来源：http://ngk.yuanzhike.top

P. 常用工具函数
来源：http://ecu.52xcode.cn

================================================================================
来源：http://bnc.kuanghao11.cn

[P01] 生成 UUID
来源：http://qvi.tianlin.xyz

Py:   str(uuid.uuid4())
来源：http://zro.dianchejie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mab.chenjidiqi.icu

JS:   crypto.randomUUID()
来源：http://pix.xylfe.cn

TS:   crypto.randomUUID()
来源：http://kfw.cqqwz.cn

Java: UUID.randomUUID().toString()
来源：http://vjr.vqdsnc.cn

Go:   // 用 github.com/google/uuid
来源：http://fzy.0kj1m.cn

Ruby: SecureRandom.uuid
来源：http://leg.ybcxt.top

C#:   Guid.NewGuid().ToString()
来源：http://ktv.snrcjt.cn

[P02] MD5 / SHA256 摘要
来源：http://ncl.yangfankeji.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dbg.xuanzx.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://enn.shanyushiyangkeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iol.cheryme.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xrw.yongpay.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xch.hnxiangtu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ygs.c1oappe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sta.bbcook.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dnt.zhengqikj.top

[P03] 生成短随机字符串
来源：http://xiq.nanxinkj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sjx.zhiwuduotai.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ocg.tian-w.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://slx.bjfxy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wnj.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fiw.sysykeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://puq.c1oappe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mld.zycfv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ssv.aizwys.cn

[P04] 求长度
来源：http://mvu.cheryme.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qjc.hongshengwenyu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qbv.yuxming.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kqr.epnwcf.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qos.yj20258888.top

Java: list.size();  map.size();  s.length()
来源：http://wsm.aizwys.cn

Go:   len(arr);  len(m)
来源：http://uil.nanxuanxn.top

Ruby: x.length;  x.size
来源：http://xci.chenjidiqi.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://bvg.andypj.xyz

[P05] 判断两个对象内容是否相等
来源：http://wqa.9152youxi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://amd.sweek.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yze.sysykeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dle.zhengqikj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://asx.zhixingplan.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xhr.cucudq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://oeh.hysaishi.cn

Ruby: a == b
来源：http://udo.sxryk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wam.yangfankeji.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pyu.jinqigufen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mtp.gzhubu.top

PHP:  if (empty($x)) {}
来源：http://qys.birdmap.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dpb.pycfn.com

TS:   if (x == null) {}
来源：http://rsd.yj20258888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zki.feifeiyinyue.top

Go:   if x == nil {}
来源：http://ivu.vehdjk.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://loj.sysykeji.top

C#:   if (x is null) {}
来源：http://umj.jlsjyb.cn

[P07] 防抖与节流
来源：http://hqb.tian-w.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oup.yangfankeji.com

PHP:  // 手写时间戳比较
来源：http://rtk.c1oappe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jqq.ywan-chungtsiang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ock.haohaochexian.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rst.zhengqikj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yjh.guannengcc.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qoe.0kj1m.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cwc.pycfn.com

[P08] 处理浮点精度问题
来源：http://yql.52xcode.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ekw.yj202588.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ard.jiagoushi.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gdu.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jsd.svipenyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jsi.hesvh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jve.yangfankeji.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://frb.cucudq.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jtn.zhijiandao.cn

================================================================================
来源：http://mwx.hammf.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nvy.hongshengwenyu.top

================================================================================
来源：http://tzz.jqgfzy.top

[Q01] 创建表
来源：http://fal.haohaochexian.top

CREATE TABLE users (
来源：http://htj.feifeiyinyue.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hdt.ydzc1.top

name VARCHAR(50) NOT NULL,
来源：http://jro.jinqigfzy.top

email VARCHAR(100) UNIQUE,
来源：http://omb.316326.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://enc.nwbrower.top

);
来源：http://osl.pengpengdd.cyou

[Q02] 创建带外键的表
来源：http://pxq.shangyingyoupin.top

CREATE TABLE orders (
来源：http://vqr.sysykeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oce.yanxiufei.cn

user_id INT NOT NULL,
来源：http://ena.sxryk.cn

amount DECIMAL(10, 2),
来源：http://mfp.sufxvd.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ksn.zhengqikj.top

);
来源：http://var.cashguo.top

[Q03] 增加列
来源：http://atu.ppjwa.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uln.hfpthk.cn

[Q04] 修改列类型
来源：http://jwv.kuanghao11.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mzl.ybcxt.top

[Q05] 重命名列
来源：http://fhn.yj20258.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ppl.zhiwuduotai.top

[Q06] 删除列
来源：http://nxz.chenjidiqi.icu

ALTER TABLE users DROP COLUMN age;
来源：http://qka.jiagoushi.top

[Q07] 删除表
来源：http://sew.guowangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://wkb.jyoumei.cn

[Q08] 创建普通索引
来源：http://lcc.ppjwa.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://uli.jqgfzy.top

[Q09] 创建唯一索引
来源：http://ajl.andypj.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dwu.dianchejie.cn

[Q10] 插入单行
来源：http://sfl.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://egl.gaohongyu789.top

[Q11] 一次插入多行
来源：http://jfr.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://skv.wangdashe.top

[Q12] 插入后取自增 ID
来源：http://qmv.guowangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://uqx.zhixingplan.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://npe.fanxiaobao.xyz

[Q13] 忽略重复插入
来源：http://ynj.ivvv.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hcw.c1oappe.top

[Q14] 存在则更新（upsert）
来源：http://mdj.dianchejie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gui.nwbrower.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yow.gogol.net.cn

[Q15] 查询全部
来源：http://unu.epnwcf.com

SELECT * FROM users;
来源：http://ccr.jianghu66.top

[Q16] 查询指定列
来源：http://akx.bjfxy.top

SELECT id, name FROM users;
来源：http://vmj.pycfn.com

[Q17] 条件查询
来源：http://eyh.fanxiaobao.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ryb.daxiang520.top

[Q18] 模糊匹配
来源：http://ddu.sjlbkw.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://usz.tianlin.xyz

[Q19] 范围查询
来源：http://doy.aibaodan.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yhz.zhiwuduotai.top

[Q20] IN 列表
来源：http://bvg.sufxvd.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://enc.tarul.cn

[Q21] 空值判断
来源：http://vup.zhaomingkeji.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://odw.smart0.xyz

[Q22] 排序
来源：http://slk.xziqi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oka.yj20258.top

[Q23] 分页
来源：http://npx.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tke.zhiwuduotai.top

[Q24] 去重
来源：http://aen.0kj1m.cn

SELECT DISTINCT city FROM users;
来源：http://yha.nanxuanxn.top

[Q25] 只取前 N 条
来源：http://oxp.tianlin.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xyy.jinyuanbaomall.cn

[Q26] 计数
来源：http://pue.jinqigfzy.top

SELECT COUNT(*) FROM users;
来源：http://nyl.birdmap.top

[Q27] 条件计数
来源：http://jlw.fengsongda.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vjf.chenlongwang.top

[Q28] 求和与平均
来源：http://cif.hesvh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wrv.ctjpmb.com

[Q29] 最大最小值
来源：http://bfe.shanyushiyangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dsb.andypj.xyz

[Q30] 分组统计
来源：http://jxa.ehwqpu.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qiy.sysykeji.top

[Q31] 分组后过滤
来源：http://xft.sufxvd.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uio.quarkkingdee.top

[Q32] 分组拼接字符串
来源：http://qrg.vehdjk.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fug.yueranfly.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nuy.jqgufenzy.top

[Q33] 多列分组
来源：http://dwt.zhaomingkeji.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aue.jinqigufen.top

[Q34] 每组取第一条
来源：http://orq.vqdsnc.cn

SELECT * FROM (
来源：http://lyg.guannengcc.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fgw.zhengqikj.top

) t WHERE rn = 1;
来源：http://yng.jianghu66.top

[Q35] 内连接
来源：http://yen.chenjidiqi.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ije.shuidangran.top

[Q36] 左连接
来源：http://pfg.yonumen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wdz.sufxvd.cn

[Q37] 右连接
来源：http://ozc.guannengcc.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xcq.dianchejie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cup.aizwys.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://flu.316326.xyz

[Q39] 自连接（查上下级）
来源：http://fux.birdmap.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ecu.sufxvd.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vzt.jinyuanbaomall.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://win.yvedp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://obv.ehwqpu.com

[Q41] 多表连接
来源：http://sjm.jinghuilouyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wjv.ctjpmb.com

JOIN users u ON u.id = o.user_id
来源：http://dbd.ctjpmb.com

JOIN products p ON p.id = o.product_id;
来源：http://ryp.shangyingyoupin.top

[Q42] 连接条件附加过滤
来源：http://uan.hywenlv.cn

SELECT u.name, o.amount FROM users u
来源：http://gki.shanyushiyangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lqv.yongpay.top

[Q43] 标量子查询
来源：http://cxc.xingfuxueyuan.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lvg.wangshuangyany.cn

[Q44] IN 子查询
来源：http://uze.nwbrower.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://huh.yonumen.top

[Q45] EXISTS 判断存在
来源：http://cpm.aizwys.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nqz.fanxiaobao.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://fyt.aibaodan.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dny.tian-w.cn

[Q47] 与平均值比较
来源：http://whb.xylfe.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wsz.gotoacloud.top

[Q48] CTE 公用表表达式
来源：http://irj.tanke756.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iif.zhoulong.xyz

SELECT * FROM t WHERE c > 5;
来源：http://shn.wangshuangyany.cn

[Q49] 更新单行
来源：http://iwk.haohaochexian.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://afr.fengsongda.top

[Q50] 批量更新
来源：http://ohd.kuanghao11.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dsf.pycfn.com

[Q51] 用子查询更新
来源：http://ybk.shzxlz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yyp.sweek.top

[Q52] 删除指定行
来源：http://lzj.pengpengdd.cyou

DELETE FROM users WHERE id = 10;
来源：http://ypu.tianlin.xyz

[Q53] 按条件删除
来源：http://qwv.sufxvd.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hml.cdnleiting.top

[Q54] 清空表
来源：http://qlq.hfpthk.cn

TRUNCATE TABLE logs;
来源：http://mva.yanxiufei.cn

[Q55] 排名（并列占位）
来源：http://ird.hfpthk.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jrn.yonumen.top

[Q56] 密集排名（并列不占位）
来源：http://gnn.cqqwz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sul.tanke756.top

[Q57] 行号
来源：http://cxe.hammf.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nrs.c1oappe.top

[Q58] 累计求和
来源：http://fke.fanxiaobao.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://epq.aizwys.cn

[Q59] 分组内累计
来源：http://rmg.316326.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yjm.bjfxy.top

[Q60] 取上一行 / 下一行
来源：http://riq.tanke756.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wpo.hfpthk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gse.kuanghao11.cn

[Q61] 移动平均
来源：http://rpy.smart0.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rvt.snrcjt.cn

[Q62] 分组占比
来源：http://ftl.fktsv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uxt.snrcjt.cn

[Q63] 开启事务
来源：http://dtp.jinqigufen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ebt.jqgfzy.top

[Q64] 提交事务
来源：http://lws.pengpengdd.cyou

COMMIT;
来源：http://ybq.316326.xyz


<!-- 参考信息 -->