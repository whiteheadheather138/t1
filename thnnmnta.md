代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://crc.9152youxi.cn

JS:   console.error("err")
来源：http://lvk.yj20258.top

TS:   console.error("err")
来源：http://von.yfazqb.com

Java: System.err.println("err")
来源：http://bat.cqqwz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://prw.vehdjk.com

Ruby: warn "err"
来源：http://adv.feifeiyinyue.top

C#:   Console.Error.WriteLine("err")
来源：http://kat.sysykeji.top

[M07] 判断是否为主入口
来源：http://wuy.xuetiantiany.cn

Py:   if __name__ == "__main__":
来源：http://tak.jinghuilouyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xiw.yuxming.cn

JS:   require.main === module
来源：http://fox.andypj.xyz

TS:   require.main === module
来源：http://wps.aibaodan.cn

Java: public static void main(String[] args)
来源：http://qeh.chenzaomai.com

Go:   func main()
来源：http://run.vqdsnc.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://atp.havefunace.top

C#:   static void Main(string[] args)
来源：http://ppk.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://jjv.fktsv.cn

Py:   platform.system();  platform.python_version()
来源：http://nmt.svipenyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://xfm.jinyuanbaomall.cn

JS:   process.platform;  process.version
来源：http://rse.guannengcc.top

TS:   process.platform;  process.version
来源：http://mjo.kuanghao11.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ivd.fehbvm.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://lyx.vehdjk.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gng.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jqb.bjfxy.top

================================================================================
来源：http://ljr.haohaochexian.top

N. 数据结构与算法
来源：http://kor.hnxiangtu.top

================================================================================
来源：http://apk.pengpengdd.cyou

[N01] 二分查找（有序数组）
来源：http://klw.sweek.top

Py:   bisect.bisect_left(arr, x)
来源：http://xiu.yanxiufei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nwx.xuetiantiany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xqc.zhixingplan.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nsv.tianlin.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://ovk.cheryme.top

Go:   sort.SearchInts(arr, x)
来源：http://mba.ehwqpu.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://gvw.ehwqpu.com

C#:   Array.BinarySearch(arr, x)
来源：http://xdh.ivvv.top

[N02] 排序（工程实践用内置实现）
来源：http://vrh.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://yrx.zhongyouzk.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oea.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ihe.yonumen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://bka.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vyo.yangfankeji.com

Go:   slices.Sort(arr)
来源：http://dwu.vqdsnc.cn

Ruby: arr.sort
来源：http://jud.c1oappe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://biv.haohaochexian.top

[N03] 快速排序（分治示例）
来源：http://luf.tian-w.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dso.daria6918.cn

PHP:  // 递归实现，或用 usort
来源：http://awr.kuanghao11.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uzl.nanxinkj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nki.birdmap.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zir.jinqigufen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ija.zhongyouzk.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://umv.cdnleiting.top

C#:   // 手写递归，或 Array.Sort
来源：http://itl.jinqigufen.top

[N04] 斐波那契数列
来源：http://uqo.jinqigufen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://obe.redwolf501.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xrj.ehwqpu.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aya.smart0.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://abq.gotoacloud.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://evg.yj202588.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://udr.zhaomingkeji.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fdy.dashuyun.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vpg.aizwys.cn

[N05] 最大公约数
来源：http://hvm.sjlbkw.cn

Py:   math.gcd(a, b)
来源：http://fys.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eog.ybcxt.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zbo.shanyushiyangtech.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vdp.hammf.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qal.birdmap.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fqb.tianlin.xyz

Ruby: a.gcd(b)
来源：http://uql.fehbvm.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://brt.zhaomingkeji.xyz

[N06] 判断回文字符串
来源：http://esh.gogol.net.cn

Py:   s == s[::-1]
来源：http://rwb.xinyue.icu

PHP:  $s === strrev($s);
来源：http://vim.dashuyun.cn

JS:   s === [...s].reverse().join("")
来源：http://kvl.zdbjq.cn

TS:   s === [...s].reverse().join("")
来源：http://zvr.bbcook.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gfp.ydjk.org.cn

Go:   // 双指针从两端比较
来源：http://sty.aibaodan.cn

Ruby: s == s.reverse
来源：http://lvy.jinqigfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gxp.sweek.top

[N07] 两数之和（返回下标）
来源：http://jdv.birdmap.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jkw.gzhubu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://orw.bbcook.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jco.hfpthk.cn

TS:   // 手写 Map<string, number>
来源：http://stb.0kj1m.cn

Java: // 手写 HashMap
来源：http://hoa.uphjek.com

Go:   // 手写 map[int]int
来源：http://voq.yueranfly.top

Ruby: // 手写 Hash
来源：http://drt.fanxiaobao.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://fgd.yuanzhike.top

[N08] 生成全排列
来源：http://tje.cheryme.top

Py:   itertools.permutations(arr)
来源：http://fcb.svipenyu.cn

PHP:  // 手写递归交换
来源：http://mwy.snrcjt.cn

JS:   // 手写回溯递归
来源：http://oyh.tianlin.xyz

TS:   // 手写回溯递归
来源：http://hfm.chenzaomai.com

Java: // 手写回溯递归
来源：http://knl.daxiang520.top

Go:   // 手写回溯递归
来源：http://rks.vehdjk.com

Ruby: arr.permutation.to_a
来源：http://exe.tian-w.cn

C#:   // 手写回溯递归
来源：http://mfg.wangshuangyany.cn

[N09] 栈与队列
来源：http://oho.pengpengdd.cyou

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yhm.ybcxt.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://prj.cashguo.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ntc.yuxming.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hzl.zdbjq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nxv.epnwcf.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vtg.yvedp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lsf.sjlbkw.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://evg.zhengqikj.top

[N10] 链表节点定义
来源：http://uor.jinghuilouyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qgy.xingfuxueyuan.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://nzg.gogol.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xjo.hcnkem.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fjj.uphjek.com

Java: class Node { int v; Node next; }
来源：http://vxo.hfpthk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cns.xuanzx.com

Ruby: Node = Struct.new(:v, :next)
来源：http://mve.hesvh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sds.yj20258888.top

[N11] 二叉树中序遍历
来源：http://awc.shzxlz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uns.gzhubu.top

PHP:  // 手写递归函数
来源：http://imh.jinghuilouyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ccq.shanyushiyangtech.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vto.tanke756.top

Java: // 手写递归
来源：http://buo.haohaochexian.top

Go:   // 手写递归
来源：http://efo.iojbl.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fjd.gzhubu.top

C#:   // 手写递归
来源：http://grr.tianlin.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://scg.hysaishi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qyg.aizwys.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://olp.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bll.0kj1m.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qaf.hammf.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://aoy.quarkkingdee.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sds.iojbl.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bnn.dashuyun.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kqe.zhiwuduotai.top

================================================================================
来源：http://gpu.tarul.cn

O. 并发与异步
来源：http://srp.smart0.xyz

================================================================================
来源：http://rwj.xziqi.cn

[O01] 启动一个线程
来源：http://tum.zdqjudy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fnw.kuanghao11.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jbj.nwbrower.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hym.xuetiantiany.cn

TS:   // 同 JS
来源：http://rre.sufxvd.cn

Java: new Thread(() -> f()).start()
来源：http://gxi.gaohongyu789.top

Go:   go f()
来源：http://usx.zdbjq.cn

Ruby: Thread.new { f }
来源：http://mou.quarkkingdee.top

C#:   Task.Run(() => F());
来源：http://knp.guowangkeji.top

[O02] 使用线程池
来源：http://qes.haohaochexian.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://koy.zhiwuduotai.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pqx.xingfuxueyuan.xyz

JS:   // worker_threads 线程池
来源：http://qdn.dashuyun.cn

TS:   // worker_threads 线程池
来源：http://zxb.zhoulong.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://xhz.zhiwuduotai.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kft.aizwys.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uhp.fehbvm.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cbk.xingfuxueyuan.xyz

[O03] 加锁保护共享数据
来源：http://ael.chenjidiqi.icu

Py:   with lock: shared += 1
来源：http://vhu.svipenyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://jfh.dashuyun.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pne.gzhubu.top

TS:   // 同 JS
来源：http://jxp.52xcode.cn

Java: synchronized (this) { shared++; }
来源：http://sar.yvedp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://shy.ydjk.org.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vwq.dashuyun.cn

C#:   lock (gate) { shared++; }
来源：http://fcv.xziqi.cn

[O04] 定义异步函数并等待
来源：http://czc.meibo888.top

Py:   async def f():⏎    await g()
来源：http://xzw.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bjh.xingfuxueyuan.xyz

JS:   async function f() { await g(); }
来源：http://ejb.zhiwuduotai.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vyd.xuetiantiany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kwj.9152youxi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lso.jyoumei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rmc.hnqzz.top

C#:   async Task F() { await G(); }
来源：http://qzw.gotoacloud.top

[O05] 并发执行并等待全部完成
来源：http://ttc.ywan-chungtsiang.top

Py:   asyncio.gather(*tasks)
来源：http://jum.yuxming.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kcp.nanxuanxn.top

JS:   await Promise.all(tasks)
来源：http://plw.cdnleiting.top

TS:   await Promise.all(tasks)
来源：http://eud.cucudq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://unt.jlsjyb.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lgg.9152youxi.cn

Ruby: threads.map(&:join)
来源：http://top.shuidangran.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hsl.shanyushiyangkeji.top

[O06] 使用进程池
来源：http://uyw.yfazqb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jlu.yangfankeji.com

PHP:  // pcntl_fork 或多进程队列
来源：http://gzm.yuanzhike.top

JS:   // child_process / cluster 模块
来源：http://svy.hesvh.cn

TS:   // child_process / cluster 模块
来源：http://vin.yonumen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fsw.wangshuangyany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cdi.fengsongda.top

Ruby: // fork 块
来源：http://gfe.hesvh.cn

C#:   Parallel.For
来源：http://khk.316326.xyz

================================================================================
来源：http://yzo.haohaochexian.top

P. 常用工具函数
来源：http://udx.zdbjq.cn

================================================================================
来源：http://wlo.gogol.net.cn

[P01] 生成 UUID
来源：http://jko.yonumen.top

Py:   str(uuid.uuid4())
来源：http://gdk.nanxuanxn.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pby.shanyushiyangtech.top

JS:   crypto.randomUUID()
来源：http://dwm.zhengqikj.top

TS:   crypto.randomUUID()
来源：http://kbx.fzhhl.top

Java: UUID.randomUUID().toString()
来源：http://iey.jiagoushi.top

Go:   // 用 github.com/google/uuid
来源：http://xfe.gogol.net.cn

Ruby: SecureRandom.uuid
来源：http://lvd.jiagoushi.top

C#:   Guid.NewGuid().ToString()
来源：http://zdy.tanke756.top

[P02] MD5 / SHA256 摘要
来源：http://gqw.zhoulong.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vsz.zhengqikj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://glg.daria6918.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xpa.jyoumei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kch.cheryme.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gkl.quarkkingdee.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lua.gotoacloud.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://thg.xziqi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gfj.birdmap.top

[P03] 生成短随机字符串
来源：http://qss.jinghuilouyu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pin.sufxvd.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ydz.jyoumei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://muh.ydjk.org.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qbf.cashguo.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mxq.daria6918.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fba.sxryk.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://iho.ybcxt.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eew.havefunace.top

[P04] 求长度
来源：http://mxi.9152youxi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://knr.sweek.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vwu.vehdjk.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zyc.fktsv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iok.ybcxt.top

Java: list.size();  map.size();  s.length()
来源：http://fpa.chenzaomai.com

Go:   len(arr);  len(m)
来源：http://gds.yongpay.top

Ruby: x.length;  x.size
来源：http://lej.svipenyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xhx.pengpengdd.cyou

[P05] 判断两个对象内容是否相等
来源：http://kji.snrcjt.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rvn.zdqjudy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xzn.ybcxt.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qaq.ybcxt.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cho.chenlongwang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://udc.feifeiyinyue.top

Go:   reflect.DeepEqual(a, b)
来源：http://voq.hnxiangtu.top

Ruby: a == b
来源：http://mqm.yfazqb.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qrq.yangfankeji.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bhn.tian-w.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://btw.ivvv.top

PHP:  if (empty($x)) {}
来源：http://jhl.hongshengwenyu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eoz.zhoulong.xyz

TS:   if (x == null) {}
来源：http://fan.uphjek.com

Java: if (x == null || x.isEmpty()) {}
来源：http://mux.yj20258.top

Go:   if x == nil {}
来源：http://fib.xziqi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qcs.shanyushiyangkeji.top

C#:   if (x is null) {}
来源：http://aqv.bbcook.cn

[P07] 防抖与节流
来源：http://bru.gotoacloud.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pbd.wangshuangyany.cn

PHP:  // 手写时间戳比较
来源：http://nsk.daria6918.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zut.hnqzz.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dbv.nanxuanxn.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vgm.gotoacloud.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eyq.zhaomingkeji.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://rgz.yonumen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uen.xingfuxueyuan.xyz

[P08] 处理浮点精度问题
来源：http://wxz.meibo888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ggv.jinghuilouyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ndd.yfazqb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sak.yj20258888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hce.cheryme.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ugu.yanxiufei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cqd.iojbl.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://npz.tianlin.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mwp.zdqjudy.top

================================================================================
来源：http://nbv.smart0.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ekz.chenlongwang.top

================================================================================
来源：http://rhs.cdnleiting.top

[Q01] 创建表
来源：http://qjj.52xcode.cn

CREATE TABLE users (
来源：http://sqh.zhaomingkeji.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ayi.pycfn.com

name VARCHAR(50) NOT NULL,
来源：http://vfw.vehdjk.com

email VARCHAR(100) UNIQUE,
来源：http://ztn.ehwqpu.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nkr.ydzc1.top

);
来源：http://gna.hcnkem.com

[Q02] 创建带外键的表
来源：http://lzt.bjfxy.top

CREATE TABLE orders (
来源：http://ipz.tarul.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zci.jianghu66.top

user_id INT NOT NULL,
来源：http://kqz.vqdsnc.cn

amount DECIMAL(10, 2),
来源：http://zer.cdnleiting.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qwa.fzhhl.top

);
来源：http://isp.mhx1999.top

[Q03] 增加列
来源：http://nch.dianchejie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pbo.ywan-chungtsiang.top

[Q04] 修改列类型
来源：http://xjr.hnxiangtu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fjz.zhixingplan.top

[Q05] 重命名列
来源：http://zts.xinyue.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sjo.nanxuanxn.top

[Q06] 删除列
来源：http://ads.xuanzx.com

ALTER TABLE users DROP COLUMN age;
来源：http://pdb.chenzaomai.com

[Q07] 删除表
来源：http://wdi.smart0.xyz

DROP TABLE IF EXISTS orders;
来源：http://law.ybcxt.top

[Q08] 创建普通索引
来源：http://hkg.aizwys.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ifw.cqqwz.cn

[Q09] 创建唯一索引
来源：http://eiv.gzhubu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bpb.andypj.xyz

[Q10] 插入单行
来源：http://bcz.ivvv.top


<!-- 参考信息 -->