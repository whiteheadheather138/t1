代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://cwi.hammf.cn

TS:   s === [...s].reverse().join("")
来源：http://biw.xingfuxueyuan.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qly.jianghu66.top

Go:   // 双指针从两端比较
来源：http://hvf.yfazqb.com

Ruby: s == s.reverse
来源：http://mrr.aizwys.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://djy.dashuyun.cn

[N07] 两数之和（返回下标）
来源：http://jjq.hysaishi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dnx.yanxiufei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ppe.sxryk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fbc.shangyingyoupin.top

TS:   // 手写 Map<string, number>
来源：http://dxm.jqgufenzy.top

Java: // 手写 HashMap
来源：http://lvl.hysaishi.cn

Go:   // 手写 map[int]int
来源：http://gav.guannengcc.top

Ruby: // 手写 Hash
来源：http://uiv.yangfankeji.com

C#:   // 手写 Dictionary<int, int>
来源：http://ier.hysaishi.cn

[N08] 生成全排列
来源：http://mwu.daxiang520.top

Py:   itertools.permutations(arr)
来源：http://weq.xuanzx.com

PHP:  // 手写递归交换
来源：http://gxb.meibo888.top

JS:   // 手写回溯递归
来源：http://iey.tanke756.top

TS:   // 手写回溯递归
来源：http://czw.zhixingplan.top

Java: // 手写回溯递归
来源：http://wpp.hcnkem.com

Go:   // 手写回溯递归
来源：http://ech.chenjidiqi.icu

Ruby: arr.permutation.to_a
来源：http://rmv.9152youxi.cn

C#:   // 手写回溯递归
来源：http://gbu.xuanzx.com

[N09] 栈与队列
来源：http://bzm.xinyue.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qba.tarul.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ljd.jqgufenzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jqp.xuetiantiany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://loc.jinqigufen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aux.ehwqpu.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://guz.yuanzhike.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://msw.haohaochexian.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://trs.uphjek.com

[N10] 链表节点定义
来源：http://qqj.c1oappe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qbe.bjfxy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mah.fktsv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://twc.shanyushiyangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dnx.jianghu66.top

Java: class Node { int v; Node next; }
来源：http://gpn.chenzaomai.com

Go:   type Node struct { V int; Next *Node }
来源：http://knu.zhiwuduotai.top

Ruby: Node = Struct.new(:v, :next)
来源：http://idh.xuetiantiany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lmx.shangyingyoupin.top

[N11] 二叉树中序遍历
来源：http://bkn.vehdjk.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fht.ydzc1.top

PHP:  // 手写递归函数
来源：http://mbf.dashuyun.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lpf.chenzaomai.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://deh.zdbjq.cn

Java: // 手写递归
来源：http://toq.hnxiangtu.top

Go:   // 手写递归
来源：http://jqi.chenzaomai.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qyo.ywan-chungtsiang.top

C#:   // 手写递归
来源：http://ytj.zhijiandao.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://utb.bjfxy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zys.yanxiufei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ccj.hnqzz.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jds.quarkkingdee.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ddd.dianchejie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jez.xziqi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tja.tian-w.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://swm.cucudq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tym.hammf.cn

================================================================================
来源：http://vwj.cashguo.top

O. 并发与异步
来源：http://tta.haohaochexian.top

================================================================================
来源：http://hdd.hcnkem.com

[O01] 启动一个线程
来源：http://qfz.yuxming.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ukz.jqgfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cuq.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hrr.xinyue.icu

TS:   // 同 JS
来源：http://bgr.hnqzz.top

Java: new Thread(() -> f()).start()
来源：http://rmk.zhongyouzk.top

Go:   go f()
来源：http://wfv.jinqigufen.top

Ruby: Thread.new { f }
来源：http://vtg.sysykeji.top

C#:   Task.Run(() => F());
来源：http://pkf.xuanzx.com

[O02] 使用线程池
来源：http://pxk.cheryme.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://utf.zdqjudy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hfo.jinyuanbaomall.cn

JS:   // worker_threads 线程池
来源：http://jyb.tarul.cn

TS:   // worker_threads 线程池
来源：http://vcz.haohaochexian.top

Java: Executors.newFixedThreadPool(4)
来源：http://jmg.9152youxi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://azi.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tks.xziqi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rtz.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://khw.hywenlv.cn

Py:   with lock: shared += 1
来源：http://qdu.yanxiufei.cn

PHP:  // 用 flock() 做文件锁
来源：http://fbh.zycfv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mvh.gogol.net.cn

TS:   // 同 JS
来源：http://vyd.vqdsnc.cn

Java: synchronized (this) { shared++; }
来源：http://ylu.aizwys.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://haz.cheryme.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://pbl.jiagoushi.top

C#:   lock (gate) { shared++; }
来源：http://hxb.ybcxt.top

[O04] 定义异步函数并等待
来源：http://pgy.chenjidiqi.icu

Py:   async def f():⏎    await g()
来源：http://kzk.hywenlv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://urf.pengpengdd.cyou

JS:   async function f() { await g(); }
来源：http://zbu.meibo888.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dpn.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cmy.hfpthk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://atx.gaohongyu789.top

Ruby: # 用 Fiber 或 async gem
来源：http://lot.ctjpmb.com

C#:   async Task F() { await G(); }
来源：http://wkq.kuanghao11.cn

[O05] 并发执行并等待全部完成
来源：http://bem.bjfxy.top

Py:   asyncio.gather(*tasks)
来源：http://cvy.sxryk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ylh.sufxvd.cn

JS:   await Promise.all(tasks)
来源：http://ndf.jinghuilouyu.cn

TS:   await Promise.all(tasks)
来源：http://xfa.jianghu66.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ial.c1oappe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zju.yfazqb.com

Ruby: threads.map(&:join)
来源：http://zjh.smart0.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://yvv.sysykeji.top

[O06] 使用进程池
来源：http://avi.xingfuxueyuan.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://axt.ydjk.org.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jls.sxryk.cn

JS:   // child_process / cluster 模块
来源：http://izj.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://rdf.ybcxt.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fdg.hesvh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hql.chenlongwang.top

Ruby: // fork 块
来源：http://vtj.gotoacloud.top

C#:   Parallel.For
来源：http://fyi.zdqjudy.top

================================================================================
来源：http://dsa.zhiwuduotai.top

P. 常用工具函数
来源：http://jqg.yvedp.cn

================================================================================
来源：http://jvw.shuidangran.top

[P01] 生成 UUID
来源：http://lgk.zdbjq.cn

Py:   str(uuid.uuid4())
来源：http://xfq.ctjpmb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://crp.zhijiandao.cn

JS:   crypto.randomUUID()
来源：http://xas.zdqjudy.top

TS:   crypto.randomUUID()
来源：http://uyz.gzhubu.top

Java: UUID.randomUUID().toString()
来源：http://ovl.shzxlz.cn

Go:   // 用 github.com/google/uuid
来源：http://hkk.chenlongwang.top

Ruby: SecureRandom.uuid
来源：http://mjo.vqdsnc.cn

C#:   Guid.NewGuid().ToString()
来源：http://vqs.sysykeji.top

[P02] MD5 / SHA256 摘要
来源：http://vsz.cqqwz.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ktc.yfazqb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://plh.0kj1m.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://twh.tarul.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fcc.yj20258888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qny.zhixingplan.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bgj.redwolf501.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://atw.daria6918.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rgv.pengpengdd.cyou

[P03] 生成短随机字符串
来源：http://pqe.zhoulong.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vem.wangdashe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://koy.svipenyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jps.zhongyouzk.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bfm.sjlbkw.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pez.yanxiufei.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lvf.tianlin.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://uud.0kj1m.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bka.jqgfzy.top

[P04] 求长度
来源：http://guh.cdnleiting.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uwt.nanxuanxn.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tkk.andypj.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ucz.ydzc1.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://whn.quarkkingdee.top

Java: list.size();  map.size();  s.length()
来源：http://qlr.ydjk.org.cn

Go:   len(arr);  len(m)
来源：http://tlp.yj202588.top

Ruby: x.length;  x.size
来源：http://iqu.redwolf501.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zgo.guannengcc.top

[P05] 判断两个对象内容是否相等
来源：http://ihb.sysykeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qeh.gotoacloud.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vtj.guannengcc.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ofk.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vri.9152youxi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bli.jinqigfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://ahu.yj202588.top

Ruby: a == b
来源：http://njx.bjfxy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bav.jqgfzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://awi.svipenyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kne.ydzc1.top

PHP:  if (empty($x)) {}
来源：http://xno.tian-w.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://klk.svipenyu.cn

TS:   if (x == null) {}
来源：http://igu.chenlongwang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://paa.shanyushiyangtech.top

Go:   if x == nil {}
来源：http://roc.hnxiangtu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fly.hnqzz.top

C#:   if (x is null) {}
来源：http://zca.ydzc1.top

[P07] 防抖与节流
来源：http://ura.sjlbkw.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://paw.0kj1m.cn

PHP:  // 手写时间戳比较
来源：http://zjg.fzhhl.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hiu.zycfv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lzy.jlsjyb.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gwr.xinyue.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ppz.sufxvd.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://aka.jiagoushi.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xlq.hfpthk.cn

[P08] 处理浮点精度问题
来源：http://akb.jiagoushi.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gpi.shanyushiyangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kkx.hfpthk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pjd.tianlin.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dom.xuanzx.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ldx.shanyushiyangtech.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bri.vehdjk.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vjd.ctjpmb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rfs.bjfxy.top

================================================================================
来源：http://bld.hnxiangtu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://anb.c1oappe.top

================================================================================
来源：http://qwb.ybcxt.top

[Q01] 创建表
来源：http://hvz.mhx1999.top

CREATE TABLE users (
来源：http://wue.jinyuanbaomall.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hwp.0kj1m.cn

name VARCHAR(50) NOT NULL,
来源：http://aoi.aizwys.cn

email VARCHAR(100) UNIQUE,
来源：http://tto.smart0.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bex.316326.xyz

);
来源：http://tzr.0kj1m.cn

[Q02] 创建带外键的表
来源：http://toh.tanke756.top

CREATE TABLE orders (
来源：http://ggp.shanyushiyangtech.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://twa.shzxlz.cn

user_id INT NOT NULL,
来源：http://aor.zdqjudy.top

amount DECIMAL(10, 2),
来源：http://ruy.cucudq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vtm.jinqigufen.top

);
来源：http://cms.tian-w.cn

[Q03] 增加列
来源：http://vys.gzhubu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gvi.gaohongyu789.top

[Q04] 修改列类型
来源：http://qll.zhiwuduotai.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kpc.uphjek.com

[Q05] 重命名列
来源：http://jjs.jianghu66.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bmo.zdqjudy.top

[Q06] 删除列
来源：http://tda.zhiwuduotai.top

ALTER TABLE users DROP COLUMN age;
来源：http://spp.yongpay.top

[Q07] 删除表
来源：http://rls.yongpay.top

DROP TABLE IF EXISTS orders;
来源：http://epg.shanyushiyangtech.top

[Q08] 创建普通索引
来源：http://gaj.mhx1999.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pty.hysaishi.cn

[Q09] 创建唯一索引
来源：http://mgb.jinqigfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rzq.gaohongyu789.top

[Q10] 插入单行
来源：http://bqx.daxiang520.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://axz.tianlin.xyz

[Q11] 一次插入多行
来源：http://sui.haohaochexian.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qvl.fengsongda.top

[Q12] 插入后取自增 ID
来源：http://nei.yonumen.top

INSERT INTO users (name) VALUES ('C');
来源：http://lbd.bjfxy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dtp.chenlongwang.top

[Q13] 忽略重复插入
来源：http://bks.jlsjyb.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tyf.nanxuanxn.top

[Q14] 存在则更新（upsert）
来源：http://nny.shuidangran.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hdn.hywenlv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gam.guannengcc.top

[Q15] 查询全部
来源：http://xjv.yangfankeji.com

SELECT * FROM users;
来源：http://gky.ppjwa.cn

[Q16] 查询指定列
来源：http://hxk.chenjidiqi.icu

SELECT id, name FROM users;
来源：http://jia.9152youxi.cn

[Q17] 条件查询
来源：http://fpi.zycfv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mmb.meibo888.top

[Q18] 模糊匹配
来源：http://xhx.pengpengdd.cyou

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xoc.meibo888.top

[Q19] 范围查询
来源：http://rxa.ctjpmb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fsn.hysaishi.cn

[Q20] IN 列表
来源：http://qrn.fehbvm.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hqv.bjfxy.top

[Q21] 空值判断
来源：http://rnl.hnxiangtu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bxv.snrcjt.cn

[Q22] 排序
来源：http://igc.havefunace.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tzk.haohaochexian.top

[Q23] 分页
来源：http://ogj.svipenyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kjx.shzxlz.cn

[Q24] 去重
来源：http://hnc.yj202588.top

SELECT DISTINCT city FROM users;
来源：http://wnz.xuanzx.com

[Q25] 只取前 N 条
来源：http://znt.smart0.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://afx.hongshengwenyu.top

[Q26] 计数
来源：http://kvp.guowangkeji.top

SELECT COUNT(*) FROM users;
来源：http://fvq.hcnkem.com

[Q27] 条件计数
来源：http://hyb.0kj1m.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jst.jinyuanbaomall.cn

[Q28] 求和与平均
来源：http://idy.yvedp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xtk.zhoulong.xyz

[Q29] 最大最小值
来源：http://bnq.nanxinkj.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ueo.sjlbkw.cn

[Q30] 分组统计
来源：http://ftb.quarkkingdee.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dte.sufxvd.cn

[Q31] 分组后过滤
来源：http://vfy.xingfuxueyuan.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lpt.andypj.xyz

[Q32] 分组拼接字符串
来源：http://quc.bbcook.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://obm.guannengcc.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ndh.jqgufenzy.top

[Q33] 多列分组
来源：http://ylx.yuanzhike.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hwx.shzxlz.cn

[Q34] 每组取第一条
来源：http://ucv.gaohongyu789.top

SELECT * FROM (
来源：http://hdk.sxryk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rmm.ybcxt.top

) t WHERE rn = 1;
来源：http://gmf.zhoulong.xyz

[Q35] 内连接
来源：http://jim.iojbl.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qog.snrcjt.cn

[Q36] 左连接
来源：http://uyb.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lmo.zhijiandao.cn

[Q37] 右连接
来源：http://ovv.yvedp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wkn.guowangkeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://xgi.snrcjt.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uwe.0kj1m.cn

[Q39] 自连接（查上下级）
来源：http://kef.jinqigufen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://eom.tanke756.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lpf.hfpthk.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ajc.guannengcc.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nuw.nwbrower.top

[Q41] 多表连接
来源：http://gvj.9152youxi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lsb.zhiwuduotai.top

JOIN users u ON u.id = o.user_id
来源：http://fmi.guowangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://fgv.shzxlz.cn

[Q42] 连接条件附加过滤
来源：http://hvb.gaohongyu789.top

SELECT u.name, o.amount FROM users u
来源：http://gym.jinyuanbaomall.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xie.redwolf501.top

[Q43] 标量子查询
来源：http://xew.hfpthk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nip.52xcode.cn


<!-- 参考信息 -->