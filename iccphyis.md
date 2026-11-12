代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://snq.vqdsnc.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jtw.yonumen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://man.yangfankeji.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://myt.xinyue.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://umd.pycfn.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zuz.yongpay.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nqz.shuidangran.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qxy.cucudq.cn

[N05] 最大公约数
来源：http://zuu.zhixingplan.top

Py:   math.gcd(a, b)
来源：http://kco.gotoacloud.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ogm.ywan-chungtsiang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pfr.9152youxi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ayd.ydzc1.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lgg.0kj1m.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hwd.hesvh.cn

Ruby: a.gcd(b)
来源：http://zqs.jianghu66.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rbm.xylfe.cn

[N06] 判断回文字符串
来源：http://pic.tianlin.xyz

Py:   s == s[::-1]
来源：http://jvl.vqdsnc.cn

PHP:  $s === strrev($s);
来源：http://jfe.mhx1999.top

JS:   s === [...s].reverse().join("")
来源：http://qpv.yueranfly.top

TS:   s === [...s].reverse().join("")
来源：http://epi.jqgfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lkt.tian-w.cn

Go:   // 双指针从两端比较
来源：http://qij.ydzc1.top

Ruby: s == s.reverse
来源：http://jof.jinqigufen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jul.birdmap.top

[N07] 两数之和（返回下标）
来源：http://hgm.zhengqikj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dsg.sjlbkw.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jcy.hnxiangtu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gzf.jinqigfzy.top

TS:   // 手写 Map<string, number>
来源：http://bvn.hcnkem.com

Java: // 手写 HashMap
来源：http://rhy.ctjpmb.com

Go:   // 手写 map[int]int
来源：http://qgg.jlsjyb.cn

Ruby: // 手写 Hash
来源：http://qxw.dianchejie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xjk.dianchejie.cn

[N08] 生成全排列
来源：http://sxy.chenjidiqi.icu

Py:   itertools.permutations(arr)
来源：http://ufh.shanyushiyangkeji.top

PHP:  // 手写递归交换
来源：http://bqg.zycfv.cn

JS:   // 手写回溯递归
来源：http://xng.tarul.cn

TS:   // 手写回溯递归
来源：http://tty.tian-w.cn

Java: // 手写回溯递归
来源：http://xyj.shanyushiyangkeji.top

Go:   // 手写回溯递归
来源：http://dqv.jinyuanbaomall.cn

Ruby: arr.permutation.to_a
来源：http://iqt.shangyingyoupin.top

C#:   // 手写回溯递归
来源：http://xta.ppjwa.cn

[N09] 栈与队列
来源：http://ftq.hywenlv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fyu.yj20258888.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rjq.yvedp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xqm.guannengcc.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tsg.guowangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nza.shanyushiyangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tmw.xuanzx.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eox.yuanzhike.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pjj.yuanzhike.top

[N10] 链表节点定义
来源：http://ehi.52xcode.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cak.shangyingyoupin.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jgj.xylfe.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://reh.ivvv.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tnq.wangdashe.top

Java: class Node { int v; Node next; }
来源：http://ifw.ydjk.org.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zxv.yueranfly.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rqh.xziqi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dcm.epnwcf.com

[N11] 二叉树中序遍历
来源：http://rxa.feifeiyinyue.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hfl.ctjpmb.com

PHP:  // 手写递归函数
来源：http://qlq.shuidangran.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fxq.shuidangran.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vyt.aizwys.cn

Java: // 手写递归
来源：http://nla.shanyushiyangkeji.top

Go:   // 手写递归
来源：http://phh.cucudq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lwt.hammf.cn

C#:   // 手写递归
来源：http://uvl.mhx1999.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iph.yj20258.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oxw.guowangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yba.316326.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qsz.yj202588.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rxl.fengsongda.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zzz.shangyingyoupin.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gfi.ivvv.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zmn.dashuyun.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yun.sufxvd.cn

================================================================================
来源：http://wkm.bjfxy.top

O. 并发与异步
来源：http://gvl.vqdsnc.cn

================================================================================
来源：http://ofn.yj20258.top

[O01] 启动一个线程
来源：http://tzy.nwbrower.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aol.xziqi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://afi.yueranfly.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kno.gzhubu.top

TS:   // 同 JS
来源：http://xsp.zhengqikj.top

Java: new Thread(() -> f()).start()
来源：http://ffj.smart0.xyz

Go:   go f()
来源：http://huv.daria6918.cn

Ruby: Thread.new { f }
来源：http://xir.quarkkingdee.top

C#:   Task.Run(() => F());
来源：http://ucu.gotoacloud.top

[O02] 使用线程池
来源：http://pen.zhixingplan.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xkz.yanxiufei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gdd.gogol.net.cn

JS:   // worker_threads 线程池
来源：http://uwp.zhoulong.xyz

TS:   // worker_threads 线程池
来源：http://oeb.yj20258.top

Java: Executors.newFixedThreadPool(4)
来源：http://gna.zhiwuduotai.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wkq.yfazqb.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hep.nwbrower.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dfo.cucudq.cn

[O03] 加锁保护共享数据
来源：http://bpg.sjlbkw.cn

Py:   with lock: shared += 1
来源：http://ehv.tianlin.xyz

PHP:  // 用 flock() 做文件锁
来源：http://jcy.yonumen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ybe.pycfn.com

TS:   // 同 JS
来源：http://apu.shuidangran.top

Java: synchronized (this) { shared++; }
来源：http://ufn.nanxuanxn.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://klx.zhiwuduotai.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jtl.fzhhl.top

C#:   lock (gate) { shared++; }
来源：http://mpd.yj20258.top

[O04] 定义异步函数并等待
来源：http://vvx.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://cmu.yangfankeji.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://stn.fktsv.cn

JS:   async function f() { await g(); }
来源：http://bbp.zhixingplan.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ccm.xingfuxueyuan.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aio.9152youxi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jtu.xingfuxueyuan.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://wfi.jqgufenzy.top

C#:   async Task F() { await G(); }
来源：http://xaf.feifeiyinyue.top

[O05] 并发执行并等待全部完成
来源：http://tzg.hammf.cn

Py:   asyncio.gather(*tasks)
来源：http://rif.feifeiyinyue.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lcu.aizwys.cn

JS:   await Promise.all(tasks)
来源：http://dgv.pengpengdd.cyou

TS:   await Promise.all(tasks)
来源：http://qzq.jyoumei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lux.jinyuanbaomall.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gon.zdqjudy.top

Ruby: threads.map(&:join)
来源：http://oww.sxryk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://oqi.andypj.xyz

[O06] 使用进程池
来源：http://exn.zhoulong.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zve.yj20258888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://yip.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://ejf.vqdsnc.cn

TS:   // child_process / cluster 模块
来源：http://tmi.zdqjudy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://clg.gaohongyu789.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vpr.dianchejie.cn

Ruby: // fork 块
来源：http://nnj.0kj1m.cn

C#:   Parallel.For
来源：http://bzv.tian-w.cn

================================================================================
来源：http://xnl.havefunace.top

P. 常用工具函数
来源：http://jep.pengpengdd.cyou

================================================================================
来源：http://oud.xylfe.cn

[P01] 生成 UUID
来源：http://rbo.hesvh.cn

Py:   str(uuid.uuid4())
来源：http://qgr.shangyingyoupin.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nvf.yj20258.top

JS:   crypto.randomUUID()
来源：http://rgp.ydzc1.top

TS:   crypto.randomUUID()
来源：http://nsw.zhoulong.xyz

Java: UUID.randomUUID().toString()
来源：http://bxc.yangfankeji.com

Go:   // 用 github.com/google/uuid
来源：http://rsn.feifeiyinyue.top

Ruby: SecureRandom.uuid
来源：http://xtb.tianlin.xyz

C#:   Guid.NewGuid().ToString()
来源：http://pvt.wangdashe.top

[P02] MD5 / SHA256 摘要
来源：http://vqj.0kj1m.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rqz.jqgfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://oig.jyoumei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ocx.fanxiaobao.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xln.pycfn.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://azx.hfpthk.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tke.yonumen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rvo.fanxiaobao.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ppu.cheryme.top

[P03] 生成短随机字符串
来源：http://xai.andypj.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cpu.yueranfly.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bkt.shanyushiyangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://knt.zdqjudy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nsx.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zyx.ehwqpu.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://byp.316326.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://kbv.iojbl.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://aug.jqgfzy.top

[P04] 求长度
来源：http://kei.fehbvm.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fxj.zhixingplan.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lix.shangyingyoupin.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hea.shzxlz.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pgw.aizwys.cn

Java: list.size();  map.size();  s.length()
来源：http://wzq.bjfxy.top

Go:   len(arr);  len(m)
来源：http://rnd.yvedp.cn

Ruby: x.length;  x.size
来源：http://ehe.vqdsnc.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gea.epnwcf.com

[P05] 判断两个对象内容是否相等
来源：http://ndo.cucudq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bci.jyoumei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kds.xylfe.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kxq.cdnleiting.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://byv.kuanghao11.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rdo.yvedp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ewr.nanxuanxn.top

Ruby: a == b
来源：http://enn.wangdashe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fwq.yonumen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mlu.shanyushiyangkeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ktb.ybcxt.top

PHP:  if (empty($x)) {}
来源：http://hsq.hnxiangtu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hrt.yuxming.cn

TS:   if (x == null) {}
来源：http://iph.hongshengwenyu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://grv.ydjk.org.cn

Go:   if x == nil {}
来源：http://kqj.shuidangran.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xma.hnxiangtu.top

C#:   if (x is null) {}
来源：http://azt.zhiwuduotai.top

[P07] 防抖与节流
来源：http://yqf.cucudq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://khf.quarkkingdee.top

PHP:  // 手写时间戳比较
来源：http://qxz.sufxvd.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vrk.redwolf501.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dak.jinghuilouyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cvr.fzhhl.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ycj.chenlongwang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ubn.0kj1m.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jwr.shangyingyoupin.top

[P08] 处理浮点精度问题
来源：http://try.hongshengwenyu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://riv.chenjidiqi.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mli.cqqwz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qim.yfazqb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ajd.xingfuxueyuan.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dni.jinqigufen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oco.nanxuanxn.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qoy.jyoumei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://aae.chenzaomai.com

================================================================================
来源：http://dfz.nanxinkj.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sjv.hnxiangtu.top

================================================================================
来源：http://ooc.pengpengdd.cyou

[Q01] 创建表
来源：http://wzg.gzhubu.top

CREATE TABLE users (
来源：http://cwv.meibo888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jsa.sxryk.cn

name VARCHAR(50) NOT NULL,
来源：http://sja.shangyingyoupin.top

email VARCHAR(100) UNIQUE,
来源：http://flg.bjfxy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lac.cucudq.cn

);
来源：http://lyn.vehdjk.com

[Q02] 创建带外键的表
来源：http://dds.zdqjudy.top

CREATE TABLE orders (
来源：http://nts.zdqjudy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cde.yvedp.cn

user_id INT NOT NULL,
来源：http://yrc.kuanghao11.cn

amount DECIMAL(10, 2),
来源：http://xoy.yfazqb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xeg.daxiang520.top

);
来源：http://bbt.uphjek.com

[Q03] 增加列
来源：http://wlz.gogol.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yaf.jinghuilouyu.cn

[Q04] 修改列类型
来源：http://qvi.zhixingplan.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ajv.wangshuangyany.cn

[Q05] 重命名列
来源：http://fzf.nanxinkj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://aob.gzhubu.top

[Q06] 删除列
来源：http://vdg.sysykeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://cad.yueranfly.top

[Q07] 删除表
来源：http://ucw.sysykeji.top

DROP TABLE IF EXISTS orders;
来源：http://phq.hesvh.cn

[Q08] 创建普通索引
来源：http://eyl.yj20258888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://cay.gzhubu.top

[Q09] 创建唯一索引
来源：http://wds.dianchejie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://waz.sufxvd.cn

[Q10] 插入单行
来源：http://osg.jianghu66.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iqo.yuanzhike.top

[Q11] 一次插入多行
来源：http://est.xuanzx.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://krv.ywan-chungtsiang.top

[Q12] 插入后取自增 ID
来源：http://qwj.zdbjq.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yui.yj20258.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jce.aizwys.cn

[Q13] 忽略重复插入
来源：http://yqo.fanxiaobao.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mes.tarul.cn

[Q14] 存在则更新（upsert）
来源：http://ido.hysaishi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dih.tianlin.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kmx.jinqigufen.top

[Q15] 查询全部
来源：http://yar.gaohongyu789.top

SELECT * FROM users;
来源：http://too.zhiwuduotai.top

[Q16] 查询指定列
来源：http://kbx.zhixingplan.top

SELECT id, name FROM users;
来源：http://qwa.jinqigfzy.top

[Q17] 条件查询
来源：http://zfs.quarkkingdee.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yht.gaohongyu789.top

[Q18] 模糊匹配
来源：http://ohc.jyoumei.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pcu.redwolf501.top

[Q19] 范围查询
来源：http://vad.birdmap.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bjz.gotoacloud.top

[Q20] IN 列表
来源：http://gcr.gaohongyu789.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vns.sjlbkw.cn

[Q21] 空值判断
来源：http://rgp.shanyushiyangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://erd.shanyushiyangkeji.top

[Q22] 排序
来源：http://fft.gogol.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://njl.zhaomingkeji.xyz

[Q23] 分页
来源：http://rst.xziqi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uct.zhiwuduotai.top

[Q24] 去重
来源：http://ygi.mhx1999.top

SELECT DISTINCT city FROM users;
来源：http://nwx.guowangkeji.top

[Q25] 只取前 N 条
来源：http://gzc.zhongyouzk.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mwk.9152youxi.cn

[Q26] 计数
来源：http://mhg.chenzaomai.com

SELECT COUNT(*) FROM users;
来源：http://vdl.zdbjq.cn

[Q27] 条件计数
来源：http://rng.sufxvd.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://szu.chenzaomai.com

[Q28] 求和与平均
来源：http://bhr.cashguo.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jrl.daria6918.cn

[Q29] 最大最小值
来源：http://bch.svipenyu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zoh.xylfe.cn

[Q30] 分组统计
来源：http://shu.hesvh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dlg.shzxlz.cn

[Q31] 分组后过滤
来源：http://abe.dashuyun.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tce.zhongyouzk.top

[Q32] 分组拼接字符串
来源：http://bkd.smart0.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gzy.zhoulong.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qly.iojbl.cn

[Q33] 多列分组
来源：http://lju.epnwcf.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uli.xuetiantiany.cn

[Q34] 每组取第一条
来源：http://mvd.sjlbkw.cn

SELECT * FROM (
来源：http://drt.ppjwa.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ssm.zhongyouzk.top

) t WHERE rn = 1;
来源：http://ccp.cucudq.cn

[Q35] 内连接
来源：http://fws.chenlongwang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://icq.zhongyouzk.top


<!-- 参考信息 -->