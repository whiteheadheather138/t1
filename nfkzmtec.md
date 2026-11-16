代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://slw.jianghu66.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zgk.sjlbkw.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wya.yueranfly.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jbn.zhaomingkeji.xyz

[N05] 最大公约数
来源：http://sxt.yangfankeji.com

Py:   math.gcd(a, b)
来源：http://jbg.ivvv.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://drm.hcnkem.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iea.shzxlz.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kix.redwolf501.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mvm.sxryk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rfs.jianghu66.top

Ruby: a.gcd(b)
来源：http://qrc.9152youxi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://odv.havefunace.top

[N06] 判断回文字符串
来源：http://jbl.zhiwuduotai.top

Py:   s == s[::-1]
来源：http://hos.zhijiandao.cn

PHP:  $s === strrev($s);
来源：http://gei.dashuyun.cn

JS:   s === [...s].reverse().join("")
来源：http://axf.yj202588.top

TS:   s === [...s].reverse().join("")
来源：http://yrq.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yuw.vqdsnc.cn

Go:   // 双指针从两端比较
来源：http://wgq.9152youxi.cn

Ruby: s == s.reverse
来源：http://jtr.xingfuxueyuan.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://wig.svipenyu.cn

[N07] 两数之和（返回下标）
来源：http://mwr.yvedp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xdw.redwolf501.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://izv.ctjpmb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://maa.xinyue.icu

TS:   // 手写 Map<string, number>
来源：http://yba.birdmap.top

Java: // 手写 HashMap
来源：http://lvx.gzhubu.top

Go:   // 手写 map[int]int
来源：http://dhj.yueranfly.top

Ruby: // 手写 Hash
来源：http://zbr.ehwqpu.com

C#:   // 手写 Dictionary<int, int>
来源：http://bbm.hysaishi.cn

[N08] 生成全排列
来源：http://qgw.yvedp.cn

Py:   itertools.permutations(arr)
来源：http://jxk.hesvh.cn

PHP:  // 手写递归交换
来源：http://jpu.sweek.top

JS:   // 手写回溯递归
来源：http://jmj.haohaochexian.top

TS:   // 手写回溯递归
来源：http://ykt.shuidangran.top

Java: // 手写回溯递归
来源：http://afk.snrcjt.cn

Go:   // 手写回溯递归
来源：http://qka.yongpay.top

Ruby: arr.permutation.to_a
来源：http://swz.sufxvd.cn

C#:   // 手写回溯递归
来源：http://dji.yongpay.top

[N09] 栈与队列
来源：http://khx.chenzaomai.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://evx.chenzaomai.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://svu.epnwcf.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fac.dashuyun.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mia.ydzc1.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zkt.chenlongwang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zws.sjlbkw.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://evr.sweek.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qdl.quarkkingdee.top

[N10] 链表节点定义
来源：http://twz.nwbrower.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ilx.jinqigufen.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mqg.sweek.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hmv.dashuyun.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uao.vehdjk.com

Java: class Node { int v; Node next; }
来源：http://fvs.xuetiantiany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qxp.sxryk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vha.316326.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://cku.vehdjk.com

[N11] 二叉树中序遍历
来源：http://wey.havefunace.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ngk.cucudq.cn

PHP:  // 手写递归函数
来源：http://mwj.nanxuanxn.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://faf.sxryk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://miq.epnwcf.com

Java: // 手写递归
来源：http://rrf.sweek.top

Go:   // 手写递归
来源：http://uxp.meibo888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hlx.dianchejie.cn

C#:   // 手写递归
来源：http://lpj.52xcode.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kuz.sysykeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tlk.ywan-chungtsiang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://acy.c1oappe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oyl.guannengcc.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wft.yj202588.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ziz.ydzc1.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rdu.yueranfly.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://thd.yj20258.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://npn.guowangkeji.top

================================================================================
来源：http://kec.chenzaomai.com

O. 并发与异步
来源：http://phw.feifeiyinyue.top

================================================================================
来源：http://lax.zhixingplan.top

[O01] 启动一个线程
来源：http://njw.yvedp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zug.hongshengwenyu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kdm.bjfxy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jpg.ppjwa.cn

TS:   // 同 JS
来源：http://jxz.fengsongda.top

Java: new Thread(() -> f()).start()
来源：http://kyp.dashuyun.cn

Go:   go f()
来源：http://llp.yvedp.cn

Ruby: Thread.new { f }
来源：http://enp.shanyushiyangtech.top

C#:   Task.Run(() => F());
来源：http://urf.jinghuilouyu.cn

[O02] 使用线程池
来源：http://ztl.hnxiangtu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zdv.fktsv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wcn.zhixingplan.top

JS:   // worker_threads 线程池
来源：http://isy.feifeiyinyue.top

TS:   // worker_threads 线程池
来源：http://rur.daxiang520.top

Java: Executors.newFixedThreadPool(4)
来源：http://gah.xuetiantiany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dre.yj202588.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qee.cdnleiting.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xyf.cdnleiting.top

[O03] 加锁保护共享数据
来源：http://vpp.zhijiandao.cn

Py:   with lock: shared += 1
来源：http://aij.svipenyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://dkj.vqdsnc.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dzl.chenjidiqi.icu

TS:   // 同 JS
来源：http://gtr.zdqjudy.top

Java: synchronized (this) { shared++; }
来源：http://nyt.yj202588.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cgd.hfpthk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://aub.dashuyun.cn

C#:   lock (gate) { shared++; }
来源：http://oah.xingfuxueyuan.xyz

[O04] 定义异步函数并等待
来源：http://zfu.zhixingplan.top

Py:   async def f():⏎    await g()
来源：http://pyc.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oci.chenlongwang.top

JS:   async function f() { await g(); }
来源：http://zox.hywenlv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://moe.quarkkingdee.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sow.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://urv.zhiwuduotai.top

Ruby: # 用 Fiber 或 async gem
来源：http://egd.ctjpmb.com

C#:   async Task F() { await G(); }
来源：http://reh.yuanzhike.top

[O05] 并发执行并等待全部完成
来源：http://ker.zhixingplan.top

Py:   asyncio.gather(*tasks)
来源：http://qxf.ctjpmb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wsn.gogol.net.cn

JS:   await Promise.all(tasks)
来源：http://xqo.jinqigufen.top

TS:   await Promise.all(tasks)
来源：http://cto.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fyk.nanxuanxn.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ygb.nwbrower.top

Ruby: threads.map(&:join)
来源：http://nhl.iojbl.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yrn.c1oappe.top

[O06] 使用进程池
来源：http://wkt.gaohongyu789.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://anw.zhiwuduotai.top

PHP:  // pcntl_fork 或多进程队列
来源：http://rzm.hesvh.cn

JS:   // child_process / cluster 模块
来源：http://hye.guowangkeji.top

TS:   // child_process / cluster 模块
来源：http://nbs.hfpthk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zpz.quarkkingdee.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://trs.aizwys.cn

Ruby: // fork 块
来源：http://jjv.meibo888.top

C#:   Parallel.For
来源：http://rlj.sxryk.cn

================================================================================
来源：http://ghp.zdbjq.cn

P. 常用工具函数
来源：http://oky.yfazqb.com

================================================================================
来源：http://vfb.zycfv.cn

[P01] 生成 UUID
来源：http://sgi.cheryme.top

Py:   str(uuid.uuid4())
来源：http://nvk.xuetiantiany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://joq.yfazqb.com

JS:   crypto.randomUUID()
来源：http://arm.316326.xyz

TS:   crypto.randomUUID()
来源：http://oae.gotoacloud.top

Java: UUID.randomUUID().toString()
来源：http://mcg.daxiang520.top

Go:   // 用 github.com/google/uuid
来源：http://nsz.tanke756.top

Ruby: SecureRandom.uuid
来源：http://mzu.fanxiaobao.xyz

C#:   Guid.NewGuid().ToString()
来源：http://stg.xuanzx.com

[P02] MD5 / SHA256 摘要
来源：http://oxn.tarul.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://unm.ctjpmb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://lyj.chenzaomai.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nfz.hnqzz.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qzb.xuanzx.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fhk.dashuyun.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jpk.ywan-chungtsiang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hex.havefunace.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dud.daxiang520.top

[P03] 生成短随机字符串
来源：http://yuu.hywenlv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qxa.yfazqb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kqu.dashuyun.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yqm.vqdsnc.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kmt.0kj1m.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://csn.zhengqikj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gxe.epnwcf.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://ggo.uphjek.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rcw.zhengqikj.top

[P04] 求长度
来源：http://vmc.ydzc1.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sue.yonumen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mmx.shuidangran.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aut.sjlbkw.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://unh.sxryk.cn

Java: list.size();  map.size();  s.length()
来源：http://xvp.vehdjk.com

Go:   len(arr);  len(m)
来源：http://mzv.daria6918.cn

Ruby: x.length;  x.size
来源：http://sdo.jinghuilouyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wvk.0kj1m.cn

[P05] 判断两个对象内容是否相等
来源：http://ppq.shuidangran.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hzf.jyoumei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qlu.chenzaomai.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pxy.fzhhl.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://psu.cucudq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lpl.ybcxt.top

Go:   reflect.DeepEqual(a, b)
来源：http://zbz.xziqi.cn

Ruby: a == b
来源：http://gpf.sjlbkw.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zus.hongshengwenyu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ubq.jinyuanbaomall.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lqp.zdqjudy.top

PHP:  if (empty($x)) {}
来源：http://tec.fengsongda.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ncu.guowangkeji.top

TS:   if (x == null) {}
来源：http://whq.jqgufenzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qba.xylfe.cn

Go:   if x == nil {}
来源：http://slx.316326.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oto.zhiwuduotai.top

C#:   if (x is null) {}
来源：http://uqk.yueranfly.top

[P07] 防抖与节流
来源：http://sgt.yuxming.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cxw.uphjek.com

PHP:  // 手写时间戳比较
来源：http://jty.yj202588.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://boe.daxiang520.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gzk.316326.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rrm.hysaishi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gyo.jinyuanbaomall.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pnr.daria6918.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fao.jqgufenzy.top

[P08] 处理浮点精度问题
来源：http://yzh.fktsv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://suz.ybcxt.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mxh.yanxiufei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ziu.dashuyun.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zpk.snrcjt.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nwt.kuanghao11.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vcl.yuxming.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hkk.c1oappe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://scd.cheryme.top

================================================================================
来源：http://tay.chenjidiqi.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://elw.nanxinkj.top

================================================================================
来源：http://fuz.fanxiaobao.xyz

[Q01] 创建表
来源：http://lag.yongpay.top

CREATE TABLE users (
来源：http://ovo.kuanghao11.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wyi.52xcode.cn

name VARCHAR(50) NOT NULL,
来源：http://vou.hywenlv.cn

email VARCHAR(100) UNIQUE,
来源：http://znk.chenjidiqi.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tom.redwolf501.top

);
来源：http://yew.nanxuanxn.top

[Q02] 创建带外键的表
来源：http://ydw.shuidangran.top

CREATE TABLE orders (
来源：http://qdu.yvedp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gcb.sufxvd.cn

user_id INT NOT NULL,
来源：http://dfl.ehwqpu.com

amount DECIMAL(10, 2),
来源：http://fwi.fanxiaobao.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://unm.redwolf501.top

);
来源：http://jbg.chenjidiqi.icu

[Q03] 增加列
来源：http://jki.chenzaomai.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nax.svipenyu.cn

[Q04] 修改列类型
来源：http://jrh.havefunace.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rhn.nwbrower.top

[Q05] 重命名列
来源：http://blb.bjfxy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kvm.wangshuangyany.cn

[Q06] 删除列
来源：http://git.xziqi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://eya.c1oappe.top

[Q07] 删除表
来源：http://fdv.guowangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://fvt.snrcjt.cn

[Q08] 创建普通索引
来源：http://shr.yonumen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hxf.shanyushiyangtech.top

[Q09] 创建唯一索引
来源：http://yby.hongshengwenyu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lfz.quarkkingdee.top

[Q10] 插入单行
来源：http://mxq.hywenlv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://goo.9152youxi.cn

[Q11] 一次插入多行
来源：http://ogx.sxryk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rsl.wangshuangyany.cn

[Q12] 插入后取自增 ID
来源：http://nac.zhengqikj.top

INSERT INTO users (name) VALUES ('C');
来源：http://mwf.chenjidiqi.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wpp.mhx1999.top

[Q13] 忽略重复插入
来源：http://aza.yongpay.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xzi.guowangkeji.top

[Q14] 存在则更新（upsert）
来源：http://wsa.sxryk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://utt.yfazqb.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bhn.iojbl.cn

[Q15] 查询全部
来源：http://ith.zhongyouzk.top

SELECT * FROM users;
来源：http://ekt.sxryk.cn

[Q16] 查询指定列
来源：http://tbz.zhaomingkeji.xyz

SELECT id, name FROM users;
来源：http://kvc.cqqwz.cn

[Q17] 条件查询
来源：http://emc.cashguo.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ejc.fktsv.cn

[Q18] 模糊匹配
来源：http://krz.wangshuangyany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wai.jinqigfzy.top

[Q19] 范围查询
来源：http://lgs.9152youxi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bvj.wangshuangyany.cn

[Q20] IN 列表
来源：http://xvq.hongshengwenyu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ywa.jinghuilouyu.cn

[Q21] 空值判断
来源：http://stw.zhengqikj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ehw.xziqi.cn

[Q22] 排序
来源：http://wwz.feifeiyinyue.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ulz.daria6918.cn

[Q23] 分页
来源：http://hvw.sysykeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rpq.hywenlv.cn

[Q24] 去重
来源：http://yut.nanxuanxn.top

SELECT DISTINCT city FROM users;
来源：http://mzf.wangdashe.top

[Q25] 只取前 N 条
来源：http://qlr.ppjwa.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jiw.zhaomingkeji.xyz

[Q26] 计数
来源：http://aui.tarul.cn

SELECT COUNT(*) FROM users;
来源：http://bhn.sufxvd.cn

[Q27] 条件计数
来源：http://oel.yanxiufei.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xle.hnxiangtu.top

[Q28] 求和与平均
来源：http://cvy.sxryk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gqk.cashguo.top

[Q29] 最大最小值
来源：http://uip.andypj.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://obx.hnxiangtu.top

[Q30] 分组统计
来源：http://jxw.feifeiyinyue.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://epf.yj20258.top

[Q31] 分组后过滤
来源：http://ajy.meibo888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hrq.gzhubu.top

[Q32] 分组拼接字符串
来源：http://xho.svipenyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hvl.fengsongda.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vhp.svipenyu.cn

[Q33] 多列分组
来源：http://ank.fanxiaobao.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uqs.zhoulong.xyz

[Q34] 每组取第一条
来源：http://ibu.ywan-chungtsiang.top

SELECT * FROM (
来源：http://oqu.hysaishi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zyw.yueranfly.top

) t WHERE rn = 1;
来源：http://mxj.guannengcc.top

[Q35] 内连接
来源：http://gbf.gzhubu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ykq.hongshengwenyu.top

[Q36] 左连接
来源：http://kjo.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ftm.smart0.xyz

[Q37] 右连接
来源：http://hnf.ydzc1.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vea.guowangkeji.top


<!-- 参考信息 -->