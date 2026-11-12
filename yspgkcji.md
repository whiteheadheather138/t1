代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jom.guannengcc.top

Java: Arrays.binarySearch(arr, x)
来源：http://vaj.zhongyouzk.top

Go:   sort.SearchInts(arr, x)
来源：http://cym.yongpay.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://tjj.nwbrower.top

C#:   Array.BinarySearch(arr, x)
来源：http://ftq.haohaochexian.top

[N02] 排序（工程实践用内置实现）
来源：http://ctk.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://gzc.tarul.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cto.yonumen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nxd.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://tyt.fengsongda.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dfj.hywenlv.cn

Go:   slices.Sort(arr)
来源：http://oew.hysaishi.cn

Ruby: arr.sort
来源：http://wtq.zhixingplan.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gom.vqdsnc.cn

[N03] 快速排序（分治示例）
来源：http://tdj.sufxvd.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gpf.aibaodan.cn

PHP:  // 递归实现，或用 usort
来源：http://yub.sysykeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://feu.bjfxy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://srt.yuanzhike.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vbc.meibo888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zxs.hywenlv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ggf.fengsongda.top

C#:   // 手写递归，或 Array.Sort
来源：http://zss.dashuyun.cn

[N04] 斐波那契数列
来源：http://sqc.yongpay.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://art.andypj.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cza.meibo888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jza.yonumen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zdv.ywan-chungtsiang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hko.zhiwuduotai.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oax.shanyushiyangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dgq.yj202588.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mld.sweek.top

[N05] 最大公约数
来源：http://yef.xylfe.cn

Py:   math.gcd(a, b)
来源：http://cpv.c1oappe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qtv.nwbrower.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rox.chenjidiqi.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wbc.quarkkingdee.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zjo.tanke756.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qhs.ydzc1.top

Ruby: a.gcd(b)
来源：http://cpp.52xcode.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://maj.sufxvd.cn

[N06] 判断回文字符串
来源：http://fpn.zycfv.cn

Py:   s == s[::-1]
来源：http://sno.c1oappe.top

PHP:  $s === strrev($s);
来源：http://zdl.ydjk.org.cn

JS:   s === [...s].reverse().join("")
来源：http://cuf.mhx1999.top

TS:   s === [...s].reverse().join("")
来源：http://nrz.chenjidiqi.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wtv.sjlbkw.cn

Go:   // 双指针从两端比较
来源：http://uqs.52xcode.cn

Ruby: s == s.reverse
来源：http://nvm.9152youxi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fcv.hnxiangtu.top

[N07] 两数之和（返回下标）
来源：http://fsk.jlsjyb.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ftv.svipenyu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gpp.wangshuangyany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wfn.xingfuxueyuan.xyz

TS:   // 手写 Map<string, number>
来源：http://hfw.redwolf501.top

Java: // 手写 HashMap
来源：http://gik.hfpthk.cn

Go:   // 手写 map[int]int
来源：http://bld.zhiwuduotai.top

Ruby: // 手写 Hash
来源：http://frf.sweek.top

C#:   // 手写 Dictionary<int, int>
来源：http://jqh.yfazqb.com

[N08] 生成全排列
来源：http://wdq.uphjek.com

Py:   itertools.permutations(arr)
来源：http://nrg.wangdashe.top

PHP:  // 手写递归交换
来源：http://qpc.vehdjk.com

JS:   // 手写回溯递归
来源：http://pmk.sjlbkw.cn

TS:   // 手写回溯递归
来源：http://pad.xuetiantiany.cn

Java: // 手写回溯递归
来源：http://vms.wangdashe.top

Go:   // 手写回溯递归
来源：http://zkl.zhengqikj.top

Ruby: arr.permutation.to_a
来源：http://toz.cqqwz.cn

C#:   // 手写回溯递归
来源：http://nij.jqgfzy.top

[N09] 栈与队列
来源：http://hzj.ywan-chungtsiang.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://afh.yj202588.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nfk.guannengcc.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hba.xylfe.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rxo.zhongyouzk.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gni.ppjwa.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kcj.pengpengdd.cyou

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lay.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xdx.shuidangran.top

[N10] 链表节点定义
来源：http://nid.fktsv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eya.jqgfzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qhq.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ffe.hongshengwenyu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uhr.cqqwz.cn

Java: class Node { int v; Node next; }
来源：http://yum.fengsongda.top

Go:   type Node struct { V int; Next *Node }
来源：http://gjm.cheryme.top

Ruby: Node = Struct.new(:v, :next)
来源：http://lsi.yueranfly.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lpm.shangyingyoupin.top

[N11] 二叉树中序遍历
来源：http://knh.guannengcc.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lgc.cheryme.top

PHP:  // 手写递归函数
来源：http://pma.sysykeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fio.yueranfly.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vqv.zycfv.cn

Java: // 手写递归
来源：http://bgf.zhixingplan.top

Go:   // 手写递归
来源：http://ujo.kuanghao11.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vux.dianchejie.cn

C#:   // 手写递归
来源：http://bnj.nanxuanxn.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ygw.xylfe.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sua.svipenyu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nlw.yonumen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pcp.bjfxy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://swb.xylfe.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qdj.quarkkingdee.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qlt.dianchejie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://les.chenjidiqi.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qap.svipenyu.cn

================================================================================
来源：http://gag.yvedp.cn

O. 并发与异步
来源：http://vmw.daxiang520.top

================================================================================
来源：http://rgb.redwolf501.top

[O01] 启动一个线程
来源：http://omt.feifeiyinyue.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qsb.chenjidiqi.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bjf.hfpthk.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iqi.hfpthk.cn

TS:   // 同 JS
来源：http://wnk.fanxiaobao.xyz

Java: new Thread(() -> f()).start()
来源：http://qei.9152youxi.cn

Go:   go f()
来源：http://bxk.hnxiangtu.top

Ruby: Thread.new { f }
来源：http://fez.xylfe.cn

C#:   Task.Run(() => F());
来源：http://wwd.chenzaomai.com

[O02] 使用线程池
来源：http://ide.fktsv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://emb.shanyushiyangtech.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ves.xziqi.cn

JS:   // worker_threads 线程池
来源：http://elr.snrcjt.cn

TS:   // worker_threads 线程池
来源：http://bku.yj20258.top

Java: Executors.newFixedThreadPool(4)
来源：http://ypy.52xcode.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dch.hfpthk.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dti.chenzaomai.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://moe.nanxinkj.top

[O03] 加锁保护共享数据
来源：http://uuo.uphjek.com

Py:   with lock: shared += 1
来源：http://oww.yj20258.top

PHP:  // 用 flock() 做文件锁
来源：http://pmd.shuidangran.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qlq.fzhhl.top

TS:   // 同 JS
来源：http://dyl.yueranfly.top

Java: synchronized (this) { shared++; }
来源：http://mko.316326.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gjc.xuanzx.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://zuo.gogol.net.cn

C#:   lock (gate) { shared++; }
来源：http://edy.quarkkingdee.top

[O04] 定义异步函数并等待
来源：http://xcw.zhixingplan.top

Py:   async def f():⏎    await g()
来源：http://dfv.cqqwz.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kkz.iojbl.cn

JS:   async function f() { await g(); }
来源：http://cct.cashguo.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gtv.cucudq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dgm.0kj1m.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pgc.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://ogo.316326.xyz

C#:   async Task F() { await G(); }
来源：http://vkw.jiagoushi.top

[O05] 并发执行并等待全部完成
来源：http://kkh.daria6918.cn

Py:   asyncio.gather(*tasks)
来源：http://auc.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uke.haohaochexian.top

JS:   await Promise.all(tasks)
来源：http://ftk.fengsongda.top

TS:   await Promise.all(tasks)
来源：http://rcg.aizwys.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yet.tianlin.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pjv.ybcxt.top

Ruby: threads.map(&:join)
来源：http://myp.sxryk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kxy.jyoumei.cn

[O06] 使用进程池
来源：http://yyt.52xcode.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vdj.zhaomingkeji.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://ytx.chenlongwang.top

JS:   // child_process / cluster 模块
来源：http://fzz.fehbvm.com

TS:   // child_process / cluster 模块
来源：http://prx.sxryk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ltt.xziqi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gol.fanxiaobao.xyz

Ruby: // fork 块
来源：http://awn.zycfv.cn

C#:   Parallel.For
来源：http://pfx.aibaodan.cn

================================================================================
来源：http://ctw.jinghuilouyu.cn

P. 常用工具函数
来源：http://ngb.zhaomingkeji.xyz

================================================================================
来源：http://xcy.nwbrower.top

[P01] 生成 UUID
来源：http://gax.52xcode.cn

Py:   str(uuid.uuid4())
来源：http://wdx.jqgfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fyj.jinyuanbaomall.cn

JS:   crypto.randomUUID()
来源：http://rde.yj20258.top

TS:   crypto.randomUUID()
来源：http://skr.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://xwq.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://oog.tanke756.top

Ruby: SecureRandom.uuid
来源：http://xhu.cheryme.top

C#:   Guid.NewGuid().ToString()
来源：http://vzt.zhiwuduotai.top

[P02] MD5 / SHA256 摘要
来源：http://vpk.tanke756.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tpc.yfazqb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://maf.xuanzx.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ilf.gotoacloud.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qeg.zycfv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lza.shanyushiyangtech.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ngq.havefunace.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qcv.hywenlv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xaq.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://xnn.tanke756.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fnl.fehbvm.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nvj.pycfn.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fwo.hysaishi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mdd.jqgfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sva.ctjpmb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kxn.nanxinkj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://iap.hfpthk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yvt.kuanghao11.cn

[P04] 求长度
来源：http://uet.cheryme.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mla.zhixingplan.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jon.gogol.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lfx.ivvv.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rlb.uphjek.com

Java: list.size();  map.size();  s.length()
来源：http://bbe.jlsjyb.cn

Go:   len(arr);  len(m)
来源：http://qwf.jyoumei.cn

Ruby: x.length;  x.size
来源：http://pbm.hysaishi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yjz.iojbl.cn

[P05] 判断两个对象内容是否相等
来源：http://aux.cdnleiting.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://tbv.jqgufenzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sev.gogol.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qsg.chenzaomai.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://aoi.dashuyun.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jbz.zdbjq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://web.ydzc1.top

Ruby: a == b
来源：http://mof.xuanzx.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wyk.yj20258.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kll.mhx1999.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oas.gotoacloud.top

PHP:  if (empty($x)) {}
来源：http://ojs.c1oappe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ozq.dianchejie.cn

TS:   if (x == null) {}
来源：http://dcw.cdnleiting.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xfg.hysaishi.cn

Go:   if x == nil {}
来源：http://cff.aizwys.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rps.feifeiyinyue.top

C#:   if (x is null) {}
来源：http://ahf.shzxlz.cn

[P07] 防抖与节流
来源：http://rfe.xuanzx.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kyt.chenjidiqi.icu

PHP:  // 手写时间戳比较
来源：http://jmg.fanxiaobao.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kbv.zhengqikj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cqp.jqgfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mdj.ybcxt.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ezu.uphjek.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://oiw.svipenyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rtm.dianchejie.cn

[P08] 处理浮点精度问题
来源：http://waf.c1oappe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gwm.yanxiufei.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fob.hesvh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dba.shangyingyoupin.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kdb.yongpay.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bpf.vqdsnc.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cdr.daria6918.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pey.xylfe.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pbg.chenzaomai.com

================================================================================
来源：http://xqe.jiagoushi.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ucp.nwbrower.top

================================================================================
来源：http://aff.shanyushiyangkeji.top

[Q01] 创建表
来源：http://kzo.316326.xyz

CREATE TABLE users (
来源：http://sbg.andypj.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ksl.xylfe.cn

name VARCHAR(50) NOT NULL,
来源：http://jau.cqqwz.cn

email VARCHAR(100) UNIQUE,
来源：http://btv.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wmd.cucudq.cn

);
来源：http://nsr.redwolf501.top

[Q02] 创建带外键的表
来源：http://voq.sxryk.cn

CREATE TABLE orders (
来源：http://auo.ctjpmb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jdw.52xcode.cn

user_id INT NOT NULL,
来源：http://vsa.redwolf501.top

amount DECIMAL(10, 2),
来源：http://mhx.sysykeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ams.daria6918.cn

);
来源：http://dlq.ydjk.org.cn

[Q03] 增加列
来源：http://pre.fehbvm.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dfd.xinyue.icu

[Q04] 修改列类型
来源：http://epf.jlsjyb.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pbh.hywenlv.cn

[Q05] 重命名列
来源：http://asz.epnwcf.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nha.xingfuxueyuan.xyz

[Q06] 删除列
来源：http://bft.fengsongda.top

ALTER TABLE users DROP COLUMN age;
来源：http://pit.yueranfly.top

[Q07] 删除表
来源：http://uln.jyoumei.cn

DROP TABLE IF EXISTS orders;
来源：http://ldv.chenlongwang.top

[Q08] 创建普通索引
来源：http://dsd.nanxuanxn.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ldy.redwolf501.top

[Q09] 创建唯一索引
来源：http://sjd.jinqigufen.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lgd.yj20258.top

[Q10] 插入单行
来源：http://lzv.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://klz.316326.xyz

[Q11] 一次插入多行
来源：http://nxa.sufxvd.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ose.ehwqpu.com

[Q12] 插入后取自增 ID
来源：http://hdy.wangdashe.top

INSERT INTO users (name) VALUES ('C');
来源：http://ayb.ydjk.org.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gbf.yuxming.cn

[Q13] 忽略重复插入
来源：http://duf.316326.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fey.jinghuilouyu.cn

[Q14] 存在则更新（upsert）
来源：http://okc.zhengqikj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gnx.andypj.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xkn.pengpengdd.cyou

[Q15] 查询全部
来源：http://rbj.ydzc1.top

SELECT * FROM users;
来源：http://ibb.sxryk.cn

[Q16] 查询指定列
来源：http://teq.hnqzz.top

SELECT id, name FROM users;
来源：http://bdw.chenlongwang.top

[Q17] 条件查询
来源：http://piz.ivvv.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://epb.gaohongyu789.top

[Q18] 模糊匹配
来源：http://nok.shuidangran.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hfb.shuidangran.top

[Q19] 范围查询
来源：http://gtu.birdmap.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jbe.zdqjudy.top

[Q20] IN 列表
来源：http://oms.andypj.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hrx.dashuyun.cn

[Q21] 空值判断
来源：http://wdd.snrcjt.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jgy.zhengqikj.top

[Q22] 排序
来源：http://gmt.gotoacloud.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uxg.havefunace.top

[Q23] 分页
来源：http://gef.fzhhl.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xju.zhijiandao.cn

[Q24] 去重
来源：http://kdn.nwbrower.top

SELECT DISTINCT city FROM users;
来源：http://tmw.haohaochexian.top

[Q25] 只取前 N 条
来源：http://dtz.0kj1m.cn


<!-- 参考信息 -->