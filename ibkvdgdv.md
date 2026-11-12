代发 wailian999

[N05] 最大公约数
来源：http://eqv.nanxuanxn.top

Py:   math.gcd(a, b)
来源：http://rng.dashuyun.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qrm.epnwcf.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wln.cucudq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kln.yueranfly.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bwa.shanyushiyangkeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gqn.cdnleiting.top

Ruby: a.gcd(b)
来源：http://ier.sysykeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nfi.ybcxt.top

[N06] 判断回文字符串
来源：http://hnl.yonumen.top

Py:   s == s[::-1]
来源：http://imf.aizwys.cn

PHP:  $s === strrev($s);
来源：http://zzf.pengpengdd.cyou

JS:   s === [...s].reverse().join("")
来源：http://gpq.hnqzz.top

TS:   s === [...s].reverse().join("")
来源：http://qvh.ehwqpu.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kve.hesvh.cn

Go:   // 双指针从两端比较
来源：http://emi.zhiwuduotai.top

Ruby: s == s.reverse
来源：http://gbt.xuetiantiany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://omn.zhaomingkeji.xyz

[N07] 两数之和（返回下标）
来源：http://hmu.redwolf501.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uvh.cheryme.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://elj.fanxiaobao.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://rda.redwolf501.top

TS:   // 手写 Map<string, number>
来源：http://ahw.cdnleiting.top

Java: // 手写 HashMap
来源：http://ski.daria6918.cn

Go:   // 手写 map[int]int
来源：http://mzr.bjfxy.top

Ruby: // 手写 Hash
来源：http://gtg.sxryk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ljp.xuetiantiany.cn

[N08] 生成全排列
来源：http://pyq.jinghuilouyu.cn

Py:   itertools.permutations(arr)
来源：http://kzk.zhijiandao.cn

PHP:  // 手写递归交换
来源：http://qtf.wangdashe.top

JS:   // 手写回溯递归
来源：http://hry.feifeiyinyue.top

TS:   // 手写回溯递归
来源：http://clx.xingfuxueyuan.xyz

Java: // 手写回溯递归
来源：http://kte.tanke756.top

Go:   // 手写回溯递归
来源：http://mdl.shangyingyoupin.top

Ruby: arr.permutation.to_a
来源：http://aof.yongpay.top

C#:   // 手写回溯递归
来源：http://uwr.zhengqikj.top

[N09] 栈与队列
来源：http://kwe.cucudq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://syi.yuxming.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fsa.guannengcc.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vqv.redwolf501.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://snc.xuetiantiany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mhq.nanxinkj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ijo.xinyue.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gij.shanyushiyangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://frv.jqgfzy.top

[N10] 链表节点定义
来源：http://uxl.epnwcf.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://luj.sxryk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kze.ppjwa.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ylg.sxryk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zve.zhijiandao.cn

Java: class Node { int v; Node next; }
来源：http://jsu.0kj1m.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wty.gzhubu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://pev.yfazqb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://yyh.yfazqb.com

[N11] 二叉树中序遍历
来源：http://kia.jinqigfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vrr.zdbjq.cn

PHP:  // 手写递归函数
来源：http://axn.zhongyouzk.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pvo.chenlongwang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zop.meibo888.top

Java: // 手写递归
来源：http://phl.yongpay.top

Go:   // 手写递归
来源：http://hol.pycfn.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sqk.zhongyouzk.top

C#:   // 手写递归
来源：http://ght.yj20258.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vce.jiagoushi.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bjf.shangyingyoupin.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fwd.sxryk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pcw.hcnkem.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jay.xinyue.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jwz.hfpthk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://izd.hnxiangtu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uoa.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ggd.yuxming.cn

================================================================================
来源：http://wlw.52xcode.cn

O. 并发与异步
来源：http://dvt.hywenlv.cn

================================================================================
来源：http://tyl.jiagoushi.top

[O01] 启动一个线程
来源：http://tun.jiagoushi.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://phr.guannengcc.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gzv.yonumen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jxo.cashguo.top

TS:   // 同 JS
来源：http://nhr.yueranfly.top

Java: new Thread(() -> f()).start()
来源：http://kbc.52xcode.cn

Go:   go f()
来源：http://rra.snrcjt.cn

Ruby: Thread.new { f }
来源：http://wuo.fanxiaobao.xyz

C#:   Task.Run(() => F());
来源：http://kam.hnxiangtu.top

[O02] 使用线程池
来源：http://qou.tian-w.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uos.yongpay.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wav.xziqi.cn

JS:   // worker_threads 线程池
来源：http://vcg.fehbvm.com

TS:   // worker_threads 线程池
来源：http://vpa.jyoumei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yhn.smart0.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xvr.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eef.chenzaomai.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pak.ehwqpu.com

[O03] 加锁保护共享数据
来源：http://qfy.yvedp.cn

Py:   with lock: shared += 1
来源：http://hdb.chenzaomai.com

PHP:  // 用 flock() 做文件锁
来源：http://efq.zdbjq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wni.shzxlz.cn

TS:   // 同 JS
来源：http://pcl.zycfv.cn

Java: synchronized (this) { shared++; }
来源：http://wap.fengsongda.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hip.0kj1m.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://trf.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://suq.dashuyun.cn

[O04] 定义异步函数并等待
来源：http://bjc.jiagoushi.top

Py:   async def f():⏎    await g()
来源：http://atg.daxiang520.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://arg.yonumen.top

JS:   async function f() { await g(); }
来源：http://eqm.meibo888.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://iva.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uga.zhiwuduotai.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mgq.svipenyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ysk.mhx1999.top

C#:   async Task F() { await G(); }
来源：http://nvs.ydjk.org.cn

[O05] 并发执行并等待全部完成
来源：http://tsb.shangyingyoupin.top

Py:   asyncio.gather(*tasks)
来源：http://wxy.yfazqb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eyg.yj20258.top

JS:   await Promise.all(tasks)
来源：http://hpq.chenzaomai.com

TS:   await Promise.all(tasks)
来源：http://xjg.shangyingyoupin.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zez.0kj1m.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nrt.ydzc1.top

Ruby: threads.map(&:join)
来源：http://qqq.xuetiantiany.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qlo.quarkkingdee.top

[O06] 使用进程池
来源：http://sur.xylfe.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jfj.ehwqpu.com

PHP:  // pcntl_fork 或多进程队列
来源：http://als.xuanzx.com

JS:   // child_process / cluster 模块
来源：http://cte.hywenlv.cn

TS:   // child_process / cluster 模块
来源：http://ugo.yj20258.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://huv.shanyushiyangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nhi.ywan-chungtsiang.top

Ruby: // fork 块
来源：http://cjb.yj20258888.top

C#:   Parallel.For
来源：http://qqa.zhiwuduotai.top

================================================================================
来源：http://ltj.yanxiufei.cn

P. 常用工具函数
来源：http://yrq.sjlbkw.cn

================================================================================
来源：http://kbi.ydjk.org.cn

[P01] 生成 UUID
来源：http://dta.jqgufenzy.top

Py:   str(uuid.uuid4())
来源：http://ldf.xuanzx.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vbp.xingfuxueyuan.xyz

JS:   crypto.randomUUID()
来源：http://qdk.jinyuanbaomall.cn

TS:   crypto.randomUUID()
来源：http://zkx.zhengqikj.top

Java: UUID.randomUUID().toString()
来源：http://hub.zhengqikj.top

Go:   // 用 github.com/google/uuid
来源：http://wcs.cucudq.cn

Ruby: SecureRandom.uuid
来源：http://qyr.fehbvm.com

C#:   Guid.NewGuid().ToString()
来源：http://sii.redwolf501.top

[P02] MD5 / SHA256 摘要
来源：http://idm.xuetiantiany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://skq.haohaochexian.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://obq.xylfe.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ton.zhiwuduotai.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cuw.hcnkem.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xwo.yuxming.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gkv.fanxiaobao.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://myp.kuanghao11.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fvi.epnwcf.com

[P03] 生成短随机字符串
来源：http://crp.zhoulong.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://viy.zhaomingkeji.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ghq.dianchejie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fzb.zdbjq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jja.jyoumei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ert.52xcode.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hzb.chenzaomai.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://bnn.tianlin.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fob.cdnleiting.top

[P04] 求长度
来源：http://tsx.daxiang520.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rdu.cheryme.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dsx.tianlin.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ilz.sufxvd.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rhl.gaohongyu789.top

Java: list.size();  map.size();  s.length()
来源：http://uve.kuanghao11.cn

Go:   len(arr);  len(m)
来源：http://nau.ivvv.top

Ruby: x.length;  x.size
来源：http://bah.yj202588.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://mij.zdbjq.cn

[P05] 判断两个对象内容是否相等
来源：http://emc.aibaodan.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hmz.meibo888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ukz.hcnkem.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xqt.shzxlz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jtg.gotoacloud.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xtg.jiagoushi.top

Go:   reflect.DeepEqual(a, b)
来源：http://vma.yanxiufei.cn

Ruby: a == b
来源：http://hbr.tian-w.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://psb.hnxiangtu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://txe.iojbl.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gpt.jianghu66.top

PHP:  if (empty($x)) {}
来源：http://bux.yj202588.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fet.cqqwz.cn

TS:   if (x == null) {}
来源：http://gcp.cqqwz.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gfg.quarkkingdee.top

Go:   if x == nil {}
来源：http://fnm.tarul.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lkk.yj202588.top

C#:   if (x is null) {}
来源：http://zws.yongpay.top

[P07] 防抖与节流
来源：http://bns.iojbl.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ktx.sxryk.cn

PHP:  // 手写时间戳比较
来源：http://mgo.guannengcc.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kfe.bjfxy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ymo.52xcode.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mbi.hesvh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xqe.jinyuanbaomall.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cfe.pycfn.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fmd.zhijiandao.cn

[P08] 处理浮点精度问题
来源：http://ubd.jqgfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rvb.shzxlz.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kin.52xcode.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wqv.jinqigfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baz.ctjpmb.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hvs.yongpay.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xry.52xcode.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://caq.birdmap.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mvo.fengsongda.top

================================================================================
来源：http://lrz.haohaochexian.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vto.feifeiyinyue.top

================================================================================
来源：http://iol.9152youxi.cn

[Q01] 创建表
来源：http://gon.tarul.cn

CREATE TABLE users (
来源：http://bil.jinghuilouyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ero.jqgfzy.top

name VARCHAR(50) NOT NULL,
来源：http://mbq.sweek.top

email VARCHAR(100) UNIQUE,
来源：http://ttd.ydzc1.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hcv.meibo888.top

);
来源：http://jgf.cdnleiting.top

[Q02] 创建带外键的表
来源：http://xon.ehwqpu.com

CREATE TABLE orders (
来源：http://gcj.hongshengwenyu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://afp.hesvh.cn

user_id INT NOT NULL,
来源：http://bep.svipenyu.cn

amount DECIMAL(10, 2),
来源：http://yfp.sxryk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xoj.zhaomingkeji.xyz

);
来源：http://nkx.bjfxy.top

[Q03] 增加列
来源：http://ory.xziqi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jrm.ywan-chungtsiang.top

[Q04] 修改列类型
来源：http://ibf.meibo888.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ymo.daxiang520.top

[Q05] 重命名列
来源：http://dpw.kuanghao11.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kod.pycfn.com

[Q06] 删除列
来源：http://hpd.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://wfl.tanke756.top

[Q07] 删除表
来源：http://ovh.jqgfzy.top

DROP TABLE IF EXISTS orders;
来源：http://kjj.gogol.net.cn

[Q08] 创建普通索引
来源：http://hwp.jqgfzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vnh.yfazqb.com

[Q09] 创建唯一索引
来源：http://aav.gotoacloud.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mub.ydzc1.top

[Q10] 插入单行
来源：http://jfj.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iti.dianchejie.cn

[Q11] 一次插入多行
来源：http://tsr.fktsv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zux.zhijiandao.cn

[Q12] 插入后取自增 ID
来源：http://lje.chenjidiqi.icu

INSERT INTO users (name) VALUES ('C');
来源：http://gqw.316326.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://foc.meibo888.top

[Q13] 忽略重复插入
来源：http://jxw.yanxiufei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pxa.jiagoushi.top

[Q14] 存在则更新（upsert）
来源：http://eks.feifeiyinyue.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ftn.316326.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wvq.zhiwuduotai.top

[Q15] 查询全部
来源：http://pjp.52xcode.cn

SELECT * FROM users;
来源：http://ajp.hysaishi.cn

[Q16] 查询指定列
来源：http://nha.epnwcf.com

SELECT id, name FROM users;
来源：http://gyi.hammf.cn

[Q17] 条件查询
来源：http://gwm.hfpthk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://syt.hywenlv.cn

[Q18] 模糊匹配
来源：http://qul.zhijiandao.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nmz.fktsv.cn

[Q19] 范围查询
来源：http://gkl.guannengcc.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hxy.yongpay.top

[Q20] IN 列表
来源：http://dio.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vbo.xziqi.cn

[Q21] 空值判断
来源：http://qqj.yvedp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ppz.zdqjudy.top

[Q22] 排序
来源：http://jcv.svipenyu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fkz.wangshuangyany.cn

[Q23] 分页
来源：http://spq.316326.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tww.zycfv.cn

[Q24] 去重
来源：http://ray.havefunace.top

SELECT DISTINCT city FROM users;
来源：http://aph.andypj.xyz

[Q25] 只取前 N 条
来源：http://uam.zhaomingkeji.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wzw.hongshengwenyu.top

[Q26] 计数
来源：http://tug.kuanghao11.cn

SELECT COUNT(*) FROM users;
来源：http://bjj.chenzaomai.com

[Q27] 条件计数
来源：http://scp.jyoumei.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vtd.dashuyun.cn

[Q28] 求和与平均
来源：http://zqq.jqgufenzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fxg.ywan-chungtsiang.top

[Q29] 最大最小值
来源：http://ers.ehwqpu.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://jet.tanke756.top

[Q30] 分组统计
来源：http://tlq.zycfv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://svg.zhengqikj.top

[Q31] 分组后过滤
来源：http://qot.zdqjudy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sox.gogol.net.cn

[Q32] 分组拼接字符串
来源：http://dqv.shuidangran.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nri.zhixingplan.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tjx.yonumen.top

[Q33] 多列分组
来源：http://xsz.fengsongda.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://olj.ctjpmb.com

[Q34] 每组取第一条
来源：http://hpg.yj20258888.top

SELECT * FROM (
来源：http://how.zhijiandao.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hrl.havefunace.top

) t WHERE rn = 1;
来源：http://hna.guannengcc.top

[Q35] 内连接
来源：http://pxm.nanxinkj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://arl.dashuyun.cn

[Q36] 左连接
来源：http://zfv.jinqigfzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rul.52xcode.cn

[Q37] 右连接
来源：http://btd.jlsjyb.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gcg.zhongyouzk.top

[Q38] 全外连接（PostgreSQL）
来源：http://bes.guowangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xrp.xingfuxueyuan.xyz

[Q39] 自连接（查上下级）
来源：http://scw.yvedp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zvz.tian-w.cn


<!-- 参考信息 -->