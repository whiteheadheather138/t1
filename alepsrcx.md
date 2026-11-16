代发 wailian999

[N05] 最大公约数
来源：http://iug.ctjpmb.com

Py:   math.gcd(a, b)
来源：http://xww.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tnu.xziqi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qqt.hywenlv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pyp.tanke756.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jke.sxryk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bpz.hysaishi.cn

Ruby: a.gcd(b)
来源：http://ptw.tian-w.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mot.hfpthk.cn

[N06] 判断回文字符串
来源：http://qrx.mhx1999.top

Py:   s == s[::-1]
来源：http://zfi.fzhhl.top

PHP:  $s === strrev($s);
来源：http://yzx.zhiwuduotai.top

JS:   s === [...s].reverse().join("")
来源：http://wzo.0kj1m.cn

TS:   s === [...s].reverse().join("")
来源：http://pph.chenzaomai.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ywu.c1oappe.top

Go:   // 双指针从两端比较
来源：http://ino.hnxiangtu.top

Ruby: s == s.reverse
来源：http://vkc.yanxiufei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yyr.xinyue.icu

[N07] 两数之和（返回下标）
来源：http://dbe.cdnleiting.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tgy.yfazqb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qlf.zdbjq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dmi.zycfv.cn

TS:   // 手写 Map<string, number>
来源：http://xjx.tian-w.cn

Java: // 手写 HashMap
来源：http://uuh.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://yzd.svipenyu.cn

Ruby: // 手写 Hash
来源：http://vei.fengsongda.top

C#:   // 手写 Dictionary<int, int>
来源：http://qza.sysykeji.top

[N08] 生成全排列
来源：http://izz.redwolf501.top

Py:   itertools.permutations(arr)
来源：http://znq.birdmap.top

PHP:  // 手写递归交换
来源：http://xrn.zdbjq.cn

JS:   // 手写回溯递归
来源：http://abn.feifeiyinyue.top

TS:   // 手写回溯递归
来源：http://tpm.shangyingyoupin.top

Java: // 手写回溯递归
来源：http://upk.0kj1m.cn

Go:   // 手写回溯递归
来源：http://ujc.c1oappe.top

Ruby: arr.permutation.to_a
来源：http://pxs.sjlbkw.cn

C#:   // 手写回溯递归
来源：http://cie.yangfankeji.com

[N09] 栈与队列
来源：http://szz.aibaodan.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aac.jiagoushi.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://emj.daria6918.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rrz.zhongyouzk.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gta.epnwcf.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://umj.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://irg.sysykeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eob.dashuyun.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mai.tanke756.top

[N10] 链表节点定义
来源：http://frr.havefunace.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://esw.jinqigufen.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jvi.jqgfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rnr.guowangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://icb.zhaomingkeji.xyz

Java: class Node { int v; Node next; }
来源：http://osx.jyoumei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oar.chenlongwang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uzl.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bmd.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://zif.jinyuanbaomall.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wyt.jianghu66.top

PHP:  // 手写递归函数
来源：http://fyv.sxryk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iyn.wangshuangyany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yoq.sysykeji.top

Java: // 手写递归
来源：http://laa.hnqzz.top

Go:   // 手写递归
来源：http://psb.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ugj.svipenyu.cn

C#:   // 手写递归
来源：http://spe.yj202588.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xib.sufxvd.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mzi.zhengqikj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uyc.fehbvm.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://umz.zhiwuduotai.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kvr.zhoulong.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fek.gogol.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xmj.316326.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fkl.hongshengwenyu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xps.daxiang520.top

================================================================================
来源：http://hom.hysaishi.cn

O. 并发与异步
来源：http://etz.aibaodan.cn

================================================================================
来源：http://koq.svipenyu.cn

[O01] 启动一个线程
来源：http://dmr.havefunace.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mnw.hesvh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://twy.sweek.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lzw.ppjwa.cn

TS:   // 同 JS
来源：http://xpw.pengpengdd.cyou

Java: new Thread(() -> f()).start()
来源：http://hdy.sweek.top

Go:   go f()
来源：http://aoj.c1oappe.top

Ruby: Thread.new { f }
来源：http://gpy.xinyue.icu

C#:   Task.Run(() => F());
来源：http://lzu.pengpengdd.cyou

[O02] 使用线程池
来源：http://gir.hysaishi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cms.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zbl.ybcxt.top

JS:   // worker_threads 线程池
来源：http://sxb.sxryk.cn

TS:   // worker_threads 线程池
来源：http://lja.9152youxi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rgc.fengsongda.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mhj.jqgufenzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ptj.zhoulong.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://auj.aibaodan.cn

[O03] 加锁保护共享数据
来源：http://bil.zycfv.cn

Py:   with lock: shared += 1
来源：http://tlg.xinyue.icu

PHP:  // 用 flock() 做文件锁
来源：http://jdo.daxiang520.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iyw.xinyue.icu

TS:   // 同 JS
来源：http://the.c1oappe.top

Java: synchronized (this) { shared++; }
来源：http://qgi.yongpay.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uus.jiagoushi.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://yar.havefunace.top

C#:   lock (gate) { shared++; }
来源：http://anr.gaohongyu789.top

[O04] 定义异步函数并等待
来源：http://ujk.chenjidiqi.icu

Py:   async def f():⏎    await g()
来源：http://qmk.yj202588.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hpb.fehbvm.com

JS:   async function f() { await g(); }
来源：http://mls.gzhubu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xtq.sysykeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vce.iojbl.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sxd.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://gcl.vehdjk.com

C#:   async Task F() { await G(); }
来源：http://hci.feifeiyinyue.top

[O05] 并发执行并等待全部完成
来源：http://oto.sufxvd.cn

Py:   asyncio.gather(*tasks)
来源：http://lyn.ppjwa.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://whq.hesvh.cn

JS:   await Promise.all(tasks)
来源：http://vun.iojbl.cn

TS:   await Promise.all(tasks)
来源：http://gvs.guannengcc.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yar.jianghu66.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cog.hongshengwenyu.top

Ruby: threads.map(&:join)
来源：http://txo.ydzc1.top

C#:   await Task.WhenAll(t1, t2)
来源：http://boe.tian-w.cn

[O06] 使用进程池
来源：http://gui.zhijiandao.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tzi.zycfv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nwm.uphjek.com

JS:   // child_process / cluster 模块
来源：http://vxo.dashuyun.cn

TS:   // child_process / cluster 模块
来源：http://xkf.wangdashe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qte.sjlbkw.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qos.redwolf501.top

Ruby: // fork 块
来源：http://mkc.pengpengdd.cyou

C#:   Parallel.For
来源：http://mji.nanxuanxn.top

================================================================================
来源：http://ijn.yongpay.top

P. 常用工具函数
来源：http://uqi.shangyingyoupin.top

================================================================================
来源：http://ivw.haohaochexian.top

[P01] 生成 UUID
来源：http://fkg.chenzaomai.com

Py:   str(uuid.uuid4())
来源：http://uec.sjlbkw.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://koz.xuetiantiany.cn

JS:   crypto.randomUUID()
来源：http://ztm.hongshengwenyu.top

TS:   crypto.randomUUID()
来源：http://gjc.hcnkem.com

Java: UUID.randomUUID().toString()
来源：http://gvw.cashguo.top

Go:   // 用 github.com/google/uuid
来源：http://gze.hnqzz.top

Ruby: SecureRandom.uuid
来源：http://pmm.shuidangran.top

C#:   Guid.NewGuid().ToString()
来源：http://cdy.chenjidiqi.icu

[P02] MD5 / SHA256 摘要
来源：http://foj.cashguo.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jgp.jinghuilouyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dyh.dianchejie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kym.mhx1999.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jif.birdmap.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mil.chenzaomai.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jdl.chenzaomai.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xjl.jinghuilouyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://akr.tianlin.xyz

[P03] 生成短随机字符串
来源：http://hdd.bjfxy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vgs.xziqi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mab.wangshuangyany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pdz.haohaochexian.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wkb.9152youxi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://obk.zhengqikj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kvt.tarul.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kpu.birdmap.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zgl.yueranfly.top

[P04] 求长度
来源：http://bid.zdbjq.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://squ.wangdashe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mzz.zhixingplan.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://emz.zhengqikj.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qmt.gotoacloud.top

Java: list.size();  map.size();  s.length()
来源：http://yyu.jinqigfzy.top

Go:   len(arr);  len(m)
来源：http://lwn.ivvv.top

Ruby: x.length;  x.size
来源：http://sbw.hcnkem.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://agy.hnqzz.top

[P05] 判断两个对象内容是否相等
来源：http://nmy.tarul.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hyh.zhoulong.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://egl.gogol.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://caq.xuanzx.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ioz.fzhhl.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mdw.ybcxt.top

Go:   reflect.DeepEqual(a, b)
来源：http://pme.xinyue.icu

Ruby: a == b
来源：http://pzd.zhoulong.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bll.havefunace.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xir.feifeiyinyue.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vxb.52xcode.cn

PHP:  if (empty($x)) {}
来源：http://wqj.hammf.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fxt.0kj1m.cn

TS:   if (x == null) {}
来源：http://ona.316326.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://the.dashuyun.cn

Go:   if x == nil {}
来源：http://qkl.birdmap.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lld.chenlongwang.top

C#:   if (x is null) {}
来源：http://bbi.feifeiyinyue.top

[P07] 防抖与节流
来源：http://peb.ehwqpu.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ksq.xinyue.icu

PHP:  // 手写时间戳比较
来源：http://twk.xylfe.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xnb.tian-w.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jys.hongshengwenyu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xjf.yongpay.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rgy.jinghuilouyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pjm.yj202588.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ymm.gzhubu.top

[P08] 处理浮点精度问题
来源：http://qjj.guowangkeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kss.zhongyouzk.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zaj.zhijiandao.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nbb.dianchejie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kxt.52xcode.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jdg.fktsv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rkm.zdqjudy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yzq.nanxuanxn.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qif.jinyuanbaomall.cn

================================================================================
来源：http://ogc.jyoumei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lwa.jqgufenzy.top

================================================================================
来源：http://wub.jyoumei.cn

[Q01] 创建表
来源：http://ggr.wangshuangyany.cn

CREATE TABLE users (
来源：http://byo.quarkkingdee.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tvv.316326.xyz

name VARCHAR(50) NOT NULL,
来源：http://xmw.ydzc1.top

email VARCHAR(100) UNIQUE,
来源：http://pvh.nwbrower.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eva.ywan-chungtsiang.top

);
来源：http://rrj.yangfankeji.com

[Q02] 创建带外键的表
来源：http://kaa.yj20258888.top

CREATE TABLE orders (
来源：http://vzu.fzhhl.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://djv.jianghu66.top

user_id INT NOT NULL,
来源：http://pqe.tarul.cn

amount DECIMAL(10, 2),
来源：http://eez.jianghu66.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dru.gogol.net.cn

);
来源：http://hgb.jqgufenzy.top

[Q03] 增加列
来源：http://bqy.ydjk.org.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eyy.ppjwa.cn

[Q04] 修改列类型
来源：http://jea.yvedp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ooo.feifeiyinyue.top

[Q05] 重命名列
来源：http://dss.jyoumei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rex.pengpengdd.cyou

[Q06] 删除列
来源：http://pcg.andypj.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://rom.9152youxi.cn

[Q07] 删除表
来源：http://ymk.xziqi.cn

DROP TABLE IF EXISTS orders;
来源：http://eld.nwbrower.top

[Q08] 创建普通索引
来源：http://vvt.fzhhl.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xwm.cheryme.top

[Q09] 创建唯一索引
来源：http://nwy.jinyuanbaomall.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tnz.zhengqikj.top

[Q10] 插入单行
来源：http://fos.tanke756.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vvg.shanyushiyangtech.top

[Q11] 一次插入多行
来源：http://azt.shzxlz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iwi.daria6918.cn

[Q12] 插入后取自增 ID
来源：http://jaa.kuanghao11.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mys.redwolf501.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ylz.fanxiaobao.xyz

[Q13] 忽略重复插入
来源：http://yel.hammf.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://shl.shangyingyoupin.top

[Q14] 存在则更新（upsert）
来源：http://zwe.yanxiufei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rpf.meibo888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://acm.nanxuanxn.top

[Q15] 查询全部
来源：http://fpf.yj20258888.top

SELECT * FROM users;
来源：http://yjf.0kj1m.cn

[Q16] 查询指定列
来源：http://ofb.jiagoushi.top

SELECT id, name FROM users;
来源：http://zri.fktsv.cn

[Q17] 条件查询
来源：http://cbs.ydjk.org.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gec.guannengcc.top

[Q18] 模糊匹配
来源：http://bkt.wangdashe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zog.hesvh.cn

[Q19] 范围查询
来源：http://goc.guowangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fmi.dashuyun.cn

[Q20] IN 列表
来源：http://toi.snrcjt.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gae.snrcjt.cn

[Q21] 空值判断
来源：http://kje.xuetiantiany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ool.shuidangran.top

[Q22] 排序
来源：http://xlz.jiagoushi.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dit.zhixingplan.top

[Q23] 分页
来源：http://gfr.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bkj.aibaodan.cn

[Q24] 去重
来源：http://vcz.sysykeji.top

SELECT DISTINCT city FROM users;
来源：http://rxx.ctjpmb.com

[Q25] 只取前 N 条
来源：http://nbo.316326.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://psl.chenlongwang.top

[Q26] 计数
来源：http://iwv.fehbvm.com

SELECT COUNT(*) FROM users;
来源：http://nkc.yvedp.cn

[Q27] 条件计数
来源：http://uua.tian-w.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kjd.52xcode.cn

[Q28] 求和与平均
来源：http://ypi.shangyingyoupin.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kax.andypj.xyz

[Q29] 最大最小值
来源：http://huj.pengpengdd.cyou

SELECT MAX(age), MIN(age) FROM users;
来源：http://wqm.zhixingplan.top

[Q30] 分组统计
来源：http://tyn.gotoacloud.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ndp.redwolf501.top

[Q31] 分组后过滤
来源：http://eat.gotoacloud.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fti.sufxvd.cn

[Q32] 分组拼接字符串
来源：http://kmg.quarkkingdee.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qhp.yonumen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kst.ydjk.org.cn

[Q33] 多列分组
来源：http://xgk.fengsongda.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://inj.jyoumei.cn

[Q34] 每组取第一条
来源：http://guw.hnqzz.top

SELECT * FROM (
来源：http://app.ctjpmb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hpx.jlsjyb.cn

) t WHERE rn = 1;
来源：http://qrh.sysykeji.top

[Q35] 内连接
来源：http://myq.vehdjk.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://epo.dashuyun.cn

[Q36] 左连接
来源：http://cui.daxiang520.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bgo.zhixingplan.top

[Q37] 右连接
来源：http://zqz.sweek.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wlv.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rec.cashguo.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zui.sjlbkw.cn

[Q39] 自连接（查上下级）
来源：http://cfv.pengpengdd.cyou

SELECT e.name, m.name AS manager FROM employees e
来源：http://gpa.chenjidiqi.icu


<!-- 参考信息 -->