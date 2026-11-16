代发 wailian999

Java: // 手写回溯递归
来源：http://bhm.nanxinkj.top

Go:   // 手写回溯递归
来源：http://ers.jinqigfzy.top

Ruby: arr.permutation.to_a
来源：http://ooi.pycfn.com

C#:   // 手写回溯递归
来源：http://lmd.cheryme.top

[N09] 栈与队列
来源：http://byp.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sti.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fnp.shangyingyoupin.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hhr.dianchejie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ejd.zhixingplan.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lza.yvedp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oys.cashguo.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rrf.havefunace.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uyh.jiagoushi.top

[N10] 链表节点定义
来源：http://fyt.birdmap.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pst.sjlbkw.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qmp.jiagoushi.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bmo.fktsv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fyr.kuanghao11.cn

Java: class Node { int v; Node next; }
来源：http://mok.yj20258888.top

Go:   type Node struct { V int; Next *Node }
来源：http://pyd.guannengcc.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vbo.tanke756.top

C#:   class Node { public int V; public Node? Next; }
来源：http://adi.fengsongda.top

[N11] 二叉树中序遍历
来源：http://pvj.quarkkingdee.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eiy.ppjwa.cn

PHP:  // 手写递归函数
来源：http://azs.iojbl.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oyn.yonumen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nem.9152youxi.cn

Java: // 手写递归
来源：http://sij.zycfv.cn

Go:   // 手写递归
来源：http://voq.havefunace.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jws.jiagoushi.top

C#:   // 手写递归
来源：http://fml.ppjwa.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xke.yuxming.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://slg.guannengcc.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ryk.yangfankeji.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baf.fengsongda.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gmc.sjlbkw.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mlt.shzxlz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gwp.chenlongwang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sqa.fktsv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://clu.nanxuanxn.top

================================================================================
来源：http://eng.cheryme.top

O. 并发与异步
来源：http://wkc.wangdashe.top

================================================================================
来源：http://cni.gzhubu.top

[O01] 启动一个线程
来源：http://mco.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wte.zhiwuduotai.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://spj.tian-w.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xbd.chenlongwang.top

TS:   // 同 JS
来源：http://ijx.meibo888.top

Java: new Thread(() -> f()).start()
来源：http://kxj.havefunace.top

Go:   go f()
来源：http://lfb.shzxlz.cn

Ruby: Thread.new { f }
来源：http://tii.dashuyun.cn

C#:   Task.Run(() => F());
来源：http://gpc.cqqwz.cn

[O02] 使用线程池
来源：http://coi.sweek.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yhk.ctjpmb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ymx.dashuyun.cn

JS:   // worker_threads 线程池
来源：http://keo.wangshuangyany.cn

TS:   // worker_threads 线程池
来源：http://uas.uphjek.com

Java: Executors.newFixedThreadPool(4)
来源：http://wks.bbcook.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hvb.zhengqikj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gom.tianlin.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oky.xuetiantiany.cn

[O03] 加锁保护共享数据
来源：http://hfx.chenlongwang.top

Py:   with lock: shared += 1
来源：http://hrk.uphjek.com

PHP:  // 用 flock() 做文件锁
来源：http://qbl.vehdjk.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hwh.haohaochexian.top

TS:   // 同 JS
来源：http://uap.hesvh.cn

Java: synchronized (this) { shared++; }
来源：http://oqi.jinqigfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wra.birdmap.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qxb.snrcjt.cn

C#:   lock (gate) { shared++; }
来源：http://psv.ctjpmb.com

[O04] 定义异步函数并等待
来源：http://dwt.daria6918.cn

Py:   async def f():⏎    await g()
来源：http://vde.snrcjt.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cpe.xinyue.icu

JS:   async function f() { await g(); }
来源：http://nag.feifeiyinyue.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ajg.zhiwuduotai.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mcp.meibo888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jex.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://pos.jlsjyb.cn

C#:   async Task F() { await G(); }
来源：http://tlx.cqqwz.cn

[O05] 并发执行并等待全部完成
来源：http://vyz.epnwcf.com

Py:   asyncio.gather(*tasks)
来源：http://trl.shangyingyoupin.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sjb.zdqjudy.top

JS:   await Promise.all(tasks)
来源：http://nfq.smart0.xyz

TS:   await Promise.all(tasks)
来源：http://bzp.smart0.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://itm.zhaomingkeji.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zlr.chenjidiqi.icu

Ruby: threads.map(&:join)
来源：http://vin.jyoumei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ztw.uphjek.com

[O06] 使用进程池
来源：http://bkb.hnqzz.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fod.shangyingyoupin.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mzo.meibo888.top

JS:   // child_process / cluster 模块
来源：http://nws.zhiwuduotai.top

TS:   // child_process / cluster 模块
来源：http://slv.dianchejie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rkr.jinqigufen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rzd.smart0.xyz

Ruby: // fork 块
来源：http://ewx.9152youxi.cn

C#:   Parallel.For
来源：http://guh.jiagoushi.top

================================================================================
来源：http://jvz.svipenyu.cn

P. 常用工具函数
来源：http://uyj.sjlbkw.cn

================================================================================
来源：http://vnm.cashguo.top

[P01] 生成 UUID
来源：http://yux.birdmap.top

Py:   str(uuid.uuid4())
来源：http://dsi.hammf.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://aig.yfazqb.com

JS:   crypto.randomUUID()
来源：http://gpj.hcnkem.com

TS:   crypto.randomUUID()
来源：http://qyl.gogol.net.cn

Java: UUID.randomUUID().toString()
来源：http://opj.yuanzhike.top

Go:   // 用 github.com/google/uuid
来源：http://dwc.epnwcf.com

Ruby: SecureRandom.uuid
来源：http://mfe.yongpay.top

C#:   Guid.NewGuid().ToString()
来源：http://yet.xuetiantiany.cn

[P02] MD5 / SHA256 摘要
来源：http://oke.jyoumei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lae.xziqi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zni.gogol.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vjj.xziqi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vcb.yongpay.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cuz.zhoulong.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uag.jqgufenzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cwi.tanke756.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yig.yuanzhike.top

[P03] 生成短随机字符串
来源：http://csv.snrcjt.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oqs.kuanghao11.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oiz.vehdjk.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hgn.fehbvm.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ihi.hammf.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qhh.sjlbkw.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jit.jinqigufen.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://qpm.0kj1m.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://clm.hysaishi.cn

[P04] 求长度
来源：http://ijy.wangdashe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sik.chenzaomai.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ikz.ehwqpu.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dnc.c1oappe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pfs.vqdsnc.cn

Java: list.size();  map.size();  s.length()
来源：http://kjv.tarul.cn

Go:   len(arr);  len(m)
来源：http://qet.yuanzhike.top

Ruby: x.length;  x.size
来源：http://xve.hfpthk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mws.vqdsnc.cn

[P05] 判断两个对象内容是否相等
来源：http://nkl.fanxiaobao.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://qto.fanxiaobao.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dwp.chenjidiqi.icu

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hii.jianghu66.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mfw.quarkkingdee.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zmw.yanxiufei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gsj.ywan-chungtsiang.top

Ruby: a == b
来源：http://jud.jyoumei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://klx.jyoumei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dcb.yuanzhike.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bzs.gzhubu.top

PHP:  if (empty($x)) {}
来源：http://drk.0kj1m.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kwz.ppjwa.cn

TS:   if (x == null) {}
来源：http://cdz.yuanzhike.top

Java: if (x == null || x.isEmpty()) {}
来源：http://nmw.epnwcf.com

Go:   if x == nil {}
来源：http://mdk.jqgfzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rjq.aizwys.cn

C#:   if (x is null) {}
来源：http://scy.yongpay.top

[P07] 防抖与节流
来源：http://uzj.daxiang520.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ctf.ywan-chungtsiang.top

PHP:  // 手写时间戳比较
来源：http://lzx.xingfuxueyuan.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cgg.chenlongwang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gfj.zhengqikj.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xpx.316326.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tbm.sxryk.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://uzp.pengpengdd.cyou

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nkb.bjfxy.top

[P08] 处理浮点精度问题
来源：http://cmq.hammf.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bme.zhijiandao.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pus.gotoacloud.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pmk.xinyue.icu

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wlu.hammf.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://icq.ctjpmb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mmg.zhijiandao.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rbw.xuetiantiany.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fxw.xziqi.cn

================================================================================
来源：http://mlp.sxryk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pji.shzxlz.cn

================================================================================
来源：http://bye.yanxiufei.cn

[Q01] 创建表
来源：http://jka.c1oappe.top

CREATE TABLE users (
来源：http://qlw.dashuyun.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ouw.sjlbkw.cn

name VARCHAR(50) NOT NULL,
来源：http://rce.jyoumei.cn

email VARCHAR(100) UNIQUE,
来源：http://mqm.jinqigufen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ofg.shuidangran.top

);
来源：http://fzr.birdmap.top

[Q02] 创建带外键的表
来源：http://svx.tarul.cn

CREATE TABLE orders (
来源：http://pfd.sufxvd.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uzd.yuanzhike.top

user_id INT NOT NULL,
来源：http://net.xuanzx.com

amount DECIMAL(10, 2),
来源：http://wvi.jianghu66.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://una.zdqjudy.top

);
来源：http://tlv.gotoacloud.top

[Q03] 增加列
来源：http://glr.chenlongwang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pdm.gogol.net.cn

[Q04] 修改列类型
来源：http://xuc.jianghu66.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fjz.shuidangran.top

[Q05] 重命名列
来源：http://ehk.nanxinkj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ukb.sjlbkw.cn

[Q06] 删除列
来源：http://euk.ppjwa.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ltk.mhx1999.top

[Q07] 删除表
来源：http://smg.shuidangran.top

DROP TABLE IF EXISTS orders;
来源：http://uqj.ydjk.org.cn

[Q08] 创建普通索引
来源：http://jsk.jianghu66.top

CREATE INDEX idx_users_email ON users(email);
来源：http://csa.zhoulong.xyz

[Q09] 创建唯一索引
来源：http://bld.fzhhl.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wfw.cashguo.top

[Q10] 插入单行
来源：http://opv.cdnleiting.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lbo.316326.xyz

[Q11] 一次插入多行
来源：http://mpq.chenlongwang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rwg.hongshengwenyu.top

[Q12] 插入后取自增 ID
来源：http://yiz.hysaishi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hoo.chenzaomai.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gha.ivvv.top

[Q13] 忽略重复插入
来源：http://mwd.vehdjk.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ocv.gzhubu.top

[Q14] 存在则更新（upsert）
来源：http://vat.yfazqb.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://izh.ybcxt.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dep.snrcjt.cn

[Q15] 查询全部
来源：http://xit.yuxming.cn

SELECT * FROM users;
来源：http://xgs.zdbjq.cn

[Q16] 查询指定列
来源：http://dyl.snrcjt.cn

SELECT id, name FROM users;
来源：http://dxt.fktsv.cn

[Q17] 条件查询
来源：http://amj.mhx1999.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://msv.nwbrower.top

[Q18] 模糊匹配
来源：http://rpb.52xcode.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mjp.cheryme.top

[Q19] 范围查询
来源：http://jwo.guannengcc.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bnx.yanxiufei.cn

[Q20] IN 列表
来源：http://exh.cashguo.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dlq.xylfe.cn

[Q21] 空值判断
来源：http://aoe.shanyushiyangtech.top

SELECT * FROM users WHERE email IS NULL;
来源：http://cyu.pengpengdd.cyou

[Q22] 排序
来源：http://kaj.ywan-chungtsiang.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kqt.ywan-chungtsiang.top

[Q23] 分页
来源：http://oqv.bjfxy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pzy.jinqigfzy.top

[Q24] 去重
来源：http://jad.xziqi.cn

SELECT DISTINCT city FROM users;
来源：http://nuw.ybcxt.top

[Q25] 只取前 N 条
来源：http://ypi.ybcxt.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://evb.sufxvd.cn

[Q26] 计数
来源：http://pyt.hfpthk.cn

SELECT COUNT(*) FROM users;
来源：http://inx.tian-w.cn

[Q27] 条件计数
来源：http://xfv.shangyingyoupin.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://etu.yanxiufei.cn

[Q28] 求和与平均
来源：http://afi.yj20258.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qgu.zdqjudy.top

[Q29] 最大最小值
来源：http://yqp.snrcjt.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ivl.yfazqb.com

[Q30] 分组统计
来源：http://qhg.xuetiantiany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fag.sysykeji.top

[Q31] 分组后过滤
来源：http://ywj.epnwcf.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vxx.nwbrower.top

[Q32] 分组拼接字符串
来源：http://jhk.nwbrower.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wcc.chenzaomai.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vjb.nanxinkj.top

[Q33] 多列分组
来源：http://hlv.ehwqpu.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tyj.sxryk.cn

[Q34] 每组取第一条
来源：http://hqy.wangshuangyany.cn

SELECT * FROM (
来源：http://asv.pycfn.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uxx.shangyingyoupin.top

) t WHERE rn = 1;
来源：http://ygo.zycfv.cn

[Q35] 内连接
来源：http://yqv.chenzaomai.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ray.chenlongwang.top

[Q36] 左连接
来源：http://wta.tanke756.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mll.fzhhl.top

[Q37] 右连接
来源：http://gpq.fktsv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gdf.yj20258888.top

[Q38] 全外连接（PostgreSQL）
来源：http://gmn.yfazqb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mim.yongpay.top

[Q39] 自连接（查上下级）
来源：http://kdh.hammf.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gwh.ehwqpu.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ssw.yanxiufei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ria.9152youxi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jge.sysykeji.top

[Q41] 多表连接
来源：http://bxk.tianlin.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://naj.havefunace.top

JOIN users u ON u.id = o.user_id
来源：http://mpi.quarkkingdee.top

JOIN products p ON p.id = o.product_id;
来源：http://hes.tanke756.top

[Q42] 连接条件附加过滤
来源：http://tva.yueranfly.top

SELECT u.name, o.amount FROM users u
来源：http://iyd.daria6918.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ejo.smart0.xyz

[Q43] 标量子查询
来源：http://gii.ehwqpu.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://crj.svipenyu.cn

[Q44] IN 子查询
来源：http://ltd.xuanzx.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vif.zhoulong.xyz

[Q45] EXISTS 判断存在
来源：http://npl.0kj1m.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zxu.yfazqb.com

[Q46] NOT EXISTS 判断不存在
来源：http://prd.zdbjq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mla.xuanzx.com

[Q47] 与平均值比较
来源：http://tcv.chenzaomai.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kjp.cashguo.top

[Q48] CTE 公用表表达式
来源：http://tvc.0kj1m.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bxj.yueranfly.top

SELECT * FROM t WHERE c > 5;
来源：http://bez.chenzaomai.com

[Q49] 更新单行
来源：http://jgc.redwolf501.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ugd.hammf.cn

[Q50] 批量更新
来源：http://blk.zhijiandao.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oos.pycfn.com

[Q51] 用子查询更新
来源：http://yod.yonumen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dya.bjfxy.top

[Q52] 删除指定行
来源：http://zkg.zhongyouzk.top

DELETE FROM users WHERE id = 10;
来源：http://rel.gotoacloud.top

[Q53] 按条件删除
来源：http://dxb.yj20258888.top


<!-- 参考信息 -->