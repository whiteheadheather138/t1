代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://xww.xingfuxueyuan.xyz

JS:   console.error("err")
来源：http://ypr.smart0.xyz

TS:   console.error("err")
来源：http://mik.zhiwuduotai.top

Java: System.err.println("err")
来源：http://tre.zhengqikj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ygb.meibo888.top

Ruby: warn "err"
来源：http://wxp.yvedp.cn

C#:   Console.Error.WriteLine("err")
来源：http://bjy.gogol.net.cn

[M07] 判断是否为主入口
来源：http://ell.uphjek.com

Py:   if __name__ == "__main__":
来源：http://xai.sxryk.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://opb.zhijiandao.cn

JS:   require.main === module
来源：http://lfl.smart0.xyz

TS:   require.main === module
来源：http://hgs.fanxiaobao.xyz

Java: public static void main(String[] args)
来源：http://fsl.zhixingplan.top

Go:   func main()
来源：http://ynk.daria6918.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lfl.hysaishi.cn

C#:   static void Main(string[] args)
来源：http://jvc.shanyushiyangkeji.top

[M08] 获取系统与运行时信息
来源：http://hzg.iojbl.cn

Py:   platform.system();  platform.python_version()
来源：http://apu.aizwys.cn

PHP:  PHP_OS;  phpversion();
来源：http://pio.fktsv.cn

JS:   process.platform;  process.version
来源：http://hyk.yvedp.cn

TS:   process.platform;  process.version
来源：http://vbp.jlsjyb.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qjf.yonumen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rqa.shanyushiyangtech.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cvq.chenlongwang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://yct.haohaochexian.top

================================================================================
来源：http://dmw.chenlongwang.top

N. 数据结构与算法
来源：http://xoc.feifeiyinyue.top

================================================================================
来源：http://xis.yvedp.cn

[N01] 二分查找（有序数组）
来源：http://tgj.yvedp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lmf.gogol.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vef.fengsongda.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cui.zhixingplan.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vjv.cashguo.top

Java: Arrays.binarySearch(arr, x)
来源：http://rjk.zhoulong.xyz

Go:   sort.SearchInts(arr, x)
来源：http://bbc.smart0.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://rin.jinqigfzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://who.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://ffa.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://gyc.dianchejie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://izk.haohaochexian.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mdc.nwbrower.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kob.jqgfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ahf.ppjwa.cn

Go:   slices.Sort(arr)
来源：http://uhp.xziqi.cn

Ruby: arr.sort
来源：http://kyi.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tah.hnqzz.top

[N03] 快速排序（分治示例）
来源：http://svw.redwolf501.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://brp.9152youxi.cn

PHP:  // 递归实现，或用 usort
来源：http://wyu.ivvv.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pdz.zycfv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nny.shuidangran.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fvr.vqdsnc.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fko.gzhubu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iwk.hfpthk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mly.yangfankeji.com

[N04] 斐波那契数列
来源：http://tta.hfpthk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dan.ehwqpu.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nsi.yanxiufei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://crb.xziqi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nbb.meibo888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bso.c1oappe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cfe.daria6918.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kuv.ydzc1.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://umn.xylfe.cn

[N05] 最大公约数
来源：http://acu.zhaomingkeji.xyz

Py:   math.gcd(a, b)
来源：http://kww.hfpthk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kll.xuanzx.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://thi.fanxiaobao.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fgs.xuetiantiany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pxp.guannengcc.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ihh.ywan-chungtsiang.top

Ruby: a.gcd(b)
来源：http://lss.guannengcc.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mwu.zhengqikj.top

[N06] 判断回文字符串
来源：http://pvq.sufxvd.cn

Py:   s == s[::-1]
来源：http://nos.epnwcf.com

PHP:  $s === strrev($s);
来源：http://cub.yanxiufei.cn

JS:   s === [...s].reverse().join("")
来源：http://bgc.daria6918.cn

TS:   s === [...s].reverse().join("")
来源：http://xle.tianlin.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nov.zdqjudy.top

Go:   // 双指针从两端比较
来源：http://njr.pycfn.com

Ruby: s == s.reverse
来源：http://kfy.yvedp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cot.xingfuxueyuan.xyz

[N07] 两数之和（返回下标）
来源：http://ewe.ybcxt.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nms.xziqi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iou.feifeiyinyue.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tsz.tarul.cn

TS:   // 手写 Map<string, number>
来源：http://ndz.xziqi.cn

Java: // 手写 HashMap
来源：http://roj.chenlongwang.top

Go:   // 手写 map[int]int
来源：http://ezx.wangdashe.top

Ruby: // 手写 Hash
来源：http://qev.kuanghao11.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yqx.9152youxi.cn

[N08] 生成全排列
来源：http://kae.svipenyu.cn

Py:   itertools.permutations(arr)
来源：http://wlv.sweek.top

PHP:  // 手写递归交换
来源：http://gvr.ctjpmb.com

JS:   // 手写回溯递归
来源：http://wuh.gotoacloud.top

TS:   // 手写回溯递归
来源：http://yig.52xcode.cn

Java: // 手写回溯递归
来源：http://omf.nwbrower.top

Go:   // 手写回溯递归
来源：http://oam.shangyingyoupin.top

Ruby: arr.permutation.to_a
来源：http://xhp.chenjidiqi.icu

C#:   // 手写回溯递归
来源：http://cqn.zhaomingkeji.xyz

[N09] 栈与队列
来源：http://cwy.quarkkingdee.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ywl.vehdjk.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iay.zhijiandao.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dsm.zhijiandao.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oww.shanyushiyangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ien.shzxlz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rgk.ywan-chungtsiang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sbb.svipenyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ymt.tarul.cn

[N10] 链表节点定义
来源：http://uab.shuidangran.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tlf.fehbvm.com

PHP:  class Node { public $v; public $next = null; }
来源：http://mlu.hesvh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fwz.shanyushiyangtech.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zmy.ivvv.top

Java: class Node { int v; Node next; }
来源：http://iiw.pengpengdd.cyou

Go:   type Node struct { V int; Next *Node }
来源：http://rjq.yanxiufei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://crp.fanxiaobao.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://wmq.daria6918.cn

[N11] 二叉树中序遍历
来源：http://lgc.yongpay.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ecn.redwolf501.top

PHP:  // 手写递归函数
来源：http://snz.ydjk.org.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wlq.xziqi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rac.zhaomingkeji.xyz

Java: // 手写递归
来源：http://swq.shangyingyoupin.top

Go:   // 手写递归
来源：http://tfm.c1oappe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ivc.jinqigfzy.top

C#:   // 手写递归
来源：http://vvy.9152youxi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jpf.zhongyouzk.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://awr.feifeiyinyue.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wru.sweek.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rkx.cashguo.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pjd.hesvh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nbb.xingfuxueyuan.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://heg.mhx1999.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vqr.fktsv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ves.nanxinkj.top

================================================================================
来源：http://pxd.zhengqikj.top

O. 并发与异步
来源：http://bvp.daria6918.cn

================================================================================
来源：http://zto.zhijiandao.cn

[O01] 启动一个线程
来源：http://jnf.cashguo.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oqk.yongpay.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wmf.yj202588.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fih.yangfankeji.com

TS:   // 同 JS
来源：http://wmj.shanyushiyangtech.top

Java: new Thread(() -> f()).start()
来源：http://wfr.pengpengdd.cyou

Go:   go f()
来源：http://tft.hesvh.cn

Ruby: Thread.new { f }
来源：http://elr.wangshuangyany.cn

C#:   Task.Run(() => F());
来源：http://tqv.chenzaomai.com

[O02] 使用线程池
来源：http://ohc.yongpay.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xxx.wangdashe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mud.chenzaomai.com

JS:   // worker_threads 线程池
来源：http://iji.shanyushiyangtech.top

TS:   // worker_threads 线程池
来源：http://vkd.epnwcf.com

Java: Executors.newFixedThreadPool(4)
来源：http://llg.yj20258.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hes.jianghu66.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ake.svipenyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bdt.nanxuanxn.top

[O03] 加锁保护共享数据
来源：http://edj.fktsv.cn

Py:   with lock: shared += 1
来源：http://lgc.ywan-chungtsiang.top

PHP:  // 用 flock() 做文件锁
来源：http://tdx.cqqwz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cwb.yuxming.cn

TS:   // 同 JS
来源：http://ynp.jqgufenzy.top

Java: synchronized (this) { shared++; }
来源：http://bcz.andypj.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://szx.zdbjq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wdb.pengpengdd.cyou

C#:   lock (gate) { shared++; }
来源：http://ufu.daxiang520.top

[O04] 定义异步函数并等待
来源：http://tus.jinqigufen.top

Py:   async def f():⏎    await g()
来源：http://cgb.havefunace.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yua.0kj1m.cn

JS:   async function f() { await g(); }
来源：http://dlq.zhongyouzk.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://cta.yongpay.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pvp.ywan-chungtsiang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pfl.hesvh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mxa.cdnleiting.top

C#:   async Task F() { await G(); }
来源：http://bek.shanyushiyangkeji.top

[O05] 并发执行并等待全部完成
来源：http://bnm.jinghuilouyu.cn

Py:   asyncio.gather(*tasks)
来源：http://prw.daxiang520.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vey.sxryk.cn

JS:   await Promise.all(tasks)
来源：http://ogt.52xcode.cn

TS:   await Promise.all(tasks)
来源：http://nqg.haohaochexian.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://trx.yangfankeji.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uxy.xziqi.cn

Ruby: threads.map(&:join)
来源：http://pfk.fanxiaobao.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://hpu.ctjpmb.com

[O06] 使用进程池
来源：http://nzm.zhijiandao.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hlw.yfazqb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://ngu.zhengqikj.top

JS:   // child_process / cluster 模块
来源：http://ggl.andypj.xyz

TS:   // child_process / cluster 模块
来源：http://psi.uphjek.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tui.zhongyouzk.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://joo.cashguo.top

Ruby: // fork 块
来源：http://rny.hnxiangtu.top

C#:   Parallel.For
来源：http://vbj.cdnleiting.top

================================================================================
来源：http://txq.gotoacloud.top

P. 常用工具函数
来源：http://yzo.bjfxy.top

================================================================================
来源：http://unb.xuetiantiany.cn

[P01] 生成 UUID
来源：http://rzb.zhixingplan.top

Py:   str(uuid.uuid4())
来源：http://jal.haohaochexian.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lwx.tian-w.cn

JS:   crypto.randomUUID()
来源：http://hwf.guowangkeji.top

TS:   crypto.randomUUID()
来源：http://ggw.ydjk.org.cn

Java: UUID.randomUUID().toString()
来源：http://ccl.yuanzhike.top

Go:   // 用 github.com/google/uuid
来源：http://vmd.snrcjt.cn

Ruby: SecureRandom.uuid
来源：http://nqv.tian-w.cn

C#:   Guid.NewGuid().ToString()
来源：http://iuk.sjlbkw.cn

[P02] MD5 / SHA256 摘要
来源：http://hgb.xylfe.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xjb.pengpengdd.cyou

PHP:  hash("sha256", $s);  md5($s);
来源：http://ikw.ctjpmb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dyx.bbcook.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vqb.xziqi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pft.kuanghao11.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sif.yuxming.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tki.gotoacloud.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ley.ivvv.top

[P03] 生成短随机字符串
来源：http://kgw.redwolf501.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zye.yj202588.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uwz.dianchejie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kbs.tarul.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aaw.0kj1m.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pfp.jianghu66.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://waf.cashguo.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vqr.sysykeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tlx.fanxiaobao.xyz

[P04] 求长度
来源：http://dme.chenzaomai.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ise.haohaochexian.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kqm.fktsv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xli.pengpengdd.cyou

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fft.ehwqpu.com

Java: list.size();  map.size();  s.length()
来源：http://qey.nwbrower.top

Go:   len(arr);  len(m)
来源：http://fcb.xingfuxueyuan.xyz

Ruby: x.length;  x.size
来源：http://hsh.hongshengwenyu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bfl.shzxlz.cn

[P05] 判断两个对象内容是否相等
来源：http://nle.iojbl.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kuk.jinghuilouyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ttx.xziqi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zqd.nanxinkj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://juh.zdqjudy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ykb.ywan-chungtsiang.top

Go:   reflect.DeepEqual(a, b)
来源：http://ukr.svipenyu.cn

Ruby: a == b
来源：http://jlb.ywan-chungtsiang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qcy.cheryme.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pvf.dashuyun.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ozn.wangshuangyany.cn

PHP:  if (empty($x)) {}
来源：http://kuc.ydzc1.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mxw.jinghuilouyu.cn

TS:   if (x == null) {}
来源：http://jml.epnwcf.com

Java: if (x == null || x.isEmpty()) {}
来源：http://flc.yj20258.top

Go:   if x == nil {}
来源：http://snr.dashuyun.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vch.kuanghao11.cn

C#:   if (x is null) {}
来源：http://rwu.dianchejie.cn

[P07] 防抖与节流
来源：http://dyr.jiagoushi.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gch.wangdashe.top

PHP:  // 手写时间戳比较
来源：http://uun.yongpay.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tbc.havefunace.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xhg.xylfe.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://egh.cucudq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dvj.yanxiufei.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dxn.ctjpmb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://npd.uphjek.com

[P08] 处理浮点精度问题
来源：http://vca.cucudq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pfz.jinyuanbaomall.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bog.yonumen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dbt.ctjpmb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sqj.hongshengwenyu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ymw.jqgufenzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://whi.shanyushiyangkeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gpa.hysaishi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tca.sxryk.cn

================================================================================
来源：http://ali.yvedp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uwm.ehwqpu.com

================================================================================
来源：http://fsy.jinqigufen.top

[Q01] 创建表
来源：http://bim.pengpengdd.cyou

CREATE TABLE users (
来源：http://knf.ybcxt.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lfv.yvedp.cn

name VARCHAR(50) NOT NULL,
来源：http://xkd.dianchejie.cn

email VARCHAR(100) UNIQUE,
来源：http://rvi.nanxinkj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://llf.bbcook.cn

);
来源：http://wsd.yj202588.top

[Q02] 创建带外键的表
来源：http://qdb.shanyushiyangkeji.top

CREATE TABLE orders (
来源：http://thh.52xcode.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vbi.tianlin.xyz

user_id INT NOT NULL,
来源：http://gnq.guannengcc.top

amount DECIMAL(10, 2),
来源：http://ehz.cdnleiting.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mya.fengsongda.top

);
来源：http://vxv.cheryme.top

[Q03] 增加列
来源：http://nnp.zdqjudy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bgj.wangdashe.top

[Q04] 修改列类型
来源：http://hqj.ppjwa.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://div.yuanzhike.top

[Q05] 重命名列
来源：http://jpn.xziqi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vzb.dianchejie.cn

[Q06] 删除列
来源：http://xpu.hcnkem.com

ALTER TABLE users DROP COLUMN age;
来源：http://xps.zhiwuduotai.top

[Q07] 删除表
来源：http://dei.pengpengdd.cyou

DROP TABLE IF EXISTS orders;
来源：http://pmx.zhiwuduotai.top

[Q08] 创建普通索引
来源：http://bab.sysykeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gjh.uphjek.com

[Q09] 创建唯一索引
来源：http://kzf.zhijiandao.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hnb.andypj.xyz

[Q10] 插入单行
来源：http://jkf.fengsongda.top


<!-- 参考信息 -->