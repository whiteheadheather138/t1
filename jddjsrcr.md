代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xyl.aizwys.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tnd.epnwcf.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ekz.jinqigufen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yil.yongpay.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://itm.0kj1m.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kmq.xuanzx.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hkw.ehwqpu.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ubp.gzhubu.top

[N05] 最大公约数
来源：http://luw.hongshengwenyu.top

Py:   math.gcd(a, b)
来源：http://sjs.nanxuanxn.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mwf.zhixingplan.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ojj.yj202588.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tlq.dianchejie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tok.nanxinkj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dpv.jiagoushi.top

Ruby: a.gcd(b)
来源：http://mup.jyoumei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://arz.0kj1m.cn

[N06] 判断回文字符串
来源：http://qoe.gzhubu.top

Py:   s == s[::-1]
来源：http://crj.ppjwa.cn

PHP:  $s === strrev($s);
来源：http://qfg.shuidangran.top

JS:   s === [...s].reverse().join("")
来源：http://xmg.xuanzx.com

TS:   s === [...s].reverse().join("")
来源：http://fuq.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zwn.zhiwuduotai.top

Go:   // 双指针从两端比较
来源：http://dko.jinqigfzy.top

Ruby: s == s.reverse
来源：http://sct.jlsjyb.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zci.sweek.top

[N07] 两数之和（返回下标）
来源：http://exk.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ucb.gaohongyu789.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qkr.andypj.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://yej.52xcode.cn

TS:   // 手写 Map<string, number>
来源：http://cae.c1oappe.top

Java: // 手写 HashMap
来源：http://ltm.fktsv.cn

Go:   // 手写 map[int]int
来源：http://yeo.fanxiaobao.xyz

Ruby: // 手写 Hash
来源：http://afl.xuetiantiany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xvx.ydjk.org.cn

[N08] 生成全排列
来源：http://qcr.jinyuanbaomall.cn

Py:   itertools.permutations(arr)
来源：http://iht.bjfxy.top

PHP:  // 手写递归交换
来源：http://lri.quarkkingdee.top

JS:   // 手写回溯递归
来源：http://yji.ivvv.top

TS:   // 手写回溯递归
来源：http://iqs.ppjwa.cn

Java: // 手写回溯递归
来源：http://cvp.jinqigufen.top

Go:   // 手写回溯递归
来源：http://rky.hcnkem.com

Ruby: arr.permutation.to_a
来源：http://cac.hysaishi.cn

C#:   // 手写回溯递归
来源：http://rfg.wangshuangyany.cn

[N09] 栈与队列
来源：http://rhb.gzhubu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lbv.shanyushiyangkeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://clp.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dhc.gzhubu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vzm.tanke756.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pnj.ppjwa.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ysu.dashuyun.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ofm.yangfankeji.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eyj.zycfv.cn

[N10] 链表节点定义
来源：http://rjt.kuanghao11.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xpz.daxiang520.top

PHP:  class Node { public $v; public $next = null; }
来源：http://pbz.zhiwuduotai.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lwq.vqdsnc.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://czx.jiagoushi.top

Java: class Node { int v; Node next; }
来源：http://ylz.ybcxt.top

Go:   type Node struct { V int; Next *Node }
来源：http://hhr.cashguo.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hkc.cucudq.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rog.jqgfzy.top

[N11] 二叉树中序遍历
来源：http://pei.yangfankeji.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ywz.yuxming.cn

PHP:  // 手写递归函数
来源：http://nsb.hfpthk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jzn.c1oappe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mrd.hysaishi.cn

Java: // 手写递归
来源：http://yzq.ctjpmb.com

Go:   // 手写递归
来源：http://cam.52xcode.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ueu.jinqigfzy.top

C#:   // 手写递归
来源：http://pff.iojbl.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cdv.nwbrower.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jpd.jlsjyb.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://iss.jqgufenzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uda.sjlbkw.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lwp.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ahq.guannengcc.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zjm.shanyushiyangtech.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lif.fktsv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gyu.kuanghao11.cn

================================================================================
来源：http://akt.yongpay.top

O. 并发与异步
来源：http://sgx.bjfxy.top

================================================================================
来源：http://iuw.xylfe.cn

[O01] 启动一个线程
来源：http://xzk.xylfe.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gvt.fehbvm.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zjp.yuanzhike.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ypa.shuidangran.top

TS:   // 同 JS
来源：http://srh.jiagoushi.top

Java: new Thread(() -> f()).start()
来源：http://hpc.hnqzz.top

Go:   go f()
来源：http://bpj.jinyuanbaomall.cn

Ruby: Thread.new { f }
来源：http://nmb.jqgfzy.top

C#:   Task.Run(() => F());
来源：http://fvz.dianchejie.cn

[O02] 使用线程池
来源：http://zgu.epnwcf.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xxd.pycfn.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uio.jlsjyb.cn

JS:   // worker_threads 线程池
来源：http://raj.jlsjyb.cn

TS:   // worker_threads 线程池
来源：http://txa.sysykeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://rmo.yonumen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fee.mhx1999.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://phs.xziqi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lgw.fehbvm.com

[O03] 加锁保护共享数据
来源：http://pji.yueranfly.top

Py:   with lock: shared += 1
来源：http://hka.bbcook.cn

PHP:  // 用 flock() 做文件锁
来源：http://ooj.kuanghao11.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hgw.cdnleiting.top

TS:   // 同 JS
来源：http://dri.jiagoushi.top

Java: synchronized (this) { shared++; }
来源：http://xfk.zhoulong.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ggs.jlsjyb.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pqw.nanxinkj.top

C#:   lock (gate) { shared++; }
来源：http://ekn.yuanzhike.top

[O04] 定义异步函数并等待
来源：http://pzi.pycfn.com

Py:   async def f():⏎    await g()
来源：http://tdx.daria6918.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tcb.daria6918.cn

JS:   async function f() { await g(); }
来源：http://uqr.jqgufenzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ppc.gzhubu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pwa.jinyuanbaomall.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rwo.ppjwa.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ice.shuidangran.top

C#:   async Task F() { await G(); }
来源：http://dau.haohaochexian.top

[O05] 并发执行并等待全部完成
来源：http://unj.birdmap.top

Py:   asyncio.gather(*tasks)
来源：http://sxe.jinghuilouyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sns.zhijiandao.cn

JS:   await Promise.all(tasks)
来源：http://eit.hnxiangtu.top

TS:   await Promise.all(tasks)
来源：http://ywq.bjfxy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pst.316326.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://car.svipenyu.cn

Ruby: threads.map(&:join)
来源：http://dyu.xinyue.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://edw.haohaochexian.top

[O06] 使用进程池
来源：http://ecl.ivvv.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tfm.ctjpmb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://lvj.yj202588.top

JS:   // child_process / cluster 模块
来源：http://hoh.nanxuanxn.top

TS:   // child_process / cluster 模块
来源：http://xtc.316326.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ldq.jlsjyb.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://suv.quarkkingdee.top

Ruby: // fork 块
来源：http://qyw.jyoumei.cn

C#:   Parallel.For
来源：http://whf.hywenlv.cn

================================================================================
来源：http://hjq.snrcjt.cn

P. 常用工具函数
来源：http://iwx.316326.xyz

================================================================================
来源：http://oga.pycfn.com

[P01] 生成 UUID
来源：http://nhz.iojbl.cn

Py:   str(uuid.uuid4())
来源：http://ehw.fktsv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jsy.guowangkeji.top

JS:   crypto.randomUUID()
来源：http://jle.ehwqpu.com

TS:   crypto.randomUUID()
来源：http://axs.sweek.top

Java: UUID.randomUUID().toString()
来源：http://xij.zhengqikj.top

Go:   // 用 github.com/google/uuid
来源：http://txq.sufxvd.cn

Ruby: SecureRandom.uuid
来源：http://lva.fengsongda.top

C#:   Guid.NewGuid().ToString()
来源：http://diq.birdmap.top

[P02] MD5 / SHA256 摘要
来源：http://ody.gotoacloud.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ybj.feifeiyinyue.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xkt.uphjek.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ihe.hnxiangtu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://axu.tian-w.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://igd.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zzt.jinqigufen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://afa.chenjidiqi.icu

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hwc.guowangkeji.top

[P03] 生成短随机字符串
来源：http://wtg.jinqigfzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jvl.xinyue.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lyd.yj20258888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kqt.daxiang520.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ggc.fktsv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://awb.mhx1999.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mab.havefunace.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bjk.meibo888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tsx.hammf.cn

[P04] 求长度
来源：http://lho.guowangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tsy.52xcode.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ovv.zhoulong.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wbb.gzhubu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xiz.zhongyouzk.top

Java: list.size();  map.size();  s.length()
来源：http://xoy.jinqigufen.top

Go:   len(arr);  len(m)
来源：http://ndq.yj20258888.top

Ruby: x.length;  x.size
来源：http://ggn.chenzaomai.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://ctv.c1oappe.top

[P05] 判断两个对象内容是否相等
来源：http://hrg.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://man.fktsv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xkl.yj20258.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uxp.shzxlz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://khb.gotoacloud.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iam.0kj1m.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wzf.fengsongda.top

Ruby: a == b
来源：http://tev.smart0.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tpy.jiagoushi.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tkd.gzhubu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cwv.shangyingyoupin.top

PHP:  if (empty($x)) {}
来源：http://jof.jiagoushi.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jhb.yuanzhike.top

TS:   if (x == null) {}
来源：http://ewf.yangfankeji.com

Java: if (x == null || x.isEmpty()) {}
来源：http://zhq.haohaochexian.top

Go:   if x == nil {}
来源：http://xyk.bjfxy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fqr.zhongyouzk.top

C#:   if (x is null) {}
来源：http://bxh.iojbl.cn

[P07] 防抖与节流
来源：http://sef.ydzc1.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jes.bbcook.cn

PHP:  // 手写时间戳比较
来源：http://mtd.fktsv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rer.smart0.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xeg.chenlongwang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fpg.cqqwz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://psc.chenjidiqi.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://oxo.xuetiantiany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tde.316326.xyz

[P08] 处理浮点精度问题
来源：http://rrj.tarul.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kza.c1oappe.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gwr.ydjk.org.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://icj.cucudq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gsr.gaohongyu789.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ngq.cashguo.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://udo.birdmap.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://veu.zhongyouzk.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ooz.ctjpmb.com

================================================================================
来源：http://txw.sxryk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://edq.gogol.net.cn

================================================================================
来源：http://uem.quarkkingdee.top

[Q01] 创建表
来源：http://rhr.yongpay.top

CREATE TABLE users (
来源：http://ojm.kuanghao11.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tao.feifeiyinyue.top

name VARCHAR(50) NOT NULL,
来源：http://jxn.hnqzz.top

email VARCHAR(100) UNIQUE,
来源：http://gwb.gogol.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xop.9152youxi.cn

);
来源：http://yqr.hywenlv.cn

[Q02] 创建带外键的表
来源：http://ftg.haohaochexian.top

CREATE TABLE orders (
来源：http://bzs.nwbrower.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pxf.jyoumei.cn

user_id INT NOT NULL,
来源：http://rql.shuidangran.top

amount DECIMAL(10, 2),
来源：http://eun.vqdsnc.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fkz.ppjwa.cn

);
来源：http://smo.dashuyun.cn

[Q03] 增加列
来源：http://hil.fzhhl.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qib.zdbjq.cn

[Q04] 修改列类型
来源：http://uxt.yuanzhike.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tvc.yfazqb.com

[Q05] 重命名列
来源：http://uhm.yangfankeji.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qsu.hfpthk.cn

[Q06] 删除列
来源：http://ibt.yuanzhike.top

ALTER TABLE users DROP COLUMN age;
来源：http://fmr.fktsv.cn

[Q07] 删除表
来源：http://esp.vehdjk.com

DROP TABLE IF EXISTS orders;
来源：http://rib.jyoumei.cn

[Q08] 创建普通索引
来源：http://gog.yueranfly.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qge.xuanzx.com

[Q09] 创建唯一索引
来源：http://civ.aizwys.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uob.ppjwa.cn

[Q10] 插入单行
来源：http://gun.cqqwz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hpa.gotoacloud.top

[Q11] 一次插入多行
来源：http://orw.316326.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://imk.tian-w.cn

[Q12] 插入后取自增 ID
来源：http://dsi.jinqigfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://zro.sysykeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fgi.daxiang520.top

[Q13] 忽略重复插入
来源：http://whi.shanyushiyangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wxk.ppjwa.cn

[Q14] 存在则更新（upsert）
来源：http://cli.hammf.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hxk.hesvh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vai.tarul.cn

[Q15] 查询全部
来源：http://krp.wangshuangyany.cn

SELECT * FROM users;
来源：http://lhx.hysaishi.cn

[Q16] 查询指定列
来源：http://bkc.gotoacloud.top

SELECT id, name FROM users;
来源：http://pda.redwolf501.top

[Q17] 条件查询
来源：http://vwk.chenlongwang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://krx.sufxvd.cn

[Q18] 模糊匹配
来源：http://plo.yueranfly.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ipz.wangshuangyany.cn

[Q19] 范围查询
来源：http://omt.gogol.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://byn.fktsv.cn

[Q20] IN 列表
来源：http://atc.52xcode.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lah.c1oappe.top

[Q21] 空值判断
来源：http://nnh.yongpay.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vuc.jinqigufen.top

[Q22] 排序
来源：http://wrq.jqgfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://iwb.ywan-chungtsiang.top

[Q23] 分页
来源：http://mdr.jyoumei.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zzk.gaohongyu789.top

[Q24] 去重
来源：http://zvq.gogol.net.cn

SELECT DISTINCT city FROM users;
来源：http://pzm.andypj.xyz

[Q25] 只取前 N 条
来源：http://sys.jlsjyb.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vjo.ydzc1.top

[Q26] 计数
来源：http://nsv.zdqjudy.top

SELECT COUNT(*) FROM users;
来源：http://rss.jinqigfzy.top

[Q27] 条件计数
来源：http://srg.gaohongyu789.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hvf.gzhubu.top

[Q28] 求和与平均
来源：http://dwi.zycfv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lfv.xuetiantiany.cn

[Q29] 最大最小值
来源：http://pda.xuetiantiany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tzi.fanxiaobao.xyz

[Q30] 分组统计
来源：http://uky.yanxiufei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rnz.yvedp.cn

[Q31] 分组后过滤
来源：http://efk.tarul.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zjc.tian-w.cn

[Q32] 分组拼接字符串
来源：http://muq.jinyuanbaomall.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tur.uphjek.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hgb.xuanzx.com

[Q33] 多列分组
来源：http://blc.mhx1999.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cbz.sxryk.cn

[Q34] 每组取第一条
来源：http://yfy.xuetiantiany.cn

SELECT * FROM (
来源：http://qlu.birdmap.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tat.bbcook.cn

) t WHERE rn = 1;
来源：http://xda.jqgufenzy.top

[Q35] 内连接
来源：http://oaj.haohaochexian.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mcq.xziqi.cn


<!-- 参考信息 -->