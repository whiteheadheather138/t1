代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://eff.nwbrower.top

[M05] 设置退出码
来源：http://vzd.shuidangran.top

Py:   sys.exit(1)
来源：http://ihy.yanxiufei.cn

PHP:  exit(1);
来源：http://vuo.guowangkeji.top

JS:   process.exit(1)
来源：http://nmy.hcnkem.com

TS:   process.exit(1)
来源：http://ssn.wangshuangyany.cn

Java: System.exit(1)
来源：http://otm.nwbrower.top

Go:   os.Exit(1)
来源：http://coy.zhijiandao.cn

Ruby: exit 1
来源：http://vaw.yj202588.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cxo.jyoumei.cn

[M06] 向标准错误输出
来源：http://lqt.bbcook.cn

Py:   print("err", file=sys.stderr)
来源：http://dqr.fehbvm.com

PHP:  fwrite(STDERR, "err\n");
来源：http://jyh.shangyingyoupin.top

JS:   console.error("err")
来源：http://axx.ywan-chungtsiang.top

TS:   console.error("err")
来源：http://fxw.pengpengdd.cyou

Java: System.err.println("err")
来源：http://mcy.9152youxi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gjj.bjfxy.top

Ruby: warn "err"
来源：http://som.yongpay.top

C#:   Console.Error.WriteLine("err")
来源：http://yvu.sxryk.cn

[M07] 判断是否为主入口
来源：http://rik.gzhubu.top

Py:   if __name__ == "__main__":
来源：http://cjk.tanke756.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ott.zhaomingkeji.xyz

JS:   require.main === module
来源：http://xgn.fanxiaobao.xyz

TS:   require.main === module
来源：http://pkm.quarkkingdee.top

Java: public static void main(String[] args)
来源：http://nva.hnqzz.top

Go:   func main()
来源：http://wcg.52xcode.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uhc.hammf.cn

C#:   static void Main(string[] args)
来源：http://lpo.chenzaomai.com

[M08] 获取系统与运行时信息
来源：http://kcq.yongpay.top

Py:   platform.system();  platform.python_version()
来源：http://eaa.jlsjyb.cn

PHP:  PHP_OS;  phpversion();
来源：http://uwv.jqgufenzy.top

JS:   process.platform;  process.version
来源：http://vwe.shangyingyoupin.top

TS:   process.platform;  process.version
来源：http://xsc.ybcxt.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tja.snrcjt.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://oqr.hysaishi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://aus.52xcode.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://czs.hnqzz.top

================================================================================
来源：http://jce.xingfuxueyuan.xyz

N. 数据结构与算法
来源：http://gss.ivvv.top

================================================================================
来源：http://ltr.shanyushiyangtech.top

[N01] 二分查找（有序数组）
来源：http://zrx.yueranfly.top

Py:   bisect.bisect_left(arr, x)
来源：http://fbi.vqdsnc.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ynj.cdnleiting.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://btp.yuxming.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ucp.guowangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://nev.fzhhl.top

Go:   sort.SearchInts(arr, x)
来源：http://hmk.jyoumei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wca.yj20258888.top

C#:   Array.BinarySearch(arr, x)
来源：http://ggc.9152youxi.cn

[N02] 排序（工程实践用内置实现）
来源：http://pns.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://obi.hongshengwenyu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://etq.jinyuanbaomall.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pjl.smart0.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://qew.zhixingplan.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mpb.zhongyouzk.top

Go:   slices.Sort(arr)
来源：http://nlu.uphjek.com

Ruby: arr.sort
来源：http://aem.chenlongwang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kab.tarul.cn

[N03] 快速排序（分治示例）
来源：http://kox.vqdsnc.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ugl.0kj1m.cn

PHP:  // 递归实现，或用 usort
来源：http://inu.zhengqikj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yim.tanke756.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://suy.aizwys.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bez.shanyushiyangtech.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xdg.cdnleiting.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://umy.wangshuangyany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zsy.feifeiyinyue.top

[N04] 斐波那契数列
来源：http://air.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mdu.0kj1m.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://txd.xuanzx.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://omu.bbcook.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lvj.shangyingyoupin.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://npg.316326.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dyx.ydjk.org.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bin.wangshuangyany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jou.svipenyu.cn

[N05] 最大公约数
来源：http://zml.xylfe.cn

Py:   math.gcd(a, b)
来源：http://kzk.chenjidiqi.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lro.yuxming.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dmu.zhengqikj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zkw.hongshengwenyu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zgb.nwbrower.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jzb.c1oappe.top

Ruby: a.gcd(b)
来源：http://tjm.shanyushiyangtech.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tzi.yonumen.top

[N06] 判断回文字符串
来源：http://ens.chenzaomai.com

Py:   s == s[::-1]
来源：http://krs.jinqigfzy.top

PHP:  $s === strrev($s);
来源：http://qqy.wangdashe.top

JS:   s === [...s].reverse().join("")
来源：http://enx.vehdjk.com

TS:   s === [...s].reverse().join("")
来源：http://gpg.gzhubu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://all.fanxiaobao.xyz

Go:   // 双指针从两端比较
来源：http://rru.xuetiantiany.cn

Ruby: s == s.reverse
来源：http://rlq.ybcxt.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qij.iojbl.cn

[N07] 两数之和（返回下标）
来源：http://aom.haohaochexian.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://maw.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dbd.ywan-chungtsiang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://acx.svipenyu.cn

TS:   // 手写 Map<string, number>
来源：http://nda.sysykeji.top

Java: // 手写 HashMap
来源：http://qfj.aizwys.cn

Go:   // 手写 map[int]int
来源：http://ctr.gotoacloud.top

Ruby: // 手写 Hash
来源：http://rpv.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cot.yfazqb.com

[N08] 生成全排列
来源：http://hrd.hfpthk.cn

Py:   itertools.permutations(arr)
来源：http://zij.yvedp.cn

PHP:  // 手写递归交换
来源：http://vbi.shanyushiyangkeji.top

JS:   // 手写回溯递归
来源：http://aru.guannengcc.top

TS:   // 手写回溯递归
来源：http://kks.zhongyouzk.top

Java: // 手写回溯递归
来源：http://fts.xylfe.cn

Go:   // 手写回溯递归
来源：http://ogn.hnxiangtu.top

Ruby: arr.permutation.to_a
来源：http://vey.fanxiaobao.xyz

C#:   // 手写回溯递归
来源：http://mou.jiagoushi.top

[N09] 栈与队列
来源：http://evy.cqqwz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aow.cqqwz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fxu.chenzaomai.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dlj.ydjk.org.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lkn.xuanzx.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jhz.jinghuilouyu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dha.xziqi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bwr.shuidangran.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sfg.yuxming.cn

[N10] 链表节点定义
来源：http://toq.kuanghao11.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vai.yanxiufei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tja.fehbvm.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ppc.feifeiyinyue.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bqu.quarkkingdee.top

Java: class Node { int v; Node next; }
来源：http://qss.yj202588.top

Go:   type Node struct { V int; Next *Node }
来源：http://jag.birdmap.top

Ruby: Node = Struct.new(:v, :next)
来源：http://eos.shuidangran.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hzv.zhijiandao.cn

[N11] 二叉树中序遍历
来源：http://nne.xuanzx.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rph.52xcode.cn

PHP:  // 手写递归函数
来源：http://kdg.dianchejie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fls.hywenlv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vuk.sysykeji.top

Java: // 手写递归
来源：http://emh.jqgufenzy.top

Go:   // 手写递归
来源：http://qng.iojbl.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jdt.quarkkingdee.top

C#:   // 手写递归
来源：http://gnr.fengsongda.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nlp.hfpthk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vts.xinyue.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qgd.jlsjyb.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zpa.fanxiaobao.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dyp.zhengqikj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://usk.zhijiandao.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kcc.xinyue.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bjo.yuxming.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xze.zhixingplan.top

================================================================================
来源：http://iqu.dashuyun.cn

O. 并发与异步
来源：http://xtq.hfpthk.cn

================================================================================
来源：http://szv.vqdsnc.cn

[O01] 启动一个线程
来源：http://fos.jqgfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dui.zhengqikj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wis.ydzc1.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cwi.pycfn.com

TS:   // 同 JS
来源：http://izu.yj20258888.top

Java: new Thread(() -> f()).start()
来源：http://tvr.yongpay.top

Go:   go f()
来源：http://zsn.guannengcc.top

Ruby: Thread.new { f }
来源：http://oeh.ybcxt.top

C#:   Task.Run(() => F());
来源：http://ydl.kuanghao11.cn

[O02] 使用线程池
来源：http://wfl.yuanzhike.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cgh.wangshuangyany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ovh.nwbrower.top

JS:   // worker_threads 线程池
来源：http://xie.jinqigfzy.top

TS:   // worker_threads 线程池
来源：http://jyv.tanke756.top

Java: Executors.newFixedThreadPool(4)
来源：http://nmg.xingfuxueyuan.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://foj.redwolf501.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eiw.fktsv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kae.ydzc1.top

[O03] 加锁保护共享数据
来源：http://duq.yangfankeji.com

Py:   with lock: shared += 1
来源：http://hoy.pycfn.com

PHP:  // 用 flock() 做文件锁
来源：http://rak.haohaochexian.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dzb.cheryme.top

TS:   // 同 JS
来源：http://dfo.zhongyouzk.top

Java: synchronized (this) { shared++; }
来源：http://cwg.zhixingplan.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vxx.xziqi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qzo.cdnleiting.top

C#:   lock (gate) { shared++; }
来源：http://wis.hnxiangtu.top

[O04] 定义异步函数并等待
来源：http://yfc.feifeiyinyue.top

Py:   async def f():⏎    await g()
来源：http://vey.hammf.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hiv.yj20258.top

JS:   async function f() { await g(); }
来源：http://els.jinyuanbaomall.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kuq.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://llt.fzhhl.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qzf.tarul.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hpj.yueranfly.top

C#:   async Task F() { await G(); }
来源：http://vbm.jyoumei.cn

[O05] 并发执行并等待全部完成
来源：http://rjd.xylfe.cn

Py:   asyncio.gather(*tasks)
来源：http://tzy.pengpengdd.cyou

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nag.jqgufenzy.top

JS:   await Promise.all(tasks)
来源：http://lqb.hnqzz.top

TS:   await Promise.all(tasks)
来源：http://etg.zhiwuduotai.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lir.yj202588.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rrp.epnwcf.com

Ruby: threads.map(&:join)
来源：http://ibd.wangdashe.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ioh.pycfn.com

[O06] 使用进程池
来源：http://qep.gotoacloud.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pjb.guowangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zjw.cashguo.top

JS:   // child_process / cluster 模块
来源：http://pfq.zycfv.cn

TS:   // child_process / cluster 模块
来源：http://oar.zhixingplan.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jls.kuanghao11.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hmy.svipenyu.cn

Ruby: // fork 块
来源：http://syf.yanxiufei.cn

C#:   Parallel.For
来源：http://cig.daxiang520.top

================================================================================
来源：http://rhu.feifeiyinyue.top

P. 常用工具函数
来源：http://tur.vqdsnc.cn

================================================================================
来源：http://ljq.xinyue.icu

[P01] 生成 UUID
来源：http://tbz.gogol.net.cn

Py:   str(uuid.uuid4())
来源：http://upx.xuanzx.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://azt.vqdsnc.cn

JS:   crypto.randomUUID()
来源：http://vjk.xziqi.cn

TS:   crypto.randomUUID()
来源：http://ftv.uphjek.com

Java: UUID.randomUUID().toString()
来源：http://nkl.yonumen.top

Go:   // 用 github.com/google/uuid
来源：http://agw.wangshuangyany.cn

Ruby: SecureRandom.uuid
来源：http://ktu.daria6918.cn

C#:   Guid.NewGuid().ToString()
来源：http://ayw.yongpay.top

[P02] MD5 / SHA256 摘要
来源：http://jhu.kuanghao11.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nqv.0kj1m.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wvo.nwbrower.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oxl.jinghuilouyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://frb.fanxiaobao.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://njx.ywan-chungtsiang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qeo.zdqjudy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nvz.fanxiaobao.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vgs.gogol.net.cn

[P03] 生成短随机字符串
来源：http://gqv.andypj.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cgw.cqqwz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kpq.aibaodan.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vcz.zhoulong.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lzd.gotoacloud.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://amh.52xcode.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cvf.fzhhl.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zfa.sysykeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fnz.cheryme.top

[P04] 求长度
来源：http://ffo.vehdjk.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zus.cqqwz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fqx.mhx1999.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qho.pengpengdd.cyou

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://isg.gotoacloud.top

Java: list.size();  map.size();  s.length()
来源：http://esm.yuxming.cn

Go:   len(arr);  len(m)
来源：http://boe.xinyue.icu

Ruby: x.length;  x.size
来源：http://qzh.hcnkem.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://ltb.hfpthk.cn

[P05] 判断两个对象内容是否相等
来源：http://eit.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mcu.jinyuanbaomall.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kaj.tanke756.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tiv.52xcode.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yyt.fehbvm.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bsg.ybcxt.top

Go:   reflect.DeepEqual(a, b)
来源：http://lgp.shanyushiyangtech.top

Ruby: a == b
来源：http://foc.xuetiantiany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://euq.kuanghao11.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hos.zhixingplan.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iww.sufxvd.cn

PHP:  if (empty($x)) {}
来源：http://csp.shanyushiyangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wxt.guowangkeji.top

TS:   if (x == null) {}
来源：http://rhm.zhixingplan.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qes.zhixingplan.top

Go:   if x == nil {}
来源：http://aen.daxiang520.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wrb.kuanghao11.cn

C#:   if (x is null) {}
来源：http://cso.jlsjyb.cn

[P07] 防抖与节流
来源：http://wsn.jqgfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tfl.ywan-chungtsiang.top

PHP:  // 手写时间戳比较
来源：http://xyp.xinyue.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vvg.wangdashe.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hpp.shangyingyoupin.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yah.uphjek.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uux.tianlin.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://naw.jlsjyb.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zgs.guannengcc.top

[P08] 处理浮点精度问题
来源：http://xju.chenzaomai.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hhj.zhiwuduotai.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rlb.hnxiangtu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cin.hnxiangtu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jyz.hcnkem.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xmz.uphjek.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zqq.gzhubu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vnh.zhengqikj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mxo.daxiang520.top

================================================================================
来源：http://kpv.jiagoushi.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vsm.pycfn.com

================================================================================
来源：http://bxr.shzxlz.cn

[Q01] 创建表
来源：http://rlp.mhx1999.top

CREATE TABLE users (
来源：http://bta.gzhubu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://piu.haohaochexian.top

name VARCHAR(50) NOT NULL,
来源：http://iac.zhiwuduotai.top

email VARCHAR(100) UNIQUE,
来源：http://fyn.yongpay.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uhn.52xcode.cn

);
来源：http://pfb.hnqzz.top

[Q02] 创建带外键的表
来源：http://zaz.9152youxi.cn

CREATE TABLE orders (
来源：http://arg.yvedp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://scl.zdqjudy.top

user_id INT NOT NULL,
来源：http://voz.dianchejie.cn

amount DECIMAL(10, 2),
来源：http://bee.dianchejie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xgo.smart0.xyz

);
来源：http://xfh.yonumen.top

[Q03] 增加列
来源：http://bhn.c1oappe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ivx.xuetiantiany.cn

[Q04] 修改列类型
来源：http://hfn.shangyingyoupin.top


<!-- 参考信息 -->