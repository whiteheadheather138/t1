代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gfs.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gzu.kuanghao11.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gdj.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://umr.jyoumei.cn

[N05] 最大公约数
来源：http://vxd.epnwcf.com

Py:   math.gcd(a, b)
来源：http://bef.gaohongyu789.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xlz.cdnleiting.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nqm.xinyue.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://byb.sysykeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oih.vehdjk.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bjd.bbcook.cn

Ruby: a.gcd(b)
来源：http://fxc.yuxming.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zrd.xuanzx.com

[N06] 判断回文字符串
来源：http://eia.fktsv.cn

Py:   s == s[::-1]
来源：http://lgl.jinghuilouyu.cn

PHP:  $s === strrev($s);
来源：http://ccv.cashguo.top

JS:   s === [...s].reverse().join("")
来源：http://rne.guannengcc.top

TS:   s === [...s].reverse().join("")
来源：http://wai.yfazqb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nbu.cucudq.cn

Go:   // 双指针从两端比较
来源：http://fsf.yj20258.top

Ruby: s == s.reverse
来源：http://mqj.yangfankeji.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://xlx.meibo888.top

[N07] 两数之和（返回下标）
来源：http://dmg.hywenlv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ftm.jyoumei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dtx.fanxiaobao.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://woc.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://bwh.sufxvd.cn

Java: // 手写 HashMap
来源：http://kqs.cqqwz.cn

Go:   // 手写 map[int]int
来源：http://poi.tian-w.cn

Ruby: // 手写 Hash
来源：http://ger.sxryk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ipx.yfazqb.com

[N08] 生成全排列
来源：http://jlp.svipenyu.cn

Py:   itertools.permutations(arr)
来源：http://sur.xuetiantiany.cn

PHP:  // 手写递归交换
来源：http://zxg.dianchejie.cn

JS:   // 手写回溯递归
来源：http://bqb.xinyue.icu

TS:   // 手写回溯递归
来源：http://brb.sxryk.cn

Java: // 手写回溯递归
来源：http://ekb.nanxuanxn.top

Go:   // 手写回溯递归
来源：http://ukd.zhongyouzk.top

Ruby: arr.permutation.to_a
来源：http://mzd.yonumen.top

C#:   // 手写回溯递归
来源：http://ooh.xylfe.cn

[N09] 栈与队列
来源：http://nxx.jqgfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mgm.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xda.mhx1999.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uas.gaohongyu789.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://myv.jinghuilouyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ocp.jiagoushi.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mea.hywenlv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hyy.cheryme.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vmk.ivvv.top

[N10] 链表节点定义
来源：http://ntt.jyoumei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qyj.cashguo.top

PHP:  class Node { public $v; public $next = null; }
来源：http://exr.svipenyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dsj.yanxiufei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xsg.hongshengwenyu.top

Java: class Node { int v; Node next; }
来源：http://ltd.cheryme.top

Go:   type Node struct { V int; Next *Node }
来源：http://nsy.birdmap.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gxd.zhoulong.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://xha.xuetiantiany.cn

[N11] 二叉树中序遍历
来源：http://qoh.jlsjyb.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uus.hnqzz.top

PHP:  // 手写递归函数
来源：http://izd.chenzaomai.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://spv.daxiang520.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eja.chenjidiqi.icu

Java: // 手写递归
来源：http://szs.andypj.xyz

Go:   // 手写递归
来源：http://bxi.yj20258888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ltm.jinqigufen.top

C#:   // 手写递归
来源：http://viu.52xcode.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aiw.vqdsnc.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rvv.nwbrower.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dyz.cashguo.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xlb.jlsjyb.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vuo.hywenlv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zks.cqqwz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gtl.vehdjk.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iie.epnwcf.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yhz.tanke756.top

================================================================================
来源：http://mql.yj20258888.top

O. 并发与异步
来源：http://vsd.wangdashe.top

================================================================================
来源：http://gvo.fanxiaobao.xyz

[O01] 启动一个线程
来源：http://hie.redwolf501.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jfw.daxiang520.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lwo.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cvu.bjfxy.top

TS:   // 同 JS
来源：http://eqj.yanxiufei.cn

Java: new Thread(() -> f()).start()
来源：http://poc.sjlbkw.cn

Go:   go f()
来源：http://mqu.cheryme.top

Ruby: Thread.new { f }
来源：http://yas.guowangkeji.top

C#:   Task.Run(() => F());
来源：http://rhe.yvedp.cn

[O02] 使用线程池
来源：http://uik.tarul.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iam.zhaomingkeji.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xsc.zdbjq.cn

JS:   // worker_threads 线程池
来源：http://cdq.chenjidiqi.icu

TS:   // worker_threads 线程池
来源：http://npg.shuidangran.top

Java: Executors.newFixedThreadPool(4)
来源：http://rif.tarul.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wzg.dianchejie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://saj.yuxming.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dkb.hongshengwenyu.top

[O03] 加锁保护共享数据
来源：http://ams.chenzaomai.com

Py:   with lock: shared += 1
来源：http://jxm.hcnkem.com

PHP:  // 用 flock() 做文件锁
来源：http://vsj.hywenlv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gow.zdbjq.cn

TS:   // 同 JS
来源：http://ivk.cdnleiting.top

Java: synchronized (this) { shared++; }
来源：http://kmn.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rjd.wangshuangyany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://exl.shanyushiyangkeji.top

C#:   lock (gate) { shared++; }
来源：http://gom.jinqigfzy.top

[O04] 定义异步函数并等待
来源：http://qkd.birdmap.top

Py:   async def f():⏎    await g()
来源：http://uwk.chenlongwang.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://syw.haohaochexian.top

JS:   async function f() { await g(); }
来源：http://hrf.meibo888.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://iqm.xinyue.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wee.52xcode.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yta.xingfuxueyuan.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://nob.yj20258.top

C#:   async Task F() { await G(); }
来源：http://dbc.snrcjt.cn

[O05] 并发执行并等待全部完成
来源：http://njz.fzhhl.top

Py:   asyncio.gather(*tasks)
来源：http://erj.andypj.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vdt.ydjk.org.cn

JS:   await Promise.all(tasks)
来源：http://szl.dashuyun.cn

TS:   await Promise.all(tasks)
来源：http://zew.dianchejie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pmh.hongshengwenyu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hhu.daxiang520.top

Ruby: threads.map(&:join)
来源：http://xbm.quarkkingdee.top

C#:   await Task.WhenAll(t1, t2)
来源：http://vxo.jqgufenzy.top

[O06] 使用进程池
来源：http://xgy.xuetiantiany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vhs.jqgfzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://rui.hammf.cn

JS:   // child_process / cluster 模块
来源：http://diq.cucudq.cn

TS:   // child_process / cluster 模块
来源：http://mxe.epnwcf.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bvs.gotoacloud.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bcd.zhengqikj.top

Ruby: // fork 块
来源：http://vlo.havefunace.top

C#:   Parallel.For
来源：http://ill.haohaochexian.top

================================================================================
来源：http://yxo.cqqwz.cn

P. 常用工具函数
来源：http://xzo.ehwqpu.com

================================================================================
来源：http://dai.jlsjyb.cn

[P01] 生成 UUID
来源：http://lcn.vehdjk.com

Py:   str(uuid.uuid4())
来源：http://eat.jinqigfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wzt.zhijiandao.cn

JS:   crypto.randomUUID()
来源：http://wew.feifeiyinyue.top

TS:   crypto.randomUUID()
来源：http://wmz.gaohongyu789.top

Java: UUID.randomUUID().toString()
来源：http://tit.yueranfly.top

Go:   // 用 github.com/google/uuid
来源：http://yob.9152youxi.cn

Ruby: SecureRandom.uuid
来源：http://tzj.xziqi.cn

C#:   Guid.NewGuid().ToString()
来源：http://xox.ppjwa.cn

[P02] MD5 / SHA256 摘要
来源：http://vby.birdmap.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kym.zdbjq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dow.yvedp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rqb.fengsongda.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tdf.tian-w.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nkx.cucudq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ebz.hywenlv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://acj.jyoumei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bfx.ywan-chungtsiang.top

[P03] 生成短随机字符串
来源：http://chj.hcnkem.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wfl.fzhhl.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kyp.ppjwa.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://new.nanxinkj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wlk.cdnleiting.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://icc.xingfuxueyuan.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uce.yuanzhike.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ifr.shangyingyoupin.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jbd.zhijiandao.cn

[P04] 求长度
来源：http://wrk.jyoumei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://css.chenjidiqi.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://osn.c1oappe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ftk.zdbjq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://isz.wangshuangyany.cn

Java: list.size();  map.size();  s.length()
来源：http://xhw.zhiwuduotai.top

Go:   len(arr);  len(m)
来源：http://mjk.sweek.top

Ruby: x.length;  x.size
来源：http://cfj.fanxiaobao.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://hzf.xuanzx.com

[P05] 判断两个对象内容是否相等
来源：http://cwm.zycfv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ort.chenjidiqi.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uxk.yonumen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://teh.yanxiufei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dif.yonumen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://prq.hongshengwenyu.top

Go:   reflect.DeepEqual(a, b)
来源：http://hfa.aibaodan.cn

Ruby: a == b
来源：http://cyk.guowangkeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dlq.uphjek.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qzq.tarul.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zzi.sufxvd.cn

PHP:  if (empty($x)) {}
来源：http://iie.jqgfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ecg.zhaomingkeji.xyz

TS:   if (x == null) {}
来源：http://skl.hnqzz.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mwu.hcnkem.com

Go:   if x == nil {}
来源：http://kfu.feifeiyinyue.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dht.hywenlv.cn

C#:   if (x is null) {}
来源：http://zcp.zhoulong.xyz

[P07] 防抖与节流
来源：http://nmo.0kj1m.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pom.bjfxy.top

PHP:  // 手写时间戳比较
来源：http://qmf.jyoumei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qnj.wangshuangyany.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cly.daxiang520.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hbn.daria6918.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rms.jqgufenzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mxx.jyoumei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bmg.hcnkem.com

[P08] 处理浮点精度问题
来源：http://ccw.zhiwuduotai.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ypq.fengsongda.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vvd.gaohongyu789.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zdu.316326.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lxt.ctjpmb.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xpv.cashguo.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pfv.aibaodan.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wvx.dashuyun.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ysb.uphjek.com

================================================================================
来源：http://smg.ybcxt.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ghf.hcnkem.com

================================================================================
来源：http://pfx.shanyushiyangkeji.top

[Q01] 创建表
来源：http://nyh.hnqzz.top

CREATE TABLE users (
来源：http://sts.guowangkeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vxa.yj20258888.top

name VARCHAR(50) NOT NULL,
来源：http://qto.shangyingyoupin.top

email VARCHAR(100) UNIQUE,
来源：http://yxx.dashuyun.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nnb.epnwcf.com

);
来源：http://kwh.guowangkeji.top

[Q02] 创建带外键的表
来源：http://ldp.quarkkingdee.top

CREATE TABLE orders (
来源：http://dbv.quarkkingdee.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gms.yj20258.top

user_id INT NOT NULL,
来源：http://sbh.0kj1m.cn

amount DECIMAL(10, 2),
来源：http://bqf.chenzaomai.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://aky.cqqwz.cn

);
来源：http://ozt.sweek.top

[Q03] 增加列
来源：http://yeg.uphjek.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ong.vehdjk.com

[Q04] 修改列类型
来源：http://mfo.tian-w.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://crf.nanxuanxn.top

[Q05] 重命名列
来源：http://ebc.fanxiaobao.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kap.ywan-chungtsiang.top

[Q06] 删除列
来源：http://qci.0kj1m.cn

ALTER TABLE users DROP COLUMN age;
来源：http://iaq.aizwys.cn

[Q07] 删除表
来源：http://lji.pengpengdd.cyou

DROP TABLE IF EXISTS orders;
来源：http://vwp.tarul.cn

[Q08] 创建普通索引
来源：http://qbn.sufxvd.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rds.jyoumei.cn

[Q09] 创建唯一索引
来源：http://uoe.gaohongyu789.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xfj.vqdsnc.cn

[Q10] 插入单行
来源：http://dqc.fanxiaobao.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ngs.sufxvd.cn

[Q11] 一次插入多行
来源：http://pdn.cashguo.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yyt.ybcxt.top

[Q12] 插入后取自增 ID
来源：http://ggi.gzhubu.top

INSERT INTO users (name) VALUES ('C');
来源：http://wpv.haohaochexian.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://voz.tarul.cn

[Q13] 忽略重复插入
来源：http://jir.hnqzz.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nzs.guannengcc.top

[Q14] 存在则更新（upsert）
来源：http://cna.ywan-chungtsiang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://omy.zhixingplan.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ypr.jlsjyb.cn

[Q15] 查询全部
来源：http://sla.epnwcf.com

SELECT * FROM users;
来源：http://cpd.tarul.cn

[Q16] 查询指定列
来源：http://jyo.bbcook.cn

SELECT id, name FROM users;
来源：http://dtt.cucudq.cn

[Q17] 条件查询
来源：http://bfp.jqgfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xql.gotoacloud.top

[Q18] 模糊匹配
来源：http://uzt.shanyushiyangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hon.nanxinkj.top

[Q19] 范围查询
来源：http://swk.hywenlv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cpz.dianchejie.cn

[Q20] IN 列表
来源：http://vor.yj20258888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rfs.hcnkem.com

[Q21] 空值判断
来源：http://pmx.svipenyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rsh.zhaomingkeji.xyz

[Q22] 排序
来源：http://pur.hnxiangtu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ukc.smart0.xyz

[Q23] 分页
来源：http://mru.shanyushiyangtech.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://umg.pycfn.com

[Q24] 去重
来源：http://vfw.hcnkem.com

SELECT DISTINCT city FROM users;
来源：http://sih.andypj.xyz

[Q25] 只取前 N 条
来源：http://dfb.smart0.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://iro.yvedp.cn

[Q26] 计数
来源：http://ykn.zdbjq.cn

SELECT COUNT(*) FROM users;
来源：http://pwf.birdmap.top

[Q27] 条件计数
来源：http://obp.c1oappe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iwe.ppjwa.cn

[Q28] 求和与平均
来源：http://amk.9152youxi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ndz.epnwcf.com

[Q29] 最大最小值
来源：http://bfa.aibaodan.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bbv.sufxvd.cn

[Q30] 分组统计
来源：http://oao.jinqigufen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tcr.tianlin.xyz

[Q31] 分组后过滤
来源：http://kaj.redwolf501.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cqn.ydjk.org.cn

[Q32] 分组拼接字符串
来源：http://cxz.yj202588.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jsm.zhoulong.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qlk.quarkkingdee.top

[Q33] 多列分组
来源：http://yta.jinghuilouyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tul.iojbl.cn

[Q34] 每组取第一条
来源：http://bcj.cqqwz.cn

SELECT * FROM (
来源：http://plr.xinyue.icu

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jqs.ivvv.top

) t WHERE rn = 1;
来源：http://kqg.havefunace.top

[Q35] 内连接
来源：http://jur.hcnkem.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://irp.daria6918.cn

[Q36] 左连接
来源：http://jgd.yonumen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uxi.hfpthk.cn

[Q37] 右连接
来源：http://cjq.yuxming.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mnc.sweek.top


<!-- 参考信息 -->