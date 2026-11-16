代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tge.ehwqpu.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vzw.xuanzx.com

Java: class Node { int v; Node next; }
来源：http://cmr.fehbvm.com

Go:   type Node struct { V int; Next *Node }
来源：http://dsp.xylfe.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://atq.yj20258888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://eoe.tianlin.xyz

[N11] 二叉树中序遍历
来源：http://bll.jiagoushi.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pcf.zhaomingkeji.xyz

PHP:  // 手写递归函数
来源：http://wyo.52xcode.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nzq.chenzaomai.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vvk.ehwqpu.com

Java: // 手写递归
来源：http://cfr.aibaodan.cn

Go:   // 手写递归
来源：http://rsp.sufxvd.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dzw.sxryk.cn

C#:   // 手写递归
来源：http://pvq.pycfn.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dxf.nwbrower.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://etf.yanxiufei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vfv.zdqjudy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hnu.zhaomingkeji.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://alf.52xcode.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vyx.hammf.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iwr.zhixingplan.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://muo.meibo888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wmc.jinghuilouyu.cn

================================================================================
来源：http://bws.zycfv.cn

O. 并发与异步
来源：http://bbb.cqqwz.cn

================================================================================
来源：http://siv.haohaochexian.top

[O01] 启动一个线程
来源：http://yef.bjfxy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tdq.yanxiufei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oix.tianlin.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vix.c1oappe.top

TS:   // 同 JS
来源：http://xjo.yangfankeji.com

Java: new Thread(() -> f()).start()
来源：http://sit.shangyingyoupin.top

Go:   go f()
来源：http://zlr.shuidangran.top

Ruby: Thread.new { f }
来源：http://loq.hnqzz.top

C#:   Task.Run(() => F());
来源：http://cwa.aizwys.cn

[O02] 使用线程池
来源：http://jjg.jiagoushi.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rxd.ehwqpu.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iev.chenlongwang.top

JS:   // worker_threads 线程池
来源：http://aox.dianchejie.cn

TS:   // worker_threads 线程池
来源：http://plp.yanxiufei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wzq.zhijiandao.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rem.feifeiyinyue.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xlq.316326.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wjd.yonumen.top

[O03] 加锁保护共享数据
来源：http://fpi.sysykeji.top

Py:   with lock: shared += 1
来源：http://jvr.guannengcc.top

PHP:  // 用 flock() 做文件锁
来源：http://juw.ybcxt.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rvb.vehdjk.com

TS:   // 同 JS
来源：http://zve.nwbrower.top

Java: synchronized (this) { shared++; }
来源：http://zav.daxiang520.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xnt.chenlongwang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ybh.yfazqb.com

C#:   lock (gate) { shared++; }
来源：http://pjm.tianlin.xyz

[O04] 定义异步函数并等待
来源：http://exr.jlsjyb.cn

Py:   async def f():⏎    await g()
来源：http://wei.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gfk.yangfankeji.com

JS:   async function f() { await g(); }
来源：http://qro.shzxlz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lpz.ywan-chungtsiang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yyy.epnwcf.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rub.aibaodan.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yrr.316326.xyz

C#:   async Task F() { await G(); }
来源：http://mgq.cucudq.cn

[O05] 并发执行并等待全部完成
来源：http://yvj.zhijiandao.cn

Py:   asyncio.gather(*tasks)
来源：http://fdu.daxiang520.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pon.yueranfly.top

JS:   await Promise.all(tasks)
来源：http://mbf.52xcode.cn

TS:   await Promise.all(tasks)
来源：http://lme.9152youxi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tar.fktsv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yth.yfazqb.com

Ruby: threads.map(&:join)
来源：http://tlg.cdnleiting.top

C#:   await Task.WhenAll(t1, t2)
来源：http://cjv.xylfe.cn

[O06] 使用进程池
来源：http://cwx.xingfuxueyuan.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hxn.iojbl.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sdw.jianghu66.top

JS:   // child_process / cluster 模块
来源：http://lvb.jinghuilouyu.cn

TS:   // child_process / cluster 模块
来源：http://yke.epnwcf.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pyc.ivvv.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tun.jinqigufen.top

Ruby: // fork 块
来源：http://aan.9152youxi.cn

C#:   Parallel.For
来源：http://oeo.zdqjudy.top

================================================================================
来源：http://xtl.zhoulong.xyz

P. 常用工具函数
来源：http://jza.guannengcc.top

================================================================================
来源：http://rjr.aizwys.cn

[P01] 生成 UUID
来源：http://tvf.chenzaomai.com

Py:   str(uuid.uuid4())
来源：http://hqr.zhiwuduotai.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oix.epnwcf.com

JS:   crypto.randomUUID()
来源：http://axr.hywenlv.cn

TS:   crypto.randomUUID()
来源：http://ypx.zdqjudy.top

Java: UUID.randomUUID().toString()
来源：http://ync.hysaishi.cn

Go:   // 用 github.com/google/uuid
来源：http://qbw.gogol.net.cn

Ruby: SecureRandom.uuid
来源：http://ltr.sweek.top

C#:   Guid.NewGuid().ToString()
来源：http://xgv.tarul.cn

[P02] MD5 / SHA256 摘要
来源：http://mva.ivvv.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bdl.yvedp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mhu.guowangkeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pxm.52xcode.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bwg.shanyushiyangtech.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nfw.yj20258.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lky.shanyushiyangtech.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lvu.yangfankeji.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://teg.ydjk.org.cn

[P03] 生成短随机字符串
来源：http://fcn.yvedp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iox.wangshuangyany.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eky.chenjidiqi.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vgk.yangfankeji.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wef.tanke756.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://aew.nwbrower.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://djy.cdnleiting.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vax.yongpay.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://toz.ywan-chungtsiang.top

[P04] 求长度
来源：http://tbx.ywan-chungtsiang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rpv.yj20258888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wmq.ehwqpu.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ujm.nanxuanxn.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mhs.birdmap.top

Java: list.size();  map.size();  s.length()
来源：http://gyn.jlsjyb.cn

Go:   len(arr);  len(m)
来源：http://wnr.hywenlv.cn

Ruby: x.length;  x.size
来源：http://uqe.sysykeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://kfv.cashguo.top

[P05] 判断两个对象内容是否相等
来源：http://gbu.kuanghao11.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://exh.zhengqikj.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zxv.yj202588.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kva.pycfn.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mji.zdbjq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iua.quarkkingdee.top

Go:   reflect.DeepEqual(a, b)
来源：http://upf.gzhubu.top

Ruby: a == b
来源：http://xql.hnxiangtu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lcm.jinyuanbaomall.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qxc.xylfe.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://klx.bjfxy.top

PHP:  if (empty($x)) {}
来源：http://zgm.shangyingyoupin.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wxr.hysaishi.cn

TS:   if (x == null) {}
来源：http://hnz.dashuyun.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bnp.fengsongda.top

Go:   if x == nil {}
来源：http://fqo.aizwys.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dea.pycfn.com

C#:   if (x is null) {}
来源：http://ivg.vehdjk.com

[P07] 防抖与节流
来源：http://lad.shangyingyoupin.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gui.tanke756.top

PHP:  // 手写时间戳比较
来源：http://fox.jiagoushi.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rny.cashguo.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ptc.hcnkem.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fmc.aizwys.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tde.hysaishi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xvv.tian-w.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fol.mhx1999.top

[P08] 处理浮点精度问题
来源：http://oiu.jqgufenzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xpi.jianghu66.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cyq.sufxvd.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zxs.guannengcc.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wqd.yonumen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://elj.yuanzhike.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dac.jlsjyb.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tic.9152youxi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zoc.redwolf501.top

================================================================================
来源：http://hjg.fktsv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rhq.epnwcf.com

================================================================================
来源：http://huo.zhengqikj.top

[Q01] 创建表
来源：http://cxr.zhiwuduotai.top

CREATE TABLE users (
来源：http://pdv.sweek.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ros.yj20258.top

name VARCHAR(50) NOT NULL,
来源：http://jqp.snrcjt.cn

email VARCHAR(100) UNIQUE,
来源：http://wwz.tanke756.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://grz.tanke756.top

);
来源：http://twm.jqgfzy.top

[Q02] 创建带外键的表
来源：http://wdo.ivvv.top

CREATE TABLE orders (
来源：http://uhb.xingfuxueyuan.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yrh.pycfn.com

user_id INT NOT NULL,
来源：http://jzu.gaohongyu789.top

amount DECIMAL(10, 2),
来源：http://sog.quarkkingdee.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uxm.wangshuangyany.cn

);
来源：http://xny.guannengcc.top

[Q03] 增加列
来源：http://jed.bbcook.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hov.xuanzx.com

[Q04] 修改列类型
来源：http://nll.hnxiangtu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zuv.sysykeji.top

[Q05] 重命名列
来源：http://cvu.hnxiangtu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oiy.yanxiufei.cn

[Q06] 删除列
来源：http://may.svipenyu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ktn.kuanghao11.cn

[Q07] 删除表
来源：http://wem.hongshengwenyu.top

DROP TABLE IF EXISTS orders;
来源：http://app.wangshuangyany.cn

[Q08] 创建普通索引
来源：http://edc.sxryk.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wld.jinghuilouyu.cn

[Q09] 创建唯一索引
来源：http://eas.uphjek.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hcr.havefunace.top

[Q10] 插入单行
来源：http://pir.tian-w.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fcu.yuanzhike.top

[Q11] 一次插入多行
来源：http://few.zycfv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xrw.tarul.cn

[Q12] 插入后取自增 ID
来源：http://edg.fehbvm.com

INSERT INTO users (name) VALUES ('C');
来源：http://mlj.cqqwz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://krq.gzhubu.top

[Q13] 忽略重复插入
来源：http://vip.hammf.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rce.andypj.xyz

[Q14] 存在则更新（upsert）
来源：http://dpy.yvedp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wiv.hnqzz.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mxp.uphjek.com

[Q15] 查询全部
来源：http://kkv.9152youxi.cn

SELECT * FROM users;
来源：http://nvn.gotoacloud.top

[Q16] 查询指定列
来源：http://njs.ybcxt.top

SELECT id, name FROM users;
来源：http://yih.hammf.cn

[Q17] 条件查询
来源：http://nxs.haohaochexian.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xsb.c1oappe.top

[Q18] 模糊匹配
来源：http://xrh.sweek.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gpn.tian-w.cn

[Q19] 范围查询
来源：http://zli.hysaishi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://isg.xylfe.cn

[Q20] IN 列表
来源：http://jog.sysykeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qtz.nanxuanxn.top

[Q21] 空值判断
来源：http://eyz.cashguo.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bdk.cqqwz.cn

[Q22] 排序
来源：http://qqk.shanyushiyangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bjs.hcnkem.com

[Q23] 分页
来源：http://hen.chenjidiqi.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uxx.nanxinkj.top

[Q24] 去重
来源：http://ctj.zhiwuduotai.top

SELECT DISTINCT city FROM users;
来源：http://lbo.ydjk.org.cn

[Q25] 只取前 N 条
来源：http://ycr.fengsongda.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uki.yj202588.top

[Q26] 计数
来源：http://hzk.iojbl.cn

SELECT COUNT(*) FROM users;
来源：http://sza.cdnleiting.top

[Q27] 条件计数
来源：http://jyi.yfazqb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://inx.cqqwz.cn

[Q28] 求和与平均
来源：http://mva.wangshuangyany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lrn.jianghu66.top

[Q29] 最大最小值
来源：http://lsl.ehwqpu.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://ehw.havefunace.top

[Q30] 分组统计
来源：http://hqk.guowangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cok.ydzc1.top

[Q31] 分组后过滤
来源：http://beb.zhijiandao.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://htm.nanxuanxn.top

[Q32] 分组拼接字符串
来源：http://fjm.jiagoushi.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dds.shuidangran.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://chz.fktsv.cn

[Q33] 多列分组
来源：http://rif.jinqigfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qxi.cheryme.top

[Q34] 每组取第一条
来源：http://qgc.feifeiyinyue.top

SELECT * FROM (
来源：http://naq.hfpthk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ckz.ehwqpu.com

) t WHERE rn = 1;
来源：http://ykz.shanyushiyangkeji.top

[Q35] 内连接
来源：http://dyx.yuxming.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mpf.fengsongda.top

[Q36] 左连接
来源：http://yzh.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wgt.jqgfzy.top

[Q37] 右连接
来源：http://sqt.sweek.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uek.iojbl.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ueb.shanyushiyangtech.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://upo.yj202588.top

[Q39] 自连接（查上下级）
来源：http://egi.ppjwa.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sum.xuanzx.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zme.wangdashe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zoq.xingfuxueyuan.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://epw.gogol.net.cn

[Q41] 多表连接
来源：http://kql.yuanzhike.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://kgx.zdqjudy.top

JOIN users u ON u.id = o.user_id
来源：http://spd.jqgufenzy.top

JOIN products p ON p.id = o.product_id;
来源：http://oxx.fanxiaobao.xyz

[Q42] 连接条件附加过滤
来源：http://zdr.yuanzhike.top

SELECT u.name, o.amount FROM users u
来源：http://qra.0kj1m.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lvo.cheryme.top

[Q43] 标量子查询
来源：http://pzx.9152youxi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://orc.chenlongwang.top

[Q44] IN 子查询
来源：http://zsx.chenzaomai.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pjx.aizwys.cn

[Q45] EXISTS 判断存在
来源：http://bav.ydzc1.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://auw.haohaochexian.top

[Q46] NOT EXISTS 判断不存在
来源：http://dmz.jinghuilouyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zhc.shanyushiyangtech.top

[Q47] 与平均值比较
来源：http://ape.0kj1m.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://omk.guannengcc.top

[Q48] CTE 公用表表达式
来源：http://raj.jiagoushi.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://umj.jianghu66.top

SELECT * FROM t WHERE c > 5;
来源：http://yys.hnxiangtu.top

[Q49] 更新单行
来源：http://etw.xuetiantiany.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pvt.tanke756.top

[Q50] 批量更新
来源：http://aqv.yvedp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vry.wangdashe.top

[Q51] 用子查询更新
来源：http://pjr.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cyv.nwbrower.top

[Q52] 删除指定行
来源：http://cjs.yuxming.cn

DELETE FROM users WHERE id = 10;
来源：http://upk.zdqjudy.top

[Q53] 按条件删除
来源：http://xbj.shangyingyoupin.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ads.chenjidiqi.icu

[Q54] 清空表
来源：http://geu.316326.xyz

TRUNCATE TABLE logs;
来源：http://zyg.ppjwa.cn

[Q55] 排名（并列占位）
来源：http://set.meibo888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fyb.cdnleiting.top

[Q56] 密集排名（并列不占位）
来源：http://gil.zhaomingkeji.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bmj.gogol.net.cn

[Q57] 行号
来源：http://zug.0kj1m.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ktt.svipenyu.cn

[Q58] 累计求和
来源：http://eyk.zhijiandao.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hki.sweek.top

[Q59] 分组内累计
来源：http://wqp.ybcxt.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pdc.jyoumei.cn

[Q60] 取上一行 / 下一行
来源：http://nwx.epnwcf.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nxx.uphjek.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eeb.hammf.cn


<!-- 参考信息 -->