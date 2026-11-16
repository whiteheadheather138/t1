代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kmd.meibo888.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dcx.jinqigfzy.top

Ruby: JSON.parse(resp.body)
来源：http://tko.zhongyouzk.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cgk.chenlongwang.top

[L07] 处理 HTTP 状态码
来源：http://slo.ywan-chungtsiang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aol.zhijiandao.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rex.havefunace.top

JS:   resp.ok;  resp.status
来源：http://jyj.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://boa.pengpengdd.cyou

Java: resp.statusCode()
来源：http://czr.smart0.xyz

Go:   resp.StatusCode
来源：http://wkx.chenjidiqi.icu

Ruby: resp.code.to_i
来源：http://ren.vqdsnc.cn

C#:   (int)resp.StatusCode
来源：http://kjy.xingfuxueyuan.xyz

[L08] 并发请求多个地址
来源：http://xzu.zhoulong.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mtr.yj20258.top

PHP:  curl_multi_init() 系列
来源：http://huh.cucudq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://izw.shzxlz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cdy.aizwys.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://smh.hammf.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pje.quarkkingdee.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mhi.zhijiandao.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kps.daria6918.cn

================================================================================
来源：http://oni.xinyue.icu

M. 命令行 / 进程 / 环境
来源：http://jbt.jinqigfzy.top

================================================================================
来源：http://gub.cheryme.top

[M01] 读取命令行参数
来源：http://uum.ydzc1.top

Py:   sys.argv[1:]
来源：http://zwl.svipenyu.cn

PHP:  $argv;  $argc;
来源：http://gkl.xuanzx.com

JS:   process.argv.slice(2)
来源：http://axo.sufxvd.cn

TS:   process.argv.slice(2)
来源：http://aqn.hysaishi.cn

Java: args 数组（main 方法参数）
来源：http://oxg.fanxiaobao.xyz

Go:   os.Args[1:]
来源：http://uae.chenlongwang.top

Ruby: ARGV
来源：http://lud.xuanzx.com

C#:   args 数组（Main 方法参数）
来源：http://emq.gogol.net.cn

[M02] 读取环境变量
来源：http://cjt.bjfxy.top

Py:   os.environ.get("HOME")
来源：http://cif.svipenyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://umb.ehwqpu.com

JS:   process.env.HOME
来源：http://efp.haohaochexian.top

TS:   process.env.HOME
来源：http://zcg.xinyue.icu

Java: System.getenv("HOME")
来源：http://xml.yj20258.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://emm.bbcook.cn

Ruby: ENV["HOME"]
来源：http://xkg.zycfv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ptv.jlsjyb.cn

[M03] 执行外部命令
来源：http://loy.chenjidiqi.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jvs.yj202588.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gpl.zhongyouzk.top

JS:   child_process.execSync("ls -l").toString()
来源：http://yyx.zdqjudy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tpj.hcnkem.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tsz.smart0.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://afn.hcnkem.com

Ruby: system("ls -l");  `ls -l`
来源：http://eqh.kuanghao11.cn

C#:   Process.Start("ls", "-l");
来源：http://hrl.jlsjyb.cn

[M04] 获取当前工作目录
来源：http://sfq.52xcode.cn

Py:   os.getcwd()
来源：http://rvu.hammf.cn

PHP:  getcwd();
来源：http://kti.hfpthk.cn

JS:   process.cwd()
来源：http://tnl.gogol.net.cn

TS:   process.cwd()
来源：http://nvj.guowangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://caf.hnxiangtu.top

Go:   os.Getwd()
来源：http://dlw.zdqjudy.top

Ruby: Dir.pwd
来源：http://fma.jyoumei.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kpn.pycfn.com

[M05] 设置退出码
来源：http://jep.316326.xyz

Py:   sys.exit(1)
来源：http://wsm.ywan-chungtsiang.top

PHP:  exit(1);
来源：http://vpi.yanxiufei.cn

JS:   process.exit(1)
来源：http://uvo.hnxiangtu.top

TS:   process.exit(1)
来源：http://hwk.bbcook.cn

Java: System.exit(1)
来源：http://nqm.meibo888.top

Go:   os.Exit(1)
来源：http://nak.hfpthk.cn

Ruby: exit 1
来源：http://ogh.epnwcf.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gui.ivvv.top

[M06] 向标准错误输出
来源：http://vjs.gaohongyu789.top

Py:   print("err", file=sys.stderr)
来源：http://smt.xziqi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pgu.chenzaomai.com

JS:   console.error("err")
来源：http://mvq.yj202588.top

TS:   console.error("err")
来源：http://uiq.quarkkingdee.top

Java: System.err.println("err")
来源：http://lty.zdbjq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hgt.dianchejie.cn

Ruby: warn "err"
来源：http://jhg.jlsjyb.cn

C#:   Console.Error.WriteLine("err")
来源：http://dgq.hcnkem.com

[M07] 判断是否为主入口
来源：http://mmh.yvedp.cn

Py:   if __name__ == "__main__":
来源：http://igq.yongpay.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xfl.havefunace.top

JS:   require.main === module
来源：http://kml.ywan-chungtsiang.top

TS:   require.main === module
来源：http://iww.fktsv.cn

Java: public static void main(String[] args)
来源：http://uti.316326.xyz

Go:   func main()
来源：http://aod.meibo888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://waj.yj202588.top

C#:   static void Main(string[] args)
来源：http://gea.ppjwa.cn

[M08] 获取系统与运行时信息
来源：http://rpw.guowangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://rlx.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://vba.cucudq.cn

JS:   process.platform;  process.version
来源：http://kpa.feifeiyinyue.top

TS:   process.platform;  process.version
来源：http://tdm.jinqigufen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bnz.quarkkingdee.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mdx.gotoacloud.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nxv.cqqwz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://icn.xuanzx.com

================================================================================
来源：http://djr.yj20258.top

N. 数据结构与算法
来源：http://cqr.316326.xyz

================================================================================
来源：http://mxi.0kj1m.cn

[N01] 二分查找（有序数组）
来源：http://bts.xziqi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://brx.zhiwuduotai.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wrv.ehwqpu.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jcv.sweek.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nmv.jinyuanbaomall.cn

Java: Arrays.binarySearch(arr, x)
来源：http://frt.nanxuanxn.top

Go:   sort.SearchInts(arr, x)
来源：http://ttu.wangdashe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cjh.redwolf501.top

C#:   Array.BinarySearch(arr, x)
来源：http://cau.guannengcc.top

[N02] 排序（工程实践用内置实现）
来源：http://bic.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://jhl.daxiang520.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mcg.yueranfly.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://wva.316326.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://llu.iojbl.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hpv.bbcook.cn

Go:   slices.Sort(arr)
来源：http://hul.daxiang520.top

Ruby: arr.sort
来源：http://vpv.chenjidiqi.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://mql.shangyingyoupin.top

[N03] 快速排序（分治示例）
来源：http://bty.jyoumei.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ftm.wangdashe.top

PHP:  // 递归实现，或用 usort
来源：http://sou.jinqigufen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pyp.9152youxi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ycu.ywan-chungtsiang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sbt.yuxming.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://alc.yueranfly.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mnn.meibo888.top

C#:   // 手写递归，或 Array.Sort
来源：http://ktt.zhongyouzk.top

[N04] 斐波那契数列
来源：http://zgt.fengsongda.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://msg.tian-w.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tvd.tarul.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://toy.sjlbkw.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vzd.jinqigufen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ptr.yonumen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sop.shanyushiyangtech.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nsk.sysykeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xyi.jinghuilouyu.cn

[N05] 最大公约数
来源：http://amf.hfpthk.cn

Py:   math.gcd(a, b)
来源：http://rvx.jiagoushi.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ihs.chenzaomai.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dno.chenlongwang.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://htm.mhx1999.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tbv.zhengqikj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://opo.shanyushiyangkeji.top

Ruby: a.gcd(b)
来源：http://smg.hnxiangtu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wgq.jinqigfzy.top

[N06] 判断回文字符串
来源：http://bvc.hongshengwenyu.top

Py:   s == s[::-1]
来源：http://qoe.jinghuilouyu.cn

PHP:  $s === strrev($s);
来源：http://kyx.ybcxt.top

JS:   s === [...s].reverse().join("")
来源：http://tjs.fzhhl.top

TS:   s === [...s].reverse().join("")
来源：http://cxm.yj202588.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blz.guannengcc.top

Go:   // 双指针从两端比较
来源：http://rry.aibaodan.cn

Ruby: s == s.reverse
来源：http://nyf.yfazqb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://waa.jqgfzy.top

[N07] 两数之和（返回下标）
来源：http://qrj.haohaochexian.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dlm.aizwys.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://adp.ppjwa.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://snm.shangyingyoupin.top

TS:   // 手写 Map<string, number>
来源：http://rje.xinyue.icu

Java: // 手写 HashMap
来源：http://gsq.xziqi.cn

Go:   // 手写 map[int]int
来源：http://oiu.xingfuxueyuan.xyz

Ruby: // 手写 Hash
来源：http://oji.ydzc1.top

C#:   // 手写 Dictionary<int, int>
来源：http://xha.ywan-chungtsiang.top

[N08] 生成全排列
来源：http://ftp.yongpay.top

Py:   itertools.permutations(arr)
来源：http://vfb.havefunace.top

PHP:  // 手写递归交换
来源：http://wdq.iojbl.cn

JS:   // 手写回溯递归
来源：http://phx.uphjek.com

TS:   // 手写回溯递归
来源：http://hxs.jinqigufen.top

Java: // 手写回溯递归
来源：http://exe.dianchejie.cn

Go:   // 手写回溯递归
来源：http://kgt.jqgfzy.top

Ruby: arr.permutation.to_a
来源：http://nuk.yuxming.cn

C#:   // 手写回溯递归
来源：http://xwl.shuidangran.top

[N09] 栈与队列
来源：http://ycq.tarul.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://skq.gzhubu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dvn.wangshuangyany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nsh.yonumen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kut.xylfe.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mjz.0kj1m.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cts.snrcjt.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nni.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rta.jinyuanbaomall.cn

[N10] 链表节点定义
来源：http://arp.ywan-chungtsiang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qpk.zdbjq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://niz.wangshuangyany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ash.zycfv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rbt.jlsjyb.cn

Java: class Node { int v; Node next; }
来源：http://flg.chenzaomai.com

Go:   type Node struct { V int; Next *Node }
来源：http://ffg.chenjidiqi.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://khz.kuanghao11.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jnh.ctjpmb.com

[N11] 二叉树中序遍历
来源：http://bti.yueranfly.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bho.chenzaomai.com

PHP:  // 手写递归函数
来源：http://zne.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://urx.hongshengwenyu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tpd.ctjpmb.com

Java: // 手写递归
来源：http://tqp.yuxming.cn

Go:   // 手写递归
来源：http://kag.chenzaomai.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lvd.guannengcc.top

C#:   // 手写递归
来源：http://njf.aibaodan.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qci.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kfw.ydzc1.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rpy.guannengcc.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://phg.yanxiufei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wri.ppjwa.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tab.haohaochexian.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vpg.pycfn.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://obf.sufxvd.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://edn.yanxiufei.cn

================================================================================
来源：http://vsz.feifeiyinyue.top

O. 并发与异步
来源：http://khq.jinqigfzy.top

================================================================================
来源：http://ejh.dashuyun.cn

[O01] 启动一个线程
来源：http://kjh.cdnleiting.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jfe.hesvh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zuu.ydzc1.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vkt.tianlin.xyz

TS:   // 同 JS
来源：http://exo.pengpengdd.cyou

Java: new Thread(() -> f()).start()
来源：http://dbc.chenzaomai.com

Go:   go f()
来源：http://wyp.cdnleiting.top

Ruby: Thread.new { f }
来源：http://adu.zhongyouzk.top

C#:   Task.Run(() => F());
来源：http://xhr.dianchejie.cn

[O02] 使用线程池
来源：http://ssp.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hfy.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bez.dianchejie.cn

JS:   // worker_threads 线程池
来源：http://owj.yj20258.top

TS:   // worker_threads 线程池
来源：http://dwz.uphjek.com

Java: Executors.newFixedThreadPool(4)
来源：http://nkh.cheryme.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xlx.nanxuanxn.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sja.iojbl.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cjq.hammf.cn

[O03] 加锁保护共享数据
来源：http://yck.chenlongwang.top

Py:   with lock: shared += 1
来源：http://yet.birdmap.top

PHP:  // 用 flock() 做文件锁
来源：http://owo.sxryk.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gwn.xuetiantiany.cn

TS:   // 同 JS
来源：http://fwd.jinyuanbaomall.cn

Java: synchronized (this) { shared++; }
来源：http://yum.zhengqikj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ppj.yangfankeji.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://vwq.cdnleiting.top

C#:   lock (gate) { shared++; }
来源：http://hag.yangfankeji.com

[O04] 定义异步函数并等待
来源：http://xcx.guowangkeji.top

Py:   async def f():⏎    await g()
来源：http://rhj.sufxvd.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ffx.fengsongda.top

JS:   async function f() { await g(); }
来源：http://jqz.hfpthk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wte.fanxiaobao.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dcz.cashguo.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rhx.yuxming.cn

Ruby: # 用 Fiber 或 async gem
来源：http://keo.feifeiyinyue.top

C#:   async Task F() { await G(); }
来源：http://pxe.meibo888.top

[O05] 并发执行并等待全部完成
来源：http://owl.xylfe.cn

Py:   asyncio.gather(*tasks)
来源：http://uzu.hfpthk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ijf.jianghu66.top

JS:   await Promise.all(tasks)
来源：http://joa.daria6918.cn

TS:   await Promise.all(tasks)
来源：http://guv.vqdsnc.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dkq.jlsjyb.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oup.hnxiangtu.top

Ruby: threads.map(&:join)
来源：http://iit.tian-w.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://thv.yanxiufei.cn

[O06] 使用进程池
来源：http://xkz.tianlin.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uln.redwolf501.top

PHP:  // pcntl_fork 或多进程队列
来源：http://unn.pengpengdd.cyou

JS:   // child_process / cluster 模块
来源：http://aoq.gogol.net.cn

TS:   // child_process / cluster 模块
来源：http://psg.andypj.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rmu.bjfxy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qoh.jyoumei.cn

Ruby: // fork 块
来源：http://jgl.tanke756.top

C#:   Parallel.For
来源：http://wsy.yuxming.cn

================================================================================
来源：http://dgj.aizwys.cn

P. 常用工具函数
来源：http://nqk.ydzc1.top

================================================================================
来源：http://dpx.wangdashe.top

[P01] 生成 UUID
来源：http://iwl.birdmap.top

Py:   str(uuid.uuid4())
来源：http://cie.yj20258888.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://slz.jinyuanbaomall.cn

JS:   crypto.randomUUID()
来源：http://jhr.andypj.xyz

TS:   crypto.randomUUID()
来源：http://oot.zhiwuduotai.top

Java: UUID.randomUUID().toString()
来源：http://ggz.ctjpmb.com

Go:   // 用 github.com/google/uuid
来源：http://fdp.jianghu66.top

Ruby: SecureRandom.uuid
来源：http://asn.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://jes.sweek.top

[P02] MD5 / SHA256 摘要
来源：http://wvi.fktsv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oft.feifeiyinyue.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mkr.c1oappe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://myv.svipenyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mci.xuanzx.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ram.feifeiyinyue.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cii.zhongyouzk.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://chd.yongpay.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lpg.hongshengwenyu.top

[P03] 生成短随机字符串
来源：http://ngi.hammf.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ign.wangdashe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://boi.zdqjudy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jei.xuanzx.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gfl.zhengqikj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gms.yuxming.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wyn.hnqzz.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xcv.zdbjq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gkc.yj20258.top

[P04] 求长度
来源：http://pwa.fehbvm.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tol.dashuyun.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://udf.hcnkem.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tlw.cheryme.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eng.vehdjk.com


<!-- 参考信息 -->