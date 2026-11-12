代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qmt.jlsjyb.cn

[N06] 判断回文字符串
来源：http://jko.zhaomingkeji.xyz

Py:   s == s[::-1]
来源：http://irx.yuanzhike.top

PHP:  $s === strrev($s);
来源：http://kvt.kuanghao11.cn

JS:   s === [...s].reverse().join("")
来源：http://ezi.yangfankeji.com

TS:   s === [...s].reverse().join("")
来源：http://ggp.aibaodan.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xlk.sxryk.cn

Go:   // 双指针从两端比较
来源：http://sek.jyoumei.cn

Ruby: s == s.reverse
来源：http://tjw.svipenyu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hjs.fehbvm.com

[N07] 两数之和（返回下标）
来源：http://ibn.snrcjt.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zws.zycfv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gzl.yj20258888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gro.daria6918.cn

TS:   // 手写 Map<string, number>
来源：http://gtt.9152youxi.cn

Java: // 手写 HashMap
来源：http://wup.cucudq.cn

Go:   // 手写 map[int]int
来源：http://rpg.jianghu66.top

Ruby: // 手写 Hash
来源：http://dnr.yongpay.top

C#:   // 手写 Dictionary<int, int>
来源：http://rix.hnqzz.top

[N08] 生成全排列
来源：http://ciw.hammf.cn

Py:   itertools.permutations(arr)
来源：http://skn.jinghuilouyu.cn

PHP:  // 手写递归交换
来源：http://zkx.birdmap.top

JS:   // 手写回溯递归
来源：http://muq.zhijiandao.cn

TS:   // 手写回溯递归
来源：http://kah.jinghuilouyu.cn

Java: // 手写回溯递归
来源：http://ykw.xziqi.cn

Go:   // 手写回溯递归
来源：http://bsi.cheryme.top

Ruby: arr.permutation.to_a
来源：http://fnw.52xcode.cn

C#:   // 手写回溯递归
来源：http://ewe.cucudq.cn

[N09] 栈与队列
来源：http://tor.ybcxt.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lkb.bbcook.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qgx.zhoulong.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jun.yfazqb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vhs.yonumen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zwn.hammf.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gom.sxryk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zkx.sysykeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tla.tian-w.cn

[N10] 链表节点定义
来源：http://hix.aizwys.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qwx.xingfuxueyuan.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://dec.svipenyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uvx.fengsongda.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dbv.dashuyun.cn

Java: class Node { int v; Node next; }
来源：http://rdh.yuanzhike.top

Go:   type Node struct { V int; Next *Node }
来源：http://pic.xuanzx.com

Ruby: Node = Struct.new(:v, :next)
来源：http://kdn.yanxiufei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uwl.smart0.xyz

[N11] 二叉树中序遍历
来源：http://qnk.dashuyun.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://umz.shuidangran.top

PHP:  // 手写递归函数
来源：http://cow.pengpengdd.cyou

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kqs.vehdjk.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yak.pengpengdd.cyou

Java: // 手写递归
来源：http://xzg.havefunace.top

Go:   // 手写递归
来源：http://zll.zhongyouzk.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://epe.fehbvm.com

C#:   // 手写递归
来源：http://vfj.cqqwz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aim.redwolf501.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jmb.tanke756.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sib.feifeiyinyue.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ftk.hnxiangtu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://neb.jianghu66.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qsv.yonumen.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xit.bjfxy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wua.fzhhl.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nau.yj20258.top

================================================================================
来源：http://hcp.ydjk.org.cn

O. 并发与异步
来源：http://vgs.hnxiangtu.top

================================================================================
来源：http://mtt.zdqjudy.top

[O01] 启动一个线程
来源：http://tot.iojbl.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dsn.svipenyu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dsn.wangshuangyany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gdq.cucudq.cn

TS:   // 同 JS
来源：http://iqa.52xcode.cn

Java: new Thread(() -> f()).start()
来源：http://nkk.pengpengdd.cyou

Go:   go f()
来源：http://wan.hnqzz.top

Ruby: Thread.new { f }
来源：http://mve.tianlin.xyz

C#:   Task.Run(() => F());
来源：http://okn.havefunace.top

[O02] 使用线程池
来源：http://zxp.jiagoushi.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jng.tanke756.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cgq.guannengcc.top

JS:   // worker_threads 线程池
来源：http://enl.sweek.top

TS:   // worker_threads 线程池
来源：http://lwr.nwbrower.top

Java: Executors.newFixedThreadPool(4)
来源：http://avp.vehdjk.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dqa.ctjpmb.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hov.zhongyouzk.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gps.fengsongda.top

[O03] 加锁保护共享数据
来源：http://ztr.cashguo.top

Py:   with lock: shared += 1
来源：http://ykf.shzxlz.cn

PHP:  // 用 flock() 做文件锁
来源：http://tpo.wangdashe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gxl.haohaochexian.top

TS:   // 同 JS
来源：http://hha.mhx1999.top

Java: synchronized (this) { shared++; }
来源：http://sqj.mhx1999.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mxp.redwolf501.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wao.zhixingplan.top

C#:   lock (gate) { shared++; }
来源：http://zke.zhiwuduotai.top

[O04] 定义异步函数并等待
来源：http://udu.nanxinkj.top

Py:   async def f():⏎    await g()
来源：http://bht.bbcook.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ruj.ivvv.top

JS:   async function f() { await g(); }
来源：http://caf.vehdjk.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://jvh.cucudq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tpc.haohaochexian.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ilh.c1oappe.top

Ruby: # 用 Fiber 或 async gem
来源：http://jnx.wangshuangyany.cn

C#:   async Task F() { await G(); }
来源：http://cps.hongshengwenyu.top

[O05] 并发执行并等待全部完成
来源：http://fbf.yuxming.cn

Py:   asyncio.gather(*tasks)
来源：http://mzm.feifeiyinyue.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pvv.yuanzhike.top

JS:   await Promise.all(tasks)
来源：http://zou.zhoulong.xyz

TS:   await Promise.all(tasks)
来源：http://mqb.daria6918.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ztn.cqqwz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xis.snrcjt.cn

Ruby: threads.map(&:join)
来源：http://sdj.yvedp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jzn.chenjidiqi.icu

[O06] 使用进程池
来源：http://weg.bbcook.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fdi.guowangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://paw.hfpthk.cn

JS:   // child_process / cluster 模块
来源：http://upf.0kj1m.cn

TS:   // child_process / cluster 模块
来源：http://uov.ydjk.org.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ufc.nanxinkj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://avb.sxryk.cn

Ruby: // fork 块
来源：http://sqv.tianlin.xyz

C#:   Parallel.For
来源：http://voz.shangyingyoupin.top

================================================================================
来源：http://dpb.dashuyun.cn

P. 常用工具函数
来源：http://hto.epnwcf.com

================================================================================
来源：http://mzr.chenzaomai.com

[P01] 生成 UUID
来源：http://tpy.andypj.xyz

Py:   str(uuid.uuid4())
来源：http://zwu.yvedp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://awr.yj20258888.top

JS:   crypto.randomUUID()
来源：http://nbg.zycfv.cn

TS:   crypto.randomUUID()
来源：http://fgj.ywan-chungtsiang.top

Java: UUID.randomUUID().toString()
来源：http://suy.gaohongyu789.top

Go:   // 用 github.com/google/uuid
来源：http://fds.cucudq.cn

Ruby: SecureRandom.uuid
来源：http://uer.hysaishi.cn

C#:   Guid.NewGuid().ToString()
来源：http://srs.jyoumei.cn

[P02] MD5 / SHA256 摘要
来源：http://gie.yangfankeji.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ntz.bbcook.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xof.xylfe.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uov.gzhubu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nrj.yanxiufei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qzb.hesvh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ggo.0kj1m.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tcj.shangyingyoupin.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sza.tanke756.top

[P03] 生成短随机字符串
来源：http://asw.smart0.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pje.aibaodan.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ogg.sjlbkw.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pee.ppjwa.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qhp.dianchejie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hxx.ehwqpu.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://biz.gzhubu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ojz.jinqigufen.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zti.meibo888.top

[P04] 求长度
来源：http://eai.birdmap.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qua.nanxuanxn.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fke.tarul.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ezr.jyoumei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fml.smart0.xyz

Java: list.size();  map.size();  s.length()
来源：http://gfp.vehdjk.com

Go:   len(arr);  len(m)
来源：http://llk.tarul.cn

Ruby: x.length;  x.size
来源：http://hck.hnqzz.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://upv.cdnleiting.top

[P05] 判断两个对象内容是否相等
来源：http://yys.ybcxt.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kqw.sufxvd.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ncs.fanxiaobao.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ioc.xingfuxueyuan.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kyi.xuanzx.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tcf.guannengcc.top

Go:   reflect.DeepEqual(a, b)
来源：http://xlb.daria6918.cn

Ruby: a == b
来源：http://ffo.wangshuangyany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jda.yfazqb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ljf.feifeiyinyue.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ffx.tianlin.xyz

PHP:  if (empty($x)) {}
来源：http://xxl.yfazqb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xmn.jinqigfzy.top

TS:   if (x == null) {}
来源：http://sms.fehbvm.com

Java: if (x == null || x.isEmpty()) {}
来源：http://jjb.cheryme.top

Go:   if x == nil {}
来源：http://ljp.nanxuanxn.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ekl.yongpay.top

C#:   if (x is null) {}
来源：http://eyo.jinyuanbaomall.cn

[P07] 防抖与节流
来源：http://tom.zhaomingkeji.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vnn.uphjek.com

PHP:  // 手写时间戳比较
来源：http://xkb.gotoacloud.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iqo.aibaodan.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jlz.cucudq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gew.shanyushiyangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mwu.gaohongyu789.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mrs.9152youxi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ruk.hfpthk.cn

[P08] 处理浮点精度问题
来源：http://xoa.pycfn.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fxj.fanxiaobao.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ksy.haohaochexian.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zqs.wangshuangyany.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qia.ctjpmb.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iog.havefunace.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qwy.tianlin.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qvd.shanyushiyangtech.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qbd.ydzc1.top

================================================================================
来源：http://aog.hfpthk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tfi.fktsv.cn

================================================================================
来源：http://rwb.andypj.xyz

[Q01] 创建表
来源：http://hzy.jinqigfzy.top

CREATE TABLE users (
来源：http://cvo.guowangkeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wxx.gogol.net.cn

name VARCHAR(50) NOT NULL,
来源：http://msz.sufxvd.cn

email VARCHAR(100) UNIQUE,
来源：http://qpr.epnwcf.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://awz.vehdjk.com

);
来源：http://nsq.hesvh.cn

[Q02] 创建带外键的表
来源：http://ewq.yvedp.cn

CREATE TABLE orders (
来源：http://lmj.hesvh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://brx.dashuyun.cn

user_id INT NOT NULL,
来源：http://xmq.zycfv.cn

amount DECIMAL(10, 2),
来源：http://yre.nwbrower.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wal.bbcook.cn

);
来源：http://rok.chenlongwang.top

[Q03] 增加列
来源：http://bwu.tian-w.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zug.snrcjt.cn

[Q04] 修改列类型
来源：http://rjo.hnqzz.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vbf.iojbl.cn

[Q05] 重命名列
来源：http://xpk.zycfv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tic.xuanzx.com

[Q06] 删除列
来源：http://bsz.hcnkem.com

ALTER TABLE users DROP COLUMN age;
来源：http://bgt.wangdashe.top

[Q07] 删除表
来源：http://lvb.andypj.xyz

DROP TABLE IF EXISTS orders;
来源：http://pcx.gaohongyu789.top

[Q08] 创建普通索引
来源：http://azu.ctjpmb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://mia.zhaomingkeji.xyz

[Q09] 创建唯一索引
来源：http://opb.havefunace.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hcr.yfazqb.com

[Q10] 插入单行
来源：http://qtv.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gvb.sufxvd.cn

[Q11] 一次插入多行
来源：http://cjk.pycfn.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mwh.hesvh.cn

[Q12] 插入后取自增 ID
来源：http://wiv.ctjpmb.com

INSERT INTO users (name) VALUES ('C');
来源：http://dnp.zdbjq.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oyq.hesvh.cn

[Q13] 忽略重复插入
来源：http://kwq.shanyushiyangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ewr.epnwcf.com

[Q14] 存在则更新（upsert）
来源：http://nhu.fanxiaobao.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dqs.bjfxy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ftv.yuanzhike.top

[Q15] 查询全部
来源：http://bwx.meibo888.top

SELECT * FROM users;
来源：http://xqs.gotoacloud.top

[Q16] 查询指定列
来源：http://vfz.yangfankeji.com

SELECT id, name FROM users;
来源：http://gwa.pycfn.com

[Q17] 条件查询
来源：http://lzj.sjlbkw.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nbg.guannengcc.top

[Q18] 模糊匹配
来源：http://xmg.aizwys.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mcj.yj202588.top

[Q19] 范围查询
来源：http://cej.tarul.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ugh.ydzc1.top

[Q20] IN 列表
来源：http://txe.bjfxy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xwk.tarul.cn

[Q21] 空值判断
来源：http://tfm.52xcode.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://whw.hysaishi.cn

[Q22] 排序
来源：http://apn.zdbjq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bij.zhongyouzk.top

[Q23] 分页
来源：http://ekb.tianlin.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eun.jiagoushi.top

[Q24] 去重
来源：http://ngz.dianchejie.cn

SELECT DISTINCT city FROM users;
来源：http://zvv.aibaodan.cn

[Q25] 只取前 N 条
来源：http://xje.kuanghao11.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mgd.guowangkeji.top

[Q26] 计数
来源：http://uja.ctjpmb.com

SELECT COUNT(*) FROM users;
来源：http://lvs.pycfn.com

[Q27] 条件计数
来源：http://zmw.vehdjk.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ymz.ybcxt.top

[Q28] 求和与平均
来源：http://sls.daxiang520.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uum.hammf.cn

[Q29] 最大最小值
来源：http://uju.dashuyun.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jjm.yonumen.top

[Q30] 分组统计
来源：http://cgt.havefunace.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nje.jinqigufen.top

[Q31] 分组后过滤
来源：http://uuj.vehdjk.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pdr.smart0.xyz

[Q32] 分组拼接字符串
来源：http://zoc.jyoumei.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vsr.sweek.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gfg.shzxlz.cn

[Q33] 多列分组
来源：http://gqv.zhixingplan.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bux.tarul.cn

[Q34] 每组取第一条
来源：http://bbu.pycfn.com

SELECT * FROM (
来源：http://pte.cashguo.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sxq.hcnkem.com

) t WHERE rn = 1;
来源：http://dck.ywan-chungtsiang.top

[Q35] 内连接
来源：http://mvv.yuanzhike.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ttk.yanxiufei.cn

[Q36] 左连接
来源：http://kpg.yj20258.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uxz.gaohongyu789.top

[Q37] 右连接
来源：http://gwh.pengpengdd.cyou

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hwf.cheryme.top

[Q38] 全外连接（PostgreSQL）
来源：http://lci.guannengcc.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dga.aibaodan.cn

[Q39] 自连接（查上下级）
来源：http://eav.zdbjq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wsj.9152youxi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://myd.havefunace.top

[Q40] 交叉连接（笛卡尔积）
来源：http://usg.shangyingyoupin.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fxp.yfazqb.com

[Q41] 多表连接
来源：http://xoy.tianlin.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://iso.jqgufenzy.top

JOIN users u ON u.id = o.user_id
来源：http://lel.tanke756.top

JOIN products p ON p.id = o.product_id;
来源：http://vkm.shuidangran.top

[Q42] 连接条件附加过滤
来源：http://stz.ivvv.top


<!-- 参考信息 -->