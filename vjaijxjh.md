代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://myz.zycfv.cn

JS:   console.error("err")
来源：http://yqd.dianchejie.cn

TS:   console.error("err")
来源：http://pce.sysykeji.top

Java: System.err.println("err")
来源：http://fpk.jqgufenzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fap.birdmap.top

Ruby: warn "err"
来源：http://mpm.vqdsnc.cn

C#:   Console.Error.WriteLine("err")
来源：http://sdt.chenjidiqi.icu

[M07] 判断是否为主入口
来源：http://qna.sufxvd.cn

Py:   if __name__ == "__main__":
来源：http://qhf.hnxiangtu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wha.yongpay.top

JS:   require.main === module
来源：http://xww.fanxiaobao.xyz

TS:   require.main === module
来源：http://imi.daxiang520.top

Java: public static void main(String[] args)
来源：http://mrk.xuanzx.com

Go:   func main()
来源：http://cfd.hammf.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fcv.tianlin.xyz

C#:   static void Main(string[] args)
来源：http://xsz.aibaodan.cn

[M08] 获取系统与运行时信息
来源：http://gyf.yj20258888.top

Py:   platform.system();  platform.python_version()
来源：http://pse.jlsjyb.cn

PHP:  PHP_OS;  phpversion();
来源：http://ncu.zhijiandao.cn

JS:   process.platform;  process.version
来源：http://fek.aibaodan.cn

TS:   process.platform;  process.version
来源：http://yff.yvedp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://eql.wangshuangyany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tft.fzhhl.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uql.yanxiufei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nzt.guowangkeji.top

================================================================================
来源：http://ixy.fanxiaobao.xyz

N. 数据结构与算法
来源：http://ugx.hammf.cn

================================================================================
来源：http://vkp.gogol.net.cn

[N01] 二分查找（有序数组）
来源：http://lug.daxiang520.top

Py:   bisect.bisect_left(arr, x)
来源：http://ybn.jinqigufen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hrw.yj20258.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zxq.gzhubu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dzw.yj20258888.top

Java: Arrays.binarySearch(arr, x)
来源：http://vbg.wangshuangyany.cn

Go:   sort.SearchInts(arr, x)
来源：http://fqc.cashguo.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ker.vehdjk.com

C#:   Array.BinarySearch(arr, x)
来源：http://fvy.fanxiaobao.xyz

[N02] 排序（工程实践用内置实现）
来源：http://cyn.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://etf.redwolf501.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mdk.yangfankeji.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://xmo.hfpthk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vfc.52xcode.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rrs.fanxiaobao.xyz

Go:   slices.Sort(arr)
来源：http://dqw.c1oappe.top

Ruby: arr.sort
来源：http://gzm.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://thc.vqdsnc.cn

[N03] 快速排序（分治示例）
来源：http://rzd.yueranfly.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ojk.guowangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://ejj.kuanghao11.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bpa.snrcjt.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mbj.guannengcc.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://knp.redwolf501.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xfq.bbcook.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mky.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://odl.snrcjt.cn

[N04] 斐波那契数列
来源：http://fug.feifeiyinyue.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rod.bbcook.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fzf.yj202588.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mem.yanxiufei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xdr.mhx1999.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bmy.ehwqpu.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ruu.hnxiangtu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qbw.chenjidiqi.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zcm.fengsongda.top

[N05] 最大公约数
来源：http://pmt.sxryk.cn

Py:   math.gcd(a, b)
来源：http://bfo.hongshengwenyu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fuc.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dca.yueranfly.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hwe.shanyushiyangtech.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hka.feifeiyinyue.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nwe.cucudq.cn

Ruby: a.gcd(b)
来源：http://fcv.yfazqb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wbp.yanxiufei.cn

[N06] 判断回文字符串
来源：http://iqr.hesvh.cn

Py:   s == s[::-1]
来源：http://mxt.vqdsnc.cn

PHP:  $s === strrev($s);
来源：http://lma.zhiwuduotai.top

JS:   s === [...s].reverse().join("")
来源：http://vzu.fengsongda.top

TS:   s === [...s].reverse().join("")
来源：http://ftn.zhoulong.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bsl.mhx1999.top

Go:   // 双指针从两端比较
来源：http://rgw.cqqwz.cn

Ruby: s == s.reverse
来源：http://kci.zdbjq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fcy.jinqigfzy.top

[N07] 两数之和（返回下标）
来源：http://awa.zdqjudy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fje.yongpay.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ixs.zhijiandao.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cmd.yj20258.top

TS:   // 手写 Map<string, number>
来源：http://tse.fzhhl.top

Java: // 手写 HashMap
来源：http://njw.jinghuilouyu.cn

Go:   // 手写 map[int]int
来源：http://jeg.zycfv.cn

Ruby: // 手写 Hash
来源：http://cql.hammf.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lfd.fktsv.cn

[N08] 生成全排列
来源：http://upe.zhoulong.xyz

Py:   itertools.permutations(arr)
来源：http://hls.zhoulong.xyz

PHP:  // 手写递归交换
来源：http://puh.yongpay.top

JS:   // 手写回溯递归
来源：http://ykx.hongshengwenyu.top

TS:   // 手写回溯递归
来源：http://jud.haohaochexian.top

Java: // 手写回溯递归
来源：http://ies.nanxinkj.top

Go:   // 手写回溯递归
来源：http://ecx.zycfv.cn

Ruby: arr.permutation.to_a
来源：http://euv.tian-w.cn

C#:   // 手写回溯递归
来源：http://via.gogol.net.cn

[N09] 栈与队列
来源：http://oei.yfazqb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tnk.nanxinkj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vnn.nanxuanxn.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://krv.ywan-chungtsiang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://acj.cucudq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xdj.zhoulong.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eeu.ivvv.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qzx.yvedp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ayc.52xcode.cn

[N10] 链表节点定义
来源：http://pkv.hongshengwenyu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tor.bjfxy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://oep.bbcook.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gjy.shanyushiyangtech.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vfh.yueranfly.top

Java: class Node { int v; Node next; }
来源：http://jbj.zhaomingkeji.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://pfj.dianchejie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cly.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lqz.kuanghao11.cn

[N11] 二叉树中序遍历
来源：http://xjx.daria6918.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aew.ybcxt.top

PHP:  // 手写递归函数
来源：http://vxy.xziqi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jgk.jinqigfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pnu.dianchejie.cn

Java: // 手写递归
来源：http://yiw.vqdsnc.cn

Go:   // 手写递归
来源：http://fxb.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ouw.dianchejie.cn

C#:   // 手写递归
来源：http://mty.andypj.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cjw.daxiang520.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cze.shanyushiyangtech.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cii.nanxuanxn.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zrf.meibo888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fjl.jqgfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kpv.havefunace.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vcy.zdbjq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ttd.yuanzhike.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://orh.wangshuangyany.cn

================================================================================
来源：http://ykm.yuanzhike.top

O. 并发与异步
来源：http://cwq.gotoacloud.top

================================================================================
来源：http://oas.tarul.cn

[O01] 启动一个线程
来源：http://dgs.cashguo.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zue.cqqwz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mzs.zhixingplan.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iwi.sysykeji.top

TS:   // 同 JS
来源：http://szk.kuanghao11.cn

Java: new Thread(() -> f()).start()
来源：http://ihf.zdbjq.cn

Go:   go f()
来源：http://hgt.zycfv.cn

Ruby: Thread.new { f }
来源：http://lto.fengsongda.top

C#:   Task.Run(() => F());
来源：http://mig.hcnkem.com

[O02] 使用线程池
来源：http://xvf.ydzc1.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://onw.shzxlz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wee.gzhubu.top

JS:   // worker_threads 线程池
来源：http://ogl.daxiang520.top

TS:   // worker_threads 线程池
来源：http://uie.zhiwuduotai.top

Java: Executors.newFixedThreadPool(4)
来源：http://xcr.chenlongwang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rxu.iojbl.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vop.zhiwuduotai.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rng.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://wez.yanxiufei.cn

Py:   with lock: shared += 1
来源：http://eso.bbcook.cn

PHP:  // 用 flock() 做文件锁
来源：http://acq.wangdashe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ozo.fehbvm.com

TS:   // 同 JS
来源：http://sfu.gzhubu.top

Java: synchronized (this) { shared++; }
来源：http://hyb.jqgufenzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eax.ivvv.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qpu.yfazqb.com

C#:   lock (gate) { shared++; }
来源：http://qmk.ppjwa.cn

[O04] 定义异步函数并等待
来源：http://fbk.meibo888.top

Py:   async def f():⏎    await g()
来源：http://ixm.ppjwa.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eqh.iojbl.cn

JS:   async function f() { await g(); }
来源：http://dya.yuanzhike.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://yij.haohaochexian.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lds.mhx1999.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ans.pycfn.com

Ruby: # 用 Fiber 或 async gem
来源：http://ndq.wangshuangyany.cn

C#:   async Task F() { await G(); }
来源：http://mtv.zhixingplan.top

[O05] 并发执行并等待全部完成
来源：http://xzy.ydjk.org.cn

Py:   asyncio.gather(*tasks)
来源：http://zoo.yuanzhike.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ztr.ydzc1.top

JS:   await Promise.all(tasks)
来源：http://sfu.zhongyouzk.top

TS:   await Promise.all(tasks)
来源：http://fan.hnqzz.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://crz.fktsv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ujk.xylfe.cn

Ruby: threads.map(&:join)
来源：http://nbp.aizwys.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zhu.cashguo.top

[O06] 使用进程池
来源：http://vim.chenjidiqi.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xjh.yj202588.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xss.dashuyun.cn

JS:   // child_process / cluster 模块
来源：http://ejh.zhengqikj.top

TS:   // child_process / cluster 模块
来源：http://cdq.xylfe.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jvx.iojbl.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oam.hywenlv.cn

Ruby: // fork 块
来源：http://lwg.jinghuilouyu.cn

C#:   Parallel.For
来源：http://hsz.sweek.top

================================================================================
来源：http://uas.fanxiaobao.xyz

P. 常用工具函数
来源：http://paa.52xcode.cn

================================================================================
来源：http://ush.tarul.cn

[P01] 生成 UUID
来源：http://bbb.guannengcc.top

Py:   str(uuid.uuid4())
来源：http://ihc.jqgufenzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://aix.chenlongwang.top

JS:   crypto.randomUUID()
来源：http://vcq.zdqjudy.top

TS:   crypto.randomUUID()
来源：http://git.aibaodan.cn

Java: UUID.randomUUID().toString()
来源：http://inh.pycfn.com

Go:   // 用 github.com/google/uuid
来源：http://ytc.sxryk.cn

Ruby: SecureRandom.uuid
来源：http://tyx.dashuyun.cn

C#:   Guid.NewGuid().ToString()
来源：http://skm.zhongyouzk.top

[P02] MD5 / SHA256 摘要
来源：http://xbs.gogol.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ete.316326.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://bus.zhixingplan.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vgd.yueranfly.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mik.ybcxt.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hii.sjlbkw.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lga.feifeiyinyue.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hge.ywan-chungtsiang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pfo.iojbl.cn

[P03] 生成短随机字符串
来源：http://zxm.yueranfly.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cwz.pycfn.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cqf.ppjwa.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aef.zdqjudy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xnl.hnqzz.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hug.dianchejie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://urv.birdmap.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mxk.chenzaomai.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rfd.hcnkem.com

[P04] 求长度
来源：http://mte.aibaodan.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://okc.zhixingplan.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ykn.hnqzz.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pzq.bjfxy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xtp.c1oappe.top

Java: list.size();  map.size();  s.length()
来源：http://ypo.shzxlz.cn

Go:   len(arr);  len(m)
来源：http://qen.guowangkeji.top

Ruby: x.length;  x.size
来源：http://zcb.birdmap.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gau.tianlin.xyz

[P05] 判断两个对象内容是否相等
来源：http://sid.jyoumei.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mxc.fzhhl.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iem.snrcjt.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ike.sysykeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://htr.vehdjk.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jpy.yangfankeji.com

Go:   reflect.DeepEqual(a, b)
来源：http://jzm.gotoacloud.top

Ruby: a == b
来源：http://ksv.ywan-chungtsiang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dcc.tianlin.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vej.yonumen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://irp.0kj1m.cn

PHP:  if (empty($x)) {}
来源：http://chg.hfpthk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zhh.aibaodan.cn

TS:   if (x == null) {}
来源：http://eas.fehbvm.com

Java: if (x == null || x.isEmpty()) {}
来源：http://vvj.bjfxy.top

Go:   if x == nil {}
来源：http://lim.hnxiangtu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dyd.xingfuxueyuan.xyz

C#:   if (x is null) {}
来源：http://org.ctjpmb.com

[P07] 防抖与节流
来源：http://aym.epnwcf.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hbl.tianlin.xyz

PHP:  // 手写时间戳比较
来源：http://naj.fanxiaobao.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hod.wangshuangyany.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://duf.shanyushiyangtech.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://onu.yj20258.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vfo.yuanzhike.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hcd.yuanzhike.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fqz.fanxiaobao.xyz

[P08] 处理浮点精度问题
来源：http://iiu.fehbvm.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wli.hesvh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ega.yfazqb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sfm.daria6918.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ome.guowangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bht.c1oappe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ufs.yuxming.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lng.epnwcf.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yxp.yonumen.top

================================================================================
来源：http://gnn.xuanzx.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lmh.c1oappe.top

================================================================================
来源：http://vzh.shangyingyoupin.top

[Q01] 创建表
来源：http://tvh.tian-w.cn

CREATE TABLE users (
来源：http://ask.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jcm.shanyushiyangtech.top

name VARCHAR(50) NOT NULL,
来源：http://tbj.epnwcf.com

email VARCHAR(100) UNIQUE,
来源：http://vgw.yongpay.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mxm.ehwqpu.com

);
来源：http://bjh.c1oappe.top

[Q02] 创建带外键的表
来源：http://hlw.cdnleiting.top

CREATE TABLE orders (
来源：http://kfj.chenlongwang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oot.kuanghao11.cn

user_id INT NOT NULL,
来源：http://inp.gaohongyu789.top

amount DECIMAL(10, 2),
来源：http://kml.ehwqpu.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://igt.shangyingyoupin.top

);
来源：http://nzb.zhijiandao.cn

[Q03] 增加列
来源：http://zgk.daxiang520.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oqr.birdmap.top

[Q04] 修改列类型
来源：http://ait.fzhhl.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hwq.hammf.cn

[Q05] 重命名列
来源：http://pbu.hcnkem.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://saj.hesvh.cn

[Q06] 删除列
来源：http://bnz.gotoacloud.top

ALTER TABLE users DROP COLUMN age;
来源：http://vlg.jqgfzy.top

[Q07] 删除表
来源：http://uhf.pengpengdd.cyou

DROP TABLE IF EXISTS orders;
来源：http://roo.yueranfly.top

[Q08] 创建普通索引
来源：http://gne.yj20258888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://axo.shzxlz.cn

[Q09] 创建唯一索引
来源：http://acm.hammf.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dom.yuxming.cn

[Q10] 插入单行
来源：http://voi.xuanzx.com


<!-- 参考信息 -->