代发 wailian999

Ruby: exit 1
来源：http://sco.fanxiaobao.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pko.mhx1999.top

[M06] 向标准错误输出
来源：http://uuh.quarkkingdee.top

Py:   print("err", file=sys.stderr)
来源：http://umz.chenlongwang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qsg.sjlbkw.cn

JS:   console.error("err")
来源：http://nza.yuanzhike.top

TS:   console.error("err")
来源：http://xfl.tianlin.xyz

Java: System.err.println("err")
来源：http://bdw.redwolf501.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nyl.jqgfzy.top

Ruby: warn "err"
来源：http://xdp.hnxiangtu.top

C#:   Console.Error.WriteLine("err")
来源：http://dpn.yj20258.top

[M07] 判断是否为主入口
来源：http://wzk.hongshengwenyu.top

Py:   if __name__ == "__main__":
来源：http://yjr.meibo888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hia.chenzaomai.com

JS:   require.main === module
来源：http://vmq.wangshuangyany.cn

TS:   require.main === module
来源：http://jyk.yangfankeji.com

Java: public static void main(String[] args)
来源：http://jrf.yongpay.top

Go:   func main()
来源：http://qcl.pycfn.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jvd.yvedp.cn

C#:   static void Main(string[] args)
来源：http://qas.ydjk.org.cn

[M08] 获取系统与运行时信息
来源：http://zbd.fzhhl.top

Py:   platform.system();  platform.python_version()
来源：http://wqr.bbcook.cn

PHP:  PHP_OS;  phpversion();
来源：http://hfg.daxiang520.top

JS:   process.platform;  process.version
来源：http://cxg.chenlongwang.top

TS:   process.platform;  process.version
来源：http://qwh.xylfe.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lbt.mhx1999.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://taa.zhaomingkeji.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lay.316326.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://kjd.tanke756.top

================================================================================
来源：http://qsk.jlsjyb.cn

N. 数据结构与算法
来源：http://ggp.cqqwz.cn

================================================================================
来源：http://cup.yvedp.cn

[N01] 二分查找（有序数组）
来源：http://ooi.jinghuilouyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ztw.xuetiantiany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vnf.jinqigfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fwy.sweek.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xpe.zdqjudy.top

Java: Arrays.binarySearch(arr, x)
来源：http://tmz.vqdsnc.cn

Go:   sort.SearchInts(arr, x)
来源：http://jht.daria6918.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://axt.ydzc1.top

C#:   Array.BinarySearch(arr, x)
来源：http://fth.birdmap.top

[N02] 排序（工程实践用内置实现）
来源：http://zvc.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://qup.nanxuanxn.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://use.vehdjk.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://zms.hysaishi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cou.guannengcc.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bnx.fktsv.cn

Go:   slices.Sort(arr)
来源：http://phi.xziqi.cn

Ruby: arr.sort
来源：http://mso.xinyue.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://vjj.jinyuanbaomall.cn

[N03] 快速排序（分治示例）
来源：http://afg.jqgfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mcy.dashuyun.cn

PHP:  // 递归实现，或用 usort
来源：http://oiw.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://asr.hongshengwenyu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://szq.andypj.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://elw.zhiwuduotai.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wtq.gotoacloud.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sii.yueranfly.top

C#:   // 手写递归，或 Array.Sort
来源：http://zyt.nanxuanxn.top

[N04] 斐波那契数列
来源：http://hru.fehbvm.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zxr.zhengqikj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yhp.shuidangran.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fwn.nanxuanxn.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://msb.bbcook.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://enl.c1oappe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://trd.uphjek.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://crz.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dum.cheryme.top

[N05] 最大公约数
来源：http://yqr.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://mds.bjfxy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lkf.smart0.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lmm.pycfn.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bxz.quarkkingdee.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blf.jinqigufen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ecq.yanxiufei.cn

Ruby: a.gcd(b)
来源：http://eep.yonumen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://upb.cheryme.top

[N06] 判断回文字符串
来源：http://fiz.haohaochexian.top

Py:   s == s[::-1]
来源：http://gxd.c1oappe.top

PHP:  $s === strrev($s);
来源：http://rrd.fktsv.cn

JS:   s === [...s].reverse().join("")
来源：http://qzv.shangyingyoupin.top

TS:   s === [...s].reverse().join("")
来源：http://coy.haohaochexian.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bfm.zhoulong.xyz

Go:   // 双指针从两端比较
来源：http://jfm.shanyushiyangkeji.top

Ruby: s == s.reverse
来源：http://vpa.hfpthk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vme.52xcode.cn

[N07] 两数之和（返回下标）
来源：http://usd.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fvk.redwolf501.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://beq.nwbrower.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kxj.andypj.xyz

TS:   // 手写 Map<string, number>
来源：http://qdv.jyoumei.cn

Java: // 手写 HashMap
来源：http://ner.hcnkem.com

Go:   // 手写 map[int]int
来源：http://apz.fktsv.cn

Ruby: // 手写 Hash
来源：http://qks.gaohongyu789.top

C#:   // 手写 Dictionary<int, int>
来源：http://ifr.tarul.cn

[N08] 生成全排列
来源：http://bya.zycfv.cn

Py:   itertools.permutations(arr)
来源：http://vuk.ydzc1.top

PHP:  // 手写递归交换
来源：http://mcb.quarkkingdee.top

JS:   // 手写回溯递归
来源：http://oyy.vehdjk.com

TS:   // 手写回溯递归
来源：http://gux.shangyingyoupin.top

Java: // 手写回溯递归
来源：http://utc.chenzaomai.com

Go:   // 手写回溯递归
来源：http://vkh.shanyushiyangtech.top

Ruby: arr.permutation.to_a
来源：http://zjl.jinyuanbaomall.cn

C#:   // 手写回溯递归
来源：http://vpd.xylfe.cn

[N09] 栈与队列
来源：http://iem.hesvh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://amt.yangfankeji.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tsr.cucudq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zmh.xinyue.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pny.epnwcf.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jav.fanxiaobao.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dqy.shzxlz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hyz.jiagoushi.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vko.sweek.top

[N10] 链表节点定义
来源：http://tih.cashguo.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mtd.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://nlm.fzhhl.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tbc.zycfv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ypc.uphjek.com

Java: class Node { int v; Node next; }
来源：http://qrf.tanke756.top

Go:   type Node struct { V int; Next *Node }
来源：http://kyn.zhaomingkeji.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://kjo.cqqwz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fog.yj20258888.top

[N11] 二叉树中序遍历
来源：http://iwe.jinqigfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rrp.zhijiandao.cn

PHP:  // 手写递归函数
来源：http://lzy.zhengqikj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hnl.iojbl.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qxs.9152youxi.cn

Java: // 手写递归
来源：http://ahq.chenzaomai.com

Go:   // 手写递归
来源：http://yzq.xuanzx.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://njh.chenlongwang.top

C#:   // 手写递归
来源：http://msk.meibo888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jza.sufxvd.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lab.hongshengwenyu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ygi.bjfxy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qxh.c1oappe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gjm.uphjek.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ulu.meibo888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pzy.smart0.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jlt.9152youxi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://erb.haohaochexian.top

================================================================================
来源：http://kkd.gotoacloud.top

O. 并发与异步
来源：http://mbw.mhx1999.top

================================================================================
来源：http://mgh.bbcook.cn

[O01] 启动一个线程
来源：http://bjn.fengsongda.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uom.pycfn.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dwo.xuanzx.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://apn.tian-w.cn

TS:   // 同 JS
来源：http://ohi.haohaochexian.top

Java: new Thread(() -> f()).start()
来源：http://chy.birdmap.top

Go:   go f()
来源：http://pdm.nanxinkj.top

Ruby: Thread.new { f }
来源：http://ibs.ywan-chungtsiang.top

C#:   Task.Run(() => F());
来源：http://rcj.316326.xyz

[O02] 使用线程池
来源：http://kaj.zycfv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wmi.jianghu66.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gdt.dashuyun.cn

JS:   // worker_threads 线程池
来源：http://xlo.ctjpmb.com

TS:   // worker_threads 线程池
来源：http://gja.chenlongwang.top

Java: Executors.newFixedThreadPool(4)
来源：http://hmb.bjfxy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mak.zhaomingkeji.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://viz.hongshengwenyu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fva.fehbvm.com

[O03] 加锁保护共享数据
来源：http://msy.guowangkeji.top

Py:   with lock: shared += 1
来源：http://bfz.zhaomingkeji.xyz

PHP:  // 用 flock() 做文件锁
来源：http://iqu.yuanzhike.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dxr.jlsjyb.cn

TS:   // 同 JS
来源：http://tir.hesvh.cn

Java: synchronized (this) { shared++; }
来源：http://aed.hfpthk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://leb.ydzc1.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://gom.gzhubu.top

C#:   lock (gate) { shared++; }
来源：http://kpu.nanxinkj.top

[O04] 定义异步函数并等待
来源：http://tdn.jinqigfzy.top

Py:   async def f():⏎    await g()
来源：http://dvj.chenjidiqi.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://spr.tian-w.cn

JS:   async function f() { await g(); }
来源：http://lkz.ydzc1.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hfh.smart0.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lyp.hcnkem.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yoq.hnxiangtu.top

Ruby: # 用 Fiber 或 async gem
来源：http://lgl.gzhubu.top

C#:   async Task F() { await G(); }
来源：http://ppc.mhx1999.top

[O05] 并发执行并等待全部完成
来源：http://lyp.daxiang520.top

Py:   asyncio.gather(*tasks)
来源：http://zrz.yj202588.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kfg.zdqjudy.top

JS:   await Promise.all(tasks)
来源：http://xxx.ivvv.top

TS:   await Promise.all(tasks)
来源：http://pfn.ywan-chungtsiang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gak.uphjek.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qvh.9152youxi.cn

Ruby: threads.map(&:join)
来源：http://kcl.sxryk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pnn.daxiang520.top

[O06] 使用进程池
来源：http://nbt.sjlbkw.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dbg.yuanzhike.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jdh.ydzc1.top

JS:   // child_process / cluster 模块
来源：http://ini.wangshuangyany.cn

TS:   // child_process / cluster 模块
来源：http://xjw.9152youxi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://quv.wangshuangyany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rgr.cqqwz.cn

Ruby: // fork 块
来源：http://oup.zdbjq.cn

C#:   Parallel.For
来源：http://vkz.chenzaomai.com

================================================================================
来源：http://ocd.nanxinkj.top

P. 常用工具函数
来源：http://txx.pycfn.com

================================================================================
来源：http://jyz.dashuyun.cn

[P01] 生成 UUID
来源：http://zef.jqgufenzy.top

Py:   str(uuid.uuid4())
来源：http://cov.sjlbkw.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sgn.ehwqpu.com

JS:   crypto.randomUUID()
来源：http://wvp.hammf.cn

TS:   crypto.randomUUID()
来源：http://juu.nanxuanxn.top

Java: UUID.randomUUID().toString()
来源：http://ijg.sufxvd.cn

Go:   // 用 github.com/google/uuid
来源：http://mzf.pengpengdd.cyou

Ruby: SecureRandom.uuid
来源：http://oro.sxryk.cn

C#:   Guid.NewGuid().ToString()
来源：http://anb.nanxinkj.top

[P02] MD5 / SHA256 摘要
来源：http://phr.daxiang520.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oyq.chenzaomai.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://tgp.zycfv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://suy.daxiang520.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jgu.tianlin.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xif.cashguo.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ejy.zhaomingkeji.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yzk.tianlin.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kbt.kuanghao11.cn

[P03] 生成短随机字符串
来源：http://aei.guannengcc.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tbs.yuanzhike.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dfs.jqgufenzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mwv.zhijiandao.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cil.hesvh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ytq.yueranfly.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sja.yonumen.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bmr.ehwqpu.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nus.316326.xyz

[P04] 求长度
来源：http://ihj.havefunace.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jhq.meibo888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jqv.zdqjudy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sob.hnqzz.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aco.vehdjk.com

Java: list.size();  map.size();  s.length()
来源：http://rgu.xuanzx.com

Go:   len(arr);  len(m)
来源：http://kpg.fktsv.cn

Ruby: x.length;  x.size
来源：http://aqz.yj202588.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zes.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://rhz.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://atx.haohaochexian.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nel.jinqigufen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gpt.nwbrower.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://spc.iojbl.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sha.zycfv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zvl.ydjk.org.cn

Ruby: a == b
来源：http://xoh.shuidangran.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://get.fzhhl.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zgb.aizwys.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jup.fzhhl.top

PHP:  if (empty($x)) {}
来源：http://jhx.zdqjudy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kgo.aibaodan.cn

TS:   if (x == null) {}
来源：http://dhv.snrcjt.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ofe.daxiang520.top

Go:   if x == nil {}
来源：http://fhh.birdmap.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nps.mhx1999.top

C#:   if (x is null) {}
来源：http://jhv.xuetiantiany.cn

[P07] 防抖与节流
来源：http://fms.iojbl.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uut.sjlbkw.cn

PHP:  // 手写时间戳比较
来源：http://pnd.0kj1m.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nks.ybcxt.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nfu.xziqi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dqj.ybcxt.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://swb.epnwcf.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://oax.hywenlv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fxv.wangshuangyany.cn

[P08] 处理浮点精度问题
来源：http://quz.fehbvm.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ohx.dashuyun.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iit.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bzm.yj20258.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ydt.vehdjk.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ufy.zhiwuduotai.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sig.epnwcf.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://eat.yj20258.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://scl.ybcxt.top

================================================================================
来源：http://djb.zhijiandao.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sct.tanke756.top

================================================================================
来源：http://edd.sjlbkw.cn

[Q01] 创建表
来源：http://dkx.mhx1999.top

CREATE TABLE users (
来源：http://qag.tarul.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://aem.pycfn.com

name VARCHAR(50) NOT NULL,
来源：http://twh.ctjpmb.com

email VARCHAR(100) UNIQUE,
来源：http://hkx.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zds.fehbvm.com

);
来源：http://inl.sweek.top

[Q02] 创建带外键的表
来源：http://fuz.guowangkeji.top

CREATE TABLE orders (
来源：http://ckl.jinghuilouyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hez.ivvv.top

user_id INT NOT NULL,
来源：http://vys.jinqigfzy.top

amount DECIMAL(10, 2),
来源：http://olx.xylfe.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qgg.hfpthk.cn

);
来源：http://gqd.uphjek.com

[Q03] 增加列
来源：http://upg.tianlin.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zlk.yuanzhike.top

[Q04] 修改列类型
来源：http://tqt.ybcxt.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kyw.shanyushiyangtech.top

[Q05] 重命名列
来源：http://mcu.vqdsnc.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vdm.iojbl.cn

[Q06] 删除列
来源：http://yny.havefunace.top

ALTER TABLE users DROP COLUMN age;
来源：http://loa.snrcjt.cn

[Q07] 删除表
来源：http://wot.sysykeji.top

DROP TABLE IF EXISTS orders;
来源：http://peb.zhijiandao.cn

[Q08] 创建普通索引
来源：http://hco.yanxiufei.cn


<!-- 参考信息 -->