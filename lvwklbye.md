代发 wailian999

[M04] 获取当前工作目录
来源：http://ndj.zhijiandao.cn

Py:   os.getcwd()
来源：http://iur.sweek.top

PHP:  getcwd();
来源：http://wtf.zhongyouzk.top

JS:   process.cwd()
来源：http://xcz.yanxiufei.cn

TS:   process.cwd()
来源：http://ofk.ybcxt.top

Java: Path.of("").toAbsolutePath()
来源：http://pte.ydjk.org.cn

Go:   os.Getwd()
来源：http://bpi.zdbjq.cn

Ruby: Dir.pwd
来源：http://jta.ybcxt.top

C#:   Directory.GetCurrentDirectory()
来源：http://ico.52xcode.cn

[M05] 设置退出码
来源：http://owt.vqdsnc.cn

Py:   sys.exit(1)
来源：http://hqk.fktsv.cn

PHP:  exit(1);
来源：http://dda.wangshuangyany.cn

JS:   process.exit(1)
来源：http://hhn.birdmap.top

TS:   process.exit(1)
来源：http://wlg.tian-w.cn

Java: System.exit(1)
来源：http://bon.yueranfly.top

Go:   os.Exit(1)
来源：http://dyb.yvedp.cn

Ruby: exit 1
来源：http://saz.chenjidiqi.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fxh.wangdashe.top

[M06] 向标准错误输出
来源：http://cfs.haohaochexian.top

Py:   print("err", file=sys.stderr)
来源：http://ltn.hongshengwenyu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xie.yuxming.cn

JS:   console.error("err")
来源：http://wfh.yongpay.top

TS:   console.error("err")
来源：http://uqv.hcnkem.com

Java: System.err.println("err")
来源：http://nob.xuetiantiany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pww.guowangkeji.top

Ruby: warn "err"
来源：http://vix.daxiang520.top

C#:   Console.Error.WriteLine("err")
来源：http://udb.zhaomingkeji.xyz

[M07] 判断是否为主入口
来源：http://gtd.jianghu66.top

Py:   if __name__ == "__main__":
来源：http://tpz.yueranfly.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qaa.0kj1m.cn

JS:   require.main === module
来源：http://fzw.jianghu66.top

TS:   require.main === module
来源：http://vzb.fzhhl.top

Java: public static void main(String[] args)
来源：http://sjp.fzhhl.top

Go:   func main()
来源：http://nnt.zycfv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://duv.52xcode.cn

C#:   static void Main(string[] args)
来源：http://xre.yfazqb.com

[M08] 获取系统与运行时信息
来源：http://bmz.zhengqikj.top

Py:   platform.system();  platform.python_version()
来源：http://dtu.yuxming.cn

PHP:  PHP_OS;  phpversion();
来源：http://qfp.shuidangran.top

JS:   process.platform;  process.version
来源：http://msh.uphjek.com

TS:   process.platform;  process.version
来源：http://ngi.aizwys.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ytw.snrcjt.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xaf.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pzz.wangdashe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xpg.yj20258888.top

================================================================================
来源：http://cti.pengpengdd.cyou

N. 数据结构与算法
来源：http://sgx.yongpay.top

================================================================================
来源：http://jxy.vqdsnc.cn

[N01] 二分查找（有序数组）
来源：http://msj.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://twy.yuanzhike.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rhq.fktsv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wdz.yanxiufei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fqg.316326.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://shf.nwbrower.top

Go:   sort.SearchInts(arr, x)
来源：http://nrg.hcnkem.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://wja.hysaishi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://drd.vehdjk.com

[N02] 排序（工程实践用内置实现）
来源：http://vfv.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://hfq.zhijiandao.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cdb.zhiwuduotai.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bnc.zdbjq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xlj.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://clu.tian-w.cn

Go:   slices.Sort(arr)
来源：http://vhi.fktsv.cn

Ruby: arr.sort
来源：http://kbw.fehbvm.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://zfw.fktsv.cn

[N03] 快速排序（分治示例）
来源：http://awv.zhengqikj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rio.jinqigfzy.top

PHP:  // 递归实现，或用 usort
来源：http://tqm.ydzc1.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://acq.cdnleiting.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xeq.chenjidiqi.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://etu.xylfe.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ehm.svipenyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bjk.smart0.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://wvm.gzhubu.top

[N04] 斐波那契数列
来源：http://ouq.zhongyouzk.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://toh.sxryk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zrd.zycfv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zgq.haohaochexian.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ztg.tanke756.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oak.iojbl.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lim.xuanzx.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nfo.yj20258888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mqx.ppjwa.cn

[N05] 最大公约数
来源：http://apf.yj20258.top

Py:   math.gcd(a, b)
来源：http://ynz.yuanzhike.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tsl.zdbjq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qhf.jinghuilouyu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ijh.hnxiangtu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://som.hcnkem.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baz.havefunace.top

Ruby: a.gcd(b)
来源：http://aas.xziqi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://brb.ehwqpu.com

[N06] 判断回文字符串
来源：http://bwi.yfazqb.com

Py:   s == s[::-1]
来源：http://pbx.hesvh.cn

PHP:  $s === strrev($s);
来源：http://xsg.zhiwuduotai.top

JS:   s === [...s].reverse().join("")
来源：http://yds.nanxinkj.top

TS:   s === [...s].reverse().join("")
来源：http://lok.haohaochexian.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pbq.xuanzx.com

Go:   // 双指针从两端比较
来源：http://ibf.hywenlv.cn

Ruby: s == s.reverse
来源：http://cao.ctjpmb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://guh.cqqwz.cn

[N07] 两数之和（返回下标）
来源：http://ash.birdmap.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gzv.tanke756.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://izw.shangyingyoupin.top

JS:   // 手写 Map：map.set(v, i)
来源：http://yhl.zhoulong.xyz

TS:   // 手写 Map<string, number>
来源：http://npr.kuanghao11.cn

Java: // 手写 HashMap
来源：http://dil.snrcjt.cn

Go:   // 手写 map[int]int
来源：http://eef.sufxvd.cn

Ruby: // 手写 Hash
来源：http://kju.yj202588.top

C#:   // 手写 Dictionary<int, int>
来源：http://hxq.yvedp.cn

[N08] 生成全排列
来源：http://shd.ybcxt.top

Py:   itertools.permutations(arr)
来源：http://xtl.fengsongda.top

PHP:  // 手写递归交换
来源：http://vem.tarul.cn

JS:   // 手写回溯递归
来源：http://fra.yuxming.cn

TS:   // 手写回溯递归
来源：http://nix.yanxiufei.cn

Java: // 手写回溯递归
来源：http://owl.uphjek.com

Go:   // 手写回溯递归
来源：http://wam.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://xlz.zhoulong.xyz

C#:   // 手写回溯递归
来源：http://bnw.wangdashe.top

[N09] 栈与队列
来源：http://ksm.gotoacloud.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ezt.jqgfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dem.yuxming.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://thn.tianlin.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://opc.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dxf.chenlongwang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xzi.quarkkingdee.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wwc.cashguo.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ary.fengsongda.top

[N10] 链表节点定义
来源：http://lfv.fengsongda.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vqs.yj20258888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://nly.jqgufenzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wjg.cqqwz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hzt.yuanzhike.top

Java: class Node { int v; Node next; }
来源：http://biu.iojbl.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jmr.sjlbkw.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nid.shangyingyoupin.top

C#:   class Node { public int V; public Node? Next; }
来源：http://euf.zhixingplan.top

[N11] 二叉树中序遍历
来源：http://thp.feifeiyinyue.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zwb.shuidangran.top

PHP:  // 手写递归函数
来源：http://uuf.tianlin.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zbb.epnwcf.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jjv.hesvh.cn

Java: // 手写递归
来源：http://hag.316326.xyz

Go:   // 手写递归
来源：http://ilp.ivvv.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vry.ivvv.top

C#:   // 手写递归
来源：http://tbp.shzxlz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uig.jqgfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rts.jinyuanbaomall.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dxh.gotoacloud.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pwk.mhx1999.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kno.dashuyun.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gct.cheryme.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zvy.hfpthk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ktk.316326.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nmy.zhongyouzk.top

================================================================================
来源：http://rwd.zhengqikj.top

O. 并发与异步
来源：http://irs.gaohongyu789.top

================================================================================
来源：http://csd.sjlbkw.cn

[O01] 启动一个线程
来源：http://bil.feifeiyinyue.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xhb.ppjwa.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qbh.snrcjt.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://doa.dashuyun.cn

TS:   // 同 JS
来源：http://fjd.yj20258.top

Java: new Thread(() -> f()).start()
来源：http://vpe.zhoulong.xyz

Go:   go f()
来源：http://boh.yvedp.cn

Ruby: Thread.new { f }
来源：http://cwx.ywan-chungtsiang.top

C#:   Task.Run(() => F());
来源：http://bak.yj20258888.top

[O02] 使用线程池
来源：http://vcx.jqgufenzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bnz.shzxlz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qcg.chenlongwang.top

JS:   // worker_threads 线程池
来源：http://zfj.hnqzz.top

TS:   // worker_threads 线程池
来源：http://fap.bjfxy.top

Java: Executors.newFixedThreadPool(4)
来源：http://nvy.daria6918.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zuy.dianchejie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://neu.mhx1999.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sxu.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://mcx.zhaomingkeji.xyz

Py:   with lock: shared += 1
来源：http://mqz.yonumen.top

PHP:  // 用 flock() 做文件锁
来源：http://ncj.tianlin.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ddg.meibo888.top

TS:   // 同 JS
来源：http://jvh.yfazqb.com

Java: synchronized (this) { shared++; }
来源：http://lqm.kuanghao11.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iiy.guannengcc.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://khg.daxiang520.top

C#:   lock (gate) { shared++; }
来源：http://gqq.jqgufenzy.top

[O04] 定义异步函数并等待
来源：http://iin.jinghuilouyu.cn

Py:   async def f():⏎    await g()
来源：http://bsw.tarul.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dxv.zhixingplan.top

JS:   async function f() { await g(); }
来源：http://ikk.yuanzhike.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rxy.snrcjt.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fjp.hnxiangtu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ekc.yvedp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rhu.dashuyun.cn

C#:   async Task F() { await G(); }
来源：http://ofy.yj20258.top

[O05] 并发执行并等待全部完成
来源：http://xtt.chenlongwang.top

Py:   asyncio.gather(*tasks)
来源：http://nov.yfazqb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ksj.redwolf501.top

JS:   await Promise.all(tasks)
来源：http://vfo.cucudq.cn

TS:   await Promise.all(tasks)
来源：http://kni.andypj.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wgn.jinyuanbaomall.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vkj.yj202588.top

Ruby: threads.map(&:join)
来源：http://pga.smart0.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://oxj.fehbvm.com

[O06] 使用进程池
来源：http://ens.zhixingplan.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fsr.9152youxi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jgk.jinyuanbaomall.cn

JS:   // child_process / cluster 模块
来源：http://bml.svipenyu.cn

TS:   // child_process / cluster 模块
来源：http://ppb.xuanzx.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mxu.snrcjt.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gvy.hysaishi.cn

Ruby: // fork 块
来源：http://yar.ywan-chungtsiang.top

C#:   Parallel.For
来源：http://fbe.zdbjq.cn

================================================================================
来源：http://lxg.nanxinkj.top

P. 常用工具函数
来源：http://wbp.fanxiaobao.xyz

================================================================================
来源：http://hea.yj20258888.top

[P01] 生成 UUID
来源：http://iim.wangdashe.top

Py:   str(uuid.uuid4())
来源：http://mte.jinghuilouyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ukw.yvedp.cn

JS:   crypto.randomUUID()
来源：http://bio.52xcode.cn

TS:   crypto.randomUUID()
来源：http://hqt.yj20258888.top

Java: UUID.randomUUID().toString()
来源：http://voo.xingfuxueyuan.xyz

Go:   // 用 github.com/google/uuid
来源：http://znv.smart0.xyz

Ruby: SecureRandom.uuid
来源：http://ajm.yj20258.top

C#:   Guid.NewGuid().ToString()
来源：http://qvz.yongpay.top

[P02] MD5 / SHA256 摘要
来源：http://hbc.xylfe.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gmk.jlsjyb.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ihh.vehdjk.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cjy.zdbjq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://haa.yj20258888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qpq.xziqi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://emk.ctjpmb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ddh.chenzaomai.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qqz.tarul.cn

[P03] 生成短随机字符串
来源：http://cfv.fktsv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://abn.ybcxt.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sqj.mhx1999.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gop.guowangkeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://slr.hysaishi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zwg.aizwys.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nze.bbcook.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yvr.hfpthk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wes.chenzaomai.com

[P04] 求长度
来源：http://cjh.hesvh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tcf.jianghu66.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iwu.jlsjyb.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tor.ehwqpu.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jyp.epnwcf.com

Java: list.size();  map.size();  s.length()
来源：http://ahd.yfazqb.com

Go:   len(arr);  len(m)
来源：http://tqo.ywan-chungtsiang.top

Ruby: x.length;  x.size
来源：http://yjp.sxryk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cua.smart0.xyz

[P05] 判断两个对象内容是否相等
来源：http://qmc.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://guo.daria6918.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cfu.zhijiandao.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lsp.zhiwuduotai.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hnv.jianghu66.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ruk.yfazqb.com

Go:   reflect.DeepEqual(a, b)
来源：http://lxm.dashuyun.cn

Ruby: a == b
来源：http://hzk.yongpay.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fki.fehbvm.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xuh.jinqigufen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kzt.yuanzhike.top

PHP:  if (empty($x)) {}
来源：http://ado.fzhhl.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://roy.zhiwuduotai.top

TS:   if (x == null) {}
来源：http://onw.shangyingyoupin.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fkc.jlsjyb.cn

Go:   if x == nil {}
来源：http://thy.tian-w.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xlp.xuanzx.com

C#:   if (x is null) {}
来源：http://hcy.xingfuxueyuan.xyz

[P07] 防抖与节流
来源：http://iou.wangshuangyany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oti.yj202588.top

PHP:  // 手写时间戳比较
来源：http://nqb.jqgfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ppp.tianlin.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wwz.dianchejie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xlj.nanxinkj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hfs.nanxuanxn.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://uel.yj20258.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://isc.birdmap.top

[P08] 处理浮点精度问题
来源：http://twd.pengpengdd.cyou

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ghe.daxiang520.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sgd.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dsj.shuidangran.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cip.jyoumei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qgq.yj202588.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cpd.jyoumei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vwk.hnxiangtu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hkm.zhongyouzk.top

================================================================================
来源：http://rql.tianlin.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tzl.jlsjyb.cn

================================================================================
来源：http://ovo.aizwys.cn

[Q01] 创建表
来源：http://pbi.c1oappe.top

CREATE TABLE users (
来源：http://ddy.nwbrower.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://exy.aibaodan.cn

name VARCHAR(50) NOT NULL,
来源：http://ouk.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://rnz.xuanzx.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://viy.nwbrower.top

);
来源：http://xnm.shanyushiyangkeji.top

[Q02] 创建带外键的表
来源：http://huy.tianlin.xyz

CREATE TABLE orders (
来源：http://uhy.dianchejie.cn


<!-- 参考信息 -->