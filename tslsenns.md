代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://qub.cashguo.top

C#:   class Node { public int V; public Node? Next; }
来源：http://kje.zhijiandao.cn

[N11] 二叉树中序遍历
来源：http://yil.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ibd.0kj1m.cn

PHP:  // 手写递归函数
来源：http://dmf.9152youxi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hyd.zhixingplan.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tbk.ppjwa.cn

Java: // 手写递归
来源：http://mgb.52xcode.cn

Go:   // 手写递归
来源：http://kpl.jinqigfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ubd.yangfankeji.com

C#:   // 手写递归
来源：http://xky.yuxming.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kil.jinqigfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dbe.pycfn.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qxb.cheryme.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sgj.wangshuangyany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://trl.jqgfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ido.smart0.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sup.guannengcc.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vvq.zdqjudy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vvo.jianghu66.top

================================================================================
来源：http://nlu.yongpay.top

O. 并发与异步
来源：http://egk.fzhhl.top

================================================================================
来源：http://twx.xziqi.cn

[O01] 启动一个线程
来源：http://dms.shzxlz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ckf.redwolf501.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kka.jiagoushi.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fuj.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://mfk.hnqzz.top

Java: new Thread(() -> f()).start()
来源：http://nap.gzhubu.top

Go:   go f()
来源：http://phl.ivvv.top

Ruby: Thread.new { f }
来源：http://qiq.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://njb.pycfn.com

[O02] 使用线程池
来源：http://jmi.zycfv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://snl.zhiwuduotai.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cac.jianghu66.top

JS:   // worker_threads 线程池
来源：http://gpm.tian-w.cn

TS:   // worker_threads 线程池
来源：http://wwq.dashuyun.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pqc.tianlin.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xps.yonumen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rdl.dianchejie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hsi.mhx1999.top

[O03] 加锁保护共享数据
来源：http://neo.cqqwz.cn

Py:   with lock: shared += 1
来源：http://wkv.iojbl.cn

PHP:  // 用 flock() 做文件锁
来源：http://lfe.hongshengwenyu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gnp.sjlbkw.cn

TS:   // 同 JS
来源：http://yrh.andypj.xyz

Java: synchronized (this) { shared++; }
来源：http://dhk.sysykeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xdq.nanxinkj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://fvi.shanyushiyangkeji.top

C#:   lock (gate) { shared++; }
来源：http://ouw.jyoumei.cn

[O04] 定义异步函数并等待
来源：http://zbx.shanyushiyangkeji.top

Py:   async def f():⏎    await g()
来源：http://ock.xuetiantiany.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dsl.zycfv.cn

JS:   async function f() { await g(); }
来源：http://nuj.sysykeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vxn.tian-w.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mgw.ppjwa.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://skr.andypj.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://qhv.cqqwz.cn

C#:   async Task F() { await G(); }
来源：http://yqq.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://wdg.yongpay.top

Py:   asyncio.gather(*tasks)
来源：http://zwr.shanyushiyangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ttr.cucudq.cn

JS:   await Promise.all(tasks)
来源：http://ayc.hnqzz.top

TS:   await Promise.all(tasks)
来源：http://cja.yanxiufei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://grg.ydzc1.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hzb.hywenlv.cn

Ruby: threads.map(&:join)
来源：http://chf.daxiang520.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fmo.chenzaomai.com

[O06] 使用进程池
来源：http://nyj.zhoulong.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://leg.havefunace.top

PHP:  // pcntl_fork 或多进程队列
来源：http://crk.daxiang520.top

JS:   // child_process / cluster 模块
来源：http://rxm.zhengqikj.top

TS:   // child_process / cluster 模块
来源：http://gyf.ppjwa.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ppj.xuanzx.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tpi.hammf.cn

Ruby: // fork 块
来源：http://rrm.bbcook.cn

C#:   Parallel.For
来源：http://not.ywan-chungtsiang.top

================================================================================
来源：http://twm.vehdjk.com

P. 常用工具函数
来源：http://upr.zhengqikj.top

================================================================================
来源：http://tls.yangfankeji.com

[P01] 生成 UUID
来源：http://wde.hammf.cn

Py:   str(uuid.uuid4())
来源：http://jwn.zhaomingkeji.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zyo.hcnkem.com

JS:   crypto.randomUUID()
来源：http://vlq.yj20258888.top

TS:   crypto.randomUUID()
来源：http://qii.hnqzz.top

Java: UUID.randomUUID().toString()
来源：http://ecu.kuanghao11.cn

Go:   // 用 github.com/google/uuid
来源：http://mps.nanxuanxn.top

Ruby: SecureRandom.uuid
来源：http://wtz.nanxuanxn.top

C#:   Guid.NewGuid().ToString()
来源：http://jzn.ppjwa.cn

[P02] MD5 / SHA256 摘要
来源：http://mka.wangshuangyany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pko.zhaomingkeji.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://lwk.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vmz.fktsv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zrw.hongshengwenyu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dxh.mhx1999.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://obw.sweek.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hsj.cdnleiting.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hbe.fengsongda.top

[P03] 生成短随机字符串
来源：http://cim.cqqwz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dwm.ctjpmb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://saj.hcnkem.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hwi.zdbjq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yab.xuetiantiany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://azz.gotoacloud.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kkc.xylfe.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jpi.hysaishi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jwl.yonumen.top

[P04] 求长度
来源：http://vsg.snrcjt.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://izw.tianlin.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://enh.birdmap.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mzb.nanxinkj.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://stm.tianlin.xyz

Java: list.size();  map.size();  s.length()
来源：http://hmn.shzxlz.cn

Go:   len(arr);  len(m)
来源：http://zcw.hywenlv.cn

Ruby: x.length;  x.size
来源：http://ycf.52xcode.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pmy.fengsongda.top

[P05] 判断两个对象内容是否相等
来源：http://cbf.gogol.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mue.chenjidiqi.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nix.svipenyu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ncz.iojbl.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://beq.jinqigufen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mxy.52xcode.cn

Go:   reflect.DeepEqual(a, b)
来源：http://htz.zhijiandao.cn

Ruby: a == b
来源：http://bmc.fanxiaobao.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hoy.gaohongyu789.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yjz.chenzaomai.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ugm.cheryme.top

PHP:  if (empty($x)) {}
来源：http://oxx.zhaomingkeji.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jtu.sysykeji.top

TS:   if (x == null) {}
来源：http://ajm.hfpthk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cef.cdnleiting.top

Go:   if x == nil {}
来源：http://zpz.uphjek.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jvg.hfpthk.cn

C#:   if (x is null) {}
来源：http://lon.xziqi.cn

[P07] 防抖与节流
来源：http://ljz.yongpay.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bra.zhongyouzk.top

PHP:  // 手写时间戳比较
来源：http://big.cqqwz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ddc.hnxiangtu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://loz.gotoacloud.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hwv.9152youxi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pvx.hongshengwenyu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://btn.daria6918.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ibn.fehbvm.com

[P08] 处理浮点精度问题
来源：http://jmk.feifeiyinyue.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yhw.jinyuanbaomall.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://igs.fanxiaobao.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qls.hnqzz.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ibv.zhijiandao.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vyy.andypj.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eib.xinyue.icu

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sgm.cashguo.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oft.bbcook.cn

================================================================================
来源：http://lys.zycfv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://thp.yueranfly.top

================================================================================
来源：http://hbg.sufxvd.cn

[Q01] 创建表
来源：http://rbx.xuanzx.com

CREATE TABLE users (
来源：http://ctr.ywan-chungtsiang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tnz.yueranfly.top

name VARCHAR(50) NOT NULL,
来源：http://ktx.xziqi.cn

email VARCHAR(100) UNIQUE,
来源：http://box.ydjk.org.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rtx.dianchejie.cn

);
来源：http://ejm.gogol.net.cn

[Q02] 创建带外键的表
来源：http://zka.hywenlv.cn

CREATE TABLE orders (
来源：http://vlw.xylfe.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://utq.jqgfzy.top

user_id INT NOT NULL,
来源：http://bnc.hfpthk.cn

amount DECIMAL(10, 2),
来源：http://gbv.hnqzz.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zzk.zdbjq.cn

);
来源：http://ftd.fktsv.cn

[Q03] 增加列
来源：http://sfg.shanyushiyangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wsv.316326.xyz

[Q04] 修改列类型
来源：http://ndn.smart0.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tvs.xinyue.icu

[Q05] 重命名列
来源：http://dme.hesvh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://teu.jyoumei.cn

[Q06] 删除列
来源：http://jsc.zycfv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ibw.jlsjyb.cn

[Q07] 删除表
来源：http://tef.zhiwuduotai.top

DROP TABLE IF EXISTS orders;
来源：http://fev.smart0.xyz

[Q08] 创建普通索引
来源：http://sju.guannengcc.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xjf.ehwqpu.com

[Q09] 创建唯一索引
来源：http://taf.fehbvm.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qlu.ppjwa.cn

[Q10] 插入单行
来源：http://hok.316326.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gdm.gogol.net.cn

[Q11] 一次插入多行
来源：http://clx.ydzc1.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iwr.hnxiangtu.top

[Q12] 插入后取自增 ID
来源：http://dbz.shanyushiyangtech.top

INSERT INTO users (name) VALUES ('C');
来源：http://inh.fzhhl.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mox.jqgfzy.top

[Q13] 忽略重复插入
来源：http://scz.xuetiantiany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tck.aibaodan.cn

[Q14] 存在则更新（upsert）
来源：http://vii.shanyushiyangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jia.uphjek.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://shj.jqgfzy.top

[Q15] 查询全部
来源：http://cog.ivvv.top

SELECT * FROM users;
来源：http://rwf.daxiang520.top

[Q16] 查询指定列
来源：http://szb.meibo888.top

SELECT id, name FROM users;
来源：http://swq.jinghuilouyu.cn

[Q17] 条件查询
来源：http://ncl.wangshuangyany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uqd.aizwys.cn

[Q18] 模糊匹配
来源：http://njo.sjlbkw.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bkm.gotoacloud.top

[Q19] 范围查询
来源：http://kjf.daria6918.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yae.shanyushiyangtech.top

[Q20] IN 列表
来源：http://cgg.yongpay.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sgy.0kj1m.cn

[Q21] 空值判断
来源：http://zea.mhx1999.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kft.sxryk.cn

[Q22] 排序
来源：http://eli.bbcook.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mss.c1oappe.top

[Q23] 分页
来源：http://fjy.iojbl.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://olt.xuanzx.com

[Q24] 去重
来源：http://yut.tianlin.xyz

SELECT DISTINCT city FROM users;
来源：http://gxn.yvedp.cn

[Q25] 只取前 N 条
来源：http://olp.ydzc1.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bxt.yfazqb.com

[Q26] 计数
来源：http://kls.xuanzx.com

SELECT COUNT(*) FROM users;
来源：http://zgn.sxryk.cn

[Q27] 条件计数
来源：http://rup.fanxiaobao.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bnv.316326.xyz

[Q28] 求和与平均
来源：http://fxl.zdqjudy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://njf.zhiwuduotai.top

[Q29] 最大最小值
来源：http://ysp.yfazqb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://tlq.zycfv.cn

[Q30] 分组统计
来源：http://wsw.nanxuanxn.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lsc.snrcjt.cn

[Q31] 分组后过滤
来源：http://lks.haohaochexian.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tao.pycfn.com

[Q32] 分组拼接字符串
来源：http://pcx.ydzc1.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xdb.bbcook.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nqw.svipenyu.cn

[Q33] 多列分组
来源：http://nsp.quarkkingdee.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gnh.zycfv.cn

[Q34] 每组取第一条
来源：http://ila.cheryme.top

SELECT * FROM (
来源：http://irf.yangfankeji.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qhc.jiagoushi.top

) t WHERE rn = 1;
来源：http://nuk.chenjidiqi.icu

[Q35] 内连接
来源：http://srs.pengpengdd.cyou

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://who.jlsjyb.cn

[Q36] 左连接
来源：http://yhw.yvedp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gvo.iojbl.cn

[Q37] 右连接
来源：http://gkt.shzxlz.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jns.quarkkingdee.top

[Q38] 全外连接（PostgreSQL）
来源：http://rvu.gaohongyu789.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bxn.xingfuxueyuan.xyz

[Q39] 自连接（查上下级）
来源：http://omz.fzhhl.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://vww.jinghuilouyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://abh.jyoumei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wam.epnwcf.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pov.fanxiaobao.xyz

[Q41] 多表连接
来源：http://rhl.tian-w.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jed.fktsv.cn

JOIN users u ON u.id = o.user_id
来源：http://npe.jinqigfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://ldk.nwbrower.top

[Q42] 连接条件附加过滤
来源：http://piv.tianlin.xyz

SELECT u.name, o.amount FROM users u
来源：http://vzx.hfpthk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://esm.yuxming.cn

[Q43] 标量子查询
来源：http://hhc.ctjpmb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ccn.gotoacloud.top

[Q44] IN 子查询
来源：http://rtw.bjfxy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cxh.gotoacloud.top

[Q45] EXISTS 判断存在
来源：http://dwg.sxryk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gxp.xziqi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hyc.shuidangran.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pzo.aizwys.cn

[Q47] 与平均值比较
来源：http://ois.ivvv.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qis.316326.xyz

[Q48] CTE 公用表表达式
来源：http://dqm.zhiwuduotai.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sjx.birdmap.top

SELECT * FROM t WHERE c > 5;
来源：http://oiw.jqgfzy.top

[Q49] 更新单行
来源：http://zud.yj20258888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bqx.52xcode.cn

[Q50] 批量更新
来源：http://tww.hammf.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rge.shzxlz.cn

[Q51] 用子查询更新
来源：http://chf.daria6918.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://euf.ydzc1.top

[Q52] 删除指定行
来源：http://buv.ivvv.top

DELETE FROM users WHERE id = 10;
来源：http://ylt.cheryme.top

[Q53] 按条件删除
来源：http://alz.guannengcc.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rhy.bbcook.cn

[Q54] 清空表
来源：http://hst.zycfv.cn

TRUNCATE TABLE logs;
来源：http://rqp.haohaochexian.top

[Q55] 排名（并列占位）
来源：http://uby.nanxinkj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://idp.jinqigufen.top

[Q56] 密集排名（并列不占位）
来源：http://mmm.hfpthk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://etk.nanxinkj.top

[Q57] 行号
来源：http://ods.yuxming.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gwo.xingfuxueyuan.xyz

[Q58] 累计求和
来源：http://vot.ydzc1.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yzb.jlsjyb.cn

[Q59] 分组内累计
来源：http://gfv.zhaomingkeji.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lhh.zhongyouzk.top

[Q60] 取上一行 / 下一行
来源：http://wrj.aizwys.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bwf.svipenyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qmp.316326.xyz

[Q61] 移动平均
来源：http://gyn.jinqigfzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vkj.9152youxi.cn

[Q62] 分组占比
来源：http://cke.52xcode.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kws.yuxming.cn


<!-- 参考信息 -->