代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bag.shangyingyoupin.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ftl.bjfxy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wee.yvedp.cn

Ruby: a.gcd(b)
来源：http://ghs.bbcook.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nhx.pengpengdd.cyou

[N06] 判断回文字符串
来源：http://kgo.gogol.net.cn

Py:   s == s[::-1]
来源：http://uhc.fktsv.cn

PHP:  $s === strrev($s);
来源：http://rhh.hnqzz.top

JS:   s === [...s].reverse().join("")
来源：http://hma.cashguo.top

TS:   s === [...s].reverse().join("")
来源：http://qej.ybcxt.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eym.jqgfzy.top

Go:   // 双指针从两端比较
来源：http://sit.daxiang520.top

Ruby: s == s.reverse
来源：http://eks.snrcjt.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mre.zhiwuduotai.top

[N07] 两数之和（返回下标）
来源：http://ajo.feifeiyinyue.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mog.ywan-chungtsiang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://afb.yangfankeji.com

JS:   // 手写 Map：map.set(v, i)
来源：http://kjc.nanxuanxn.top

TS:   // 手写 Map<string, number>
来源：http://heu.tanke756.top

Java: // 手写 HashMap
来源：http://cbf.sxryk.cn

Go:   // 手写 map[int]int
来源：http://jxf.shzxlz.cn

Ruby: // 手写 Hash
来源：http://dzr.yueranfly.top

C#:   // 手写 Dictionary<int, int>
来源：http://lia.hysaishi.cn

[N08] 生成全排列
来源：http://rxd.xinyue.icu

Py:   itertools.permutations(arr)
来源：http://vcf.pycfn.com

PHP:  // 手写递归交换
来源：http://cvw.52xcode.cn

JS:   // 手写回溯递归
来源：http://jvx.jyoumei.cn

TS:   // 手写回溯递归
来源：http://svc.daria6918.cn

Java: // 手写回溯递归
来源：http://hqi.shangyingyoupin.top

Go:   // 手写回溯递归
来源：http://ffl.snrcjt.cn

Ruby: arr.permutation.to_a
来源：http://ozv.hfpthk.cn

C#:   // 手写回溯递归
来源：http://dvg.wangdashe.top

[N09] 栈与队列
来源：http://zts.vqdsnc.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dzr.bjfxy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pjk.ydjk.org.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dfs.jyoumei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rrs.hesvh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nlz.fktsv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uwy.wangdashe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qbt.ppjwa.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xip.hfpthk.cn

[N10] 链表节点定义
来源：http://tkt.hysaishi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vky.tianlin.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://win.hfpthk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hyq.tian-w.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dhl.nanxinkj.top

Java: class Node { int v; Node next; }
来源：http://pgx.sjlbkw.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rsa.jqgfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://lrc.vehdjk.com

C#:   class Node { public int V; public Node? Next; }
来源：http://yyb.zdbjq.cn

[N11] 二叉树中序遍历
来源：http://enp.zdqjudy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hdy.xinyue.icu

PHP:  // 手写递归函数
来源：http://fns.hfpthk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://srg.tianlin.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://goc.zhoulong.xyz

Java: // 手写递归
来源：http://tas.aizwys.cn

Go:   // 手写递归
来源：http://syf.zdqjudy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://glg.xuanzx.com

C#:   // 手写递归
来源：http://pyn.hcnkem.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zrj.sxryk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ice.hnqzz.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://puv.jiagoushi.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hcy.hnqzz.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://npt.havefunace.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xvw.yj20258.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bpn.jqgfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yrz.jinghuilouyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tch.nwbrower.top

================================================================================
来源：http://xiw.gaohongyu789.top

O. 并发与异步
来源：http://bnz.redwolf501.top

================================================================================
来源：http://kxl.zhengqikj.top

[O01] 启动一个线程
来源：http://fcp.quarkkingdee.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mfd.shanyushiyangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ngk.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ugs.snrcjt.cn

TS:   // 同 JS
来源：http://jwr.vqdsnc.cn

Java: new Thread(() -> f()).start()
来源：http://tsn.mhx1999.top

Go:   go f()
来源：http://pql.redwolf501.top

Ruby: Thread.new { f }
来源：http://xlt.chenlongwang.top

C#:   Task.Run(() => F());
来源：http://dub.bjfxy.top

[O02] 使用线程池
来源：http://smd.fehbvm.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nmd.zhiwuduotai.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gda.nanxinkj.top

JS:   // worker_threads 线程池
来源：http://fuj.snrcjt.cn

TS:   // worker_threads 线程池
来源：http://pec.vehdjk.com

Java: Executors.newFixedThreadPool(4)
来源：http://ojc.zhixingplan.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jsd.yj202588.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sfe.chenzaomai.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cvn.gogol.net.cn

[O03] 加锁保护共享数据
来源：http://mol.zdqjudy.top

Py:   with lock: shared += 1
来源：http://lhb.andypj.xyz

PHP:  // 用 flock() 做文件锁
来源：http://som.cheryme.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xde.ivvv.top

TS:   // 同 JS
来源：http://njc.cheryme.top

Java: synchronized (this) { shared++; }
来源：http://epd.gotoacloud.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gog.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wyn.ydjk.org.cn

C#:   lock (gate) { shared++; }
来源：http://szq.smart0.xyz

[O04] 定义异步函数并等待
来源：http://reh.chenlongwang.top

Py:   async def f():⏎    await g()
来源：http://dvi.hesvh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://epu.sysykeji.top

JS:   async function f() { await g(); }
来源：http://cbx.hesvh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yhe.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pgv.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rll.yj20258888.top

Ruby: # 用 Fiber 或 async gem
来源：http://wtt.cqqwz.cn

C#:   async Task F() { await G(); }
来源：http://qqr.ywan-chungtsiang.top

[O05] 并发执行并等待全部完成
来源：http://ztv.bbcook.cn

Py:   asyncio.gather(*tasks)
来源：http://nbz.jyoumei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://aud.shanyushiyangtech.top

JS:   await Promise.all(tasks)
来源：http://hky.daxiang520.top

TS:   await Promise.all(tasks)
来源：http://ncw.wangdashe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://upi.yanxiufei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vrt.ehwqpu.com

Ruby: threads.map(&:join)
来源：http://efr.sufxvd.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ono.hesvh.cn

[O06] 使用进程池
来源：http://lws.sxryk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cjv.hammf.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://str.jqgfzy.top

JS:   // child_process / cluster 模块
来源：http://ria.yongpay.top

TS:   // child_process / cluster 模块
来源：http://qaq.gogol.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baj.tarul.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://txr.cqqwz.cn

Ruby: // fork 块
来源：http://koi.shzxlz.cn

C#:   Parallel.For
来源：http://uar.sjlbkw.cn

================================================================================
来源：http://ewf.hammf.cn

P. 常用工具函数
来源：http://dej.daria6918.cn

================================================================================
来源：http://wmh.tianlin.xyz

[P01] 生成 UUID
来源：http://ruu.sufxvd.cn

Py:   str(uuid.uuid4())
来源：http://zep.316326.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://brz.hnxiangtu.top

JS:   crypto.randomUUID()
来源：http://kaj.fehbvm.com

TS:   crypto.randomUUID()
来源：http://caz.dianchejie.cn

Java: UUID.randomUUID().toString()
来源：http://lbf.sysykeji.top

Go:   // 用 github.com/google/uuid
来源：http://whq.shanyushiyangkeji.top

Ruby: SecureRandom.uuid
来源：http://rcc.pengpengdd.cyou

C#:   Guid.NewGuid().ToString()
来源：http://rpb.andypj.xyz

[P02] MD5 / SHA256 摘要
来源：http://szs.yuanzhike.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qbw.haohaochexian.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xfb.jinyuanbaomall.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ivf.quarkkingdee.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xps.nanxuanxn.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://krl.birdmap.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nxs.meibo888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mrr.feifeiyinyue.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lkx.cqqwz.cn

[P03] 生成短随机字符串
来源：http://wve.sjlbkw.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bee.ydzc1.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dju.hesvh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xmz.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vdr.yangfankeji.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ycz.gotoacloud.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://auh.mhx1999.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://iig.nwbrower.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yxy.hesvh.cn

[P04] 求长度
来源：http://apm.vehdjk.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://scx.c1oappe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fcu.ehwqpu.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sxn.cashguo.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fwp.meibo888.top

Java: list.size();  map.size();  s.length()
来源：http://jrb.sysykeji.top

Go:   len(arr);  len(m)
来源：http://ylp.xuetiantiany.cn

Ruby: x.length;  x.size
来源：http://ldh.zhijiandao.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rwg.cqqwz.cn

[P05] 判断两个对象内容是否相等
来源：http://skf.cashguo.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pjd.hfpthk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rbi.zhaomingkeji.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pnd.zhixingplan.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://geo.chenjidiqi.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ucd.guannengcc.top

Go:   reflect.DeepEqual(a, b)
来源：http://vps.jianghu66.top

Ruby: a == b
来源：http://uqi.chenzaomai.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hsi.birdmap.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qht.hnqzz.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wry.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://ocu.gaohongyu789.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xhh.gaohongyu789.top

TS:   if (x == null) {}
来源：http://zrk.yangfankeji.com

Java: if (x == null || x.isEmpty()) {}
来源：http://xje.yueranfly.top

Go:   if x == nil {}
来源：http://sps.ehwqpu.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iyr.cheryme.top

C#:   if (x is null) {}
来源：http://erl.jqgfzy.top

[P07] 防抖与节流
来源：http://jvj.fehbvm.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cwv.tianlin.xyz

PHP:  // 手写时间戳比较
来源：http://gyj.0kj1m.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mql.ctjpmb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://txp.dashuyun.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ltw.tian-w.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://npg.gzhubu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rhn.hfpthk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zjz.nanxinkj.top

[P08] 处理浮点精度问题
来源：http://svw.hnqzz.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rqp.ybcxt.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sop.zhengqikj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fqg.ydzc1.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ufl.shanyushiyangtech.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rrk.shuidangran.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gkw.bbcook.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://inn.sysykeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://avn.yonumen.top

================================================================================
来源：http://grj.aibaodan.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jpg.shanyushiyangkeji.top

================================================================================
来源：http://fuf.316326.xyz

[Q01] 创建表
来源：http://xpl.sweek.top

CREATE TABLE users (
来源：http://mzg.gogol.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://enj.xziqi.cn

name VARCHAR(50) NOT NULL,
来源：http://zxq.chenzaomai.com

email VARCHAR(100) UNIQUE,
来源：http://qno.ivvv.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bed.zhiwuduotai.top

);
来源：http://wdu.ywan-chungtsiang.top

[Q02] 创建带外键的表
来源：http://ohn.tanke756.top

CREATE TABLE orders (
来源：http://ieg.daxiang520.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bmn.yueranfly.top

user_id INT NOT NULL,
来源：http://ccp.shuidangran.top

amount DECIMAL(10, 2),
来源：http://edb.yj20258.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qdm.nanxuanxn.top

);
来源：http://khr.yj202588.top

[Q03] 增加列
来源：http://zwz.gotoacloud.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rja.jinqigfzy.top

[Q04] 修改列类型
来源：http://srr.shanyushiyangkeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rre.gzhubu.top

[Q05] 重命名列
来源：http://jxa.pycfn.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ghv.xuetiantiany.cn

[Q06] 删除列
来源：http://smr.ydzc1.top

ALTER TABLE users DROP COLUMN age;
来源：http://vkl.vehdjk.com

[Q07] 删除表
来源：http://hyj.hnxiangtu.top

DROP TABLE IF EXISTS orders;
来源：http://biz.hcnkem.com

[Q08] 创建普通索引
来源：http://vro.kuanghao11.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cxg.jinghuilouyu.cn

[Q09] 创建唯一索引
来源：http://wbg.kuanghao11.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://imj.jinyuanbaomall.cn

[Q10] 插入单行
来源：http://ryi.wangdashe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://coa.hammf.cn

[Q11] 一次插入多行
来源：http://cbt.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hio.dianchejie.cn

[Q12] 插入后取自增 ID
来源：http://sdr.xuetiantiany.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pym.gotoacloud.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lul.zdqjudy.top

[Q13] 忽略重复插入
来源：http://itm.yj202588.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kgh.zhixingplan.top

[Q14] 存在则更新（upsert）
来源：http://vvj.nanxuanxn.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ixf.cheryme.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xvz.zhixingplan.top

[Q15] 查询全部
来源：http://kul.jinghuilouyu.cn

SELECT * FROM users;
来源：http://efi.hywenlv.cn

[Q16] 查询指定列
来源：http://gei.cqqwz.cn

SELECT id, name FROM users;
来源：http://jzn.hesvh.cn

[Q17] 条件查询
来源：http://xfp.jinghuilouyu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://aio.jiagoushi.top

[Q18] 模糊匹配
来源：http://jld.yj202588.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qbg.jlsjyb.cn

[Q19] 范围查询
来源：http://cci.hammf.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ipc.zhongyouzk.top

[Q20] IN 列表
来源：http://pqp.wangshuangyany.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://syc.wangshuangyany.cn

[Q21] 空值判断
来源：http://rgv.jyoumei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lew.sysykeji.top

[Q22] 排序
来源：http://goo.chenzaomai.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://whg.fktsv.cn

[Q23] 分页
来源：http://bpc.andypj.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zww.snrcjt.cn

[Q24] 去重
来源：http://uzp.jlsjyb.cn

SELECT DISTINCT city FROM users;
来源：http://pmd.zhixingplan.top

[Q25] 只取前 N 条
来源：http://dcq.xuanzx.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://biq.aizwys.cn

[Q26] 计数
来源：http://oqw.bjfxy.top

SELECT COUNT(*) FROM users;
来源：http://xrg.zhongyouzk.top

[Q27] 条件计数
来源：http://wpv.zhongyouzk.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://onm.yanxiufei.cn

[Q28] 求和与平均
来源：http://uae.yj20258888.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lno.chenlongwang.top

[Q29] 最大最小值
来源：http://vim.jqgfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://shu.bbcook.cn

[Q30] 分组统计
来源：http://ssi.chenjidiqi.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ali.jinyuanbaomall.cn

[Q31] 分组后过滤
来源：http://fif.sysykeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mqg.fzhhl.top

[Q32] 分组拼接字符串
来源：http://tiy.dianchejie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://soq.haohaochexian.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://imj.hesvh.cn

[Q33] 多列分组
来源：http://wbi.kuanghao11.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cnl.iojbl.cn

[Q34] 每组取第一条
来源：http://erf.yj202588.top

SELECT * FROM (
来源：http://ort.redwolf501.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://isa.yueranfly.top

) t WHERE rn = 1;
来源：http://noa.xziqi.cn

[Q35] 内连接
来源：http://edv.yj20258888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://grf.bbcook.cn

[Q36] 左连接
来源：http://oea.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qcj.zhoulong.xyz

[Q37] 右连接
来源：http://kpo.xziqi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bto.xuanzx.com

[Q38] 全外连接（PostgreSQL）
来源：http://rrx.fehbvm.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zmx.yanxiufei.cn

[Q39] 自连接（查上下级）
来源：http://ihw.0kj1m.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ctm.shanyushiyangtech.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xaf.gzhubu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qji.yueranfly.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://aqv.0kj1m.cn

[Q41] 多表连接
来源：http://srp.jinghuilouyu.cn


<!-- 参考信息 -->