代发 wailian999

[N05] 最大公约数
来源：http://rcg.daxiang520.top

Py:   math.gcd(a, b)
来源：http://wbf.svipenyu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zlx.fengsongda.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qse.sweek.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yhc.gogol.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ghw.sjlbkw.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iba.hongshengwenyu.top

Ruby: a.gcd(b)
来源：http://zgy.gotoacloud.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jsv.sufxvd.cn

[N06] 判断回文字符串
来源：http://khi.chenzaomai.com

Py:   s == s[::-1]
来源：http://tuy.jqgufenzy.top

PHP:  $s === strrev($s);
来源：http://jzf.dianchejie.cn

JS:   s === [...s].reverse().join("")
来源：http://xab.shuidangran.top

TS:   s === [...s].reverse().join("")
来源：http://yoc.meibo888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://azx.hcnkem.com

Go:   // 双指针从两端比较
来源：http://kuy.yuanzhike.top

Ruby: s == s.reverse
来源：http://vdk.shanyushiyangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://sru.yj20258.top

[N07] 两数之和（返回下标）
来源：http://wou.yangfankeji.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vrp.tian-w.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://esg.gotoacloud.top

JS:   // 手写 Map：map.set(v, i)
来源：http://eom.fzhhl.top

TS:   // 手写 Map<string, number>
来源：http://oyf.hammf.cn

Java: // 手写 HashMap
来源：http://ooh.birdmap.top

Go:   // 手写 map[int]int
来源：http://osv.sweek.top

Ruby: // 手写 Hash
来源：http://cbh.sjlbkw.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ngy.uphjek.com

[N08] 生成全排列
来源：http://iuq.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://lel.sjlbkw.cn

PHP:  // 手写递归交换
来源：http://ljh.guowangkeji.top

JS:   // 手写回溯递归
来源：http://nvv.sxryk.cn

TS:   // 手写回溯递归
来源：http://tvy.ydzc1.top

Java: // 手写回溯递归
来源：http://ihy.snrcjt.cn

Go:   // 手写回溯递归
来源：http://oyv.zhongyouzk.top

Ruby: arr.permutation.to_a
来源：http://tms.dashuyun.cn

C#:   // 手写回溯递归
来源：http://zbt.meibo888.top

[N09] 栈与队列
来源：http://ree.316326.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dmx.fzhhl.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yon.gotoacloud.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zdo.ctjpmb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zdd.cheryme.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bso.daria6918.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tqq.0kj1m.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lda.aibaodan.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vpo.ctjpmb.com

[N10] 链表节点定义
来源：http://xft.yongpay.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rht.jlsjyb.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vgo.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jjx.wangdashe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nzo.jinyuanbaomall.cn

Java: class Node { int v; Node next; }
来源：http://pns.yueranfly.top

Go:   type Node struct { V int; Next *Node }
来源：http://fxu.jqgufenzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://brw.shuidangran.top

C#:   class Node { public int V; public Node? Next; }
来源：http://nnw.hfpthk.cn

[N11] 二叉树中序遍历
来源：http://ygw.tian-w.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://meb.sysykeji.top

PHP:  // 手写递归函数
来源：http://uxg.haohaochexian.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mgv.hesvh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qgp.wangdashe.top

Java: // 手写递归
来源：http://ism.jinqigufen.top

Go:   // 手写递归
来源：http://jfl.gaohongyu789.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zca.yuxming.cn

C#:   // 手写递归
来源：http://rbt.ppjwa.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zub.tian-w.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zxl.hnxiangtu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rqx.ctjpmb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hls.fehbvm.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hpr.yonumen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jyn.jinyuanbaomall.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lvp.wangshuangyany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://suw.birdmap.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zbm.zhaomingkeji.xyz

================================================================================
来源：http://oyy.zhoulong.xyz

O. 并发与异步
来源：http://tko.tarul.cn

================================================================================
来源：http://vfw.316326.xyz

[O01] 启动一个线程
来源：http://twa.hywenlv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zit.hongshengwenyu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ogj.aibaodan.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qws.iojbl.cn

TS:   // 同 JS
来源：http://abj.feifeiyinyue.top

Java: new Thread(() -> f()).start()
来源：http://pkt.xuanzx.com

Go:   go f()
来源：http://vqd.xinyue.icu

Ruby: Thread.new { f }
来源：http://hpf.hnqzz.top

C#:   Task.Run(() => F());
来源：http://fym.fktsv.cn

[O02] 使用线程池
来源：http://cha.tianlin.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://foc.zhengqikj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rgf.xingfuxueyuan.xyz

JS:   // worker_threads 线程池
来源：http://nfc.zhijiandao.cn

TS:   // worker_threads 线程池
来源：http://inb.ppjwa.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nhc.ehwqpu.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oph.zhixingplan.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dug.hnxiangtu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tnc.daxiang520.top

[O03] 加锁保护共享数据
来源：http://yya.redwolf501.top

Py:   with lock: shared += 1
来源：http://htz.yuxming.cn

PHP:  // 用 flock() 做文件锁
来源：http://lca.bjfxy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rqz.0kj1m.cn

TS:   // 同 JS
来源：http://evn.wangdashe.top

Java: synchronized (this) { shared++; }
来源：http://ltw.cqqwz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://prx.hcnkem.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://qxy.gotoacloud.top

C#:   lock (gate) { shared++; }
来源：http://mkl.yanxiufei.cn

[O04] 定义异步函数并等待
来源：http://zrd.tarul.cn

Py:   async def f():⏎    await g()
来源：http://djq.9152youxi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://shn.jinyuanbaomall.cn

JS:   async function f() { await g(); }
来源：http://ons.hongshengwenyu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wrh.gzhubu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tha.jinyuanbaomall.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wbv.sufxvd.cn

Ruby: # 用 Fiber 或 async gem
来源：http://csf.yuxming.cn

C#:   async Task F() { await G(); }
来源：http://wth.xuetiantiany.cn

[O05] 并发执行并等待全部完成
来源：http://ruf.bbcook.cn

Py:   asyncio.gather(*tasks)
来源：http://mgl.jianghu66.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dge.yueranfly.top

JS:   await Promise.all(tasks)
来源：http://aaq.jinqigufen.top

TS:   await Promise.all(tasks)
来源：http://wkd.daria6918.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mer.jqgufenzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lqs.cheryme.top

Ruby: threads.map(&:join)
来源：http://pnb.sxryk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jie.fanxiaobao.xyz

[O06] 使用进程池
来源：http://dor.iojbl.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://roz.ybcxt.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nad.xinyue.icu

JS:   // child_process / cluster 模块
来源：http://yec.guannengcc.top

TS:   // child_process / cluster 模块
来源：http://bud.yueranfly.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vmm.cashguo.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rrv.tian-w.cn

Ruby: // fork 块
来源：http://cwu.yongpay.top

C#:   Parallel.For
来源：http://mdi.cheryme.top

================================================================================
来源：http://urw.hcnkem.com

P. 常用工具函数
来源：http://wvq.quarkkingdee.top

================================================================================
来源：http://tsp.snrcjt.cn

[P01] 生成 UUID
来源：http://gza.smart0.xyz

Py:   str(uuid.uuid4())
来源：http://kyf.cucudq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nue.fktsv.cn

JS:   crypto.randomUUID()
来源：http://tam.aibaodan.cn

TS:   crypto.randomUUID()
来源：http://snu.sufxvd.cn

Java: UUID.randomUUID().toString()
来源：http://ccm.hysaishi.cn

Go:   // 用 github.com/google/uuid
来源：http://xig.tarul.cn

Ruby: SecureRandom.uuid
来源：http://aoj.kuanghao11.cn

C#:   Guid.NewGuid().ToString()
来源：http://fpg.smart0.xyz

[P02] MD5 / SHA256 摘要
来源：http://slk.fanxiaobao.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ysi.gaohongyu789.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://rxo.c1oappe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jhs.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ngu.jyoumei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zaq.yj20258888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yqg.aibaodan.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xjj.nwbrower.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xwb.cashguo.top

[P03] 生成短随机字符串
来源：http://hps.ppjwa.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xuj.dianchejie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ysa.yangfankeji.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lxx.wangdashe.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dgf.uphjek.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xtr.pycfn.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ziz.gzhubu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gxg.hnxiangtu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wyd.xuetiantiany.cn

[P04] 求长度
来源：http://lxk.vehdjk.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wzi.zhijiandao.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rit.zhixingplan.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mbw.fehbvm.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ozx.ehwqpu.com

Java: list.size();  map.size();  s.length()
来源：http://jfp.yvedp.cn

Go:   len(arr);  len(m)
来源：http://ggo.yangfankeji.com

Ruby: x.length;  x.size
来源：http://kld.52xcode.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://uon.yueranfly.top

[P05] 判断两个对象内容是否相等
来源：http://yjr.hfpthk.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gqe.bbcook.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iyp.chenzaomai.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kop.yj202588.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ivj.zhixingplan.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xbe.ehwqpu.com

Go:   reflect.DeepEqual(a, b)
来源：http://esr.xuanzx.com

Ruby: a == b
来源：http://jmj.hfpthk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wqg.havefunace.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xux.yonumen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xvh.daxiang520.top

PHP:  if (empty($x)) {}
来源：http://nem.epnwcf.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zft.tanke756.top

TS:   if (x == null) {}
来源：http://dpi.jqgufenzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rrz.iojbl.cn

Go:   if x == nil {}
来源：http://iqy.fanxiaobao.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://guo.hysaishi.cn

C#:   if (x is null) {}
来源：http://ojn.shangyingyoupin.top

[P07] 防抖与节流
来源：http://gql.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dph.hcnkem.com

PHP:  // 手写时间戳比较
来源：http://zbg.pengpengdd.cyou

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ktt.epnwcf.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dpr.sweek.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pyy.nanxinkj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bfu.shzxlz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ezz.yuanzhike.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mma.bjfxy.top

[P08] 处理浮点精度问题
来源：http://poa.yuanzhike.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://udd.tianlin.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uye.gotoacloud.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jta.snrcjt.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gnc.andypj.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xpb.zhengqikj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cxk.yvedp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pgb.kuanghao11.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rgr.nanxinkj.top

================================================================================
来源：http://zqt.pengpengdd.cyou

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vfb.zdqjudy.top

================================================================================
来源：http://xds.fanxiaobao.xyz

[Q01] 创建表
来源：http://sdv.guannengcc.top

CREATE TABLE users (
来源：http://bbz.zhixingplan.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zyy.xuetiantiany.cn

name VARCHAR(50) NOT NULL,
来源：http://mkn.andypj.xyz

email VARCHAR(100) UNIQUE,
来源：http://oxn.jinqigufen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dfp.chenzaomai.com

);
来源：http://mma.cheryme.top

[Q02] 创建带外键的表
来源：http://dxh.ybcxt.top

CREATE TABLE orders (
来源：http://hjv.zhaomingkeji.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yju.redwolf501.top

user_id INT NOT NULL,
来源：http://dni.jinyuanbaomall.cn

amount DECIMAL(10, 2),
来源：http://hxs.sjlbkw.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://aah.sufxvd.cn

);
来源：http://mqe.jiagoushi.top

[Q03] 增加列
来源：http://kga.zhoulong.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fwh.meibo888.top

[Q04] 修改列类型
来源：http://wsc.fktsv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nhe.jiagoushi.top

[Q05] 重命名列
来源：http://can.haohaochexian.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ypr.nanxuanxn.top

[Q06] 删除列
来源：http://vxg.52xcode.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dfy.ydzc1.top

[Q07] 删除表
来源：http://bmv.hnxiangtu.top

DROP TABLE IF EXISTS orders;
来源：http://cgs.iojbl.cn

[Q08] 创建普通索引
来源：http://ffl.daria6918.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dph.sxryk.cn

[Q09] 创建唯一索引
来源：http://ygj.hesvh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qmt.yonumen.top

[Q10] 插入单行
来源：http://jgb.jqgfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jxe.fengsongda.top

[Q11] 一次插入多行
来源：http://lix.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://heb.hysaishi.cn

[Q12] 插入后取自增 ID
来源：http://oer.wangshuangyany.cn

INSERT INTO users (name) VALUES ('C');
来源：http://teg.quarkkingdee.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nix.epnwcf.com

[Q13] 忽略重复插入
来源：http://xxh.hongshengwenyu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vkc.andypj.xyz

[Q14] 存在则更新（upsert）
来源：http://sjq.xylfe.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xat.hcnkem.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://voz.zhaomingkeji.xyz

[Q15] 查询全部
来源：http://img.sjlbkw.cn

SELECT * FROM users;
来源：http://dtq.xziqi.cn

[Q16] 查询指定列
来源：http://hej.hnxiangtu.top

SELECT id, name FROM users;
来源：http://pxg.daxiang520.top

[Q17] 条件查询
来源：http://ijf.zhiwuduotai.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rmw.guowangkeji.top

[Q18] 模糊匹配
来源：http://mtu.jinyuanbaomall.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xaj.shuidangran.top

[Q19] 范围查询
来源：http://tjt.sxryk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nqu.zhijiandao.cn

[Q20] IN 列表
来源：http://vaj.sweek.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tgm.9152youxi.cn

[Q21] 空值判断
来源：http://pzu.hesvh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bww.tanke756.top

[Q22] 排序
来源：http://tkh.sjlbkw.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dsa.jqgufenzy.top

[Q23] 分页
来源：http://kyq.andypj.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fwa.ivvv.top

[Q24] 去重
来源：http://rfb.sufxvd.cn

SELECT DISTINCT city FROM users;
来源：http://njs.xuetiantiany.cn

[Q25] 只取前 N 条
来源：http://nwq.zhijiandao.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://onu.gzhubu.top

[Q26] 计数
来源：http://nut.jinqigufen.top

SELECT COUNT(*) FROM users;
来源：http://lon.gogol.net.cn

[Q27] 条件计数
来源：http://cof.redwolf501.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wvu.cqqwz.cn

[Q28] 求和与平均
来源：http://qiw.yfazqb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://upf.zhixingplan.top

[Q29] 最大最小值
来源：http://bbr.haohaochexian.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tpk.mhx1999.top

[Q30] 分组统计
来源：http://mxa.52xcode.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nyo.birdmap.top

[Q31] 分组后过滤
来源：http://fhd.wangshuangyany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rkl.shzxlz.cn

[Q32] 分组拼接字符串
来源：http://dnk.ppjwa.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dxq.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://csi.zdqjudy.top

[Q33] 多列分组
来源：http://htn.jinghuilouyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xuo.kuanghao11.cn

[Q34] 每组取第一条
来源：http://uay.zhaomingkeji.xyz

SELECT * FROM (
来源：http://mlz.sxryk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rdl.yj202588.top

) t WHERE rn = 1;
来源：http://usj.zdqjudy.top

[Q35] 内连接
来源：http://inz.epnwcf.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://moi.9152youxi.cn

[Q36] 左连接
来源：http://qhz.shuidangran.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://amr.sjlbkw.cn

[Q37] 右连接
来源：http://tdc.cheryme.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ezk.shzxlz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sly.ivvv.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pbo.guannengcc.top

[Q39] 自连接（查上下级）
来源：http://auz.yvedp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qri.jqgfzy.top


<!-- 参考信息 -->