代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gjp.vehdjk.com

Ruby: warn "err"
来源：http://msj.zhixingplan.top

C#:   Console.Error.WriteLine("err")
来源：http://pxs.guannengcc.top

[M07] 判断是否为主入口
来源：http://cxc.hesvh.cn

Py:   if __name__ == "__main__":
来源：http://rtr.svipenyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mti.jinqigufen.top

JS:   require.main === module
来源：http://hya.zhongyouzk.top

TS:   require.main === module
来源：http://wbz.cucudq.cn

Java: public static void main(String[] args)
来源：http://mrb.vqdsnc.cn

Go:   func main()
来源：http://ekn.jlsjyb.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jyh.chenzaomai.com

C#:   static void Main(string[] args)
来源：http://ckj.zhijiandao.cn

[M08] 获取系统与运行时信息
来源：http://qmf.uphjek.com

Py:   platform.system();  platform.python_version()
来源：http://zcs.cucudq.cn

PHP:  PHP_OS;  phpversion();
来源：http://lhp.jqgufenzy.top

JS:   process.platform;  process.version
来源：http://fbv.tianlin.xyz

TS:   process.platform;  process.version
来源：http://rmj.yuxming.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dkp.hammf.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://obw.ivvv.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qha.hcnkem.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://cqe.hfpthk.cn

================================================================================
来源：http://ibn.dashuyun.cn

N. 数据结构与算法
来源：http://ura.guannengcc.top

================================================================================
来源：http://vzi.xuanzx.com

[N01] 二分查找（有序数组）
来源：http://vom.jinyuanbaomall.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jpo.shzxlz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rlr.cashguo.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mof.shuidangran.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xfp.yj20258.top

Java: Arrays.binarySearch(arr, x)
来源：http://yyf.kuanghao11.cn

Go:   sort.SearchInts(arr, x)
来源：http://abz.xuetiantiany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jrr.andypj.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://wqo.zdbjq.cn

[N02] 排序（工程实践用内置实现）
来源：http://ryx.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://blc.havefunace.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ion.snrcjt.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ilc.zhiwuduotai.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ops.zdbjq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iyl.aizwys.cn

Go:   slices.Sort(arr)
来源：http://hez.jyoumei.cn

Ruby: arr.sort
来源：http://cqi.chenlongwang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ozw.yvedp.cn

[N03] 快速排序（分治示例）
来源：http://qdx.yj20258.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mbb.hysaishi.cn

PHP:  // 递归实现，或用 usort
来源：http://ocg.jyoumei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dkl.svipenyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://atc.guannengcc.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ieq.wangdashe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fdb.snrcjt.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ewb.cdnleiting.top

C#:   // 手写递归，或 Array.Sort
来源：http://svv.iojbl.cn

[N04] 斐波那契数列
来源：http://zwo.hcnkem.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nem.hywenlv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dha.xziqi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://goz.epnwcf.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ekt.jinqigufen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xfg.hfpthk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pfa.iojbl.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wmt.hysaishi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ghh.vqdsnc.cn

[N05] 最大公约数
来源：http://ebv.hesvh.cn

Py:   math.gcd(a, b)
来源：http://oic.redwolf501.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oby.ydzc1.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://adq.yueranfly.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xml.jqgfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xps.wangshuangyany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cfm.yj20258.top

Ruby: a.gcd(b)
来源：http://vnq.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://okj.chenjidiqi.icu

[N06] 判断回文字符串
来源：http://zhp.snrcjt.cn

Py:   s == s[::-1]
来源：http://msb.tanke756.top

PHP:  $s === strrev($s);
来源：http://jao.jqgfzy.top

JS:   s === [...s].reverse().join("")
来源：http://dny.smart0.xyz

TS:   s === [...s].reverse().join("")
来源：http://hxm.ehwqpu.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://joy.zdqjudy.top

Go:   // 双指针从两端比较
来源：http://xdl.sysykeji.top

Ruby: s == s.reverse
来源：http://hcg.ydzc1.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zdj.nanxuanxn.top

[N07] 两数之和（返回下标）
来源：http://wiz.cheryme.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xzy.kuanghao11.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nqw.jinqigfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://hvf.zdqjudy.top

TS:   // 手写 Map<string, number>
来源：http://wil.shuidangran.top

Java: // 手写 HashMap
来源：http://pnv.haohaochexian.top

Go:   // 手写 map[int]int
来源：http://yfc.nanxinkj.top

Ruby: // 手写 Hash
来源：http://kfe.jiagoushi.top

C#:   // 手写 Dictionary<int, int>
来源：http://ini.feifeiyinyue.top

[N08] 生成全排列
来源：http://vzu.0kj1m.cn

Py:   itertools.permutations(arr)
来源：http://lyy.wangdashe.top

PHP:  // 手写递归交换
来源：http://nxx.zhongyouzk.top

JS:   // 手写回溯递归
来源：http://yie.vqdsnc.cn

TS:   // 手写回溯递归
来源：http://ofc.9152youxi.cn

Java: // 手写回溯递归
来源：http://odc.zhaomingkeji.xyz

Go:   // 手写回溯递归
来源：http://dnb.ydzc1.top

Ruby: arr.permutation.to_a
来源：http://yfv.fzhhl.top

C#:   // 手写回溯递归
来源：http://tuf.tanke756.top

[N09] 栈与队列
来源：http://ctm.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hgn.dianchejie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://izq.xylfe.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://duf.cashguo.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ykm.shzxlz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://smd.jqgufenzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xkw.ydjk.org.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://akf.guannengcc.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kyy.sxryk.cn

[N10] 链表节点定义
来源：http://xpe.0kj1m.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zpl.daria6918.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xsg.hongshengwenyu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rjd.0kj1m.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jsw.9152youxi.cn

Java: class Node { int v; Node next; }
来源：http://iut.zhaomingkeji.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://wvt.cashguo.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jlg.cdnleiting.top

C#:   class Node { public int V; public Node? Next; }
来源：http://eio.dashuyun.cn

[N11] 二叉树中序遍历
来源：http://auh.hnxiangtu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lvm.iojbl.cn

PHP:  // 手写递归函数
来源：http://fla.c1oappe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://exf.daxiang520.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fzt.jinqigfzy.top

Java: // 手写递归
来源：http://wdh.chenlongwang.top

Go:   // 手写递归
来源：http://yay.meibo888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dwn.yvedp.cn

C#:   // 手写递归
来源：http://jjf.hongshengwenyu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jkd.xingfuxueyuan.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pgc.chenlongwang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tiu.birdmap.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cbr.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mot.yanxiufei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qon.yuxming.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://erk.dianchejie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dzl.shzxlz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jaf.redwolf501.top

================================================================================
来源：http://rqe.ivvv.top

O. 并发与异步
来源：http://iab.hcnkem.com

================================================================================
来源：http://kkd.ivvv.top

[O01] 启动一个线程
来源：http://krd.nanxuanxn.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rqu.zhiwuduotai.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bwv.zhaomingkeji.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bfy.yj20258.top

TS:   // 同 JS
来源：http://prz.guannengcc.top

Java: new Thread(() -> f()).start()
来源：http://tko.meibo888.top

Go:   go f()
来源：http://bcm.hcnkem.com

Ruby: Thread.new { f }
来源：http://whk.nanxinkj.top

C#:   Task.Run(() => F());
来源：http://ydg.jinghuilouyu.cn

[O02] 使用线程池
来源：http://isn.xuanzx.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dxm.ivvv.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bdr.yongpay.top

JS:   // worker_threads 线程池
来源：http://hwa.nanxinkj.top

TS:   // worker_threads 线程池
来源：http://emk.jyoumei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lzz.hongshengwenyu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kle.hongshengwenyu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pbz.zhengqikj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ily.guannengcc.top

[O03] 加锁保护共享数据
来源：http://ksd.yanxiufei.cn

Py:   with lock: shared += 1
来源：http://eef.dashuyun.cn

PHP:  // 用 flock() 做文件锁
来源：http://fax.jiagoushi.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://afs.zhiwuduotai.top

TS:   // 同 JS
来源：http://pef.mhx1999.top

Java: synchronized (this) { shared++; }
来源：http://xtp.daria6918.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tmy.gotoacloud.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vko.smart0.xyz

C#:   lock (gate) { shared++; }
来源：http://vjm.cheryme.top

[O04] 定义异步函数并等待
来源：http://klm.jiagoushi.top

Py:   async def f():⏎    await g()
来源：http://prg.jinqigfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pga.smart0.xyz

JS:   async function f() { await g(); }
来源：http://orn.jqgfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zrv.ydjk.org.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pse.tian-w.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dts.zhijiandao.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zwi.jiagoushi.top

C#:   async Task F() { await G(); }
来源：http://xnr.shangyingyoupin.top

[O05] 并发执行并等待全部完成
来源：http://uow.hnxiangtu.top

Py:   asyncio.gather(*tasks)
来源：http://byp.xuanzx.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mqs.cheryme.top

JS:   await Promise.all(tasks)
来源：http://nyz.jinghuilouyu.cn

TS:   await Promise.all(tasks)
来源：http://pba.fehbvm.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dfj.yj202588.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bkc.cheryme.top

Ruby: threads.map(&:join)
来源：http://lbl.feifeiyinyue.top

C#:   await Task.WhenAll(t1, t2)
来源：http://njs.vehdjk.com

[O06] 使用进程池
来源：http://yzm.yanxiufei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iyd.fktsv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zpb.meibo888.top

JS:   // child_process / cluster 模块
来源：http://caj.ydzc1.top

TS:   // child_process / cluster 模块
来源：http://jtf.0kj1m.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zti.fehbvm.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wsv.zhoulong.xyz

Ruby: // fork 块
来源：http://ago.fanxiaobao.xyz

C#:   Parallel.For
来源：http://ukz.jqgufenzy.top

================================================================================
来源：http://kcm.andypj.xyz

P. 常用工具函数
来源：http://ivg.bjfxy.top

================================================================================
来源：http://xar.nwbrower.top

[P01] 生成 UUID
来源：http://ywu.shuidangran.top

Py:   str(uuid.uuid4())
来源：http://xum.fzhhl.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sxx.ppjwa.cn

JS:   crypto.randomUUID()
来源：http://iah.chenzaomai.com

TS:   crypto.randomUUID()
来源：http://kyn.yueranfly.top

Java: UUID.randomUUID().toString()
来源：http://rvc.pycfn.com

Go:   // 用 github.com/google/uuid
来源：http://lug.jyoumei.cn

Ruby: SecureRandom.uuid
来源：http://sxe.hesvh.cn

C#:   Guid.NewGuid().ToString()
来源：http://fkc.hywenlv.cn

[P02] MD5 / SHA256 摘要
来源：http://yoa.ivvv.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zun.zhiwuduotai.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://yga.fengsongda.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yih.ctjpmb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fph.bjfxy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hrk.jinyuanbaomall.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://emk.uphjek.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://njp.hcnkem.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xhc.yongpay.top

[P03] 生成短随机字符串
来源：http://gua.cheryme.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wie.xuetiantiany.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mlh.jinghuilouyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://azf.yuxming.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kdu.guannengcc.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ois.jiagoushi.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xss.aizwys.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://imy.hywenlv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uqr.sweek.top

[P04] 求长度
来源：http://rzs.iojbl.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kqa.feifeiyinyue.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hby.jinghuilouyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jik.zhoulong.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dwn.svipenyu.cn

Java: list.size();  map.size();  s.length()
来源：http://bcw.xuanzx.com

Go:   len(arr);  len(m)
来源：http://hyq.snrcjt.cn

Ruby: x.length;  x.size
来源：http://ptn.hfpthk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://epk.bjfxy.top

[P05] 判断两个对象内容是否相等
来源：http://wrp.fzhhl.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://cbt.havefunace.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mkk.jinqigufen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://axi.andypj.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xlu.zhoulong.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ass.xziqi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ilc.zhoulong.xyz

Ruby: a == b
来源：http://ezv.daxiang520.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bth.yangfankeji.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gqy.ydzc1.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://srn.jqgfzy.top

PHP:  if (empty($x)) {}
来源：http://cdh.jinghuilouyu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xjh.xinyue.icu

TS:   if (x == null) {}
来源：http://sew.mhx1999.top

Java: if (x == null || x.isEmpty()) {}
来源：http://omb.zhengqikj.top

Go:   if x == nil {}
来源：http://snz.redwolf501.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kjd.dashuyun.cn

C#:   if (x is null) {}
来源：http://hzx.tanke756.top

[P07] 防抖与节流
来源：http://nmv.feifeiyinyue.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ink.hammf.cn

PHP:  // 手写时间戳比较
来源：http://uli.cheryme.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pin.zhiwuduotai.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bmn.guowangkeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://huj.xuanzx.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ggk.dianchejie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dee.havefunace.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dtw.hysaishi.cn

[P08] 处理浮点精度问题
来源：http://cto.yj20258888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://chb.52xcode.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cgc.hywenlv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://svd.pycfn.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oqj.hywenlv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://smx.tian-w.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rgg.wangdashe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sii.jlsjyb.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nym.hongshengwenyu.top

================================================================================
来源：http://jwa.ywan-chungtsiang.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mri.gzhubu.top

================================================================================
来源：http://xov.dianchejie.cn

[Q01] 创建表
来源：http://hdv.ydjk.org.cn

CREATE TABLE users (
来源：http://jvl.svipenyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rjz.dianchejie.cn

name VARCHAR(50) NOT NULL,
来源：http://ypz.zycfv.cn

email VARCHAR(100) UNIQUE,
来源：http://ant.shangyingyoupin.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://all.nanxinkj.top

);
来源：http://znj.andypj.xyz

[Q02] 创建带外键的表
来源：http://dqg.hcnkem.com

CREATE TABLE orders (
来源：http://jvt.yj20258.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://awz.fktsv.cn

user_id INT NOT NULL,
来源：http://wre.wangshuangyany.cn

amount DECIMAL(10, 2),
来源：http://prz.zhaomingkeji.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qow.sweek.top

);
来源：http://qik.cheryme.top

[Q03] 增加列
来源：http://wam.ywan-chungtsiang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rac.xinyue.icu

[Q04] 修改列类型
来源：http://vfv.tanke756.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yjx.zdqjudy.top

[Q05] 重命名列
来源：http://tba.0kj1m.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xdn.jinyuanbaomall.cn

[Q06] 删除列
来源：http://bcw.fanxiaobao.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://oqo.vehdjk.com

[Q07] 删除表
来源：http://gdn.cqqwz.cn

DROP TABLE IF EXISTS orders;
来源：http://jib.yj20258888.top

[Q08] 创建普通索引
来源：http://vck.xuetiantiany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://axp.aibaodan.cn

[Q09] 创建唯一索引
来源：http://nvl.yj202588.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lvq.vehdjk.com

[Q10] 插入单行
来源：http://sdj.birdmap.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tdj.epnwcf.com

[Q11] 一次插入多行
来源：http://evs.nwbrower.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jyx.xziqi.cn

[Q12] 插入后取自增 ID
来源：http://lwd.zhaomingkeji.xyz


<!-- 参考信息 -->