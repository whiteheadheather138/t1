代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dgm.jinqigufen.top

[N10] 链表节点定义
来源：http://lrc.zycfv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://foo.guowangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://nlo.fanxiaobao.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kre.feifeiyinyue.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://aex.ppjwa.cn

Java: class Node { int v; Node next; }
来源：http://eoh.jinqigfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://abg.ppjwa.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bgf.tianlin.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://xhx.aibaodan.cn

[N11] 二叉树中序遍历
来源：http://huy.xuetiantiany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qrd.yuanzhike.top

PHP:  // 手写递归函数
来源：http://bja.chenzaomai.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hib.feifeiyinyue.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bto.xingfuxueyuan.xyz

Java: // 手写递归
来源：http://sst.hfpthk.cn

Go:   // 手写递归
来源：http://dtp.c1oappe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ckg.zycfv.cn

C#:   // 手写递归
来源：http://tju.jianghu66.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wev.yuxming.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ohv.ivvv.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ukk.cheryme.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://msv.52xcode.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://whi.jinghuilouyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gyq.sysykeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yzd.0kj1m.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pje.svipenyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tlv.jqgfzy.top

================================================================================
来源：http://riu.yfazqb.com

O. 并发与异步
来源：http://dbl.xingfuxueyuan.xyz

================================================================================
来源：http://cty.shangyingyoupin.top

[O01] 启动一个线程
来源：http://mox.zhoulong.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://anx.aibaodan.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qks.ydzc1.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hjl.cheryme.top

TS:   // 同 JS
来源：http://ojo.sufxvd.cn

Java: new Thread(() -> f()).start()
来源：http://spy.uphjek.com

Go:   go f()
来源：http://hep.cqqwz.cn

Ruby: Thread.new { f }
来源：http://mxo.zdbjq.cn

C#:   Task.Run(() => F());
来源：http://nqi.haohaochexian.top

[O02] 使用线程池
来源：http://ohr.cucudq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ppe.smart0.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jfb.ydjk.org.cn

JS:   // worker_threads 线程池
来源：http://zkj.sufxvd.cn

TS:   // worker_threads 线程池
来源：http://ius.uphjek.com

Java: Executors.newFixedThreadPool(4)
来源：http://mfi.sweek.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://asr.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://txi.xuanzx.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wqm.0kj1m.cn

[O03] 加锁保护共享数据
来源：http://tdn.nanxuanxn.top

Py:   with lock: shared += 1
来源：http://akh.ppjwa.cn

PHP:  // 用 flock() 做文件锁
来源：http://ghj.cheryme.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zdh.ydzc1.top

TS:   // 同 JS
来源：http://lqp.xingfuxueyuan.xyz

Java: synchronized (this) { shared++; }
来源：http://vej.chenjidiqi.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://atm.jinqigufen.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://cut.yuxming.cn

C#:   lock (gate) { shared++; }
来源：http://vbk.tarul.cn

[O04] 定义异步函数并等待
来源：http://nrp.yanxiufei.cn

Py:   async def f():⏎    await g()
来源：http://tnk.hongshengwenyu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lkm.quarkkingdee.top

JS:   async function f() { await g(); }
来源：http://ewe.jinqigfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ejz.chenzaomai.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://geb.feifeiyinyue.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vtc.birdmap.top

Ruby: # 用 Fiber 或 async gem
来源：http://vhn.316326.xyz

C#:   async Task F() { await G(); }
来源：http://sjr.nanxuanxn.top

[O05] 并发执行并等待全部完成
来源：http://kda.hammf.cn

Py:   asyncio.gather(*tasks)
来源：http://pmg.jiagoushi.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jbw.xziqi.cn

JS:   await Promise.all(tasks)
来源：http://rdj.gzhubu.top

TS:   await Promise.all(tasks)
来源：http://ddw.xylfe.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ysi.xuetiantiany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cqo.zhijiandao.cn

Ruby: threads.map(&:join)
来源：http://udc.cashguo.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fil.jqgufenzy.top

[O06] 使用进程池
来源：http://pfn.smart0.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wtr.jyoumei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pxp.ehwqpu.com

JS:   // child_process / cluster 模块
来源：http://tar.yfazqb.com

TS:   // child_process / cluster 模块
来源：http://jxg.ctjpmb.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gyq.shangyingyoupin.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yep.sysykeji.top

Ruby: // fork 块
来源：http://ndy.nanxinkj.top

C#:   Parallel.For
来源：http://qew.ydjk.org.cn

================================================================================
来源：http://msi.jiagoushi.top

P. 常用工具函数
来源：http://jkc.chenlongwang.top

================================================================================
来源：http://mei.quarkkingdee.top

[P01] 生成 UUID
来源：http://ada.yueranfly.top

Py:   str(uuid.uuid4())
来源：http://ypo.vqdsnc.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pbq.hywenlv.cn

JS:   crypto.randomUUID()
来源：http://pdy.52xcode.cn

TS:   crypto.randomUUID()
来源：http://fat.shangyingyoupin.top

Java: UUID.randomUUID().toString()
来源：http://ktc.fktsv.cn

Go:   // 用 github.com/google/uuid
来源：http://nfv.hongshengwenyu.top

Ruby: SecureRandom.uuid
来源：http://vhk.yuxming.cn

C#:   Guid.NewGuid().ToString()
来源：http://qur.chenzaomai.com

[P02] MD5 / SHA256 摘要
来源：http://wcj.hesvh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cjn.ehwqpu.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://mab.zhengqikj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uzm.fktsv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qpn.jqgfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bpt.9152youxi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bmt.gaohongyu789.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wla.vehdjk.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://byg.quarkkingdee.top

[P03] 生成短随机字符串
来源：http://dbb.yfazqb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xug.jyoumei.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://equ.316326.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cjw.zhoulong.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jze.fehbvm.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lcf.yuxming.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kyp.pycfn.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://mnn.cheryme.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vbb.aibaodan.cn

[P04] 求长度
来源：http://dsh.nanxinkj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mlg.hongshengwenyu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mdn.cheryme.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jkf.havefunace.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xeu.ydzc1.top

Java: list.size();  map.size();  s.length()
来源：http://qnv.shanyushiyangkeji.top

Go:   len(arr);  len(m)
来源：http://uxn.cheryme.top

Ruby: x.length;  x.size
来源：http://rdh.gzhubu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pyb.hfpthk.cn

[P05] 判断两个对象内容是否相等
来源：http://kro.cashguo.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rry.zhoulong.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://urm.tanke756.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wxu.ivvv.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fui.shuidangran.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bvl.zycfv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://iew.yongpay.top

Ruby: a == b
来源：http://vtx.birdmap.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xvj.ppjwa.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://phr.yj202588.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lbt.xuetiantiany.cn

PHP:  if (empty($x)) {}
来源：http://gkj.cucudq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tiw.fktsv.cn

TS:   if (x == null) {}
来源：http://cmj.chenjidiqi.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://gvo.xziqi.cn

Go:   if x == nil {}
来源：http://ksc.ybcxt.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://abi.andypj.xyz

C#:   if (x is null) {}
来源：http://bgq.nanxuanxn.top

[P07] 防抖与节流
来源：http://mim.jianghu66.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ubp.sxryk.cn

PHP:  // 手写时间戳比较
来源：http://flz.daria6918.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hkr.gotoacloud.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kat.cdnleiting.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ifs.nanxuanxn.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xyp.fzhhl.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://jmg.sufxvd.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://eql.yj20258.top

[P08] 处理浮点精度问题
来源：http://dfl.shuidangran.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sdu.iojbl.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hcs.wangshuangyany.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tdv.sweek.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rsm.tarul.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ukr.hcnkem.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nof.52xcode.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ahb.dashuyun.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gui.bbcook.cn

================================================================================
来源：http://bwl.shanyushiyangkeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qqj.cucudq.cn

================================================================================
来源：http://dmu.sxryk.cn

[Q01] 创建表
来源：http://tkn.havefunace.top

CREATE TABLE users (
来源：http://yvy.epnwcf.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://paj.zhongyouzk.top

name VARCHAR(50) NOT NULL,
来源：http://efc.meibo888.top

email VARCHAR(100) UNIQUE,
来源：http://xam.ydzc1.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jts.havefunace.top

);
来源：http://duw.zdbjq.cn

[Q02] 创建带外键的表
来源：http://tyt.hfpthk.cn

CREATE TABLE orders (
来源：http://xfo.chenzaomai.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jds.yvedp.cn

user_id INT NOT NULL,
来源：http://apf.epnwcf.com

amount DECIMAL(10, 2),
来源：http://bha.vqdsnc.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dgs.yvedp.cn

);
来源：http://mzr.jianghu66.top

[Q03] 增加列
来源：http://xzu.zhiwuduotai.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yhf.xuanzx.com

[Q04] 修改列类型
来源：http://qra.zhongyouzk.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pnf.tarul.cn

[Q05] 重命名列
来源：http://gfj.jlsjyb.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hlq.wangshuangyany.cn

[Q06] 删除列
来源：http://kwy.yfazqb.com

ALTER TABLE users DROP COLUMN age;
来源：http://ppc.jiagoushi.top

[Q07] 删除表
来源：http://ecb.hywenlv.cn

DROP TABLE IF EXISTS orders;
来源：http://iky.zhixingplan.top

[Q08] 创建普通索引
来源：http://hfo.feifeiyinyue.top

CREATE INDEX idx_users_email ON users(email);
来源：http://eel.shanyushiyangkeji.top

[Q09] 创建唯一索引
来源：http://szg.ivvv.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lpp.ivvv.top

[Q10] 插入单行
来源：http://res.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vfj.epnwcf.com

[Q11] 一次插入多行
来源：http://sfw.svipenyu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xpf.kuanghao11.cn

[Q12] 插入后取自增 ID
来源：http://tnl.chenjidiqi.icu

INSERT INTO users (name) VALUES ('C');
来源：http://llx.yonumen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jei.hongshengwenyu.top

[Q13] 忽略重复插入
来源：http://drl.gogol.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hfg.nanxinkj.top

[Q14] 存在则更新（upsert）
来源：http://jit.yongpay.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gno.zdqjudy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://noi.aizwys.cn

[Q15] 查询全部
来源：http://jxa.ydzc1.top

SELECT * FROM users;
来源：http://drc.daxiang520.top

[Q16] 查询指定列
来源：http://fkm.yanxiufei.cn

SELECT id, name FROM users;
来源：http://cgc.zdqjudy.top

[Q17] 条件查询
来源：http://uiv.yj20258.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zho.316326.xyz

[Q18] 模糊匹配
来源：http://yvp.bjfxy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tgo.nanxinkj.top

[Q19] 范围查询
来源：http://yjo.redwolf501.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mbo.pycfn.com

[Q20] IN 列表
来源：http://flo.chenjidiqi.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xea.fktsv.cn

[Q21] 空值判断
来源：http://ogk.52xcode.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://aad.xingfuxueyuan.xyz

[Q22] 排序
来源：http://ech.kuanghao11.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dsb.yonumen.top

[Q23] 分页
来源：http://vbx.hfpthk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cmn.chenjidiqi.icu

[Q24] 去重
来源：http://mrd.zycfv.cn

SELECT DISTINCT city FROM users;
来源：http://bwc.smart0.xyz

[Q25] 只取前 N 条
来源：http://ulu.gaohongyu789.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ban.jyoumei.cn

[Q26] 计数
来源：http://gss.yuxming.cn

SELECT COUNT(*) FROM users;
来源：http://jaa.gzhubu.top

[Q27] 条件计数
来源：http://dgx.wangshuangyany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://shw.shzxlz.cn

[Q28] 求和与平均
来源：http://lej.hfpthk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jli.hammf.cn

[Q29] 最大最小值
来源：http://ybh.fengsongda.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bfm.gaohongyu789.top

[Q30] 分组统计
来源：http://ljz.svipenyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bjd.feifeiyinyue.top

[Q31] 分组后过滤
来源：http://nwp.yfazqb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wty.jqgufenzy.top

[Q32] 分组拼接字符串
来源：http://htj.sysykeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zlp.shzxlz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sks.yongpay.top

[Q33] 多列分组
来源：http://tjm.wangdashe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aww.hnqzz.top

[Q34] 每组取第一条
来源：http://viy.zdbjq.cn

SELECT * FROM (
来源：http://ubo.aizwys.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ftf.nwbrower.top

) t WHERE rn = 1;
来源：http://scd.sysykeji.top

[Q35] 内连接
来源：http://yqv.smart0.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://twn.shanyushiyangtech.top

[Q36] 左连接
来源：http://jkt.quarkkingdee.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xyu.9152youxi.cn

[Q37] 右连接
来源：http://hyt.jinghuilouyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ois.aizwys.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ulj.shangyingyoupin.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lwn.gzhubu.top

[Q39] 自连接（查上下级）
来源：http://dec.vqdsnc.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hjy.jinghuilouyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vmz.meibo888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wxz.yuanzhike.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pfh.cheryme.top

[Q41] 多表连接
来源：http://oxh.fehbvm.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://raq.yanxiufei.cn

JOIN users u ON u.id = o.user_id
来源：http://lsb.epnwcf.com

JOIN products p ON p.id = o.product_id;
来源：http://vtz.bbcook.cn

[Q42] 连接条件附加过滤
来源：http://pxu.havefunace.top

SELECT u.name, o.amount FROM users u
来源：http://xuz.yonumen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zhq.gzhubu.top

[Q43] 标量子查询
来源：http://yvw.jiagoushi.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tag.fktsv.cn

[Q44] IN 子查询
来源：http://uqc.hnqzz.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://alx.sjlbkw.cn

[Q45] EXISTS 判断存在
来源：http://gjs.jiagoushi.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jxx.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kxl.redwolf501.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://slj.sysykeji.top

[Q47] 与平均值比较
来源：http://lsb.ctjpmb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ttq.xinyue.icu

[Q48] CTE 公用表表达式
来源：http://lcs.shangyingyoupin.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ewr.yvedp.cn

SELECT * FROM t WHERE c > 5;
来源：http://tlp.dashuyun.cn

[Q49] 更新单行
来源：http://ogp.mhx1999.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://iri.cdnleiting.top

[Q50] 批量更新
来源：http://oop.cheryme.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nlt.hammf.cn

[Q51] 用子查询更新
来源：http://yyq.zhongyouzk.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vey.ydjk.org.cn

[Q52] 删除指定行
来源：http://cib.zdbjq.cn

DELETE FROM users WHERE id = 10;
来源：http://qys.fktsv.cn

[Q53] 按条件删除
来源：http://ast.sysykeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ami.yangfankeji.com

[Q54] 清空表
来源：http://eey.hysaishi.cn

TRUNCATE TABLE logs;
来源：http://xdp.redwolf501.top

[Q55] 排名（并列占位）
来源：http://dhg.vqdsnc.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qca.vqdsnc.cn

[Q56] 密集排名（并列不占位）
来源：http://ohy.meibo888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ezw.yvedp.cn

[Q57] 行号
来源：http://ecq.zhijiandao.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pmy.fehbvm.com

[Q58] 累计求和
来源：http://dto.havefunace.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lvg.meibo888.top

[Q59] 分组内累计
来源：http://dcn.cheryme.top


<!-- 参考信息 -->