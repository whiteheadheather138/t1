代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://his.ywan-chungtsiang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://oxa.shanyushiyangkeji.top

TS:   // 手写 Map<string, number>
来源：http://rvj.nanxuanxn.top

Java: // 手写 HashMap
来源：http://qzg.ctjpmb.com

Go:   // 手写 map[int]int
来源：http://knx.jianghu66.top

Ruby: // 手写 Hash
来源：http://rpi.yj20258888.top

C#:   // 手写 Dictionary<int, int>
来源：http://vsx.yfazqb.com

[N08] 生成全排列
来源：http://wad.nanxuanxn.top

Py:   itertools.permutations(arr)
来源：http://dlo.52xcode.cn

PHP:  // 手写递归交换
来源：http://dhi.sweek.top

JS:   // 手写回溯递归
来源：http://iql.jianghu66.top

TS:   // 手写回溯递归
来源：http://bii.haohaochexian.top

Java: // 手写回溯递归
来源：http://jmk.ctjpmb.com

Go:   // 手写回溯递归
来源：http://erk.jlsjyb.cn

Ruby: arr.permutation.to_a
来源：http://xrc.daxiang520.top

C#:   // 手写回溯递归
来源：http://yob.sweek.top

[N09] 栈与队列
来源：http://ovf.fanxiaobao.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zhw.jinqigfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dmz.hongshengwenyu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fwj.zhongyouzk.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fid.gzhubu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oek.hnxiangtu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ckh.zhiwuduotai.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fgs.feifeiyinyue.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oqt.epnwcf.com

[N10] 链表节点定义
来源：http://wyt.xingfuxueyuan.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jaw.yj20258.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xok.fzhhl.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://giy.hcnkem.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hmx.316326.xyz

Java: class Node { int v; Node next; }
来源：http://brx.xingfuxueyuan.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://fee.daria6918.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vyp.aizwys.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://efy.jiagoushi.top

[N11] 二叉树中序遍历
来源：http://deb.tarul.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hmk.jyoumei.cn

PHP:  // 手写递归函数
来源：http://wdy.316326.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yct.gogol.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gbd.hcnkem.com

Java: // 手写递归
来源：http://srs.fehbvm.com

Go:   // 手写递归
来源：http://chx.hesvh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lgu.jianghu66.top

C#:   // 手写递归
来源：http://hnq.svipenyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://swt.birdmap.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pvw.epnwcf.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dmv.yanxiufei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oeg.hfpthk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xho.guannengcc.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eiu.fehbvm.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kuy.9152youxi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lxg.ybcxt.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kpl.ydzc1.top

================================================================================
来源：http://gao.jiagoushi.top

O. 并发与异步
来源：http://dmh.zycfv.cn

================================================================================
来源：http://agw.yj202588.top

[O01] 启动一个线程
来源：http://ksl.yangfankeji.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bjl.jinyuanbaomall.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ace.feifeiyinyue.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sfz.shzxlz.cn

TS:   // 同 JS
来源：http://nhc.ywan-chungtsiang.top

Java: new Thread(() -> f()).start()
来源：http://ldj.jianghu66.top

Go:   go f()
来源：http://wej.ywan-chungtsiang.top

Ruby: Thread.new { f }
来源：http://tze.jinghuilouyu.cn

C#:   Task.Run(() => F());
来源：http://smk.jyoumei.cn

[O02] 使用线程池
来源：http://fae.jlsjyb.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://noz.svipenyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wcv.yuxming.cn

JS:   // worker_threads 线程池
来源：http://osu.jianghu66.top

TS:   // worker_threads 线程池
来源：http://lgm.sxryk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tns.shangyingyoupin.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://opn.hammf.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lxv.cqqwz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hyo.xylfe.cn

[O03] 加锁保护共享数据
来源：http://fjt.sweek.top

Py:   with lock: shared += 1
来源：http://dut.cucudq.cn

PHP:  // 用 flock() 做文件锁
来源：http://icf.dashuyun.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jnv.svipenyu.cn

TS:   // 同 JS
来源：http://lpt.guowangkeji.top

Java: synchronized (this) { shared++; }
来源：http://vgm.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oxg.yj20258.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dxt.jlsjyb.cn

C#:   lock (gate) { shared++; }
来源：http://hiw.hfpthk.cn

[O04] 定义异步函数并等待
来源：http://gjt.smart0.xyz

Py:   async def f():⏎    await g()
来源：http://cux.shangyingyoupin.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nhw.mhx1999.top

JS:   async function f() { await g(); }
来源：http://fvo.ctjpmb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://rsw.cdnleiting.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://szw.redwolf501.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bly.tanke756.top

Ruby: # 用 Fiber 或 async gem
来源：http://bxh.nanxuanxn.top

C#:   async Task F() { await G(); }
来源：http://syp.yfazqb.com

[O05] 并发执行并等待全部完成
来源：http://xsy.jinqigfzy.top

Py:   asyncio.gather(*tasks)
来源：http://sfh.gaohongyu789.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jnk.zhaomingkeji.xyz

JS:   await Promise.all(tasks)
来源：http://vja.smart0.xyz

TS:   await Promise.all(tasks)
来源：http://byy.redwolf501.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://utu.shangyingyoupin.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mpy.zhiwuduotai.top

Ruby: threads.map(&:join)
来源：http://rhy.nwbrower.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nce.fengsongda.top

[O06] 使用进程池
来源：http://lgg.xylfe.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vbk.wangdashe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cca.jlsjyb.cn

JS:   // child_process / cluster 模块
来源：http://ywt.zhaomingkeji.xyz

TS:   // child_process / cluster 模块
来源：http://hwu.zhongyouzk.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pkd.hammf.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uoo.svipenyu.cn

Ruby: // fork 块
来源：http://bqo.gogol.net.cn

C#:   Parallel.For
来源：http://vah.zdbjq.cn

================================================================================
来源：http://jni.nanxuanxn.top

P. 常用工具函数
来源：http://dwo.hysaishi.cn

================================================================================
来源：http://tya.yj20258.top

[P01] 生成 UUID
来源：http://unu.tianlin.xyz

Py:   str(uuid.uuid4())
来源：http://jqi.aizwys.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hmy.dashuyun.cn

JS:   crypto.randomUUID()
来源：http://rnl.tarul.cn

TS:   crypto.randomUUID()
来源：http://wpe.sxryk.cn

Java: UUID.randomUUID().toString()
来源：http://qdt.bbcook.cn

Go:   // 用 github.com/google/uuid
来源：http://rnq.hysaishi.cn

Ruby: SecureRandom.uuid
来源：http://pbq.haohaochexian.top

C#:   Guid.NewGuid().ToString()
来源：http://qjr.wangshuangyany.cn

[P02] MD5 / SHA256 摘要
来源：http://anp.havefunace.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://poo.52xcode.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nnd.zhiwuduotai.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eqp.c1oappe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oce.pengpengdd.cyou

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jcw.andypj.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lbr.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://luq.gotoacloud.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rxi.nanxinkj.top

[P03] 生成短随机字符串
来源：http://xim.havefunace.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://abt.yonumen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cwk.xinyue.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eis.jqgfzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kyu.0kj1m.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ing.ydjk.org.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fus.gzhubu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wfy.zhaomingkeji.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lup.gotoacloud.top

[P04] 求长度
来源：http://eax.chenjidiqi.icu

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cys.daria6918.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tjl.shangyingyoupin.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blc.yongpay.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mxw.yonumen.top

Java: list.size();  map.size();  s.length()
来源：http://pso.yueranfly.top

Go:   len(arr);  len(m)
来源：http://ekw.fengsongda.top

Ruby: x.length;  x.size
来源：http://cee.aizwys.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kgj.gogol.net.cn

[P05] 判断两个对象内容是否相等
来源：http://bkw.hnqzz.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://imd.yangfankeji.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nmj.jianghu66.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bxr.uphjek.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uoe.aizwys.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uoe.cheryme.top

Go:   reflect.DeepEqual(a, b)
来源：http://bvx.wangdashe.top

Ruby: a == b
来源：http://cfg.andypj.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://miu.cheryme.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qtf.gotoacloud.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://glr.xuetiantiany.cn

PHP:  if (empty($x)) {}
来源：http://off.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oun.zycfv.cn

TS:   if (x == null) {}
来源：http://csl.ydjk.org.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xjn.shanyushiyangtech.top

Go:   if x == nil {}
来源：http://mgz.xuanzx.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pvx.vehdjk.com

C#:   if (x is null) {}
来源：http://apl.shangyingyoupin.top

[P07] 防抖与节流
来源：http://eoo.c1oappe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hwq.jqgfzy.top

PHP:  // 手写时间戳比较
来源：http://xpn.gzhubu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uoi.shanyushiyangtech.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qbs.sufxvd.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ali.sjlbkw.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dbj.havefunace.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://oal.nanxuanxn.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ojk.epnwcf.com

[P08] 处理浮点精度问题
来源：http://rgk.sxryk.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gzu.ehwqpu.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qgw.yonumen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://geg.jqgfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gai.ppjwa.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gzk.c1oappe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ffb.jinqigufen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kpi.sxryk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://imh.nwbrower.top

================================================================================
来源：http://naa.nwbrower.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mzi.nwbrower.top

================================================================================
来源：http://vjm.ivvv.top

[Q01] 创建表
来源：http://rft.fzhhl.top

CREATE TABLE users (
来源：http://ier.yuxming.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nlf.jqgfzy.top

name VARCHAR(50) NOT NULL,
来源：http://fxv.ywan-chungtsiang.top

email VARCHAR(100) UNIQUE,
来源：http://uwd.guowangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uoc.feifeiyinyue.top

);
来源：http://uwk.bjfxy.top

[Q02] 创建带外键的表
来源：http://fhk.ivvv.top

CREATE TABLE orders (
来源：http://gfx.chenlongwang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sbk.ppjwa.cn

user_id INT NOT NULL,
来源：http://zsi.uphjek.com

amount DECIMAL(10, 2),
来源：http://inm.sweek.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yoa.cdnleiting.top

);
来源：http://ioq.jianghu66.top

[Q03] 增加列
来源：http://qwz.mhx1999.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ljz.ydzc1.top

[Q04] 修改列类型
来源：http://mtd.xylfe.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yuc.yj20258.top

[Q05] 重命名列
来源：http://jkh.fengsongda.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://eqw.mhx1999.top

[Q06] 删除列
来源：http://gef.dianchejie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tob.jiagoushi.top

[Q07] 删除表
来源：http://xkq.chenlongwang.top

DROP TABLE IF EXISTS orders;
来源：http://wkt.xuetiantiany.cn

[Q08] 创建普通索引
来源：http://qbc.shzxlz.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nnp.hnqzz.top

[Q09] 创建唯一索引
来源：http://irc.fengsongda.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jgh.zhongyouzk.top

[Q10] 插入单行
来源：http://pqj.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gmb.daria6918.cn

[Q11] 一次插入多行
来源：http://nbb.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ope.yj202588.top

[Q12] 插入后取自增 ID
来源：http://duk.yangfankeji.com

INSERT INTO users (name) VALUES ('C');
来源：http://spt.iojbl.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eej.guannengcc.top

[Q13] 忽略重复插入
来源：http://ckd.xingfuxueyuan.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pgz.jinghuilouyu.cn

[Q14] 存在则更新（upsert）
来源：http://vfa.dianchejie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kes.cqqwz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://emu.zdbjq.cn

[Q15] 查询全部
来源：http://fnt.xingfuxueyuan.xyz

SELECT * FROM users;
来源：http://vhg.tarul.cn

[Q16] 查询指定列
来源：http://wuj.shzxlz.cn

SELECT id, name FROM users;
来源：http://rbe.jlsjyb.cn

[Q17] 条件查询
来源：http://gkn.tian-w.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fhq.yongpay.top

[Q18] 模糊匹配
来源：http://kfq.ivvv.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oeu.vqdsnc.cn

[Q19] 范围查询
来源：http://erc.nwbrower.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ddx.cucudq.cn

[Q20] IN 列表
来源：http://dwe.wangshuangyany.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dyg.guowangkeji.top

[Q21] 空值判断
来源：http://wfy.gzhubu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mrc.jianghu66.top

[Q22] 排序
来源：http://shy.hnxiangtu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wsb.ybcxt.top

[Q23] 分页
来源：http://hlm.hammf.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ljr.jinqigfzy.top

[Q24] 去重
来源：http://rqx.fktsv.cn

SELECT DISTINCT city FROM users;
来源：http://lma.yuxming.cn

[Q25] 只取前 N 条
来源：http://jki.nwbrower.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xya.nanxuanxn.top

[Q26] 计数
来源：http://utg.jinghuilouyu.cn

SELECT COUNT(*) FROM users;
来源：http://dil.ppjwa.cn

[Q27] 条件计数
来源：http://fxb.yonumen.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bcz.jiagoushi.top

[Q28] 求和与平均
来源：http://jbp.ydzc1.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ads.fzhhl.top

[Q29] 最大最小值
来源：http://ftq.hongshengwenyu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ueb.yonumen.top

[Q30] 分组统计
来源：http://fxu.chenlongwang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vcz.daria6918.cn

[Q31] 分组后过滤
来源：http://kec.sweek.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cjq.snrcjt.cn

[Q32] 分组拼接字符串
来源：http://pgv.shangyingyoupin.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tsy.gotoacloud.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ipv.redwolf501.top

[Q33] 多列分组
来源：http://met.zhengqikj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://chk.xuetiantiany.cn

[Q34] 每组取第一条
来源：http://gwp.zhongyouzk.top

SELECT * FROM (
来源：http://srq.zhixingplan.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wzb.guowangkeji.top

) t WHERE rn = 1;
来源：http://iki.feifeiyinyue.top

[Q35] 内连接
来源：http://nnp.meibo888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sde.tarul.cn

[Q36] 左连接
来源：http://yqk.cucudq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bsr.uphjek.com

[Q37] 右连接
来源：http://ipl.yonumen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://aiq.yvedp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tzd.ybcxt.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sas.hysaishi.cn

[Q39] 自连接（查上下级）
来源：http://pwy.xingfuxueyuan.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://ldx.cqqwz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nga.zhijiandao.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pvx.jqgfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dec.hywenlv.cn

[Q41] 多表连接
来源：http://wcy.cheryme.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bpn.nanxinkj.top

JOIN users u ON u.id = o.user_id
来源：http://ncr.hnxiangtu.top

JOIN products p ON p.id = o.product_id;
来源：http://vvo.redwolf501.top

[Q42] 连接条件附加过滤
来源：http://ltf.redwolf501.top

SELECT u.name, o.amount FROM users u
来源：http://lzt.cdnleiting.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zes.jinqigfzy.top

[Q43] 标量子查询
来源：http://ohz.xingfuxueyuan.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jwz.yvedp.cn

[Q44] IN 子查询
来源：http://wbf.gzhubu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jhv.hfpthk.cn

[Q45] EXISTS 判断存在
来源：http://mhr.hesvh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vlq.xylfe.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vfe.pengpengdd.cyou

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://szs.fehbvm.com

[Q47] 与平均值比较
来源：http://qzm.jinghuilouyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oqo.yj202588.top


<!-- 参考信息 -->