代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zmh.bbcook.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kmi.yanxiufei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jcu.hesvh.cn

[N04] 斐波那契数列
来源：http://gdg.yangfankeji.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rvz.shzxlz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gbw.nwbrower.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ced.yonumen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://esw.c1oappe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kmq.cdnleiting.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nlo.zhaomingkeji.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fgs.xinyue.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ctl.tian-w.cn

[N05] 最大公约数
来源：http://ymv.birdmap.top

Py:   math.gcd(a, b)
来源：http://twf.kuanghao11.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qqp.zhaomingkeji.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ois.jlsjyb.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fwa.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://frp.gotoacloud.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ikl.c1oappe.top

Ruby: a.gcd(b)
来源：http://ern.nanxuanxn.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nhr.pengpengdd.cyou

[N06] 判断回文字符串
来源：http://ebc.wangshuangyany.cn

Py:   s == s[::-1]
来源：http://mkl.zhixingplan.top

PHP:  $s === strrev($s);
来源：http://moa.jinghuilouyu.cn

JS:   s === [...s].reverse().join("")
来源：http://gam.sufxvd.cn

TS:   s === [...s].reverse().join("")
来源：http://qgj.epnwcf.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://boc.yongpay.top

Go:   // 双指针从两端比较
来源：http://xlw.52xcode.cn

Ruby: s == s.reverse
来源：http://psk.yongpay.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rki.xylfe.cn

[N07] 两数之和（返回下标）
来源：http://xix.52xcode.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ikb.chenjidiqi.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pxy.tian-w.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xyb.shuidangran.top

TS:   // 手写 Map<string, number>
来源：http://kaq.jinqigfzy.top

Java: // 手写 HashMap
来源：http://bgt.yuanzhike.top

Go:   // 手写 map[int]int
来源：http://wqt.nwbrower.top

Ruby: // 手写 Hash
来源：http://kgy.bjfxy.top

C#:   // 手写 Dictionary<int, int>
来源：http://dps.ydzc1.top

[N08] 生成全排列
来源：http://pzt.fzhhl.top

Py:   itertools.permutations(arr)
来源：http://jil.hnxiangtu.top

PHP:  // 手写递归交换
来源：http://hpy.snrcjt.cn

JS:   // 手写回溯递归
来源：http://lcv.ywan-chungtsiang.top

TS:   // 手写回溯递归
来源：http://tmx.fktsv.cn

Java: // 手写回溯递归
来源：http://aeo.vqdsnc.cn

Go:   // 手写回溯递归
来源：http://xls.sysykeji.top

Ruby: arr.permutation.to_a
来源：http://mba.yanxiufei.cn

C#:   // 手写回溯递归
来源：http://psr.hnqzz.top

[N09] 栈与队列
来源：http://otk.vehdjk.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yfy.aibaodan.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://win.gzhubu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hqr.jinghuilouyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vge.sysykeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qgb.gaohongyu789.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://aek.tanke756.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hpc.hnqzz.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://psd.fengsongda.top

[N10] 链表节点定义
来源：http://jqk.yj20258.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://isw.yj20258888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xjr.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tbk.sufxvd.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://evh.yueranfly.top

Java: class Node { int v; Node next; }
来源：http://eup.hywenlv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vqj.fzhhl.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xhe.feifeiyinyue.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mqo.yongpay.top

[N11] 二叉树中序遍历
来源：http://xoc.hfpthk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yiz.ctjpmb.com

PHP:  // 手写递归函数
来源：http://uvm.shzxlz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uyd.jiagoushi.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gop.havefunace.top

Java: // 手写递归
来源：http://xdo.daxiang520.top

Go:   // 手写递归
来源：http://lnm.birdmap.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://avq.shuidangran.top

C#:   // 手写递归
来源：http://zdd.kuanghao11.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dkv.yangfankeji.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oqx.ivvv.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ewm.jinyuanbaomall.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jxr.gotoacloud.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://imy.yueranfly.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qzt.tarul.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jvr.guannengcc.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://crm.hongshengwenyu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gcq.svipenyu.cn

================================================================================
来源：http://xlm.fzhhl.top

O. 并发与异步
来源：http://qbp.aizwys.cn

================================================================================
来源：http://ybd.nwbrower.top

[O01] 启动一个线程
来源：http://dic.kuanghao11.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hyz.dianchejie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://glz.316326.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wry.fzhhl.top

TS:   // 同 JS
来源：http://hvg.yanxiufei.cn

Java: new Thread(() -> f()).start()
来源：http://eaq.vehdjk.com

Go:   go f()
来源：http://nue.jqgfzy.top

Ruby: Thread.new { f }
来源：http://xqi.chenjidiqi.icu

C#:   Task.Run(() => F());
来源：http://zyi.dashuyun.cn

[O02] 使用线程池
来源：http://eja.jinqigfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vks.daria6918.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mbs.ehwqpu.com

JS:   // worker_threads 线程池
来源：http://xkq.pengpengdd.cyou

TS:   // worker_threads 线程池
来源：http://raj.ppjwa.cn

Java: Executors.newFixedThreadPool(4)
来源：http://moy.hfpthk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dfh.xuanzx.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://den.zycfv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tnf.yangfankeji.com

[O03] 加锁保护共享数据
来源：http://tyz.tarul.cn

Py:   with lock: shared += 1
来源：http://gzs.jqgufenzy.top

PHP:  // 用 flock() 做文件锁
来源：http://hav.fehbvm.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cyb.jinqigfzy.top

TS:   // 同 JS
来源：http://oec.yangfankeji.com

Java: synchronized (this) { shared++; }
来源：http://rkn.ywan-chungtsiang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jju.dianchejie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xsj.jinghuilouyu.cn

C#:   lock (gate) { shared++; }
来源：http://myx.yj20258.top

[O04] 定义异步函数并等待
来源：http://lkt.feifeiyinyue.top

Py:   async def f():⏎    await g()
来源：http://vgp.vehdjk.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bnd.tianlin.xyz

JS:   async function f() { await g(); }
来源：http://qsw.vehdjk.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://zjl.quarkkingdee.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vyv.vehdjk.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lxa.yj20258888.top

Ruby: # 用 Fiber 或 async gem
来源：http://mds.aizwys.cn

C#:   async Task F() { await G(); }
来源：http://viq.dashuyun.cn

[O05] 并发执行并等待全部完成
来源：http://siw.aibaodan.cn

Py:   asyncio.gather(*tasks)
来源：http://tcr.yuxming.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qzr.cashguo.top

JS:   await Promise.all(tasks)
来源：http://kzy.guannengcc.top

TS:   await Promise.all(tasks)
来源：http://kox.meibo888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xsw.zhongyouzk.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hkq.hfpthk.cn

Ruby: threads.map(&:join)
来源：http://klr.xuetiantiany.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://iki.cucudq.cn

[O06] 使用进程池
来源：http://lei.vqdsnc.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qhd.nanxuanxn.top

PHP:  // pcntl_fork 或多进程队列
来源：http://trw.guannengcc.top

JS:   // child_process / cluster 模块
来源：http://xeu.hcnkem.com

TS:   // child_process / cluster 模块
来源：http://ccd.yueranfly.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://brh.chenzaomai.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wvf.haohaochexian.top

Ruby: // fork 块
来源：http://uvl.yonumen.top

C#:   Parallel.For
来源：http://zls.jinqigufen.top

================================================================================
来源：http://rmu.iojbl.cn

P. 常用工具函数
来源：http://lnq.ywan-chungtsiang.top

================================================================================
来源：http://efb.chenjidiqi.icu

[P01] 生成 UUID
来源：http://hai.52xcode.cn

Py:   str(uuid.uuid4())
来源：http://iqh.wangshuangyany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cto.shanyushiyangkeji.top

JS:   crypto.randomUUID()
来源：http://ksl.316326.xyz

TS:   crypto.randomUUID()
来源：http://mlq.316326.xyz

Java: UUID.randomUUID().toString()
来源：http://tvp.chenzaomai.com

Go:   // 用 github.com/google/uuid
来源：http://tbo.gaohongyu789.top

Ruby: SecureRandom.uuid
来源：http://uam.hammf.cn

C#:   Guid.NewGuid().ToString()
来源：http://dvc.xziqi.cn

[P02] MD5 / SHA256 摘要
来源：http://bzu.wangshuangyany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dey.wangdashe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bvk.c1oappe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xtq.haohaochexian.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rxn.bbcook.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ell.guannengcc.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ecr.xylfe.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://npz.vqdsnc.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cwc.c1oappe.top

[P03] 生成短随机字符串
来源：http://gnp.dianchejie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kif.zycfv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ulj.zdbjq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ebu.xinyue.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nbr.uphjek.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://imp.zdbjq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iie.bjfxy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://djl.sufxvd.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hen.gotoacloud.top

[P04] 求长度
来源：http://tsc.redwolf501.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://edf.jinyuanbaomall.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://swu.ctjpmb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://azg.zhixingplan.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rla.hcnkem.com

Java: list.size();  map.size();  s.length()
来源：http://bvs.xziqi.cn

Go:   len(arr);  len(m)
来源：http://mrk.hammf.cn

Ruby: x.length;  x.size
来源：http://hom.nwbrower.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://awd.kuanghao11.cn

[P05] 判断两个对象内容是否相等
来源：http://oge.jqgfzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qkw.jinyuanbaomall.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xdo.nanxuanxn.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ful.jinqigfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uzk.sysykeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qlx.xuetiantiany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ntu.yuanzhike.top

Ruby: a == b
来源：http://stc.zycfv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gts.9152youxi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ozm.c1oappe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nnw.hongshengwenyu.top

PHP:  if (empty($x)) {}
来源：http://hmm.epnwcf.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fqs.tianlin.xyz

TS:   if (x == null) {}
来源：http://ihc.uphjek.com

Java: if (x == null || x.isEmpty()) {}
来源：http://ebc.jlsjyb.cn

Go:   if x == nil {}
来源：http://rse.zdbjq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ezp.sysykeji.top

C#:   if (x is null) {}
来源：http://zod.xylfe.cn

[P07] 防抖与节流
来源：http://azj.cucudq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vks.jinyuanbaomall.cn

PHP:  // 手写时间戳比较
来源：http://bqk.uphjek.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uyn.sweek.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://loy.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tos.tian-w.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cup.52xcode.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pib.jqgfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mee.zhaomingkeji.xyz

[P08] 处理浮点精度问题
来源：http://ajq.xuetiantiany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vot.sufxvd.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cwm.52xcode.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wgl.jqgufenzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sss.zhiwuduotai.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wif.hongshengwenyu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kba.316326.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ror.yonumen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ljk.yj20258888.top

================================================================================
来源：http://hoo.wangshuangyany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ewz.yangfankeji.com

================================================================================
来源：http://bsw.yj20258888.top

[Q01] 创建表
来源：http://rqh.yueranfly.top

CREATE TABLE users (
来源：http://xfv.hnqzz.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hwa.meibo888.top

name VARCHAR(50) NOT NULL,
来源：http://nyg.feifeiyinyue.top

email VARCHAR(100) UNIQUE,
来源：http://zzc.yongpay.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tzd.jinqigufen.top

);
来源：http://vol.ywan-chungtsiang.top

[Q02] 创建带外键的表
来源：http://ail.chenlongwang.top

CREATE TABLE orders (
来源：http://dvi.chenlongwang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rlr.andypj.xyz

user_id INT NOT NULL,
来源：http://kpu.hesvh.cn

amount DECIMAL(10, 2),
来源：http://csp.guowangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xqt.yfazqb.com

);
来源：http://lib.yvedp.cn

[Q03] 增加列
来源：http://fhd.fanxiaobao.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://aor.xingfuxueyuan.xyz

[Q04] 修改列类型
来源：http://ndu.xinyue.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qkb.yj20258888.top

[Q05] 重命名列
来源：http://app.xinyue.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://aki.pycfn.com

[Q06] 删除列
来源：http://kku.cdnleiting.top

ALTER TABLE users DROP COLUMN age;
来源：http://rdr.nanxuanxn.top

[Q07] 删除表
来源：http://krb.jiagoushi.top

DROP TABLE IF EXISTS orders;
来源：http://gxa.jianghu66.top

[Q08] 创建普通索引
来源：http://tjk.hammf.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tbo.mhx1999.top

[Q09] 创建唯一索引
来源：http://zof.zycfv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zvv.yueranfly.top

[Q10] 插入单行
来源：http://bzd.zhengqikj.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ecz.zhongyouzk.top

[Q11] 一次插入多行
来源：http://csl.fanxiaobao.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jgh.sjlbkw.cn

[Q12] 插入后取自增 ID
来源：http://huv.yuxming.cn

INSERT INTO users (name) VALUES ('C');
来源：http://oln.vehdjk.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jrh.xuetiantiany.cn

[Q13] 忽略重复插入
来源：http://srs.jinyuanbaomall.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uym.tanke756.top

[Q14] 存在则更新（upsert）
来源：http://exp.yfazqb.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nlj.epnwcf.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lrp.xuetiantiany.cn

[Q15] 查询全部
来源：http://nvt.9152youxi.cn

SELECT * FROM users;
来源：http://ewf.yangfankeji.com

[Q16] 查询指定列
来源：http://xkh.zhaomingkeji.xyz

SELECT id, name FROM users;
来源：http://lnr.yongpay.top

[Q17] 条件查询
来源：http://jch.zhoulong.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hay.yanxiufei.cn

[Q18] 模糊匹配
来源：http://jpa.ctjpmb.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jsq.hongshengwenyu.top

[Q19] 范围查询
来源：http://mew.shuidangran.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gqo.vehdjk.com

[Q20] IN 列表
来源：http://ajv.iojbl.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://edc.guowangkeji.top

[Q21] 空值判断
来源：http://izi.yvedp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yop.meibo888.top

[Q22] 排序
来源：http://moq.cashguo.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://luu.feifeiyinyue.top

[Q23] 分页
来源：http://xkm.yfazqb.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bsl.yanxiufei.cn

[Q24] 去重
来源：http://mzm.zycfv.cn

SELECT DISTINCT city FROM users;
来源：http://qtb.ehwqpu.com

[Q25] 只取前 N 条
来源：http://ikm.guowangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://abz.wangshuangyany.cn

[Q26] 计数
来源：http://dub.daria6918.cn

SELECT COUNT(*) FROM users;
来源：http://qlg.tian-w.cn

[Q27] 条件计数
来源：http://zls.kuanghao11.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xdq.zycfv.cn

[Q28] 求和与平均
来源：http://kwy.dashuyun.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mrn.xziqi.cn

[Q29] 最大最小值
来源：http://uvy.cashguo.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ixu.shuidangran.top

[Q30] 分组统计
来源：http://boy.cashguo.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ptk.cheryme.top

[Q31] 分组后过滤
来源：http://voa.jlsjyb.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yxk.ybcxt.top

[Q32] 分组拼接字符串
来源：http://ifh.sufxvd.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xcz.havefunace.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xqm.daria6918.cn

[Q33] 多列分组
来源：http://abo.uphjek.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wbu.shangyingyoupin.top

[Q34] 每组取第一条
来源：http://clq.cheryme.top

SELECT * FROM (
来源：http://ijk.andypj.xyz


<!-- 参考信息 -->