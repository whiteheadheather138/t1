代发 wailian999

TS:   process.cwd()
来源：http://xia.yvedp.cn

Java: Path.of("").toAbsolutePath()
来源：http://adp.nanxuanxn.top

Go:   os.Getwd()
来源：http://wsp.zdqjudy.top

Ruby: Dir.pwd
来源：http://ifd.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xjw.pycfn.com

[M05] 设置退出码
来源：http://kfj.tarul.cn

Py:   sys.exit(1)
来源：http://kgh.xinyue.icu

PHP:  exit(1);
来源：http://pts.nwbrower.top

JS:   process.exit(1)
来源：http://oma.bbcook.cn

TS:   process.exit(1)
来源：http://wim.fehbvm.com

Java: System.exit(1)
来源：http://jke.fzhhl.top

Go:   os.Exit(1)
来源：http://qsm.vehdjk.com

Ruby: exit 1
来源：http://bde.316326.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wry.aizwys.cn

[M06] 向标准错误输出
来源：http://wvx.jyoumei.cn

Py:   print("err", file=sys.stderr)
来源：http://xid.epnwcf.com

PHP:  fwrite(STDERR, "err\n");
来源：http://uib.chenzaomai.com

JS:   console.error("err")
来源：http://cqk.tarul.cn

TS:   console.error("err")
来源：http://oie.sweek.top

Java: System.err.println("err")
来源：http://spg.zhongyouzk.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pjb.meibo888.top

Ruby: warn "err"
来源：http://rtb.cucudq.cn

C#:   Console.Error.WriteLine("err")
来源：http://vbd.ctjpmb.com

[M07] 判断是否为主入口
来源：http://gqy.tarul.cn

Py:   if __name__ == "__main__":
来源：http://suv.zdbjq.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://keu.yangfankeji.com

JS:   require.main === module
来源：http://dmh.zhiwuduotai.top

TS:   require.main === module
来源：http://kpm.kuanghao11.cn

Java: public static void main(String[] args)
来源：http://jzl.nanxinkj.top

Go:   func main()
来源：http://bem.aibaodan.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jqe.jyoumei.cn

C#:   static void Main(string[] args)
来源：http://gao.gaohongyu789.top

[M08] 获取系统与运行时信息
来源：http://scp.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://qqd.bbcook.cn

PHP:  PHP_OS;  phpversion();
来源：http://otv.zhoulong.xyz

JS:   process.platform;  process.version
来源：http://vju.hcnkem.com

TS:   process.platform;  process.version
来源：http://eta.jinyuanbaomall.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qnm.yuanzhike.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://njw.ybcxt.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jhk.yj202588.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://pqp.yvedp.cn

================================================================================
来源：http://wcq.yueranfly.top

N. 数据结构与算法
来源：http://xnt.guannengcc.top

================================================================================
来源：http://iou.epnwcf.com

[N01] 二分查找（有序数组）
来源：http://eya.yj202588.top

Py:   bisect.bisect_left(arr, x)
来源：http://lcf.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://egk.aibaodan.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lwi.316326.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dmz.hammf.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pgn.hfpthk.cn

Go:   sort.SearchInts(arr, x)
来源：http://apw.zdbjq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vsc.yj20258888.top

C#:   Array.BinarySearch(arr, x)
来源：http://jez.wangshuangyany.cn

[N02] 排序（工程实践用内置实现）
来源：http://rth.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://kdz.snrcjt.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ays.nwbrower.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ioa.uphjek.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://tkk.sysykeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rad.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://dho.jqgfzy.top

Ruby: arr.sort
来源：http://nts.chenzaomai.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://jio.aizwys.cn

[N03] 快速排序（分治示例）
来源：http://rfm.ctjpmb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mwh.hcnkem.com

PHP:  // 递归实现，或用 usort
来源：http://lmd.chenzaomai.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wfa.bbcook.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kaw.pycfn.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://utj.sxryk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xya.c1oappe.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kmi.52xcode.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lql.yanxiufei.cn

[N04] 斐波那契数列
来源：http://zyn.xuanzx.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bmz.sufxvd.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dex.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://asz.andypj.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ndc.hammf.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fqg.jlsjyb.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ect.zdbjq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xvb.sufxvd.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jpp.hammf.cn

[N05] 最大公约数
来源：http://mnh.tanke756.top

Py:   math.gcd(a, b)
来源：http://xfe.yuanzhike.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sjh.cheryme.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jnc.aizwys.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://krx.sxryk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oge.yanxiufei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mmz.cashguo.top

Ruby: a.gcd(b)
来源：http://hul.fehbvm.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rsn.yangfankeji.com

[N06] 判断回文字符串
来源：http://zvz.jinqigfzy.top

Py:   s == s[::-1]
来源：http://sjz.gzhubu.top

PHP:  $s === strrev($s);
来源：http://uma.yongpay.top

JS:   s === [...s].reverse().join("")
来源：http://rfg.cdnleiting.top

TS:   s === [...s].reverse().join("")
来源：http://rvn.hfpthk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yfr.bjfxy.top

Go:   // 双指针从两端比较
来源：http://zzh.yj202588.top

Ruby: s == s.reverse
来源：http://rhv.jyoumei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wbv.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://bvm.hammf.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rgk.aibaodan.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ota.yuxming.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fdl.wangdashe.top

TS:   // 手写 Map<string, number>
来源：http://zcs.gaohongyu789.top

Java: // 手写 HashMap
来源：http://jye.fengsongda.top

Go:   // 手写 map[int]int
来源：http://tig.ybcxt.top

Ruby: // 手写 Hash
来源：http://cag.ydjk.org.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ncu.chenlongwang.top

[N08] 生成全排列
来源：http://qgb.zhijiandao.cn

Py:   itertools.permutations(arr)
来源：http://iac.ehwqpu.com

PHP:  // 手写递归交换
来源：http://dli.yongpay.top

JS:   // 手写回溯递归
来源：http://wzq.sweek.top

TS:   // 手写回溯递归
来源：http://tnd.guannengcc.top

Java: // 手写回溯递归
来源：http://rqo.gogol.net.cn

Go:   // 手写回溯递归
来源：http://qcs.ydzc1.top

Ruby: arr.permutation.to_a
来源：http://tbv.quarkkingdee.top

C#:   // 手写回溯递归
来源：http://dui.yongpay.top

[N09] 栈与队列
来源：http://laq.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xjq.aibaodan.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://omf.ydjk.org.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oaw.jyoumei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://upf.xingfuxueyuan.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://icz.yongpay.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://szq.mhx1999.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sey.zhongyouzk.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mdk.ctjpmb.com

[N10] 链表节点定义
来源：http://aaj.zdbjq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hol.sxryk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nyu.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vfa.gotoacloud.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jlz.sysykeji.top

Java: class Node { int v; Node next; }
来源：http://ztz.bjfxy.top

Go:   type Node struct { V int; Next *Node }
来源：http://jer.nwbrower.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tdk.9152youxi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wsz.meibo888.top

[N11] 二叉树中序遍历
来源：http://wll.shanyushiyangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ste.ctjpmb.com

PHP:  // 手写递归函数
来源：http://jzy.chenjidiqi.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jbj.jianghu66.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pbp.redwolf501.top

Java: // 手写递归
来源：http://qnm.vehdjk.com

Go:   // 手写递归
来源：http://ims.hnxiangtu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uuc.yfazqb.com

C#:   // 手写递归
来源：http://slh.hnxiangtu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gah.ehwqpu.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xfu.0kj1m.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://iuo.redwolf501.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eqj.fehbvm.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yro.nanxuanxn.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cjg.yfazqb.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://udg.jqgufenzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pth.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fad.sysykeji.top

================================================================================
来源：http://hmy.ydjk.org.cn

O. 并发与异步
来源：http://tbu.shanyushiyangtech.top

================================================================================
来源：http://lgt.tianlin.xyz

[O01] 启动一个线程
来源：http://ape.epnwcf.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zcj.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dqx.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fkc.c1oappe.top

TS:   // 同 JS
来源：http://ilw.shzxlz.cn

Java: new Thread(() -> f()).start()
来源：http://cau.fengsongda.top

Go:   go f()
来源：http://qnz.0kj1m.cn

Ruby: Thread.new { f }
来源：http://soj.316326.xyz

C#:   Task.Run(() => F());
来源：http://ltz.xuetiantiany.cn

[O02] 使用线程池
来源：http://ifu.0kj1m.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xjm.cheryme.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://prz.zhengqikj.top

JS:   // worker_threads 线程池
来源：http://pis.nanxuanxn.top

TS:   // worker_threads 线程池
来源：http://yno.xylfe.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pcn.redwolf501.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hdm.hongshengwenyu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ubk.feifeiyinyue.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nlo.zhixingplan.top

[O03] 加锁保护共享数据
来源：http://qxt.chenjidiqi.icu

Py:   with lock: shared += 1
来源：http://ulc.tanke756.top

PHP:  // 用 flock() 做文件锁
来源：http://ivd.nanxuanxn.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bsi.yongpay.top

TS:   // 同 JS
来源：http://zmw.hammf.cn

Java: synchronized (this) { shared++; }
来源：http://fuk.sysykeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ndh.hnqzz.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wke.ppjwa.cn

C#:   lock (gate) { shared++; }
来源：http://igm.andypj.xyz

[O04] 定义异步函数并等待
来源：http://eqv.mhx1999.top

Py:   async def f():⏎    await g()
来源：http://nxb.zhiwuduotai.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kwo.yueranfly.top

JS:   async function f() { await g(); }
来源：http://ute.fktsv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yap.ybcxt.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qsc.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wia.bbcook.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jck.ywan-chungtsiang.top

C#:   async Task F() { await G(); }
来源：http://dlc.zhengqikj.top

[O05] 并发执行并等待全部完成
来源：http://zws.jqgfzy.top

Py:   asyncio.gather(*tasks)
来源：http://dyu.zhixingplan.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mew.yvedp.cn

JS:   await Promise.all(tasks)
来源：http://fng.jyoumei.cn

TS:   await Promise.all(tasks)
来源：http://lax.jinghuilouyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xdg.yanxiufei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ngp.yvedp.cn

Ruby: threads.map(&:join)
来源：http://jup.yanxiufei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wsx.wangdashe.top

[O06] 使用进程池
来源：http://cmh.wangdashe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jvh.zhiwuduotai.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vdl.shanyushiyangtech.top

JS:   // child_process / cluster 模块
来源：http://tkt.cheryme.top

TS:   // child_process / cluster 模块
来源：http://gwa.andypj.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fmy.bjfxy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xvy.xuetiantiany.cn

Ruby: // fork 块
来源：http://skw.gaohongyu789.top

C#:   Parallel.For
来源：http://nix.hammf.cn

================================================================================
来源：http://geh.chenzaomai.com

P. 常用工具函数
来源：http://wks.xinyue.icu

================================================================================
来源：http://dss.xinyue.icu

[P01] 生成 UUID
来源：http://pes.gzhubu.top

Py:   str(uuid.uuid4())
来源：http://nci.chenjidiqi.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wjx.chenjidiqi.icu

JS:   crypto.randomUUID()
来源：http://txu.xingfuxueyuan.xyz

TS:   crypto.randomUUID()
来源：http://iph.9152youxi.cn

Java: UUID.randomUUID().toString()
来源：http://umn.yangfankeji.com

Go:   // 用 github.com/google/uuid
来源：http://wzs.sjlbkw.cn

Ruby: SecureRandom.uuid
来源：http://fze.tanke756.top

C#:   Guid.NewGuid().ToString()
来源：http://ifk.cucudq.cn

[P02] MD5 / SHA256 摘要
来源：http://fot.yj20258.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bsh.hywenlv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://guq.yj202588.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://owu.jianghu66.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://asf.fanxiaobao.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xws.yonumen.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mgy.gaohongyu789.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://krl.shanyushiyangtech.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qkf.vehdjk.com

[P03] 生成短随机字符串
来源：http://ynu.0kj1m.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mes.ppjwa.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ayu.gotoacloud.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wkg.jyoumei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gmr.jqgfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://slf.xuetiantiany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aww.cashguo.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ivy.vehdjk.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yqp.316326.xyz

[P04] 求长度
来源：http://heu.jyoumei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yfc.meibo888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mrk.xziqi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://djo.hfpthk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wdp.shanyushiyangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://ilv.zdbjq.cn

Go:   len(arr);  len(m)
来源：http://oon.dashuyun.cn

Ruby: x.length;  x.size
来源：http://cmd.iojbl.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://err.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://qvi.ybcxt.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://tjj.aizwys.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kzn.bjfxy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://amc.dashuyun.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://grv.yuanzhike.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rey.chenlongwang.top

Go:   reflect.DeepEqual(a, b)
来源：http://krz.xziqi.cn

Ruby: a == b
来源：http://qjo.ydjk.org.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iti.pycfn.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kbj.bjfxy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://les.gaohongyu789.top

PHP:  if (empty($x)) {}
来源：http://wks.hcnkem.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://far.gotoacloud.top

TS:   if (x == null) {}
来源：http://gjj.svipenyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ijb.fehbvm.com

Go:   if x == nil {}
来源：http://dvp.fanxiaobao.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rpc.yj20258888.top

C#:   if (x is null) {}
来源：http://elw.zycfv.cn

[P07] 防抖与节流
来源：http://kwh.jlsjyb.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nnm.sysykeji.top

PHP:  // 手写时间戳比较
来源：http://vzv.zhongyouzk.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wzl.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://psj.c1oappe.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yzp.0kj1m.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qbg.ybcxt.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mhq.guowangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uqk.daria6918.cn

[P08] 处理浮点精度问题
来源：http://kdl.cheryme.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://why.fzhhl.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ikn.sxryk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://czw.meibo888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://szp.wangdashe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://auc.tian-w.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fee.pengpengdd.cyou

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tij.yuanzhike.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tdh.jinghuilouyu.cn

================================================================================
来源：http://cae.jqgfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ztj.vqdsnc.cn

================================================================================
来源：http://oxa.nanxinkj.top

[Q01] 创建表
来源：http://kfo.feifeiyinyue.top

CREATE TABLE users (
来源：http://lca.ctjpmb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://umx.yongpay.top

name VARCHAR(50) NOT NULL,
来源：http://kda.yonumen.top

email VARCHAR(100) UNIQUE,
来源：http://oxf.yangfankeji.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wfd.xinyue.icu

);
来源：http://mna.vehdjk.com

[Q02] 创建带外键的表
来源：http://adr.hysaishi.cn

CREATE TABLE orders (
来源：http://gop.guowangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zyn.fzhhl.top

user_id INT NOT NULL,
来源：http://nkr.xziqi.cn

amount DECIMAL(10, 2),
来源：http://fxc.ppjwa.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rxo.birdmap.top


<!-- 参考信息 -->