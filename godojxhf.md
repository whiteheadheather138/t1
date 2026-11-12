代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://agr.cashguo.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iue.jinyuanbaomall.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://edx.jinqigfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://crf.ctjpmb.com

[N05] 最大公约数
来源：http://wty.cheryme.top

Py:   math.gcd(a, b)
来源：http://cfb.uphjek.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bgk.birdmap.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://huc.xuetiantiany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ipf.havefunace.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tqs.quarkkingdee.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ezc.feifeiyinyue.top

Ruby: a.gcd(b)
来源：http://pwn.ywan-chungtsiang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mbk.ydjk.org.cn

[N06] 判断回文字符串
来源：http://xml.fzhhl.top

Py:   s == s[::-1]
来源：http://tsb.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://ezz.wangshuangyany.cn

JS:   s === [...s].reverse().join("")
来源：http://cxm.kuanghao11.cn

TS:   s === [...s].reverse().join("")
来源：http://mxn.fktsv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hvk.tianlin.xyz

Go:   // 双指针从两端比较
来源：http://edp.yangfankeji.com

Ruby: s == s.reverse
来源：http://jtv.yangfankeji.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://zph.snrcjt.cn

[N07] 两数之和（返回下标）
来源：http://kuk.tanke756.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ibj.iojbl.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ddj.yj202588.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xma.zhaomingkeji.xyz

TS:   // 手写 Map<string, number>
来源：http://pec.bjfxy.top

Java: // 手写 HashMap
来源：http://pdz.fanxiaobao.xyz

Go:   // 手写 map[int]int
来源：http://cik.gaohongyu789.top

Ruby: // 手写 Hash
来源：http://slc.daria6918.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iwj.yongpay.top

[N08] 生成全排列
来源：http://xij.yfazqb.com

Py:   itertools.permutations(arr)
来源：http://nob.yangfankeji.com

PHP:  // 手写递归交换
来源：http://mmm.vqdsnc.cn

JS:   // 手写回溯递归
来源：http://nid.fzhhl.top

TS:   // 手写回溯递归
来源：http://dbc.iojbl.cn

Java: // 手写回溯递归
来源：http://jsh.yvedp.cn

Go:   // 手写回溯递归
来源：http://qub.ydjk.org.cn

Ruby: arr.permutation.to_a
来源：http://gra.fengsongda.top

C#:   // 手写回溯递归
来源：http://hlr.ydjk.org.cn

[N09] 栈与队列
来源：http://zit.tarul.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hyf.hnqzz.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hcz.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xyz.ehwqpu.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hvq.meibo888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cli.fktsv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://avv.guannengcc.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hir.jinyuanbaomall.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gpg.yonumen.top

[N10] 链表节点定义
来源：http://xup.vehdjk.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nsk.zdqjudy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kac.52xcode.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oni.xuetiantiany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ckf.xingfuxueyuan.xyz

Java: class Node { int v; Node next; }
来源：http://dpe.hfpthk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sfp.jqgfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bzl.xuanzx.com

C#:   class Node { public int V; public Node? Next; }
来源：http://gjo.hesvh.cn

[N11] 二叉树中序遍历
来源：http://ddv.cheryme.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vje.aizwys.cn

PHP:  // 手写递归函数
来源：http://sbe.zhongyouzk.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oxd.pycfn.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rnq.cucudq.cn

Java: // 手写递归
来源：http://yqh.xuetiantiany.cn

Go:   // 手写递归
来源：http://akc.tarul.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ort.vehdjk.com

C#:   // 手写递归
来源：http://tzz.hnxiangtu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bmx.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vft.zycfv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yen.jqgufenzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sqd.yj20258888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uqw.cdnleiting.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bps.ydzc1.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://apu.zhengqikj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://huh.c1oappe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mfj.xziqi.cn

================================================================================
来源：http://mti.hongshengwenyu.top

O. 并发与异步
来源：http://pme.pengpengdd.cyou

================================================================================
来源：http://iru.hcnkem.com

[O01] 启动一个线程
来源：http://ues.jinyuanbaomall.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jgf.fanxiaobao.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jai.52xcode.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lum.iojbl.cn

TS:   // 同 JS
来源：http://nik.tianlin.xyz

Java: new Thread(() -> f()).start()
来源：http://xgd.vehdjk.com

Go:   go f()
来源：http://eul.ydjk.org.cn

Ruby: Thread.new { f }
来源：http://jvw.xziqi.cn

C#:   Task.Run(() => F());
来源：http://jcs.zycfv.cn

[O02] 使用线程池
来源：http://bac.zhongyouzk.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qvq.yj20258888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kko.ydzc1.top

JS:   // worker_threads 线程池
来源：http://rdb.mhx1999.top

TS:   // worker_threads 线程池
来源：http://pyp.zhiwuduotai.top

Java: Executors.newFixedThreadPool(4)
来源：http://ihf.aibaodan.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://egy.hesvh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ugw.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nba.svipenyu.cn

[O03] 加锁保护共享数据
来源：http://ihk.ywan-chungtsiang.top

Py:   with lock: shared += 1
来源：http://cch.iojbl.cn

PHP:  // 用 flock() 做文件锁
来源：http://vmx.hammf.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gxi.tarul.cn

TS:   // 同 JS
来源：http://zfl.jlsjyb.cn

Java: synchronized (this) { shared++; }
来源：http://ghw.xingfuxueyuan.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iid.hesvh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://iqk.yj20258888.top

C#:   lock (gate) { shared++; }
来源：http://pdd.jinqigufen.top

[O04] 定义异步函数并等待
来源：http://mab.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://fun.yj20258888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uzd.chenlongwang.top

JS:   async function f() { await g(); }
来源：http://vcl.vqdsnc.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vri.sxryk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hle.sysykeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wvo.gaohongyu789.top

Ruby: # 用 Fiber 或 async gem
来源：http://pmv.cdnleiting.top

C#:   async Task F() { await G(); }
来源：http://tea.tarul.cn

[O05] 并发执行并等待全部完成
来源：http://lqn.jlsjyb.cn

Py:   asyncio.gather(*tasks)
来源：http://cqc.ydjk.org.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mdw.shanyushiyangtech.top

JS:   await Promise.all(tasks)
来源：http://tni.shanyushiyangtech.top

TS:   await Promise.all(tasks)
来源：http://fuj.hysaishi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vhf.nwbrower.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ueu.yj202588.top

Ruby: threads.map(&:join)
来源：http://mgd.gzhubu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zuv.yj20258.top

[O06] 使用进程池
来源：http://lhj.zhoulong.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fyo.yueranfly.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gok.quarkkingdee.top

JS:   // child_process / cluster 模块
来源：http://xih.wangdashe.top

TS:   // child_process / cluster 模块
来源：http://duz.ctjpmb.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xiv.pengpengdd.cyou

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rhy.ivvv.top

Ruby: // fork 块
来源：http://oqh.dianchejie.cn

C#:   Parallel.For
来源：http://cqs.shzxlz.cn

================================================================================
来源：http://hpi.guowangkeji.top

P. 常用工具函数
来源：http://djb.gzhubu.top

================================================================================
来源：http://pje.xinyue.icu

[P01] 生成 UUID
来源：http://vuh.hcnkem.com

Py:   str(uuid.uuid4())
来源：http://eow.aibaodan.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dsl.cdnleiting.top

JS:   crypto.randomUUID()
来源：http://jno.fehbvm.com

TS:   crypto.randomUUID()
来源：http://tbb.cqqwz.cn

Java: UUID.randomUUID().toString()
来源：http://qhf.tianlin.xyz

Go:   // 用 github.com/google/uuid
来源：http://tyg.jlsjyb.cn

Ruby: SecureRandom.uuid
来源：http://tix.sufxvd.cn

C#:   Guid.NewGuid().ToString()
来源：http://qtx.yj20258888.top

[P02] MD5 / SHA256 摘要
来源：http://wdv.jinqigufen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kxp.bjfxy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mva.snrcjt.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sbf.chenlongwang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://evs.zhixingplan.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ttl.vqdsnc.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rlk.yongpay.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vfk.hongshengwenyu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yng.ctjpmb.com

[P03] 生成短随机字符串
来源：http://bee.xuetiantiany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://unx.yangfankeji.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kjf.chenlongwang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://obc.hcnkem.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kgb.zhengqikj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nmw.iojbl.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yyp.guowangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://szi.smart0.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mfy.aizwys.cn

[P04] 求长度
来源：http://buk.zhongyouzk.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uku.gogol.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kel.gzhubu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qwl.svipenyu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oge.zhixingplan.top

Java: list.size();  map.size();  s.length()
来源：http://upf.shangyingyoupin.top

Go:   len(arr);  len(m)
来源：http://atu.aizwys.cn

Ruby: x.length;  x.size
来源：http://adm.hnqzz.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bdx.zhoulong.xyz

[P05] 判断两个对象内容是否相等
来源：http://baq.c1oappe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qry.shuidangran.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://api.hysaishi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bmj.jlsjyb.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xyi.9152youxi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gyf.ehwqpu.com

Go:   reflect.DeepEqual(a, b)
来源：http://nfg.jqgufenzy.top

Ruby: a == b
来源：http://dtr.fzhhl.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bvv.jlsjyb.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qte.kuanghao11.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xyb.ydzc1.top

PHP:  if (empty($x)) {}
来源：http://auu.bjfxy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xse.hnqzz.top

TS:   if (x == null) {}
来源：http://wie.ydjk.org.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://blx.guowangkeji.top

Go:   if x == nil {}
来源：http://czt.svipenyu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rvp.jiagoushi.top

C#:   if (x is null) {}
来源：http://uxs.wangshuangyany.cn

[P07] 防抖与节流
来源：http://xaf.ctjpmb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rtm.birdmap.top

PHP:  // 手写时间戳比较
来源：http://hat.shuidangran.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hmv.jinqigufen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bnx.cdnleiting.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nje.jinghuilouyu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vta.ywan-chungtsiang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xke.jinqigufen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xxt.52xcode.cn

[P08] 处理浮点精度问题
来源：http://zez.jinqigufen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://frx.ybcxt.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kkc.ydjk.org.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rqn.sjlbkw.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bsh.bbcook.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ncz.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ren.bbcook.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hrt.ivvv.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xgb.tanke756.top

================================================================================
来源：http://xsj.nwbrower.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fxl.zdbjq.cn

================================================================================
来源：http://hsj.tianlin.xyz

[Q01] 创建表
来源：http://rte.fktsv.cn

CREATE TABLE users (
来源：http://ett.pycfn.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://poi.snrcjt.cn

name VARCHAR(50) NOT NULL,
来源：http://vvv.smart0.xyz

email VARCHAR(100) UNIQUE,
来源：http://uta.nanxuanxn.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vkw.tanke756.top

);
来源：http://ffh.tanke756.top

[Q02] 创建带外键的表
来源：http://bzw.smart0.xyz

CREATE TABLE orders (
来源：http://maz.aizwys.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kve.svipenyu.cn

user_id INT NOT NULL,
来源：http://ilz.zdqjudy.top

amount DECIMAL(10, 2),
来源：http://ybn.meibo888.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ypl.jinghuilouyu.cn

);
来源：http://cuu.havefunace.top

[Q03] 增加列
来源：http://nrk.kuanghao11.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eqn.tianlin.xyz

[Q04] 修改列类型
来源：http://gab.ydjk.org.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iaw.yongpay.top

[Q05] 重命名列
来源：http://trq.xuetiantiany.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xwj.hysaishi.cn

[Q06] 删除列
来源：http://emo.daria6918.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kuy.shanyushiyangkeji.top

[Q07] 删除表
来源：http://vnt.zhiwuduotai.top

DROP TABLE IF EXISTS orders;
来源：http://rkj.dianchejie.cn

[Q08] 创建普通索引
来源：http://etx.gogol.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rzc.yuanzhike.top

[Q09] 创建唯一索引
来源：http://txw.chenjidiqi.icu

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xeu.fktsv.cn

[Q10] 插入单行
来源：http://zxe.yongpay.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bnv.wangshuangyany.cn

[Q11] 一次插入多行
来源：http://ysq.fehbvm.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aay.haohaochexian.top

[Q12] 插入后取自增 ID
来源：http://loq.pycfn.com

INSERT INTO users (name) VALUES ('C');
来源：http://jia.sweek.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ibd.jinqigufen.top

[Q13] 忽略重复插入
来源：http://vts.shangyingyoupin.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pvs.epnwcf.com

[Q14] 存在则更新（upsert）
来源：http://ayi.zhiwuduotai.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ngf.zdbjq.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://knc.bjfxy.top

[Q15] 查询全部
来源：http://vps.uphjek.com

SELECT * FROM users;
来源：http://lkt.shzxlz.cn

[Q16] 查询指定列
来源：http://ggx.zycfv.cn

SELECT id, name FROM users;
来源：http://kat.sysykeji.top

[Q17] 条件查询
来源：http://pfv.meibo888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pqt.jinghuilouyu.cn

[Q18] 模糊匹配
来源：http://haj.jqgfzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ajb.dashuyun.cn

[Q19] 范围查询
来源：http://qwk.birdmap.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cga.nanxinkj.top

[Q20] IN 列表
来源：http://jnv.yj20258888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zgx.hnxiangtu.top

[Q21] 空值判断
来源：http://jrg.cqqwz.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://apl.gotoacloud.top

[Q22] 排序
来源：http://uwv.zhengqikj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xvk.yueranfly.top

[Q23] 分页
来源：http://hsu.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rfx.hammf.cn

[Q24] 去重
来源：http://wwu.daria6918.cn

SELECT DISTINCT city FROM users;
来源：http://nda.pycfn.com

[Q25] 只取前 N 条
来源：http://cva.ppjwa.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xab.hammf.cn

[Q26] 计数
来源：http://xmr.zdbjq.cn

SELECT COUNT(*) FROM users;
来源：http://ohn.tarul.cn

[Q27] 条件计数
来源：http://mvg.sysykeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qam.gaohongyu789.top

[Q28] 求和与平均
来源：http://npl.zhoulong.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mcs.316326.xyz

[Q29] 最大最小值
来源：http://xcb.zhixingplan.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dfc.smart0.xyz

[Q30] 分组统计
来源：http://qlm.ppjwa.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://avz.iojbl.cn

[Q31] 分组后过滤
来源：http://wku.vqdsnc.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uzr.hammf.cn

[Q32] 分组拼接字符串
来源：http://lvo.haohaochexian.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zqn.ivvv.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://haz.xuetiantiany.cn

[Q33] 多列分组
来源：http://ohy.tarul.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mxc.gzhubu.top

[Q34] 每组取第一条
来源：http://yti.jinghuilouyu.cn

SELECT * FROM (
来源：http://umg.aizwys.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ksp.zdqjudy.top

) t WHERE rn = 1;
来源：http://mfp.cashguo.top

[Q35] 内连接
来源：http://wbn.xziqi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kpa.52xcode.cn

[Q36] 左连接
来源：http://kju.316326.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vbg.hcnkem.com

[Q37] 右连接
来源：http://rgh.ivvv.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qdr.jinyuanbaomall.cn


<!-- 参考信息 -->