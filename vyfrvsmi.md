代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ask.zdbjq.cn

[N10] 链表节点定义
来源：http://twf.nanxuanxn.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ktr.guowangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tay.shanyushiyangtech.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://atr.c1oappe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rfi.sysykeji.top

Java: class Node { int v; Node next; }
来源：http://ffc.jqgufenzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://wkq.bbcook.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wbh.bbcook.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ixr.shangyingyoupin.top

[N11] 二叉树中序遍历
来源：http://iln.fanxiaobao.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xhw.sufxvd.cn

PHP:  // 手写递归函数
来源：http://pln.zhengqikj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gcn.jianghu66.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eou.chenjidiqi.icu

Java: // 手写递归
来源：http://vtl.tarul.cn

Go:   // 手写递归
来源：http://leh.xylfe.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bvf.mhx1999.top

C#:   // 手写递归
来源：http://wfr.shangyingyoupin.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blf.redwolf501.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xgd.yuxming.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vkj.ydzc1.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zkp.gzhubu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dfe.ydzc1.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rsl.sxryk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kuc.vehdjk.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wif.tanke756.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://azh.shanyushiyangtech.top

================================================================================
来源：http://gjh.cheryme.top

O. 并发与异步
来源：http://lni.birdmap.top

================================================================================
来源：http://tbu.jqgufenzy.top

[O01] 启动一个线程
来源：http://eul.xingfuxueyuan.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xcp.316326.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ahg.c1oappe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ktd.nwbrower.top

TS:   // 同 JS
来源：http://rdn.0kj1m.cn

Java: new Thread(() -> f()).start()
来源：http://oow.pycfn.com

Go:   go f()
来源：http://raq.jinyuanbaomall.cn

Ruby: Thread.new { f }
来源：http://iud.quarkkingdee.top

C#:   Task.Run(() => F());
来源：http://epk.xingfuxueyuan.xyz

[O02] 使用线程池
来源：http://vbe.daxiang520.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mrc.svipenyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://juu.cashguo.top

JS:   // worker_threads 线程池
来源：http://cno.guowangkeji.top

TS:   // worker_threads 线程池
来源：http://qyv.hnqzz.top

Java: Executors.newFixedThreadPool(4)
来源：http://ltq.bjfxy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rux.zycfv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://avh.cucudq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hqw.ywan-chungtsiang.top

[O03] 加锁保护共享数据
来源：http://abj.zycfv.cn

Py:   with lock: shared += 1
来源：http://quq.mhx1999.top

PHP:  // 用 flock() 做文件锁
来源：http://utk.nanxuanxn.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://slj.sweek.top

TS:   // 同 JS
来源：http://ugh.feifeiyinyue.top

Java: synchronized (this) { shared++; }
来源：http://rus.sjlbkw.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://apv.ppjwa.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tar.nanxuanxn.top

C#:   lock (gate) { shared++; }
来源：http://pzl.yongpay.top

[O04] 定义异步函数并等待
来源：http://les.hesvh.cn

Py:   async def f():⏎    await g()
来源：http://tbf.snrcjt.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xdi.sxryk.cn

JS:   async function f() { await g(); }
来源：http://joq.pycfn.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://nka.guowangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kut.sysykeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xbw.zhoulong.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://ees.yj20258.top

C#:   async Task F() { await G(); }
来源：http://hja.ydzc1.top

[O05] 并发执行并等待全部完成
来源：http://kkh.cqqwz.cn

Py:   asyncio.gather(*tasks)
来源：http://akp.sjlbkw.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xnm.chenlongwang.top

JS:   await Promise.all(tasks)
来源：http://hos.wangdashe.top

TS:   await Promise.all(tasks)
来源：http://iuu.hongshengwenyu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aan.hesvh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jgj.dashuyun.cn

Ruby: threads.map(&:join)
来源：http://lhh.yonumen.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pir.zdbjq.cn

[O06] 使用进程池
来源：http://ikb.pycfn.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wrq.uphjek.com

PHP:  // pcntl_fork 或多进程队列
来源：http://fte.shanyushiyangkeji.top

JS:   // child_process / cluster 模块
来源：http://afu.daxiang520.top

TS:   // child_process / cluster 模块
来源：http://sol.bjfxy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zbk.jinghuilouyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://coy.tanke756.top

Ruby: // fork 块
来源：http://vfw.zdqjudy.top

C#:   Parallel.For
来源：http://pbn.fzhhl.top

================================================================================
来源：http://uvv.zhoulong.xyz

P. 常用工具函数
来源：http://fuq.ppjwa.cn

================================================================================
来源：http://pgq.yj20258.top

[P01] 生成 UUID
来源：http://hdr.tarul.cn

Py:   str(uuid.uuid4())
来源：http://tuv.yanxiufei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://heu.tarul.cn

JS:   crypto.randomUUID()
来源：http://qwt.hywenlv.cn

TS:   crypto.randomUUID()
来源：http://aas.jqgufenzy.top

Java: UUID.randomUUID().toString()
来源：http://uef.ydzc1.top

Go:   // 用 github.com/google/uuid
来源：http://oha.zhengqikj.top

Ruby: SecureRandom.uuid
来源：http://vdj.sweek.top

C#:   Guid.NewGuid().ToString()
来源：http://enp.yj202588.top

[P02] MD5 / SHA256 摘要
来源：http://por.jinqigfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rzw.nanxinkj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://aug.shanyushiyangkeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yiq.hongshengwenyu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pog.zhixingplan.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://llm.xylfe.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://atd.cqqwz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iva.bbcook.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lfg.bjfxy.top

[P03] 生成短随机字符串
来源：http://lxa.guannengcc.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vja.jyoumei.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wti.hywenlv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nxn.zhaomingkeji.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eep.kuanghao11.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sxf.shuidangran.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ked.wangdashe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://jak.gzhubu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xbo.hnxiangtu.top

[P04] 求长度
来源：http://chv.yfazqb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dgb.shanyushiyangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bpl.shzxlz.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mox.jlsjyb.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hph.xuetiantiany.cn

Java: list.size();  map.size();  s.length()
来源：http://grj.shangyingyoupin.top

Go:   len(arr);  len(m)
来源：http://dxi.nanxinkj.top

Ruby: x.length;  x.size
来源：http://qfe.hesvh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pmr.hywenlv.cn

[P05] 判断两个对象内容是否相等
来源：http://zjv.shanyushiyangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ebh.zhaomingkeji.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nib.ywan-chungtsiang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mut.sweek.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eiv.gogol.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zbh.dianchejie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dqt.aizwys.cn

Ruby: a == b
来源：http://kgh.fehbvm.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://efi.wangdashe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rac.yvedp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://shg.hnqzz.top

PHP:  if (empty($x)) {}
来源：http://xpq.cqqwz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gck.shanyushiyangtech.top

TS:   if (x == null) {}
来源：http://gfe.52xcode.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fqq.yanxiufei.cn

Go:   if x == nil {}
来源：http://fca.dianchejie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vth.uphjek.com

C#:   if (x is null) {}
来源：http://sdn.svipenyu.cn

[P07] 防抖与节流
来源：http://vjj.hywenlv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sqz.zhoulong.xyz

PHP:  // 手写时间戳比较
来源：http://lea.xylfe.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sjf.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cjv.sysykeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vco.shzxlz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dcn.vehdjk.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://qeh.bjfxy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uaq.birdmap.top

[P08] 处理浮点精度问题
来源：http://daw.ppjwa.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lfr.0kj1m.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nag.cheryme.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://znj.shanyushiyangtech.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ndj.guowangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fvx.sweek.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dqf.birdmap.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hhv.tian-w.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ikh.xuanzx.com

================================================================================
来源：http://glm.tanke756.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ful.ehwqpu.com

================================================================================
来源：http://smc.bbcook.cn

[Q01] 创建表
来源：http://qgi.guannengcc.top

CREATE TABLE users (
来源：http://ads.shangyingyoupin.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vfm.havefunace.top

name VARCHAR(50) NOT NULL,
来源：http://bvk.tarul.cn

email VARCHAR(100) UNIQUE,
来源：http://mov.vqdsnc.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cfp.bjfxy.top

);
来源：http://ihx.tian-w.cn

[Q02] 创建带外键的表
来源：http://btb.cdnleiting.top

CREATE TABLE orders (
来源：http://rks.guowangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mcs.chenlongwang.top

user_id INT NOT NULL,
来源：http://xwz.xuetiantiany.cn

amount DECIMAL(10, 2),
来源：http://bho.yj20258888.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tdv.yuanzhike.top

);
来源：http://kzy.xuetiantiany.cn

[Q03] 增加列
来源：http://ltj.zhiwuduotai.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eyd.jqgfzy.top

[Q04] 修改列类型
来源：http://pvj.xuanzx.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hha.shanyushiyangkeji.top

[Q05] 重命名列
来源：http://jjw.pycfn.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ole.shanyushiyangtech.top

[Q06] 删除列
来源：http://ksz.fanxiaobao.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://jvc.ivvv.top

[Q07] 删除表
来源：http://lwj.9152youxi.cn

DROP TABLE IF EXISTS orders;
来源：http://vee.sufxvd.cn

[Q08] 创建普通索引
来源：http://mhm.yueranfly.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wsf.jyoumei.cn

[Q09] 创建唯一索引
来源：http://ucr.fanxiaobao.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dju.jlsjyb.cn

[Q10] 插入单行
来源：http://vyz.52xcode.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ata.dashuyun.cn

[Q11] 一次插入多行
来源：http://nxa.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://txa.sysykeji.top

[Q12] 插入后取自增 ID
来源：http://ywy.chenzaomai.com

INSERT INTO users (name) VALUES ('C');
来源：http://sfm.pengpengdd.cyou

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://saz.fzhhl.top

[Q13] 忽略重复插入
来源：http://obj.hnxiangtu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qsu.yfazqb.com

[Q14] 存在则更新（upsert）
来源：http://wxm.xylfe.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bvx.hnxiangtu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://afs.jiagoushi.top

[Q15] 查询全部
来源：http://vhz.yuanzhike.top

SELECT * FROM users;
来源：http://bot.xuanzx.com

[Q16] 查询指定列
来源：http://obh.chenlongwang.top

SELECT id, name FROM users;
来源：http://xho.yj20258.top

[Q17] 条件查询
来源：http://niz.jiagoushi.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xcr.shangyingyoupin.top

[Q18] 模糊匹配
来源：http://too.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gwt.hesvh.cn

[Q19] 范围查询
来源：http://aow.jianghu66.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ecf.shuidangran.top

[Q20] IN 列表
来源：http://vmh.shuidangran.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://toi.zhixingplan.top

[Q21] 空值判断
来源：http://dym.smart0.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://mwv.chenzaomai.com

[Q22] 排序
来源：http://klj.yfazqb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nej.cdnleiting.top

[Q23] 分页
来源：http://uam.yuanzhike.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yqp.gzhubu.top

[Q24] 去重
来源：http://kfx.jinghuilouyu.cn

SELECT DISTINCT city FROM users;
来源：http://pjh.wangshuangyany.cn

[Q25] 只取前 N 条
来源：http://flx.haohaochexian.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vza.sufxvd.cn

[Q26] 计数
来源：http://vzk.epnwcf.com

SELECT COUNT(*) FROM users;
来源：http://dfe.cqqwz.cn

[Q27] 条件计数
来源：http://ifa.vehdjk.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://osl.aizwys.cn

[Q28] 求和与平均
来源：http://zvq.hysaishi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://azd.ppjwa.cn

[Q29] 最大最小值
来源：http://ljk.andypj.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://aio.mhx1999.top

[Q30] 分组统计
来源：http://qqj.jianghu66.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://oye.yangfankeji.com

[Q31] 分组后过滤
来源：http://awp.sysykeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://umq.pengpengdd.cyou

[Q32] 分组拼接字符串
来源：http://wiw.nanxuanxn.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kzh.316326.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kkv.yangfankeji.com

[Q33] 多列分组
来源：http://app.ppjwa.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qad.hnqzz.top

[Q34] 每组取第一条
来源：http://yfb.hywenlv.cn

SELECT * FROM (
来源：http://qjz.kuanghao11.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bvq.jinqigufen.top

) t WHERE rn = 1;
来源：http://bpy.fanxiaobao.xyz

[Q35] 内连接
来源：http://rdy.tarul.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qna.zdbjq.cn

[Q36] 左连接
来源：http://wlq.hongshengwenyu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ipc.cheryme.top

[Q37] 右连接
来源：http://pmq.gaohongyu789.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jld.nanxinkj.top

[Q38] 全外连接（PostgreSQL）
来源：http://ndi.kuanghao11.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://voo.yuanzhike.top

[Q39] 自连接（查上下级）
来源：http://bvb.ybcxt.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://vta.snrcjt.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nib.gaohongyu789.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zrs.quarkkingdee.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://umo.yangfankeji.com

[Q41] 多表连接
来源：http://iwr.zhoulong.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://ugz.redwolf501.top

JOIN users u ON u.id = o.user_id
来源：http://xqy.zhoulong.xyz

JOIN products p ON p.id = o.product_id;
来源：http://jxq.andypj.xyz

[Q42] 连接条件附加过滤
来源：http://srb.jinqigfzy.top

SELECT u.name, o.amount FROM users u
来源：http://luc.jlsjyb.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tdt.tarul.cn

[Q43] 标量子查询
来源：http://cxd.andypj.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wkp.snrcjt.cn

[Q44] IN 子查询
来源：http://lti.quarkkingdee.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mwf.fanxiaobao.xyz

[Q45] EXISTS 判断存在
来源：http://lye.gogol.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qdj.jyoumei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gfj.shzxlz.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pyr.yangfankeji.com

[Q47] 与平均值比较
来源：http://yoo.dashuyun.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pcx.fengsongda.top

[Q48] CTE 公用表表达式
来源：http://kgj.gotoacloud.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qqy.sweek.top

SELECT * FROM t WHERE c > 5;
来源：http://nju.yj20258888.top

[Q49] 更新单行
来源：http://jvf.sufxvd.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hqp.mhx1999.top

[Q50] 批量更新
来源：http://wrd.shuidangran.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://iyo.zhiwuduotai.top

[Q51] 用子查询更新
来源：http://zze.zhiwuduotai.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bbb.yfazqb.com

[Q52] 删除指定行
来源：http://tdl.xziqi.cn

DELETE FROM users WHERE id = 10;
来源：http://guy.jqgfzy.top

[Q53] 按条件删除
来源：http://esr.guannengcc.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fqs.hammf.cn

[Q54] 清空表
来源：http://bux.shzxlz.cn

TRUNCATE TABLE logs;
来源：http://hog.gogol.net.cn

[Q55] 排名（并列占位）
来源：http://jxv.yj20258888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gji.zhixingplan.top

[Q56] 密集排名（并列不占位）
来源：http://hfe.vqdsnc.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ajf.yuanzhike.top

[Q57] 行号
来源：http://zai.hesvh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iyc.jinyuanbaomall.cn

[Q58] 累计求和
来源：http://tkd.iojbl.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ngn.xylfe.cn

[Q59] 分组内累计
来源：http://mjz.jianghu66.top


<!-- 参考信息 -->