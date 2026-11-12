代发 wailian999

[N09] 栈与队列
来源：http://uvj.fengsongda.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qmd.fengsongda.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://auv.9152youxi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://skk.nwbrower.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xow.zhijiandao.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://odh.fanxiaobao.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hqj.sjlbkw.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hvj.yvedp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jia.fehbvm.com

[N10] 链表节点定义
来源：http://kyg.xingfuxueyuan.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yup.feifeiyinyue.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dtn.0kj1m.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gsr.sjlbkw.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kly.zdbjq.cn

Java: class Node { int v; Node next; }
来源：http://obo.mhx1999.top

Go:   type Node struct { V int; Next *Node }
来源：http://uzf.dianchejie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://han.nwbrower.top

C#:   class Node { public int V; public Node? Next; }
来源：http://cxn.dashuyun.cn

[N11] 二叉树中序遍历
来源：http://cvk.feifeiyinyue.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ndu.9152youxi.cn

PHP:  // 手写递归函数
来源：http://bjo.yvedp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bcl.jyoumei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kha.ivvv.top

Java: // 手写递归
来源：http://ptl.yfazqb.com

Go:   // 手写递归
来源：http://jiz.hywenlv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rlh.sxryk.cn

C#:   // 手写递归
来源：http://mlz.fanxiaobao.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ovq.c1oappe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wxm.cashguo.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wxq.hammf.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://azk.ywan-chungtsiang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sjt.hywenlv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://voe.ydzc1.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sga.hfpthk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://agj.meibo888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bdq.zdbjq.cn

================================================================================
来源：http://zlc.xylfe.cn

O. 并发与异步
来源：http://vky.smart0.xyz

================================================================================
来源：http://ubz.zhengqikj.top

[O01] 启动一个线程
来源：http://uob.zhoulong.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wiv.yanxiufei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qcs.zdbjq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ybj.svipenyu.cn

TS:   // 同 JS
来源：http://eym.yonumen.top

Java: new Thread(() -> f()).start()
来源：http://bra.jianghu66.top

Go:   go f()
来源：http://hzx.daxiang520.top

Ruby: Thread.new { f }
来源：http://hff.sufxvd.cn

C#:   Task.Run(() => F());
来源：http://den.redwolf501.top

[O02] 使用线程池
来源：http://dkn.jinqigufen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sjw.yuxming.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lun.fehbvm.com

JS:   // worker_threads 线程池
来源：http://ypc.dashuyun.cn

TS:   // worker_threads 线程池
来源：http://wkc.nanxinkj.top

Java: Executors.newFixedThreadPool(4)
来源：http://trx.jqgfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vjx.jianghu66.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zlx.uphjek.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zfy.sxryk.cn

[O03] 加锁保护共享数据
来源：http://trr.ydjk.org.cn

Py:   with lock: shared += 1
来源：http://rre.52xcode.cn

PHP:  // 用 flock() 做文件锁
来源：http://cel.redwolf501.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ogg.yongpay.top

TS:   // 同 JS
来源：http://dtv.ivvv.top

Java: synchronized (this) { shared++; }
来源：http://ghf.hongshengwenyu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ekl.iojbl.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mjy.jiagoushi.top

C#:   lock (gate) { shared++; }
来源：http://evs.yueranfly.top

[O04] 定义异步函数并等待
来源：http://fcx.yj20258888.top

Py:   async def f():⏎    await g()
来源：http://sqr.c1oappe.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wlt.tian-w.cn

JS:   async function f() { await g(); }
来源：http://dgq.aizwys.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jdq.hnxiangtu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cew.yuxming.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pii.zhengqikj.top

Ruby: # 用 Fiber 或 async gem
来源：http://yyf.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://rzi.jinqigfzy.top

[O05] 并发执行并等待全部完成
来源：http://vur.shzxlz.cn

Py:   asyncio.gather(*tasks)
来源：http://kcj.mhx1999.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oky.xingfuxueyuan.xyz

JS:   await Promise.all(tasks)
来源：http://sfc.chenjidiqi.icu

TS:   await Promise.all(tasks)
来源：http://dba.yueranfly.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://apc.gzhubu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qpi.guannengcc.top

Ruby: threads.map(&:join)
来源：http://coi.tarul.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lkf.ydzc1.top

[O06] 使用进程池
来源：http://vui.fengsongda.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rex.ybcxt.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mgc.hysaishi.cn

JS:   // child_process / cluster 模块
来源：http://bcr.sweek.top

TS:   // child_process / cluster 模块
来源：http://ccm.zhoulong.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ikm.xylfe.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wzs.cucudq.cn

Ruby: // fork 块
来源：http://ilv.xziqi.cn

C#:   Parallel.For
来源：http://irt.ywan-chungtsiang.top

================================================================================
来源：http://rfi.yj202588.top

P. 常用工具函数
来源：http://euf.gzhubu.top

================================================================================
来源：http://qqs.ehwqpu.com

[P01] 生成 UUID
来源：http://fqa.yuxming.cn

Py:   str(uuid.uuid4())
来源：http://gfi.yuanzhike.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://akf.zhaomingkeji.xyz

JS:   crypto.randomUUID()
来源：http://zof.yonumen.top

TS:   crypto.randomUUID()
来源：http://zvf.dashuyun.cn

Java: UUID.randomUUID().toString()
来源：http://lde.ctjpmb.com

Go:   // 用 github.com/google/uuid
来源：http://rfw.sufxvd.cn

Ruby: SecureRandom.uuid
来源：http://ddx.jianghu66.top

C#:   Guid.NewGuid().ToString()
来源：http://gvu.dianchejie.cn

[P02] MD5 / SHA256 摘要
来源：http://erm.0kj1m.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gvf.gogol.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yhy.tarul.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ivm.gotoacloud.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://biq.smart0.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fkq.316326.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fzk.vehdjk.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sjr.jianghu66.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bwx.vqdsnc.cn

[P03] 生成短随机字符串
来源：http://fza.fanxiaobao.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pxr.yangfankeji.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ulr.yonumen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tsw.tianlin.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hus.ydzc1.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://svq.dashuyun.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wdj.ywan-chungtsiang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://aqv.52xcode.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pdc.cheryme.top

[P04] 求长度
来源：http://nuz.xinyue.icu

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uzp.jianghu66.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fmf.xziqi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zba.jqgfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eik.aibaodan.cn

Java: list.size();  map.size();  s.length()
来源：http://hcz.sweek.top

Go:   len(arr);  len(m)
来源：http://uvz.guannengcc.top

Ruby: x.length;  x.size
来源：http://kov.tanke756.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://iax.zhaomingkeji.xyz

[P05] 判断两个对象内容是否相等
来源：http://ota.fengsongda.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gso.birdmap.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://com.quarkkingdee.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mov.fanxiaobao.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sxp.bjfxy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qmr.snrcjt.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tck.nanxinkj.top

Ruby: a == b
来源：http://fpw.zycfv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lde.cashguo.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wzu.hnxiangtu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://odl.sysykeji.top

PHP:  if (empty($x)) {}
来源：http://emm.sufxvd.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ixd.tianlin.xyz

TS:   if (x == null) {}
来源：http://guy.tarul.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rko.yuanzhike.top

Go:   if x == nil {}
来源：http://vpo.316326.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sor.jyoumei.cn

C#:   if (x is null) {}
来源：http://dch.aibaodan.cn

[P07] 防抖与节流
来源：http://qoh.jyoumei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tgz.bbcook.cn

PHP:  // 手写时间戳比较
来源：http://qtr.tian-w.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tzv.yj20258888.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vyv.redwolf501.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://edm.sweek.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sri.xinyue.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://bza.jqgfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ige.xziqi.cn

[P08] 处理浮点精度问题
来源：http://sfx.cucudq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://scc.vqdsnc.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://noz.hysaishi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://olp.jinghuilouyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aru.jinqigufen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uxl.gzhubu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pdj.hnqzz.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qpq.sysykeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gze.fktsv.cn

================================================================================
来源：http://ddx.yfazqb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dvd.shanyushiyangkeji.top

================================================================================
来源：http://oxg.hnqzz.top

[Q01] 创建表
来源：http://nra.xuanzx.com

CREATE TABLE users (
来源：http://hno.yj20258.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pzh.meibo888.top

name VARCHAR(50) NOT NULL,
来源：http://tnh.hywenlv.cn

email VARCHAR(100) UNIQUE,
来源：http://cbq.hongshengwenyu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yee.uphjek.com

);
来源：http://dgl.hesvh.cn

[Q02] 创建带外键的表
来源：http://yan.yj20258888.top

CREATE TABLE orders (
来源：http://djj.smart0.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mnx.zhoulong.xyz

user_id INT NOT NULL,
来源：http://zyr.bjfxy.top

amount DECIMAL(10, 2),
来源：http://idj.zhixingplan.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xiy.vehdjk.com

);
来源：http://tqu.chenzaomai.com

[Q03] 增加列
来源：http://ymg.nanxinkj.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bhi.316326.xyz

[Q04] 修改列类型
来源：http://asd.epnwcf.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ksg.zhijiandao.cn

[Q05] 重命名列
来源：http://tvs.ywan-chungtsiang.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bvu.xinyue.icu

[Q06] 删除列
来源：http://bqp.daxiang520.top

ALTER TABLE users DROP COLUMN age;
来源：http://zmt.cashguo.top

[Q07] 删除表
来源：http://icy.fktsv.cn

DROP TABLE IF EXISTS orders;
来源：http://nle.ywan-chungtsiang.top

[Q08] 创建普通索引
来源：http://tif.cucudq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fiz.cqqwz.cn

[Q09] 创建唯一索引
来源：http://kxs.aizwys.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lfo.tian-w.cn

[Q10] 插入单行
来源：http://jmz.sjlbkw.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wky.havefunace.top

[Q11] 一次插入多行
来源：http://bmy.cdnleiting.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wnj.xingfuxueyuan.xyz

[Q12] 插入后取自增 ID
来源：http://xdv.sjlbkw.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cur.yuanzhike.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fia.bbcook.cn

[Q13] 忽略重复插入
来源：http://pdf.guannengcc.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://diy.dianchejie.cn

[Q14] 存在则更新（upsert）
来源：http://vic.hammf.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dit.bjfxy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://anj.xylfe.cn

[Q15] 查询全部
来源：http://sud.gogol.net.cn

SELECT * FROM users;
来源：http://qzg.sweek.top

[Q16] 查询指定列
来源：http://thk.haohaochexian.top

SELECT id, name FROM users;
来源：http://ijc.xylfe.cn

[Q17] 条件查询
来源：http://cch.kuanghao11.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dxs.snrcjt.cn

[Q18] 模糊匹配
来源：http://wxw.jyoumei.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fku.ppjwa.cn

[Q19] 范围查询
来源：http://soc.gotoacloud.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xrg.bjfxy.top

[Q20] IN 列表
来源：http://xjz.yvedp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pgx.hysaishi.cn

[Q21] 空值判断
来源：http://ogc.pengpengdd.cyou

SELECT * FROM users WHERE email IS NULL;
来源：http://los.gotoacloud.top

[Q22] 排序
来源：http://gcb.cheryme.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jls.shangyingyoupin.top

[Q23] 分页
来源：http://uwg.hesvh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dwo.haohaochexian.top

[Q24] 去重
来源：http://xrq.dianchejie.cn

SELECT DISTINCT city FROM users;
来源：http://ych.fanxiaobao.xyz

[Q25] 只取前 N 条
来源：http://ozp.wangdashe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nmm.hcnkem.com

[Q26] 计数
来源：http://hjt.feifeiyinyue.top

SELECT COUNT(*) FROM users;
来源：http://ayt.xuetiantiany.cn

[Q27] 条件计数
来源：http://rwi.yonumen.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xgv.xylfe.cn

[Q28] 求和与平均
来源：http://hbb.cqqwz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://atc.zycfv.cn

[Q29] 最大最小值
来源：http://bhe.zhaomingkeji.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://psq.tianlin.xyz

[Q30] 分组统计
来源：http://xwn.fehbvm.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fwt.guannengcc.top

[Q31] 分组后过滤
来源：http://yus.jinqigufen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://khf.wangshuangyany.cn

[Q32] 分组拼接字符串
来源：http://hpq.jinqigufen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://edc.chenlongwang.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ltx.smart0.xyz

[Q33] 多列分组
来源：http://imh.9152youxi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bpf.hfpthk.cn

[Q34] 每组取第一条
来源：http://dle.tanke756.top

SELECT * FROM (
来源：http://pmj.xylfe.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vlw.yangfankeji.com

) t WHERE rn = 1;
来源：http://zfv.zhijiandao.cn

[Q35] 内连接
来源：http://fay.zdbjq.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://equ.jianghu66.top

[Q36] 左连接
来源：http://wew.feifeiyinyue.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://umo.hesvh.cn

[Q37] 右连接
来源：http://qwf.zdqjudy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://coi.andypj.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://vlz.gaohongyu789.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bbr.havefunace.top

[Q39] 自连接（查上下级）
来源：http://nxh.bbcook.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://azd.jyoumei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://agm.meibo888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://eni.xziqi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://acx.ppjwa.cn

[Q41] 多表连接
来源：http://hnw.hnqzz.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://eei.shzxlz.cn

JOIN users u ON u.id = o.user_id
来源：http://vho.xingfuxueyuan.xyz

JOIN products p ON p.id = o.product_id;
来源：http://ysw.yonumen.top

[Q42] 连接条件附加过滤
来源：http://wdm.gaohongyu789.top

SELECT u.name, o.amount FROM users u
来源：http://ivg.svipenyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jdm.hnqzz.top

[Q43] 标量子查询
来源：http://iwu.sjlbkw.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ywt.ivvv.top

[Q44] IN 子查询
来源：http://pxz.xylfe.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://okr.aibaodan.cn

[Q45] EXISTS 判断存在
来源：http://uyc.ydjk.org.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eub.hesvh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xdj.chenlongwang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gff.xingfuxueyuan.xyz

[Q47] 与平均值比较
来源：http://tnv.gaohongyu789.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mlt.zhongyouzk.top

[Q48] CTE 公用表表达式
来源：http://xuo.cdnleiting.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hsf.yanxiufei.cn

SELECT * FROM t WHERE c > 5;
来源：http://mia.ydjk.org.cn

[Q49] 更新单行
来源：http://ver.bjfxy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://adx.sufxvd.cn

[Q50] 批量更新
来源：http://tuu.iojbl.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tph.yangfankeji.com

[Q51] 用子查询更新
来源：http://fhu.hesvh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yci.fengsongda.top

[Q52] 删除指定行
来源：http://kmm.zdbjq.cn

DELETE FROM users WHERE id = 10;
来源：http://jmj.haohaochexian.top

[Q53] 按条件删除
来源：http://ssf.yueranfly.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://poi.ppjwa.cn

[Q54] 清空表
来源：http://lxx.ppjwa.cn

TRUNCATE TABLE logs;
来源：http://sqb.gzhubu.top

[Q55] 排名（并列占位）
来源：http://sfo.guowangkeji.top


<!-- 参考信息 -->