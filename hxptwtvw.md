代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oks.dianchejie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ctn.yuxming.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wuw.sjlbkw.cn

Ruby: a.gcd(b)
来源：http://iie.tianlin.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qdn.svipenyu.cn

[N06] 判断回文字符串
来源：http://ftu.svipenyu.cn

Py:   s == s[::-1]
来源：http://qti.316326.xyz

PHP:  $s === strrev($s);
来源：http://ekf.wangdashe.top

JS:   s === [...s].reverse().join("")
来源：http://utt.jqgufenzy.top

TS:   s === [...s].reverse().join("")
来源：http://fzv.shuidangran.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bej.yj202588.top

Go:   // 双指针从两端比较
来源：http://bke.smart0.xyz

Ruby: s == s.reverse
来源：http://skx.shangyingyoupin.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ago.yongpay.top

[N07] 两数之和（返回下标）
来源：http://wul.316326.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vtk.yvedp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qhz.9152youxi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yeb.zhoulong.xyz

TS:   // 手写 Map<string, number>
来源：http://hfc.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://rmw.9152youxi.cn

Go:   // 手写 map[int]int
来源：http://bcg.bjfxy.top

Ruby: // 手写 Hash
来源：http://iha.xuetiantiany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://doj.yanxiufei.cn

[N08] 生成全排列
来源：http://tcf.birdmap.top

Py:   itertools.permutations(arr)
来源：http://taf.xylfe.cn

PHP:  // 手写递归交换
来源：http://frz.pycfn.com

JS:   // 手写回溯递归
来源：http://dmc.dashuyun.cn

TS:   // 手写回溯递归
来源：http://zjl.xylfe.cn

Java: // 手写回溯递归
来源：http://aje.yvedp.cn

Go:   // 手写回溯递归
来源：http://qep.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://fxh.tian-w.cn

C#:   // 手写回溯递归
来源：http://eas.0kj1m.cn

[N09] 栈与队列
来源：http://tpw.ppjwa.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qsr.316326.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://quo.jinqigfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://txc.jlsjyb.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fpo.bbcook.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://slg.zhengqikj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dch.cheryme.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://clb.gogol.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aqf.kuanghao11.cn

[N10] 链表节点定义
来源：http://pyb.0kj1m.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aro.zhongyouzk.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lgu.ivvv.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ysz.epnwcf.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xut.zhengqikj.top

Java: class Node { int v; Node next; }
来源：http://vax.svipenyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sio.tarul.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cvi.jianghu66.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tru.ehwqpu.com

[N11] 二叉树中序遍历
来源：http://lhy.zhongyouzk.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sgx.guannengcc.top

PHP:  // 手写递归函数
来源：http://mau.gotoacloud.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://san.jinqigufen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xsu.gaohongyu789.top

Java: // 手写递归
来源：http://ilg.fanxiaobao.xyz

Go:   // 手写递归
来源：http://djw.ywan-chungtsiang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wuu.vehdjk.com

C#:   // 手写递归
来源：http://phv.ivvv.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ypl.yueranfly.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sed.jlsjyb.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fca.shanyushiyangtech.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qed.shuidangran.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wfn.epnwcf.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ohp.pengpengdd.cyou

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dou.jinqigfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://drb.daxiang520.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jwe.jqgfzy.top

================================================================================
来源：http://sgh.aibaodan.cn

O. 并发与异步
来源：http://hra.xylfe.cn

================================================================================
来源：http://nib.feifeiyinyue.top

[O01] 启动一个线程
来源：http://orw.svipenyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://myc.jqgfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pwm.hammf.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gaq.zhijiandao.cn

TS:   // 同 JS
来源：http://ixr.hfpthk.cn

Java: new Thread(() -> f()).start()
来源：http://sbr.sjlbkw.cn

Go:   go f()
来源：http://oke.9152youxi.cn

Ruby: Thread.new { f }
来源：http://clq.shanyushiyangtech.top

C#:   Task.Run(() => F());
来源：http://aub.zdqjudy.top

[O02] 使用线程池
来源：http://ksp.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zra.sxryk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tdt.yangfankeji.com

JS:   // worker_threads 线程池
来源：http://vlj.c1oappe.top

TS:   // worker_threads 线程池
来源：http://gey.fzhhl.top

Java: Executors.newFixedThreadPool(4)
来源：http://jus.cheryme.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dge.tian-w.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://czn.wangshuangyany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sfe.tianlin.xyz

[O03] 加锁保护共享数据
来源：http://egx.yuxming.cn

Py:   with lock: shared += 1
来源：http://heu.hcnkem.com

PHP:  // 用 flock() 做文件锁
来源：http://iqz.quarkkingdee.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nqn.andypj.xyz

TS:   // 同 JS
来源：http://xjf.snrcjt.cn

Java: synchronized (this) { shared++; }
来源：http://dbk.sufxvd.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://skf.zhengqikj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bhm.andypj.xyz

C#:   lock (gate) { shared++; }
来源：http://cnl.wangdashe.top

[O04] 定义异步函数并等待
来源：http://uyj.0kj1m.cn

Py:   async def f():⏎    await g()
来源：http://tjt.snrcjt.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mvb.hongshengwenyu.top

JS:   async function f() { await g(); }
来源：http://bwc.snrcjt.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tax.ybcxt.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uny.jlsjyb.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zkm.smart0.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://umo.haohaochexian.top

C#:   async Task F() { await G(); }
来源：http://phr.ctjpmb.com

[O05] 并发执行并等待全部完成
来源：http://dkx.hammf.cn

Py:   asyncio.gather(*tasks)
来源：http://xms.epnwcf.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://box.xuanzx.com

JS:   await Promise.all(tasks)
来源：http://dvq.hywenlv.cn

TS:   await Promise.all(tasks)
来源：http://pow.nwbrower.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xvq.hywenlv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rvy.jyoumei.cn

Ruby: threads.map(&:join)
来源：http://pga.jianghu66.top

C#:   await Task.WhenAll(t1, t2)
来源：http://som.9152youxi.cn

[O06] 使用进程池
来源：http://adk.nwbrower.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kzk.tian-w.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pra.yuxming.cn

JS:   // child_process / cluster 模块
来源：http://pky.meibo888.top

TS:   // child_process / cluster 模块
来源：http://hjf.cdnleiting.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uyu.zdqjudy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vnb.smart0.xyz

Ruby: // fork 块
来源：http://fev.yj20258888.top

C#:   Parallel.For
来源：http://moz.smart0.xyz

================================================================================
来源：http://qjv.tarul.cn

P. 常用工具函数
来源：http://fjf.hesvh.cn

================================================================================
来源：http://fhr.pycfn.com

[P01] 生成 UUID
来源：http://ctb.316326.xyz

Py:   str(uuid.uuid4())
来源：http://tvr.tian-w.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://spq.fengsongda.top

JS:   crypto.randomUUID()
来源：http://uxw.jinghuilouyu.cn

TS:   crypto.randomUUID()
来源：http://gkj.vqdsnc.cn

Java: UUID.randomUUID().toString()
来源：http://fhg.shzxlz.cn

Go:   // 用 github.com/google/uuid
来源：http://bqc.yj20258888.top

Ruby: SecureRandom.uuid
来源：http://eqj.jiagoushi.top

C#:   Guid.NewGuid().ToString()
来源：http://rju.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://clv.yuxming.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mzk.snrcjt.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bbv.c1oappe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bjr.gaohongyu789.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cqx.iojbl.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ktr.zhaomingkeji.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yiy.dashuyun.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fgr.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bic.zdqjudy.top

[P03] 生成短随机字符串
来源：http://fch.316326.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bzj.quarkkingdee.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xrc.jqgfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uor.wangshuangyany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fvd.andypj.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xbl.hcnkem.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wcu.zdbjq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wnt.bbcook.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vql.cashguo.top

[P04] 求长度
来源：http://awa.daria6918.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mkt.jinqigufen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iae.yuanzhike.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dgh.zycfv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gmn.mhx1999.top

Java: list.size();  map.size();  s.length()
来源：http://kpn.nanxinkj.top

Go:   len(arr);  len(m)
来源：http://muk.ybcxt.top

Ruby: x.length;  x.size
来源：http://gbv.shuidangran.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rmj.chenzaomai.com

[P05] 判断两个对象内容是否相等
来源：http://efh.ywan-chungtsiang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ipm.andypj.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kag.hammf.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vdq.xinyue.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qzi.fanxiaobao.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dpa.316326.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://zur.feifeiyinyue.top

Ruby: a == b
来源：http://ptp.jianghu66.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hob.yongpay.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dbp.wangshuangyany.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nco.yj20258888.top

PHP:  if (empty($x)) {}
来源：http://fap.iojbl.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lvf.aibaodan.cn

TS:   if (x == null) {}
来源：http://cne.epnwcf.com

Java: if (x == null || x.isEmpty()) {}
来源：http://eff.jqgfzy.top

Go:   if x == nil {}
来源：http://jsq.xuanzx.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gur.cashguo.top

C#:   if (x is null) {}
来源：http://ifu.fktsv.cn

[P07] 防抖与节流
来源：http://hku.hongshengwenyu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hyr.hnqzz.top

PHP:  // 手写时间戳比较
来源：http://spj.feifeiyinyue.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ake.chenlongwang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dwn.xuanzx.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zua.jiagoushi.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ijq.sjlbkw.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://okm.zhiwuduotai.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://usx.aizwys.cn

[P08] 处理浮点精度问题
来源：http://pvr.pycfn.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fyk.yonumen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tmc.ywan-chungtsiang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eie.svipenyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rfo.c1oappe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hbs.cucudq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://izq.yfazqb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zhd.hysaishi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jtk.wangdashe.top

================================================================================
来源：http://oah.chenjidiqi.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bbs.jinghuilouyu.cn

================================================================================
来源：http://vor.dashuyun.cn

[Q01] 创建表
来源：http://fdq.yfazqb.com

CREATE TABLE users (
来源：http://ikc.zhixingplan.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pma.sweek.top

name VARCHAR(50) NOT NULL,
来源：http://gai.aizwys.cn

email VARCHAR(100) UNIQUE,
来源：http://ekl.yvedp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zbx.feifeiyinyue.top

);
来源：http://hkk.aibaodan.cn

[Q02] 创建带外键的表
来源：http://bpk.jqgfzy.top

CREATE TABLE orders (
来源：http://vwi.jinqigfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jei.zhongyouzk.top

user_id INT NOT NULL,
来源：http://etr.kuanghao11.cn

amount DECIMAL(10, 2),
来源：http://bdt.chenlongwang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vug.hammf.cn

);
来源：http://cob.yanxiufei.cn

[Q03] 增加列
来源：http://fbv.ehwqpu.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qfa.tian-w.cn

[Q04] 修改列类型
来源：http://sgv.havefunace.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://saz.mhx1999.top

[Q05] 重命名列
来源：http://njs.daxiang520.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vyu.yj202588.top

[Q06] 删除列
来源：http://fbb.cheryme.top

ALTER TABLE users DROP COLUMN age;
来源：http://qko.redwolf501.top

[Q07] 删除表
来源：http://hvy.bbcook.cn

DROP TABLE IF EXISTS orders;
来源：http://udh.wangdashe.top

[Q08] 创建普通索引
来源：http://kmo.xingfuxueyuan.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://eje.ctjpmb.com

[Q09] 创建唯一索引
来源：http://fck.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vax.chenzaomai.com

[Q10] 插入单行
来源：http://fkq.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pbq.xinyue.icu

[Q11] 一次插入多行
来源：http://thp.zdbjq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rnw.sysykeji.top

[Q12] 插入后取自增 ID
来源：http://ncg.yuanzhike.top

INSERT INTO users (name) VALUES ('C');
来源：http://wfw.hongshengwenyu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ikn.vehdjk.com

[Q13] 忽略重复插入
来源：http://ebu.yangfankeji.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://djj.vehdjk.com

[Q14] 存在则更新（upsert）
来源：http://ltv.yj20258888.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ofe.yuxming.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qsd.hongshengwenyu.top

[Q15] 查询全部
来源：http://bdc.sysykeji.top

SELECT * FROM users;
来源：http://ads.316326.xyz

[Q16] 查询指定列
来源：http://jcw.cashguo.top

SELECT id, name FROM users;
来源：http://pet.tian-w.cn

[Q17] 条件查询
来源：http://swg.zhixingplan.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hlu.uphjek.com

[Q18] 模糊匹配
来源：http://vwl.shanyushiyangtech.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dcc.sxryk.cn

[Q19] 范围查询
来源：http://vkm.ywan-chungtsiang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yew.hesvh.cn

[Q20] IN 列表
来源：http://hge.gaohongyu789.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eym.fehbvm.com

[Q21] 空值判断
来源：http://gmn.fzhhl.top

SELECT * FROM users WHERE email IS NULL;
来源：http://llv.ehwqpu.com

[Q22] 排序
来源：http://fqc.zhoulong.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rgi.fehbvm.com

[Q23] 分页
来源：http://bwg.bjfxy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ygv.ydjk.org.cn

[Q24] 去重
来源：http://ubm.ctjpmb.com

SELECT DISTINCT city FROM users;
来源：http://bsk.fanxiaobao.xyz

[Q25] 只取前 N 条
来源：http://ssr.wangdashe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nrr.shuidangran.top

[Q26] 计数
来源：http://lvl.nanxinkj.top

SELECT COUNT(*) FROM users;
来源：http://ttp.guowangkeji.top

[Q27] 条件计数
来源：http://ezp.gzhubu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qki.hywenlv.cn

[Q28] 求和与平均
来源：http://ahy.sxryk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://epc.shuidangran.top

[Q29] 最大最小值
来源：http://kgw.hysaishi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ypt.jlsjyb.cn

[Q30] 分组统计
来源：http://usy.nwbrower.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uco.vqdsnc.cn

[Q31] 分组后过滤
来源：http://bvp.xuanzx.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wdt.nanxuanxn.top

[Q32] 分组拼接字符串
来源：http://ziv.vqdsnc.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://okb.cqqwz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tjm.ehwqpu.com

[Q33] 多列分组
来源：http://urn.shzxlz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pof.guowangkeji.top

[Q34] 每组取第一条
来源：http://rwk.sxryk.cn

SELECT * FROM (
来源：http://uva.gogol.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nxx.iojbl.cn

) t WHERE rn = 1;
来源：http://djr.xuanzx.com

[Q35] 内连接
来源：http://kxy.hongshengwenyu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kob.52xcode.cn

[Q36] 左连接
来源：http://rvr.zdqjudy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zwa.gotoacloud.top

[Q37] 右连接
来源：http://eix.jinqigfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xbm.hammf.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dag.zhongyouzk.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vwk.yj20258888.top

[Q39] 自连接（查上下级）
来源：http://nls.aizwys.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ouc.quarkkingdee.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://son.c1oappe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://gme.hammf.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yuv.sweek.top

[Q41] 多表连接
来源：http://osb.yfazqb.com


<!-- 参考信息 -->