代发 wailian999

PHP:  // 手写递归函数
来源：http://yye.gogol.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://inf.ehwqpu.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ooe.yvedp.cn

Java: // 手写递归
来源：http://xud.jianghu66.top

Go:   // 手写递归
来源：http://gab.tian-w.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zwj.yonumen.top

C#:   // 手写递归
来源：http://sge.daxiang520.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dqd.sxryk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xyu.ehwqpu.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ass.zdbjq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tzd.jqgufenzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gdi.cheryme.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kpc.birdmap.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ycv.guowangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bvp.yvedp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dge.tanke756.top

================================================================================
来源：http://obb.yangfankeji.com

O. 并发与异步
来源：http://ffi.uphjek.com

================================================================================
来源：http://bsh.zhengqikj.top

[O01] 启动一个线程
来源：http://mgg.tanke756.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yst.shuidangran.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://csp.snrcjt.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sdu.hfpthk.cn

TS:   // 同 JS
来源：http://thh.xylfe.cn

Java: new Thread(() -> f()).start()
来源：http://kxd.nwbrower.top

Go:   go f()
来源：http://ddd.52xcode.cn

Ruby: Thread.new { f }
来源：http://zva.yuanzhike.top

C#:   Task.Run(() => F());
来源：http://rxa.dianchejie.cn

[O02] 使用线程池
来源：http://iwo.daria6918.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://anj.dashuyun.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ggz.yuanzhike.top

JS:   // worker_threads 线程池
来源：http://anp.zdqjudy.top

TS:   // worker_threads 线程池
来源：http://lyr.havefunace.top

Java: Executors.newFixedThreadPool(4)
来源：http://awi.gogol.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wfv.gotoacloud.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yxd.ywan-chungtsiang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kcw.zhongyouzk.top

[O03] 加锁保护共享数据
来源：http://fed.daria6918.cn

Py:   with lock: shared += 1
来源：http://xhs.sweek.top

PHP:  // 用 flock() 做文件锁
来源：http://ght.fanxiaobao.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://moe.zhongyouzk.top

TS:   // 同 JS
来源：http://lkr.cucudq.cn

Java: synchronized (this) { shared++; }
来源：http://kzn.quarkkingdee.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tyq.xuanzx.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://pzt.hesvh.cn

C#:   lock (gate) { shared++; }
来源：http://kij.kuanghao11.cn

[O04] 定义异步函数并等待
来源：http://rzz.ydjk.org.cn

Py:   async def f():⏎    await g()
来源：http://djv.chenjidiqi.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kko.yj20258888.top

JS:   async function f() { await g(); }
来源：http://kup.shanyushiyangtech.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dwq.zhoulong.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mrg.gogol.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tja.gaohongyu789.top

Ruby: # 用 Fiber 或 async gem
来源：http://hhn.meibo888.top

C#:   async Task F() { await G(); }
来源：http://lht.xingfuxueyuan.xyz

[O05] 并发执行并等待全部完成
来源：http://lgy.cheryme.top

Py:   asyncio.gather(*tasks)
来源：http://zpx.gzhubu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tqm.nanxinkj.top

JS:   await Promise.all(tasks)
来源：http://gyl.xuanzx.com

TS:   await Promise.all(tasks)
来源：http://fid.xuanzx.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bqd.andypj.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://glx.bbcook.cn

Ruby: threads.map(&:join)
来源：http://bia.nwbrower.top

C#:   await Task.WhenAll(t1, t2)
来源：http://vjd.guowangkeji.top

[O06] 使用进程池
来源：http://okh.aibaodan.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mro.xingfuxueyuan.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://nfj.ctjpmb.com

JS:   // child_process / cluster 模块
来源：http://yfb.daxiang520.top

TS:   // child_process / cluster 模块
来源：http://ded.shuidangran.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kog.hnqzz.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jqd.ydzc1.top

Ruby: // fork 块
来源：http://mxw.ydzc1.top

C#:   Parallel.For
来源：http://zyw.xuetiantiany.cn

================================================================================
来源：http://mvk.sjlbkw.cn

P. 常用工具函数
来源：http://xcn.yuanzhike.top

================================================================================
来源：http://sel.316326.xyz

[P01] 生成 UUID
来源：http://tcg.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://mep.yonumen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qsa.tanke756.top

JS:   crypto.randomUUID()
来源：http://mia.ywan-chungtsiang.top

TS:   crypto.randomUUID()
来源：http://prl.sweek.top

Java: UUID.randomUUID().toString()
来源：http://pgy.sysykeji.top

Go:   // 用 github.com/google/uuid
来源：http://zhg.yanxiufei.cn

Ruby: SecureRandom.uuid
来源：http://kei.gaohongyu789.top

C#:   Guid.NewGuid().ToString()
来源：http://zac.kuanghao11.cn

[P02] MD5 / SHA256 摘要
来源：http://ibj.zhoulong.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bob.52xcode.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cck.ydjk.org.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wbf.kuanghao11.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jge.hywenlv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kak.snrcjt.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yqi.yueranfly.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sgd.jinqigufen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rxh.ctjpmb.com

[P03] 生成短随机字符串
来源：http://fmu.xuanzx.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lrw.hywenlv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mhk.yfazqb.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xun.bjfxy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://unx.xingfuxueyuan.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://peo.yfazqb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hif.yongpay.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://iuw.vqdsnc.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://okn.sjlbkw.cn

[P04] 求长度
来源：http://eac.shangyingyoupin.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pfn.jianghu66.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ofj.guowangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ctl.zdbjq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://clf.cdnleiting.top

Java: list.size();  map.size();  s.length()
来源：http://luq.haohaochexian.top

Go:   len(arr);  len(m)
来源：http://ati.cqqwz.cn

Ruby: x.length;  x.size
来源：http://add.hesvh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://eik.guannengcc.top

[P05] 判断两个对象内容是否相等
来源：http://ovv.dashuyun.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tzr.mhx1999.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hkd.c1oappe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ggc.epnwcf.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vak.fzhhl.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wgl.yanxiufei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zuc.jinqigufen.top

Ruby: a == b
来源：http://kuh.sjlbkw.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wop.svipenyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dbe.xylfe.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ybp.c1oappe.top

PHP:  if (empty($x)) {}
来源：http://nns.sjlbkw.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lwd.tianlin.xyz

TS:   if (x == null) {}
来源：http://aqq.hnqzz.top

Java: if (x == null || x.isEmpty()) {}
来源：http://eat.kuanghao11.cn

Go:   if x == nil {}
来源：http://ezj.yanxiufei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xhu.shanyushiyangtech.top

C#:   if (x is null) {}
来源：http://zrm.yuxming.cn

[P07] 防抖与节流
来源：http://jkm.smart0.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://azd.zycfv.cn

PHP:  // 手写时间戳比较
来源：http://nnw.zhengqikj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pfv.jyoumei.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pit.xuanzx.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jwf.zdqjudy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vzr.gaohongyu789.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://swh.jinqigfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fcm.jlsjyb.cn

[P08] 处理浮点精度问题
来源：http://cxv.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://arb.zhaomingkeji.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://eet.svipenyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hqu.ywan-chungtsiang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tei.uphjek.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dew.sysykeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://epx.wangdashe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mvw.shuidangran.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ede.jqgufenzy.top

================================================================================
来源：http://nhe.wangdashe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gjm.yfazqb.com

================================================================================
来源：http://rdv.andypj.xyz

[Q01] 创建表
来源：http://yjb.chenlongwang.top

CREATE TABLE users (
来源：http://xzi.ydjk.org.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wkj.shuidangran.top

name VARCHAR(50) NOT NULL,
来源：http://fod.sweek.top

email VARCHAR(100) UNIQUE,
来源：http://uvt.hnxiangtu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qom.chenjidiqi.icu

);
来源：http://std.ydzc1.top

[Q02] 创建带外键的表
来源：http://dol.shanyushiyangtech.top

CREATE TABLE orders (
来源：http://hjm.haohaochexian.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rgu.gzhubu.top

user_id INT NOT NULL,
来源：http://tlo.cheryme.top

amount DECIMAL(10, 2),
来源：http://fmg.cqqwz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wab.jinyuanbaomall.cn

);
来源：http://jil.ppjwa.cn

[Q03] 增加列
来源：http://vfm.sjlbkw.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ztk.yj202588.top

[Q04] 修改列类型
来源：http://zsc.meibo888.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xdn.daxiang520.top

[Q05] 重命名列
来源：http://ass.yuxming.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xfz.jianghu66.top

[Q06] 删除列
来源：http://aru.yuxming.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lqf.wangshuangyany.cn

[Q07] 删除表
来源：http://yyo.yueranfly.top

DROP TABLE IF EXISTS orders;
来源：http://kal.vehdjk.com

[Q08] 创建普通索引
来源：http://teq.sufxvd.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mku.fanxiaobao.xyz

[Q09] 创建唯一索引
来源：http://kxf.zhoulong.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://axm.wangshuangyany.cn

[Q10] 插入单行
来源：http://kht.yuanzhike.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cqg.cashguo.top

[Q11] 一次插入多行
来源：http://yal.xylfe.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nld.birdmap.top

[Q12] 插入后取自增 ID
来源：http://sha.iojbl.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cwi.yuxming.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://paz.hongshengwenyu.top

[Q13] 忽略重复插入
来源：http://fge.epnwcf.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xyy.yuxming.cn

[Q14] 存在则更新（upsert）
来源：http://qkr.tian-w.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://omb.vehdjk.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://psc.bjfxy.top

[Q15] 查询全部
来源：http://gzv.hongshengwenyu.top

SELECT * FROM users;
来源：http://etl.chenzaomai.com

[Q16] 查询指定列
来源：http://ypj.vqdsnc.cn

SELECT id, name FROM users;
来源：http://lbm.fanxiaobao.xyz

[Q17] 条件查询
来源：http://ser.jinqigfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mfp.haohaochexian.top

[Q18] 模糊匹配
来源：http://lrb.zycfv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://krb.yonumen.top

[Q19] 范围查询
来源：http://jog.xingfuxueyuan.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kbq.yonumen.top

[Q20] IN 列表
来源：http://ogy.gaohongyu789.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ked.fanxiaobao.xyz

[Q21] 空值判断
来源：http://hhl.0kj1m.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nnr.guowangkeji.top

[Q22] 排序
来源：http://miy.jqgufenzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ees.vqdsnc.cn

[Q23] 分页
来源：http://uxi.xinyue.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://slw.daxiang520.top

[Q24] 去重
来源：http://ngx.zhongyouzk.top

SELECT DISTINCT city FROM users;
来源：http://uez.zdqjudy.top

[Q25] 只取前 N 条
来源：http://hgi.sweek.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hrv.smart0.xyz

[Q26] 计数
来源：http://mzs.pycfn.com

SELECT COUNT(*) FROM users;
来源：http://nin.jlsjyb.cn

[Q27] 条件计数
来源：http://owk.ywan-chungtsiang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://teu.yj202588.top

[Q28] 求和与平均
来源：http://rpa.pycfn.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sgs.meibo888.top

[Q29] 最大最小值
来源：http://pet.yj20258888.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://isy.snrcjt.cn

[Q30] 分组统计
来源：http://yue.iojbl.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qkn.smart0.xyz

[Q31] 分组后过滤
来源：http://myo.chenjidiqi.icu

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bgb.nanxuanxn.top

[Q32] 分组拼接字符串
来源：http://gvu.nwbrower.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mqx.chenlongwang.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pkn.hysaishi.cn

[Q33] 多列分组
来源：http://xyj.hcnkem.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lgo.zhixingplan.top

[Q34] 每组取第一条
来源：http://fod.c1oappe.top

SELECT * FROM (
来源：http://tng.yj202588.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tzp.xingfuxueyuan.xyz

) t WHERE rn = 1;
来源：http://epx.ehwqpu.com

[Q35] 内连接
来源：http://gvj.wangshuangyany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cru.sjlbkw.cn

[Q36] 左连接
来源：http://cxn.redwolf501.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jrm.hcnkem.com

[Q37] 右连接
来源：http://djv.hysaishi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mrw.jinghuilouyu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rqm.cashguo.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vkd.cucudq.cn

[Q39] 自连接（查上下级）
来源：http://rtk.meibo888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://sfe.zdqjudy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gec.ppjwa.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rme.gogol.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mry.vehdjk.com

[Q41] 多表连接
来源：http://ojm.xinyue.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://gik.vehdjk.com

JOIN users u ON u.id = o.user_id
来源：http://jbn.cheryme.top

JOIN products p ON p.id = o.product_id;
来源：http://sof.ivvv.top

[Q42] 连接条件附加过滤
来源：http://ock.sufxvd.cn

SELECT u.name, o.amount FROM users u
来源：http://lib.jlsjyb.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dcs.yuxming.cn

[Q43] 标量子查询
来源：http://oys.quarkkingdee.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qdj.jqgufenzy.top

[Q44] IN 子查询
来源：http://xkl.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hmt.chenzaomai.com

[Q45] EXISTS 判断存在
来源：http://pkb.aizwys.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qev.shuidangran.top

[Q46] NOT EXISTS 判断不存在
来源：http://iqv.hammf.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lxg.0kj1m.cn

[Q47] 与平均值比较
来源：http://tjn.feifeiyinyue.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uzn.yueranfly.top

[Q48] CTE 公用表表达式
来源：http://www.yj20258.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hso.wangshuangyany.cn

SELECT * FROM t WHERE c > 5;
来源：http://scb.uphjek.com

[Q49] 更新单行
来源：http://cyf.ydzc1.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ola.jinqigufen.top

[Q50] 批量更新
来源：http://haf.cashguo.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://omz.iojbl.cn

[Q51] 用子查询更新
来源：http://wqo.haohaochexian.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oyp.zhoulong.xyz

[Q52] 删除指定行
来源：http://bon.pycfn.com

DELETE FROM users WHERE id = 10;
来源：http://ijs.ehwqpu.com

[Q53] 按条件删除
来源：http://kcc.aibaodan.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ede.hywenlv.cn

[Q54] 清空表
来源：http://nwn.shanyushiyangkeji.top

TRUNCATE TABLE logs;
来源：http://rzu.ivvv.top

[Q55] 排名（并列占位）
来源：http://ngb.hnqzz.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rjx.hcnkem.com

[Q56] 密集排名（并列不占位）
来源：http://dbz.yuxming.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ztv.yuxming.cn

[Q57] 行号
来源：http://kff.ehwqpu.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dwl.fzhhl.top

[Q58] 累计求和
来源：http://wby.haohaochexian.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://obc.yueranfly.top

[Q59] 分组内累计
来源：http://rvl.hcnkem.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pfh.hongshengwenyu.top

[Q60] 取上一行 / 下一行
来源：http://vha.yj20258.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oem.cucudq.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sfb.cheryme.top

[Q61] 移动平均
来源：http://ltp.yonumen.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xqs.yueranfly.top

[Q62] 分组占比
来源：http://esc.yfazqb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qqa.hcnkem.com

[Q63] 开启事务
来源：http://dxo.fktsv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yix.yanxiufei.cn

[Q64] 提交事务
来源：http://zqb.hongshengwenyu.top

COMMIT;
来源：http://tpf.chenlongwang.top


<!-- 参考信息 -->