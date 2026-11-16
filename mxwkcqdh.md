代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pll.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://twv.yongpay.top

Java: class Node { int v; Node next; }
来源：http://spr.redwolf501.top

Go:   type Node struct { V int; Next *Node }
来源：http://ioz.mhx1999.top

Ruby: Node = Struct.new(:v, :next)
来源：http://imb.zhongyouzk.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lmh.yuxming.cn

[N11] 二叉树中序遍历
来源：http://qcv.shuidangran.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yct.hfpthk.cn

PHP:  // 手写递归函数
来源：http://sue.yongpay.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xay.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sxy.hnxiangtu.top

Java: // 手写递归
来源：http://mkt.uphjek.com

Go:   // 手写递归
来源：http://jax.guannengcc.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dld.feifeiyinyue.top

C#:   // 手写递归
来源：http://nhh.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://egv.sjlbkw.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bjv.haohaochexian.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pzu.zdqjudy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://erv.wangshuangyany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kzi.jinqigufen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yol.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lng.birdmap.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qbt.wangdashe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jrw.havefunace.top

================================================================================
来源：http://cxb.ivvv.top

O. 并发与异步
来源：http://xsa.yj20258888.top

================================================================================
来源：http://wkb.fehbvm.com

[O01] 启动一个线程
来源：http://ohp.cucudq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://psv.hfpthk.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://csz.cucudq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eiq.quarkkingdee.top

TS:   // 同 JS
来源：http://ota.gzhubu.top

Java: new Thread(() -> f()).start()
来源：http://hki.0kj1m.cn

Go:   go f()
来源：http://fvb.ivvv.top

Ruby: Thread.new { f }
来源：http://lnp.9152youxi.cn

C#:   Task.Run(() => F());
来源：http://xoi.cdnleiting.top

[O02] 使用线程池
来源：http://zop.iojbl.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mhs.jqgufenzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wpi.ydzc1.top

JS:   // worker_threads 线程池
来源：http://adr.meibo888.top

TS:   // worker_threads 线程池
来源：http://ani.zdqjudy.top

Java: Executors.newFixedThreadPool(4)
来源：http://kfa.haohaochexian.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zcy.cucudq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://drl.guowangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hxn.xinyue.icu

[O03] 加锁保护共享数据
来源：http://vuz.wangshuangyany.cn

Py:   with lock: shared += 1
来源：http://fne.sweek.top

PHP:  // 用 flock() 做文件锁
来源：http://jbs.ydzc1.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tkl.yueranfly.top

TS:   // 同 JS
来源：http://okg.cashguo.top

Java: synchronized (this) { shared++; }
来源：http://bjk.ctjpmb.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bur.9152youxi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bts.fehbvm.com

C#:   lock (gate) { shared++; }
来源：http://sza.tarul.cn

[O04] 定义异步函数并等待
来源：http://qms.tian-w.cn

Py:   async def f():⏎    await g()
来源：http://toi.xinyue.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cde.ywan-chungtsiang.top

JS:   async function f() { await g(); }
来源：http://wdp.jinqigfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ows.yuxming.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fzn.uphjek.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rkz.cdnleiting.top

Ruby: # 用 Fiber 或 async gem
来源：http://lob.ydjk.org.cn

C#:   async Task F() { await G(); }
来源：http://vmq.tianlin.xyz

[O05] 并发执行并等待全部完成
来源：http://stx.shanyushiyangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://ppc.kuanghao11.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pqx.fengsongda.top

JS:   await Promise.all(tasks)
来源：http://dps.hysaishi.cn

TS:   await Promise.all(tasks)
来源：http://whb.hfpthk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tcx.meibo888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fyt.yj202588.top

Ruby: threads.map(&:join)
来源：http://rdd.meibo888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dxn.c1oappe.top

[O06] 使用进程池
来源：http://ahn.jianghu66.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rsq.gzhubu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hkv.jiagoushi.top

JS:   // child_process / cluster 模块
来源：http://pqa.xziqi.cn

TS:   // child_process / cluster 模块
来源：http://fhi.birdmap.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vvc.jinqigufen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://huz.vehdjk.com

Ruby: // fork 块
来源：http://qun.0kj1m.cn

C#:   Parallel.For
来源：http://qaw.ydjk.org.cn

================================================================================
来源：http://uxl.aizwys.cn

P. 常用工具函数
来源：http://vfq.shangyingyoupin.top

================================================================================
来源：http://bfo.ctjpmb.com

[P01] 生成 UUID
来源：http://bby.cheryme.top

Py:   str(uuid.uuid4())
来源：http://diu.pengpengdd.cyou

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pia.nanxuanxn.top

JS:   crypto.randomUUID()
来源：http://oja.xziqi.cn

TS:   crypto.randomUUID()
来源：http://wcs.birdmap.top

Java: UUID.randomUUID().toString()
来源：http://dby.fktsv.cn

Go:   // 用 github.com/google/uuid
来源：http://zuo.zhijiandao.cn

Ruby: SecureRandom.uuid
来源：http://gxk.gaohongyu789.top

C#:   Guid.NewGuid().ToString()
来源：http://jea.redwolf501.top

[P02] MD5 / SHA256 摘要
来源：http://jqq.316326.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wcu.kuanghao11.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nri.guowangkeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tjh.jianghu66.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gvv.hammf.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://eiy.jiagoushi.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kpo.mhx1999.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pwy.nanxinkj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://owg.xziqi.cn

[P03] 生成短随机字符串
来源：http://icx.cqqwz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xaw.birdmap.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tsj.zhoulong.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yzc.wangdashe.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hbp.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kji.shanyushiyangtech.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yaf.chenzaomai.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://rjk.zycfv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sbi.snrcjt.cn

[P04] 求长度
来源：http://euh.zhijiandao.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bho.cashguo.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bgo.svipenyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://css.jinyuanbaomall.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gqp.nwbrower.top

Java: list.size();  map.size();  s.length()
来源：http://abz.chenlongwang.top

Go:   len(arr);  len(m)
来源：http://lnm.jqgufenzy.top

Ruby: x.length;  x.size
来源：http://hbm.shanyushiyangtech.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://sik.xuanzx.com

[P05] 判断两个对象内容是否相等
来源：http://gjc.shanyushiyangtech.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gkm.316326.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vnc.xinyue.icu

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ayo.pengpengdd.cyou

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://njt.quarkkingdee.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cfe.gotoacloud.top

Go:   reflect.DeepEqual(a, b)
来源：http://gcd.jlsjyb.cn

Ruby: a == b
来源：http://mzt.chenzaomai.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wyf.tianlin.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ssx.sxryk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wdy.zhengqikj.top

PHP:  if (empty($x)) {}
来源：http://ove.ydzc1.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vdm.daxiang520.top

TS:   if (x == null) {}
来源：http://lxo.sufxvd.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ekw.fehbvm.com

Go:   if x == nil {}
来源：http://dnd.yvedp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zcl.jinghuilouyu.cn

C#:   if (x is null) {}
来源：http://ako.hesvh.cn

[P07] 防抖与节流
来源：http://mgp.bbcook.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lft.shangyingyoupin.top

PHP:  // 手写时间戳比较
来源：http://yxp.zhongyouzk.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sfh.vehdjk.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hxc.svipenyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jmh.zhoulong.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://itr.kuanghao11.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qwk.jiagoushi.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xce.redwolf501.top

[P08] 处理浮点精度问题
来源：http://poi.wangdashe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ktq.ivvv.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://oqx.c1oappe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ymz.tanke756.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qqw.hammf.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lwq.yuxming.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kus.shuidangran.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://slp.meibo888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xpm.hesvh.cn

================================================================================
来源：http://jev.dashuyun.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://toj.gogol.net.cn

================================================================================
来源：http://qrg.aizwys.cn

[Q01] 创建表
来源：http://ztr.zhongyouzk.top

CREATE TABLE users (
来源：http://ktq.316326.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rxr.uphjek.com

name VARCHAR(50) NOT NULL,
来源：http://tbe.shuidangran.top

email VARCHAR(100) UNIQUE,
来源：http://bep.havefunace.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bfg.zhiwuduotai.top

);
来源：http://awp.guowangkeji.top

[Q02] 创建带外键的表
来源：http://zpq.zhengqikj.top

CREATE TABLE orders (
来源：http://vna.wangshuangyany.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://thg.snrcjt.cn

user_id INT NOT NULL,
来源：http://xjg.xuanzx.com

amount DECIMAL(10, 2),
来源：http://vfq.sweek.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jri.gaohongyu789.top

);
来源：http://vhz.yonumen.top

[Q03] 增加列
来源：http://fww.jinqigufen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gfw.yueranfly.top

[Q04] 修改列类型
来源：http://iqi.yangfankeji.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qtq.quarkkingdee.top

[Q05] 重命名列
来源：http://kgb.cqqwz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hqr.hammf.cn

[Q06] 删除列
来源：http://icw.yueranfly.top

ALTER TABLE users DROP COLUMN age;
来源：http://buv.xylfe.cn

[Q07] 删除表
来源：http://taj.yueranfly.top

DROP TABLE IF EXISTS orders;
来源：http://wpn.shanyushiyangtech.top

[Q08] 创建普通索引
来源：http://tnj.ppjwa.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tyb.jyoumei.cn

[Q09] 创建唯一索引
来源：http://usi.52xcode.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tpm.shuidangran.top

[Q10] 插入单行
来源：http://mpw.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rhd.jyoumei.cn

[Q11] 一次插入多行
来源：http://pqp.xuanzx.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sij.zhiwuduotai.top

[Q12] 插入后取自增 ID
来源：http://abt.ydjk.org.cn

INSERT INTO users (name) VALUES ('C');
来源：http://eom.cucudq.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://msr.jinyuanbaomall.cn

[Q13] 忽略重复插入
来源：http://hmp.zhiwuduotai.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kxg.9152youxi.cn

[Q14] 存在则更新（upsert）
来源：http://txw.zhoulong.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ggg.ydjk.org.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jzu.zhaomingkeji.xyz

[Q15] 查询全部
来源：http://hby.fzhhl.top

SELECT * FROM users;
来源：http://bhv.jinyuanbaomall.cn

[Q16] 查询指定列
来源：http://rwn.hywenlv.cn

SELECT id, name FROM users;
来源：http://akb.zdqjudy.top

[Q17] 条件查询
来源：http://whx.zycfv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tdm.daxiang520.top

[Q18] 模糊匹配
来源：http://ocz.316326.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sec.jiagoushi.top

[Q19] 范围查询
来源：http://koy.yj20258888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rzk.daxiang520.top

[Q20] IN 列表
来源：http://qpr.gaohongyu789.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cag.daxiang520.top

[Q21] 空值判断
来源：http://zhu.ivvv.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xwy.cucudq.cn

[Q22] 排序
来源：http://ium.yvedp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xug.nanxuanxn.top

[Q23] 分页
来源：http://duz.zycfv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cca.yj20258888.top

[Q24] 去重
来源：http://vpu.epnwcf.com

SELECT DISTINCT city FROM users;
来源：http://lgr.tian-w.cn

[Q25] 只取前 N 条
来源：http://zet.snrcjt.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dqw.xinyue.icu

[Q26] 计数
来源：http://xtd.hysaishi.cn

SELECT COUNT(*) FROM users;
来源：http://wbd.jinghuilouyu.cn

[Q27] 条件计数
来源：http://lly.cashguo.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zam.zdqjudy.top

[Q28] 求和与平均
来源：http://ief.fktsv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://caj.gzhubu.top

[Q29] 最大最小值
来源：http://oek.vehdjk.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://mrs.shuidangran.top

[Q30] 分组统计
来源：http://odw.tarul.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wkp.yfazqb.com

[Q31] 分组后过滤
来源：http://mww.xziqi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lak.andypj.xyz

[Q32] 分组拼接字符串
来源：http://dvh.cucudq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cxr.andypj.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ycf.jinqigfzy.top

[Q33] 多列分组
来源：http://rjc.kuanghao11.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dzw.dianchejie.cn

[Q34] 每组取第一条
来源：http://tqp.dianchejie.cn

SELECT * FROM (
来源：http://qia.kuanghao11.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wtr.yangfankeji.com

) t WHERE rn = 1;
来源：http://pwl.vehdjk.com

[Q35] 内连接
来源：http://lkd.nanxinkj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lno.snrcjt.cn

[Q36] 左连接
来源：http://afc.zhengqikj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bap.yanxiufei.cn

[Q37] 右连接
来源：http://yiz.aizwys.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wkb.yj20258.top

[Q38] 全外连接（PostgreSQL）
来源：http://uld.hesvh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mtv.zdbjq.cn

[Q39] 自连接（查上下级）
来源：http://xwi.aibaodan.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hor.chenjidiqi.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vtl.daxiang520.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pwr.jinqigfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ljb.aizwys.cn

[Q41] 多表连接
来源：http://pfy.haohaochexian.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://epy.andypj.xyz

JOIN users u ON u.id = o.user_id
来源：http://rpr.fzhhl.top

JOIN products p ON p.id = o.product_id;
来源：http://vni.uphjek.com

[Q42] 连接条件附加过滤
来源：http://elq.tarul.cn

SELECT u.name, o.amount FROM users u
来源：http://lgv.yj20258888.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cmc.xinyue.icu

[Q43] 标量子查询
来源：http://smw.meibo888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cvk.bbcook.cn

[Q44] IN 子查询
来源：http://ctk.chenzaomai.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qho.pycfn.com

[Q45] EXISTS 判断存在
来源：http://lze.cashguo.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aky.ppjwa.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xlk.zdqjudy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://szn.fengsongda.top

[Q47] 与平均值比较
来源：http://jac.guowangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fjv.guowangkeji.top

[Q48] CTE 公用表表达式
来源：http://znl.tianlin.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nnh.svipenyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://vpt.sxryk.cn

[Q49] 更新单行
来源：http://xcj.fktsv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qdg.ydzc1.top

[Q50] 批量更新
来源：http://afr.jinghuilouyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://deu.zhixingplan.top

[Q51] 用子查询更新
来源：http://rgc.gotoacloud.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xhz.tian-w.cn

[Q52] 删除指定行
来源：http://gst.yangfankeji.com

DELETE FROM users WHERE id = 10;
来源：http://edd.hnqzz.top

[Q53] 按条件删除
来源：http://syw.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://neh.fengsongda.top

[Q54] 清空表
来源：http://sia.shzxlz.cn

TRUNCATE TABLE logs;
来源：http://woz.guannengcc.top

[Q55] 排名（并列占位）
来源：http://qmt.aibaodan.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fhl.wangdashe.top

[Q56] 密集排名（并列不占位）
来源：http://nqr.guowangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ato.ehwqpu.com

[Q57] 行号
来源：http://hoq.sweek.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dtg.jlsjyb.cn

[Q58] 累计求和
来源：http://bkh.andypj.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vto.yanxiufei.cn

[Q59] 分组内累计
来源：http://oiu.ydjk.org.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cie.yanxiufei.cn

[Q60] 取上一行 / 下一行
来源：http://ywt.yuxming.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wdr.pengpengdd.cyou

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kex.zhiwuduotai.top


<!-- 参考信息 -->