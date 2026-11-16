代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://wfr.zhixingplan.top

[N02] 排序（工程实践用内置实现）
来源：http://ewp.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://ibl.gotoacloud.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lzh.meibo888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://oqo.snrcjt.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lfu.xuanzx.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cim.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://wly.zhixingplan.top

Ruby: arr.sort
来源：http://fwk.kuanghao11.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://aat.hesvh.cn

[N03] 快速排序（分治示例）
来源：http://khr.wangshuangyany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cjo.gzhubu.top

PHP:  // 递归实现，或用 usort
来源：http://fai.haohaochexian.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hgp.ivvv.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xqq.aizwys.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zek.smart0.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kny.vehdjk.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wdq.chenjidiqi.icu

C#:   // 手写递归，或 Array.Sort
来源：http://dcq.yj20258888.top

[N04] 斐波那契数列
来源：http://ape.zhoulong.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://znb.jqgufenzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kcn.zhongyouzk.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kmy.birdmap.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://olj.yanxiufei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vyw.bbcook.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://meh.birdmap.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wbg.gogol.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jnn.cqqwz.cn

[N05] 最大公约数
来源：http://yik.wangdashe.top

Py:   math.gcd(a, b)
来源：http://fqg.yuxming.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lkk.sysykeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dsv.nwbrower.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aax.xuetiantiany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yms.meibo888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vxl.zhengqikj.top

Ruby: a.gcd(b)
来源：http://tgv.yj20258888.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://udp.hfpthk.cn

[N06] 判断回文字符串
来源：http://imm.chenjidiqi.icu

Py:   s == s[::-1]
来源：http://oxr.yuxming.cn

PHP:  $s === strrev($s);
来源：http://byu.jiagoushi.top

JS:   s === [...s].reverse().join("")
来源：http://wbk.jqgfzy.top

TS:   s === [...s].reverse().join("")
来源：http://mws.bjfxy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jsv.ybcxt.top

Go:   // 双指针从两端比较
来源：http://hyz.ppjwa.cn

Ruby: s == s.reverse
来源：http://sfu.ydzc1.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jlp.jiagoushi.top

[N07] 两数之和（返回下标）
来源：http://npk.yuanzhike.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dvt.zdqjudy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://emc.chenjidiqi.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://qhd.xuetiantiany.cn

TS:   // 手写 Map<string, number>
来源：http://phs.cucudq.cn

Java: // 手写 HashMap
来源：http://ioo.hysaishi.cn

Go:   // 手写 map[int]int
来源：http://isd.smart0.xyz

Ruby: // 手写 Hash
来源：http://dtj.jiagoushi.top

C#:   // 手写 Dictionary<int, int>
来源：http://nls.guowangkeji.top

[N08] 生成全排列
来源：http://vvd.hysaishi.cn

Py:   itertools.permutations(arr)
来源：http://wkj.sjlbkw.cn

PHP:  // 手写递归交换
来源：http://eib.yvedp.cn

JS:   // 手写回溯递归
来源：http://zth.xziqi.cn

TS:   // 手写回溯递归
来源：http://pih.c1oappe.top

Java: // 手写回溯递归
来源：http://zna.fengsongda.top

Go:   // 手写回溯递归
来源：http://wqk.cqqwz.cn

Ruby: arr.permutation.to_a
来源：http://ddw.cucudq.cn

C#:   // 手写回溯递归
来源：http://pvz.kuanghao11.cn

[N09] 栈与队列
来源：http://reu.fzhhl.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://acm.52xcode.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yld.havefunace.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ljq.yj202588.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rta.zycfv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://guj.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dtr.fktsv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vju.hywenlv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vgx.yfazqb.com

[N10] 链表节点定义
来源：http://nds.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gbw.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rbc.chenjidiqi.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oxq.cqqwz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zxu.jiagoushi.top

Java: class Node { int v; Node next; }
来源：http://wjc.chenzaomai.com

Go:   type Node struct { V int; Next *Node }
来源：http://buf.316326.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://beu.hfpthk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bfl.shanyushiyangkeji.top

[N11] 二叉树中序遍历
来源：http://vfb.fzhhl.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lgv.bbcook.cn

PHP:  // 手写递归函数
来源：http://zoj.vehdjk.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://apl.jinyuanbaomall.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uis.shanyushiyangkeji.top

Java: // 手写递归
来源：http://nue.zhixingplan.top

Go:   // 手写递归
来源：http://qaf.gzhubu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fwl.fanxiaobao.xyz

C#:   // 手写递归
来源：http://czj.mhx1999.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cwu.chenlongwang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://udb.yanxiufei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ifi.wangshuangyany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hma.quarkkingdee.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bfs.nwbrower.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xui.jinghuilouyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pwp.gogol.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pum.nanxuanxn.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://evx.fanxiaobao.xyz

================================================================================
来源：http://opn.pengpengdd.cyou

O. 并发与异步
来源：http://imt.hnxiangtu.top

================================================================================
来源：http://ege.redwolf501.top

[O01] 启动一个线程
来源：http://wwi.jinqigufen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ycs.shanyushiyangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wdu.redwolf501.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ujn.zhongyouzk.top

TS:   // 同 JS
来源：http://fng.gogol.net.cn

Java: new Thread(() -> f()).start()
来源：http://aji.cheryme.top

Go:   go f()
来源：http://fmz.hywenlv.cn

Ruby: Thread.new { f }
来源：http://kns.daxiang520.top

C#:   Task.Run(() => F());
来源：http://pyf.meibo888.top

[O02] 使用线程池
来源：http://kxg.dashuyun.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kit.xinyue.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fni.bbcook.cn

JS:   // worker_threads 线程池
来源：http://ahm.xuanzx.com

TS:   // worker_threads 线程池
来源：http://jdx.jinyuanbaomall.cn

Java: Executors.newFixedThreadPool(4)
来源：http://iga.hcnkem.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://skq.yj20258.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rrg.gogol.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oah.sjlbkw.cn

[O03] 加锁保护共享数据
来源：http://tun.jinqigfzy.top

Py:   with lock: shared += 1
来源：http://lfx.zhixingplan.top

PHP:  // 用 flock() 做文件锁
来源：http://bdl.yuxming.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tis.ydzc1.top

TS:   // 同 JS
来源：http://dvd.xziqi.cn

Java: synchronized (this) { shared++; }
来源：http://ycf.hysaishi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gsd.zhixingplan.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dgc.yj202588.top

C#:   lock (gate) { shared++; }
来源：http://idr.zdqjudy.top

[O04] 定义异步函数并等待
来源：http://pqm.nwbrower.top

Py:   async def f():⏎    await g()
来源：http://kzy.zhaomingkeji.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qix.zycfv.cn

JS:   async function f() { await g(); }
来源：http://fpt.cashguo.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tyu.chenjidiqi.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qtg.wangshuangyany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xoz.shanyushiyangtech.top

Ruby: # 用 Fiber 或 async gem
来源：http://dbm.hongshengwenyu.top

C#:   async Task F() { await G(); }
来源：http://xmd.daria6918.cn

[O05] 并发执行并等待全部完成
来源：http://kdm.tarul.cn

Py:   asyncio.gather(*tasks)
来源：http://cak.sufxvd.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gcs.hnxiangtu.top

JS:   await Promise.all(tasks)
来源：http://dfk.jianghu66.top

TS:   await Promise.all(tasks)
来源：http://grr.zhixingplan.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ocs.yonumen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lxg.zhixingplan.top

Ruby: threads.map(&:join)
来源：http://icy.redwolf501.top

C#:   await Task.WhenAll(t1, t2)
来源：http://njc.chenlongwang.top

[O06] 使用进程池
来源：http://bht.ppjwa.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sze.hnqzz.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mau.hywenlv.cn

JS:   // child_process / cluster 模块
来源：http://isv.aizwys.cn

TS:   // child_process / cluster 模块
来源：http://yzg.gaohongyu789.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zii.bjfxy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kui.yonumen.top

Ruby: // fork 块
来源：http://cuk.yj20258.top

C#:   Parallel.For
来源：http://jor.gotoacloud.top

================================================================================
来源：http://jhm.ydjk.org.cn

P. 常用工具函数
来源：http://jlk.yongpay.top

================================================================================
来源：http://mlz.chenzaomai.com

[P01] 生成 UUID
来源：http://lbc.yvedp.cn

Py:   str(uuid.uuid4())
来源：http://ewc.xinyue.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kfy.jyoumei.cn

JS:   crypto.randomUUID()
来源：http://sca.haohaochexian.top

TS:   crypto.randomUUID()
来源：http://zqb.svipenyu.cn

Java: UUID.randomUUID().toString()
来源：http://eds.guowangkeji.top

Go:   // 用 github.com/google/uuid
来源：http://jpb.cdnleiting.top

Ruby: SecureRandom.uuid
来源：http://ybk.birdmap.top

C#:   Guid.NewGuid().ToString()
来源：http://yrw.jinqigufen.top

[P02] MD5 / SHA256 摘要
来源：http://adb.ctjpmb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dyc.gotoacloud.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lnt.chenzaomai.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lkz.yuanzhike.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nkd.epnwcf.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jys.yj202588.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://age.fengsongda.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rgz.hnqzz.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jmk.xuanzx.com

[P03] 生成短随机字符串
来源：http://hgx.jinqigufen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fth.tanke756.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ncg.dashuyun.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qyt.nwbrower.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://umh.snrcjt.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ohs.pengpengdd.cyou

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sms.dashuyun.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tqk.zhoulong.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hxx.shuidangran.top

[P04] 求长度
来源：http://pxz.daxiang520.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vfr.shanyushiyangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kgh.hnxiangtu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hnl.aibaodan.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://buj.daxiang520.top

Java: list.size();  map.size();  s.length()
来源：http://ejk.zhongyouzk.top

Go:   len(arr);  len(m)
来源：http://txp.jianghu66.top

Ruby: x.length;  x.size
来源：http://ovr.ctjpmb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://clj.zhongyouzk.top

[P05] 判断两个对象内容是否相等
来源：http://zti.jinqigufen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nnt.chenjidiqi.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vqf.daria6918.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ftg.vehdjk.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lay.sufxvd.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xdg.tanke756.top

Go:   reflect.DeepEqual(a, b)
来源：http://bpm.guannengcc.top

Ruby: a == b
来源：http://dkb.cashguo.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kfw.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cwg.xinyue.icu

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bpi.xuanzx.com

PHP:  if (empty($x)) {}
来源：http://wsu.hnqzz.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tmn.mhx1999.top

TS:   if (x == null) {}
来源：http://kid.pycfn.com

Java: if (x == null || x.isEmpty()) {}
来源：http://exj.xuetiantiany.cn

Go:   if x == nil {}
来源：http://cli.ctjpmb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cub.zdqjudy.top

C#:   if (x is null) {}
来源：http://fun.jinqigfzy.top

[P07] 防抖与节流
来源：http://dpu.epnwcf.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zry.zhoulong.xyz

PHP:  // 手写时间戳比较
来源：http://acy.yangfankeji.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kur.zdbjq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cyp.fanxiaobao.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ggx.jianghu66.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qlp.fanxiaobao.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://src.sysykeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nxg.zhaomingkeji.xyz

[P08] 处理浮点精度问题
来源：http://blk.epnwcf.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iim.sysykeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vrs.chenzaomai.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nfc.zhijiandao.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hpf.sjlbkw.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cnu.kuanghao11.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nbr.jinqigufen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://prn.zhixingplan.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ecd.sufxvd.cn

================================================================================
来源：http://ccg.jyoumei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dyo.shanyushiyangkeji.top

================================================================================
来源：http://dis.guowangkeji.top

[Q01] 创建表
来源：http://xud.meibo888.top

CREATE TABLE users (
来源：http://dqj.feifeiyinyue.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://waf.zhaomingkeji.xyz

name VARCHAR(50) NOT NULL,
来源：http://hcp.hnqzz.top

email VARCHAR(100) UNIQUE,
来源：http://fin.guannengcc.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yrq.guannengcc.top

);
来源：http://dgj.pycfn.com

[Q02] 创建带外键的表
来源：http://fyo.aibaodan.cn

CREATE TABLE orders (
来源：http://wgm.sjlbkw.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qsp.meibo888.top

user_id INT NOT NULL,
来源：http://chg.pengpengdd.cyou

amount DECIMAL(10, 2),
来源：http://lox.cdnleiting.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pap.pycfn.com

);
来源：http://ulb.52xcode.cn

[Q03] 增加列
来源：http://zld.shuidangran.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vuf.fengsongda.top

[Q04] 修改列类型
来源：http://mws.uphjek.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zta.hywenlv.cn

[Q05] 重命名列
来源：http://rtx.meibo888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://agw.nanxuanxn.top

[Q06] 删除列
来源：http://uae.yanxiufei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qnx.pycfn.com

[Q07] 删除表
来源：http://zrv.tianlin.xyz

DROP TABLE IF EXISTS orders;
来源：http://jpt.fzhhl.top

[Q08] 创建普通索引
来源：http://amn.fzhhl.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xhn.ctjpmb.com

[Q09] 创建唯一索引
来源：http://wfz.kuanghao11.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dqu.zhoulong.xyz

[Q10] 插入单行
来源：http://wvx.fktsv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xhr.xuetiantiany.cn

[Q11] 一次插入多行
来源：http://flk.gotoacloud.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mhz.shzxlz.cn

[Q12] 插入后取自增 ID
来源：http://ott.yonumen.top

INSERT INTO users (name) VALUES ('C');
来源：http://gby.wangshuangyany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blj.nwbrower.top

[Q13] 忽略重复插入
来源：http://vna.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bga.ybcxt.top

[Q14] 存在则更新（upsert）
来源：http://fgi.fktsv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://muo.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ywt.hammf.cn

[Q15] 查询全部
来源：http://izu.jqgufenzy.top

SELECT * FROM users;
来源：http://gyp.gaohongyu789.top

[Q16] 查询指定列
来源：http://bze.meibo888.top

SELECT id, name FROM users;
来源：http://awx.cashguo.top

[Q17] 条件查询
来源：http://qks.shzxlz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mgo.cashguo.top

[Q18] 模糊匹配
来源：http://dni.birdmap.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://etv.shanyushiyangtech.top

[Q19] 范围查询
来源：http://uej.zhaomingkeji.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xxy.jqgfzy.top

[Q20] IN 列表
来源：http://gpa.mhx1999.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ldu.sysykeji.top

[Q21] 空值判断
来源：http://rnv.chenjidiqi.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://ejd.jiagoushi.top

[Q22] 排序
来源：http://ofq.meibo888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mxd.tian-w.cn

[Q23] 分页
来源：http://zqp.gogol.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uyr.chenjidiqi.icu

[Q24] 去重
来源：http://jns.zdbjq.cn

SELECT DISTINCT city FROM users;
来源：http://ojh.zdqjudy.top

[Q25] 只取前 N 条
来源：http://jen.gaohongyu789.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qoj.yuxming.cn

[Q26] 计数
来源：http://pay.smart0.xyz

SELECT COUNT(*) FROM users;
来源：http://umn.ybcxt.top

[Q27] 条件计数
来源：http://dtw.yuxming.cn


<!-- 参考信息 -->