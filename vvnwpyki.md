代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lyu.nanxuanxn.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://frv.xinyue.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kio.xylfe.cn

Ruby: a.gcd(b)
来源：http://aua.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eaw.yongpay.top

[N06] 判断回文字符串
来源：http://obh.kuanghao11.cn

Py:   s == s[::-1]
来源：http://vus.shanyushiyangkeji.top

PHP:  $s === strrev($s);
来源：http://cos.shanyushiyangtech.top

JS:   s === [...s].reverse().join("")
来源：http://lkq.hnqzz.top

TS:   s === [...s].reverse().join("")
来源：http://ttw.fengsongda.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ooz.sxryk.cn

Go:   // 双指针从两端比较
来源：http://yrm.fehbvm.com

Ruby: s == s.reverse
来源：http://hmy.mhx1999.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mjc.hfpthk.cn

[N07] 两数之和（返回下标）
来源：http://tuf.xziqi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dos.hesvh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yjg.yj202588.top

JS:   // 手写 Map：map.set(v, i)
来源：http://stt.jianghu66.top

TS:   // 手写 Map<string, number>
来源：http://jag.yueranfly.top

Java: // 手写 HashMap
来源：http://tjn.sufxvd.cn

Go:   // 手写 map[int]int
来源：http://qpz.yangfankeji.com

Ruby: // 手写 Hash
来源：http://xgq.ppjwa.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jmr.hongshengwenyu.top

[N08] 生成全排列
来源：http://gtk.hysaishi.cn

Py:   itertools.permutations(arr)
来源：http://psy.ivvv.top

PHP:  // 手写递归交换
来源：http://blx.hysaishi.cn

JS:   // 手写回溯递归
来源：http://xud.aizwys.cn

TS:   // 手写回溯递归
来源：http://tqb.pycfn.com

Java: // 手写回溯递归
来源：http://kuo.xuetiantiany.cn

Go:   // 手写回溯递归
来源：http://rva.shuidangran.top

Ruby: arr.permutation.to_a
来源：http://bxt.sweek.top

C#:   // 手写回溯递归
来源：http://cof.sysykeji.top

[N09] 栈与队列
来源：http://kqs.0kj1m.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://usd.xylfe.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qfd.gzhubu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ype.uphjek.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gpg.cdnleiting.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://btl.haohaochexian.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ogj.gogol.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://buy.ydjk.org.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pmv.vqdsnc.cn

[N10] 链表节点定义
来源：http://twt.pengpengdd.cyou

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zlb.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tls.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://srv.tian-w.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lia.xingfuxueyuan.xyz

Java: class Node { int v; Node next; }
来源：http://xmq.jinyuanbaomall.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gxm.hnqzz.top

Ruby: Node = Struct.new(:v, :next)
来源：http://arp.zhixingplan.top

C#:   class Node { public int V; public Node? Next; }
来源：http://eia.316326.xyz

[N11] 二叉树中序遍历
来源：http://lbs.jianghu66.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mpy.yfazqb.com

PHP:  // 手写递归函数
来源：http://bwc.zhijiandao.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ftv.nanxuanxn.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qic.xuanzx.com

Java: // 手写递归
来源：http://ztr.fktsv.cn

Go:   // 手写递归
来源：http://mlx.yuxming.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://niu.jiagoushi.top

C#:   // 手写递归
来源：http://hyw.hysaishi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gmr.tianlin.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qza.ivvv.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://caj.zhengqikj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://abv.havefunace.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vyf.vqdsnc.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vsu.zhaomingkeji.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ehm.shanyushiyangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xvz.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wev.gotoacloud.top

================================================================================
来源：http://khx.ppjwa.cn

O. 并发与异步
来源：http://qxq.daxiang520.top

================================================================================
来源：http://pqe.zhengqikj.top

[O01] 启动一个线程
来源：http://slg.daria6918.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://onq.nanxinkj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kwg.9152youxi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hmx.gotoacloud.top

TS:   // 同 JS
来源：http://iqv.cheryme.top

Java: new Thread(() -> f()).start()
来源：http://ozy.zhijiandao.cn

Go:   go f()
来源：http://bas.feifeiyinyue.top

Ruby: Thread.new { f }
来源：http://pxw.zdqjudy.top

C#:   Task.Run(() => F());
来源：http://olr.vehdjk.com

[O02] 使用线程池
来源：http://zuc.shzxlz.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rih.hammf.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://smi.nanxuanxn.top

JS:   // worker_threads 线程池
来源：http://gyj.fktsv.cn

TS:   // worker_threads 线程池
来源：http://gde.yj20258.top

Java: Executors.newFixedThreadPool(4)
来源：http://qlm.andypj.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lia.aibaodan.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ohq.nwbrower.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://idf.gotoacloud.top

[O03] 加锁保护共享数据
来源：http://qte.jinqigfzy.top

Py:   with lock: shared += 1
来源：http://fhx.dianchejie.cn

PHP:  // 用 flock() 做文件锁
来源：http://hoa.ywan-chungtsiang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zpj.sweek.top

TS:   // 同 JS
来源：http://iwh.tian-w.cn

Java: synchronized (this) { shared++; }
来源：http://der.chenlongwang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lfr.jinqigfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qfb.yj20258.top

C#:   lock (gate) { shared++; }
来源：http://jaf.haohaochexian.top

[O04] 定义异步函数并等待
来源：http://urb.tian-w.cn

Py:   async def f():⏎    await g()
来源：http://nph.guannengcc.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uoc.quarkkingdee.top

JS:   async function f() { await g(); }
来源：http://urs.dashuyun.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fod.sufxvd.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tbo.fzhhl.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wcq.chenzaomai.com

Ruby: # 用 Fiber 或 async gem
来源：http://xfi.shuidangran.top

C#:   async Task F() { await G(); }
来源：http://ovt.ybcxt.top

[O05] 并发执行并等待全部完成
来源：http://pqj.snrcjt.cn

Py:   asyncio.gather(*tasks)
来源：http://vnx.xziqi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xio.vehdjk.com

JS:   await Promise.all(tasks)
来源：http://cfi.hfpthk.cn

TS:   await Promise.all(tasks)
来源：http://qwg.vehdjk.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zbb.xylfe.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mzk.iojbl.cn

Ruby: threads.map(&:join)
来源：http://lne.meibo888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xlx.chenlongwang.top

[O06] 使用进程池
来源：http://tsr.sxryk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lvt.xziqi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zuz.svipenyu.cn

JS:   // child_process / cluster 模块
来源：http://sxd.xuetiantiany.cn

TS:   // child_process / cluster 模块
来源：http://ozn.hfpthk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sdl.svipenyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qpe.ydzc1.top

Ruby: // fork 块
来源：http://auy.yongpay.top

C#:   Parallel.For
来源：http://miz.nanxuanxn.top

================================================================================
来源：http://zpu.uphjek.com

P. 常用工具函数
来源：http://zwh.dashuyun.cn

================================================================================
来源：http://ooi.hysaishi.cn

[P01] 生成 UUID
来源：http://tzd.xziqi.cn

Py:   str(uuid.uuid4())
来源：http://qof.zhaomingkeji.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yzm.yonumen.top

JS:   crypto.randomUUID()
来源：http://lkv.ywan-chungtsiang.top

TS:   crypto.randomUUID()
来源：http://iik.cdnleiting.top

Java: UUID.randomUUID().toString()
来源：http://fkp.svipenyu.cn

Go:   // 用 github.com/google/uuid
来源：http://xgj.zdqjudy.top

Ruby: SecureRandom.uuid
来源：http://mlh.sxryk.cn

C#:   Guid.NewGuid().ToString()
来源：http://bgt.ehwqpu.com

[P02] MD5 / SHA256 摘要
来源：http://pyr.cashguo.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lbf.guannengcc.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://kos.feifeiyinyue.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ecy.cucudq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qvk.jlsjyb.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cly.guowangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cgg.zhengqikj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hwm.wangdashe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bjx.xziqi.cn

[P03] 生成短随机字符串
来源：http://agj.hnqzz.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ulf.tanke756.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uhe.quarkkingdee.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://myh.jlsjyb.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pqv.smart0.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hgd.yanxiufei.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wkw.bjfxy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://umt.zhiwuduotai.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ckd.jyoumei.cn

[P04] 求长度
来源：http://aos.yj20258.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lvw.cashguo.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cqo.snrcjt.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qin.wangshuangyany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xxo.0kj1m.cn

Java: list.size();  map.size();  s.length()
来源：http://qya.chenlongwang.top

Go:   len(arr);  len(m)
来源：http://erm.uphjek.com

Ruby: x.length;  x.size
来源：http://xak.iojbl.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hed.xingfuxueyuan.xyz

[P05] 判断两个对象内容是否相等
来源：http://rzc.xinyue.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://xcd.sysykeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bac.wangdashe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bdn.hcnkem.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://njs.jiagoushi.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yot.xuetiantiany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vwn.feifeiyinyue.top

Ruby: a == b
来源：http://tge.hywenlv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lev.shanyushiyangtech.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pzg.zhijiandao.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zfy.wangdashe.top

PHP:  if (empty($x)) {}
来源：http://vla.zdqjudy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hvh.tanke756.top

TS:   if (x == null) {}
来源：http://zeg.316326.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://npo.sufxvd.cn

Go:   if x == nil {}
来源：http://ilp.yfazqb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vuf.redwolf501.top

C#:   if (x is null) {}
来源：http://ucf.zhengqikj.top

[P07] 防抖与节流
来源：http://rsb.fehbvm.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pzz.yanxiufei.cn

PHP:  // 手写时间戳比较
来源：http://bja.hongshengwenyu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ott.shzxlz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lug.iojbl.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qlf.redwolf501.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://atj.yueranfly.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://byr.gotoacloud.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://drj.jyoumei.cn

[P08] 处理浮点精度问题
来源：http://vxy.iojbl.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fpf.bbcook.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fvt.zdqjudy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wha.epnwcf.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://whx.ywan-chungtsiang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vcs.uphjek.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uke.zhixingplan.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://izh.svipenyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xjn.ydzc1.top

================================================================================
来源：http://zkm.wangshuangyany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://njp.bjfxy.top

================================================================================
来源：http://zoo.fzhhl.top

[Q01] 创建表
来源：http://agv.zhixingplan.top

CREATE TABLE users (
来源：http://tsp.316326.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hyr.snrcjt.cn

name VARCHAR(50) NOT NULL,
来源：http://ggg.9152youxi.cn

email VARCHAR(100) UNIQUE,
来源：http://unl.zhixingplan.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ent.wangshuangyany.cn

);
来源：http://uwx.yueranfly.top

[Q02] 创建带外键的表
来源：http://pwm.ydzc1.top

CREATE TABLE orders (
来源：http://sbu.bjfxy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ovx.yongpay.top

user_id INT NOT NULL,
来源：http://lul.jqgufenzy.top

amount DECIMAL(10, 2),
来源：http://qdu.hnxiangtu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fco.fktsv.cn

);
来源：http://gvn.dashuyun.cn

[Q03] 增加列
来源：http://xki.xuanzx.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qeu.kuanghao11.cn

[Q04] 修改列类型
来源：http://mff.smart0.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tgw.zdqjudy.top

[Q05] 重命名列
来源：http://zmy.jlsjyb.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bfc.pengpengdd.cyou

[Q06] 删除列
来源：http://jfc.hesvh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://iae.sxryk.cn

[Q07] 删除表
来源：http://vpr.jiagoushi.top

DROP TABLE IF EXISTS orders;
来源：http://jyc.xingfuxueyuan.xyz

[Q08] 创建普通索引
来源：http://wbn.xuetiantiany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tyv.fanxiaobao.xyz

[Q09] 创建唯一索引
来源：http://kru.shzxlz.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ubz.hongshengwenyu.top

[Q10] 插入单行
来源：http://vwn.fktsv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lvt.dashuyun.cn

[Q11] 一次插入多行
来源：http://cyw.sjlbkw.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jbi.meibo888.top

[Q12] 插入后取自增 ID
来源：http://jzm.ywan-chungtsiang.top

INSERT INTO users (name) VALUES ('C');
来源：http://kad.cheryme.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oxv.yonumen.top

[Q13] 忽略重复插入
来源：http://crv.0kj1m.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://klw.havefunace.top

[Q14] 存在则更新（upsert）
来源：http://vet.pycfn.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dfb.hesvh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uet.haohaochexian.top

[Q15] 查询全部
来源：http://hju.sxryk.cn

SELECT * FROM users;
来源：http://bde.zycfv.cn

[Q16] 查询指定列
来源：http://ocj.hnxiangtu.top

SELECT id, name FROM users;
来源：http://ohk.dianchejie.cn

[Q17] 条件查询
来源：http://gdz.ydjk.org.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fak.redwolf501.top

[Q18] 模糊匹配
来源：http://kxq.jlsjyb.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hpk.haohaochexian.top

[Q19] 范围查询
来源：http://kyf.vehdjk.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cgp.zhaomingkeji.xyz

[Q20] IN 列表
来源：http://uxi.daxiang520.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hcl.zhixingplan.top

[Q21] 空值判断
来源：http://jje.mhx1999.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rqy.yonumen.top

[Q22] 排序
来源：http://pqn.fktsv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cwm.aibaodan.cn

[Q23] 分页
来源：http://efw.epnwcf.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tyy.jiagoushi.top

[Q24] 去重
来源：http://azr.cdnleiting.top

SELECT DISTINCT city FROM users;
来源：http://mtz.shangyingyoupin.top

[Q25] 只取前 N 条
来源：http://hqs.aibaodan.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nwl.jinghuilouyu.cn

[Q26] 计数
来源：http://rsv.feifeiyinyue.top

SELECT COUNT(*) FROM users;
来源：http://olq.ivvv.top

[Q27] 条件计数
来源：http://uam.hysaishi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xhd.shzxlz.cn

[Q28] 求和与平均
来源：http://scz.52xcode.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ahq.zhixingplan.top

[Q29] 最大最小值
来源：http://bxt.ehwqpu.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://yqu.jinghuilouyu.cn

[Q30] 分组统计
来源：http://xde.snrcjt.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qjw.hammf.cn

[Q31] 分组后过滤
来源：http://hoz.feifeiyinyue.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bij.wangshuangyany.cn

[Q32] 分组拼接字符串
来源：http://evq.feifeiyinyue.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nux.hongshengwenyu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xex.uphjek.com

[Q33] 多列分组
来源：http://hgc.zhoulong.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xzp.ivvv.top

[Q34] 每组取第一条
来源：http://beh.yangfankeji.com

SELECT * FROM (
来源：http://dbg.uphjek.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ywr.ctjpmb.com

) t WHERE rn = 1;
来源：http://dnj.hysaishi.cn

[Q35] 内连接
来源：http://zjv.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tji.sweek.top

[Q36] 左连接
来源：http://erz.hysaishi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://anv.fengsongda.top

[Q37] 右连接
来源：http://fzr.gzhubu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nzi.xylfe.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qfz.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://drb.cheryme.top

[Q39] 自连接（查上下级）
来源：http://tzp.yuanzhike.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zzp.zhaomingkeji.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dlk.hcnkem.com

[Q40] 交叉连接（笛卡尔积）
来源：http://ccx.fktsv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://npm.tian-w.cn

[Q41] 多表连接
来源：http://udk.meibo888.top


<!-- 参考信息 -->