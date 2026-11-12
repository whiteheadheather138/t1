代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://krs.jlsjyb.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tsd.ivvv.top

Ruby: system("ls -l");  `ls -l`
来源：http://oto.gzhubu.top

C#:   Process.Start("ls", "-l");
来源：http://lku.daria6918.cn

[M04] 获取当前工作目录
来源：http://elo.gaohongyu789.top

Py:   os.getcwd()
来源：http://azn.quarkkingdee.top

PHP:  getcwd();
来源：http://jtt.tanke756.top

JS:   process.cwd()
来源：http://wor.shzxlz.cn

TS:   process.cwd()
来源：http://ssn.yangfankeji.com

Java: Path.of("").toAbsolutePath()
来源：http://skn.kuanghao11.cn

Go:   os.Getwd()
来源：http://wif.gotoacloud.top

Ruby: Dir.pwd
来源：http://hug.zhoulong.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://jwr.sysykeji.top

[M05] 设置退出码
来源：http://cir.jiagoushi.top

Py:   sys.exit(1)
来源：http://azt.yj20258888.top

PHP:  exit(1);
来源：http://xkq.chenlongwang.top

JS:   process.exit(1)
来源：http://gvt.fanxiaobao.xyz

TS:   process.exit(1)
来源：http://nkv.zdqjudy.top

Java: System.exit(1)
来源：http://cml.daria6918.cn

Go:   os.Exit(1)
来源：http://rhb.shangyingyoupin.top

Ruby: exit 1
来源：http://oqa.yvedp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cth.birdmap.top

[M06] 向标准错误输出
来源：http://edy.zhaomingkeji.xyz

Py:   print("err", file=sys.stderr)
来源：http://dqd.gotoacloud.top

PHP:  fwrite(STDERR, "err\n");
来源：http://umo.uphjek.com

JS:   console.error("err")
来源：http://qgs.cashguo.top

TS:   console.error("err")
来源：http://zhr.ybcxt.top

Java: System.err.println("err")
来源：http://tgt.yonumen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yxm.yj20258888.top

Ruby: warn "err"
来源：http://gof.chenzaomai.com

C#:   Console.Error.WriteLine("err")
来源：http://kwj.ivvv.top

[M07] 判断是否为主入口
来源：http://pmj.quarkkingdee.top

Py:   if __name__ == "__main__":
来源：http://iot.hesvh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mvc.nanxuanxn.top

JS:   require.main === module
来源：http://llz.shuidangran.top

TS:   require.main === module
来源：http://ecr.9152youxi.cn

Java: public static void main(String[] args)
来源：http://tga.yonumen.top

Go:   func main()
来源：http://mhm.zhijiandao.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ndz.yuxming.cn

C#:   static void Main(string[] args)
来源：http://bsp.hammf.cn

[M08] 获取系统与运行时信息
来源：http://smw.uphjek.com

Py:   platform.system();  platform.python_version()
来源：http://gyv.jqgufenzy.top

PHP:  PHP_OS;  phpversion();
来源：http://qpo.hcnkem.com

JS:   process.platform;  process.version
来源：http://rzg.hammf.cn

TS:   process.platform;  process.version
来源：http://jxz.shuidangran.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://eob.bbcook.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cfw.ydzc1.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://edh.ppjwa.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bca.fktsv.cn

================================================================================
来源：http://sev.cashguo.top

N. 数据结构与算法
来源：http://evc.xuetiantiany.cn

================================================================================
来源：http://jph.yj20258.top

[N01] 二分查找（有序数组）
来源：http://cww.pengpengdd.cyou

Py:   bisect.bisect_left(arr, x)
来源：http://wvs.bjfxy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pqp.yuxming.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yxx.yvedp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zon.jqgufenzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://rbm.fzhhl.top

Go:   sort.SearchInts(arr, x)
来源：http://ucc.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bzq.tanke756.top

C#:   Array.BinarySearch(arr, x)
来源：http://dhp.sxryk.cn

[N02] 排序（工程实践用内置实现）
来源：http://dev.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://lxh.chenlongwang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wyu.chenjidiqi.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://fob.ywan-chungtsiang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fzw.mhx1999.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pyo.yanxiufei.cn

Go:   slices.Sort(arr)
来源：http://nct.ivvv.top

Ruby: arr.sort
来源：http://eyx.zhengqikj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qyk.jinqigfzy.top

[N03] 快速排序（分治示例）
来源：http://fzf.yongpay.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://izq.nanxinkj.top

PHP:  // 递归实现，或用 usort
来源：http://dgv.guannengcc.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lrk.xingfuxueyuan.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uua.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vnp.birdmap.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zbk.tian-w.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ckd.chenzaomai.com

C#:   // 手写递归，或 Array.Sort
来源：http://yae.wangdashe.top

[N04] 斐波那契数列
来源：http://iyv.shangyingyoupin.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dyt.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jzk.pengpengdd.cyou

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tvh.nanxuanxn.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bea.aibaodan.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zum.hcnkem.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hdt.xinyue.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pwz.ctjpmb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://etm.pengpengdd.cyou

[N05] 最大公约数
来源：http://vnn.ywan-chungtsiang.top

Py:   math.gcd(a, b)
来源：http://rlw.daria6918.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://itu.haohaochexian.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oqy.snrcjt.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sxm.hammf.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lub.yvedp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pvp.ppjwa.cn

Ruby: a.gcd(b)
来源：http://jba.redwolf501.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dfj.tarul.cn

[N06] 判断回文字符串
来源：http://fzd.fktsv.cn

Py:   s == s[::-1]
来源：http://mqc.andypj.xyz

PHP:  $s === strrev($s);
来源：http://wkc.yuxming.cn

JS:   s === [...s].reverse().join("")
来源：http://kom.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://fho.jinqigufen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qgy.jlsjyb.cn

Go:   // 双指针从两端比较
来源：http://oad.wangdashe.top

Ruby: s == s.reverse
来源：http://upi.nanxuanxn.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://emp.sxryk.cn

[N07] 两数之和（返回下标）
来源：http://syz.yfazqb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ewh.ehwqpu.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wgi.shuidangran.top

JS:   // 手写 Map：map.set(v, i)
来源：http://cix.bbcook.cn

TS:   // 手写 Map<string, number>
来源：http://psi.ctjpmb.com

Java: // 手写 HashMap
来源：http://qbk.yuxming.cn

Go:   // 手写 map[int]int
来源：http://jsh.svipenyu.cn

Ruby: // 手写 Hash
来源：http://xyg.c1oappe.top

C#:   // 手写 Dictionary<int, int>
来源：http://ddt.guannengcc.top

[N08] 生成全排列
来源：http://rvo.gzhubu.top

Py:   itertools.permutations(arr)
来源：http://wht.meibo888.top

PHP:  // 手写递归交换
来源：http://tex.zdbjq.cn

JS:   // 手写回溯递归
来源：http://rde.iojbl.cn

TS:   // 手写回溯递归
来源：http://wve.jinyuanbaomall.cn

Java: // 手写回溯递归
来源：http://kbg.hysaishi.cn

Go:   // 手写回溯递归
来源：http://aey.yuanzhike.top

Ruby: arr.permutation.to_a
来源：http://lha.fzhhl.top

C#:   // 手写回溯递归
来源：http://phf.jyoumei.cn

[N09] 栈与队列
来源：http://hkn.shanyushiyangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ndv.0kj1m.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ynp.yangfankeji.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pam.zdbjq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mzq.fanxiaobao.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pcq.yanxiufei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://whc.tanke756.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cgs.yueranfly.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://whr.fktsv.cn

[N10] 链表节点定义
来源：http://nas.fanxiaobao.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nuy.uphjek.com

PHP:  class Node { public $v; public $next = null; }
来源：http://qcr.jinghuilouyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qgi.ctjpmb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ctv.xuanzx.com

Java: class Node { int v; Node next; }
来源：http://jix.zdqjudy.top

Go:   type Node struct { V int; Next *Node }
来源：http://wro.chenlongwang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://scp.shanyushiyangtech.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ejk.meibo888.top

[N11] 二叉树中序遍历
来源：http://xap.zdqjudy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lzd.hongshengwenyu.top

PHP:  // 手写递归函数
来源：http://ecr.shzxlz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wzz.xuetiantiany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pwy.sufxvd.cn

Java: // 手写递归
来源：http://wrx.zycfv.cn

Go:   // 手写递归
来源：http://nop.xziqi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rre.shzxlz.cn

C#:   // 手写递归
来源：http://dve.zhengqikj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vot.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wpe.guannengcc.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://crg.hnxiangtu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://joh.c1oappe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zwq.svipenyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xlh.zhoulong.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jia.wangshuangyany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gsh.shuidangran.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dgz.zhongyouzk.top

================================================================================
来源：http://qrn.hywenlv.cn

O. 并发与异步
来源：http://oxf.kuanghao11.cn

================================================================================
来源：http://gtd.hammf.cn

[O01] 启动一个线程
来源：http://txo.wangdashe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qln.zycfv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wcp.tarul.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gak.aizwys.cn

TS:   // 同 JS
来源：http://fsn.ppjwa.cn

Java: new Thread(() -> f()).start()
来源：http://gzr.guowangkeji.top

Go:   go f()
来源：http://dzh.yueranfly.top

Ruby: Thread.new { f }
来源：http://xhe.jqgufenzy.top

C#:   Task.Run(() => F());
来源：http://zii.jinqigufen.top

[O02] 使用线程池
来源：http://ypi.hcnkem.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ivs.zhoulong.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rpy.jlsjyb.cn

JS:   // worker_threads 线程池
来源：http://ovj.ctjpmb.com

TS:   // worker_threads 线程池
来源：http://uoc.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wzs.sufxvd.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://amu.ppjwa.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xjw.pengpengdd.cyou

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xeb.mhx1999.top

[O03] 加锁保护共享数据
来源：http://bvz.tarul.cn

Py:   with lock: shared += 1
来源：http://fos.yuanzhike.top

PHP:  // 用 flock() 做文件锁
来源：http://agf.hnqzz.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rso.sjlbkw.cn

TS:   // 同 JS
来源：http://jrl.yongpay.top

Java: synchronized (this) { shared++; }
来源：http://xqx.shzxlz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wub.birdmap.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hoc.cdnleiting.top

C#:   lock (gate) { shared++; }
来源：http://tby.wangshuangyany.cn

[O04] 定义异步函数并等待
来源：http://obe.fengsongda.top

Py:   async def f():⏎    await g()
来源：http://vxl.zhongyouzk.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iso.feifeiyinyue.top

JS:   async function f() { await g(); }
来源：http://wfy.zdbjq.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mla.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pnf.gzhubu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ipw.ivvv.top

Ruby: # 用 Fiber 或 async gem
来源：http://bgw.jinqigfzy.top

C#:   async Task F() { await G(); }
来源：http://ppj.nanxuanxn.top

[O05] 并发执行并等待全部完成
来源：http://euq.zdqjudy.top

Py:   asyncio.gather(*tasks)
来源：http://fqn.jinqigfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://afq.xylfe.cn

JS:   await Promise.all(tasks)
来源：http://fry.havefunace.top

TS:   await Promise.all(tasks)
来源：http://kky.kuanghao11.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ody.pengpengdd.cyou

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://das.zdbjq.cn

Ruby: threads.map(&:join)
来源：http://tyk.xziqi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://add.wangshuangyany.cn

[O06] 使用进程池
来源：http://uck.shangyingyoupin.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://who.cheryme.top

PHP:  // pcntl_fork 或多进程队列
来源：http://tqg.ywan-chungtsiang.top

JS:   // child_process / cluster 模块
来源：http://pqk.sweek.top

TS:   // child_process / cluster 模块
来源：http://btu.9152youxi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://afg.cdnleiting.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rtc.tianlin.xyz

Ruby: // fork 块
来源：http://ljc.gzhubu.top

C#:   Parallel.For
来源：http://gsv.yj20258888.top

================================================================================
来源：http://nwk.dashuyun.cn

P. 常用工具函数
来源：http://bhs.0kj1m.cn

================================================================================
来源：http://orc.316326.xyz

[P01] 生成 UUID
来源：http://fve.zhengqikj.top

Py:   str(uuid.uuid4())
来源：http://gec.shuidangran.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bqr.gogol.net.cn

JS:   crypto.randomUUID()
来源：http://bfw.hnqzz.top

TS:   crypto.randomUUID()
来源：http://rug.pycfn.com

Java: UUID.randomUUID().toString()
来源：http://bxa.xuetiantiany.cn

Go:   // 用 github.com/google/uuid
来源：http://mry.yueranfly.top

Ruby: SecureRandom.uuid
来源：http://qiv.smart0.xyz

C#:   Guid.NewGuid().ToString()
来源：http://dfj.hesvh.cn

[P02] MD5 / SHA256 摘要
来源：http://ajx.zhongyouzk.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lph.guannengcc.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lra.bjfxy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://twt.hesvh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://frz.meibo888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mhc.jinghuilouyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hfv.vqdsnc.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ltw.vehdjk.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aif.jlsjyb.cn

[P03] 生成短随机字符串
来源：http://cdw.tanke756.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ygs.hesvh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wqj.shangyingyoupin.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://epw.tanke756.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://klr.yj20258888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dyi.smart0.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hxe.c1oappe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://hid.xingfuxueyuan.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tdt.smart0.xyz

[P04] 求长度
来源：http://jhq.guannengcc.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jlc.yj20258.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bic.jinyuanbaomall.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dql.yfazqb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sbl.daxiang520.top

Java: list.size();  map.size();  s.length()
来源：http://ykw.gzhubu.top

Go:   len(arr);  len(m)
来源：http://bdv.uphjek.com

Ruby: x.length;  x.size
来源：http://qde.wangdashe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://cyq.tianlin.xyz

[P05] 判断两个对象内容是否相等
来源：http://iky.svipenyu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kcz.cashguo.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ubh.vehdjk.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cuy.ywan-chungtsiang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qwz.cqqwz.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://elw.yonumen.top

Go:   reflect.DeepEqual(a, b)
来源：http://jse.ivvv.top

Ruby: a == b
来源：http://vgh.fengsongda.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wxd.sufxvd.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wns.0kj1m.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dyk.pycfn.com

PHP:  if (empty($x)) {}
来源：http://cvz.mhx1999.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yhu.tian-w.cn

TS:   if (x == null) {}
来源：http://xbm.zhixingplan.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tgr.ydzc1.top

Go:   if x == nil {}
来源：http://rdf.haohaochexian.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cxu.hysaishi.cn

C#:   if (x is null) {}
来源：http://wqz.jinqigfzy.top

[P07] 防抖与节流
来源：http://fda.chenlongwang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kvl.pengpengdd.cyou

PHP:  // 手写时间戳比较
来源：http://nzk.yj202588.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://imp.shzxlz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://glw.zdqjudy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lje.kuanghao11.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://buy.9152youxi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qyw.kuanghao11.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wbw.52xcode.cn

[P08] 处理浮点精度问题
来源：http://bpd.yj20258888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uvq.zhixingplan.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ndk.aibaodan.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://npy.shanyushiyangtech.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vdk.fanxiaobao.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bkd.jqgufenzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ekx.jiagoushi.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://thp.aizwys.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bah.jyoumei.cn

================================================================================
来源：http://owa.nwbrower.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://emm.vqdsnc.cn

================================================================================
来源：http://acx.snrcjt.cn

[Q01] 创建表
来源：http://tge.tian-w.cn

CREATE TABLE users (
来源：http://dya.jlsjyb.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://crk.feifeiyinyue.top

name VARCHAR(50) NOT NULL,
来源：http://hxh.snrcjt.cn

email VARCHAR(100) UNIQUE,
来源：http://jhv.yuxming.cn


<!-- 参考信息 -->