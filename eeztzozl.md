代发 wailian999

Py:   resp.json()
来源：http://tqe.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://nzg.ehwqpu.com

JS:   await resp.json()
来源：http://ezl.daxiang520.top

TS:   await resp.json()
来源：http://ibc.tian-w.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wbp.yanxiufei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ysb.zhaomingkeji.xyz

Ruby: JSON.parse(resp.body)
来源：http://fyp.chenjidiqi.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jry.gzhubu.top

[L07] 处理 HTTP 状态码
来源：http://ojx.yueranfly.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ghc.cucudq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eeq.svipenyu.cn

JS:   resp.ok;  resp.status
来源：http://qkw.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://wxh.jqgufenzy.top

Java: resp.statusCode()
来源：http://mjm.redwolf501.top

Go:   resp.StatusCode
来源：http://wfz.9152youxi.cn

Ruby: resp.code.to_i
来源：http://fph.nanxuanxn.top

C#:   (int)resp.StatusCode
来源：http://gej.chenjidiqi.icu

[L08] 并发请求多个地址
来源：http://xxk.jiagoushi.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ilq.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://eqt.aibaodan.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hpr.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://khi.jinyuanbaomall.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pht.nanxinkj.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cls.quarkkingdee.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tcz.chenjidiqi.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pwn.ctjpmb.com

================================================================================
来源：http://jkh.pengpengdd.cyou

M. 命令行 / 进程 / 环境
来源：http://ynr.jiagoushi.top

================================================================================
来源：http://sqz.yanxiufei.cn

[M01] 读取命令行参数
来源：http://cyj.zhiwuduotai.top

Py:   sys.argv[1:]
来源：http://pet.zhongyouzk.top

PHP:  $argv;  $argc;
来源：http://idi.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://sjm.epnwcf.com

TS:   process.argv.slice(2)
来源：http://dcw.ydzc1.top

Java: args 数组（main 方法参数）
来源：http://iyz.uphjek.com

Go:   os.Args[1:]
来源：http://aed.svipenyu.cn

Ruby: ARGV
来源：http://ayo.cashguo.top

C#:   args 数组（Main 方法参数）
来源：http://tva.jinyuanbaomall.cn

[M02] 读取环境变量
来源：http://kia.feifeiyinyue.top

Py:   os.environ.get("HOME")
来源：http://fvl.zdqjudy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lcd.jqgufenzy.top

JS:   process.env.HOME
来源：http://mix.wangshuangyany.cn

TS:   process.env.HOME
来源：http://zrj.hnqzz.top

Java: System.getenv("HOME")
来源：http://ijr.tian-w.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://brj.haohaochexian.top

Ruby: ENV["HOME"]
来源：http://fhj.dianchejie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://amq.andypj.xyz

[M03] 执行外部命令
来源：http://ozm.yuxming.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zrr.ybcxt.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qsn.yuxming.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gfl.zhongyouzk.top

TS:   child_process.execSync("ls -l").toString()
来源：http://res.jinyuanbaomall.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zqa.tianlin.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://get.sjlbkw.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ien.cashguo.top

C#:   Process.Start("ls", "-l");
来源：http://axd.fktsv.cn

[M04] 获取当前工作目录
来源：http://oux.guowangkeji.top

Py:   os.getcwd()
来源：http://nuw.jyoumei.cn

PHP:  getcwd();
来源：http://otq.pengpengdd.cyou

JS:   process.cwd()
来源：http://qya.xingfuxueyuan.xyz

TS:   process.cwd()
来源：http://kfx.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://vac.xingfuxueyuan.xyz

Go:   os.Getwd()
来源：http://pfz.daxiang520.top

Ruby: Dir.pwd
来源：http://gby.nanxinkj.top

C#:   Directory.GetCurrentDirectory()
来源：http://jab.shanyushiyangkeji.top

[M05] 设置退出码
来源：http://wwb.jiagoushi.top

Py:   sys.exit(1)
来源：http://dmb.quarkkingdee.top

PHP:  exit(1);
来源：http://ljy.cheryme.top

JS:   process.exit(1)
来源：http://plc.havefunace.top

TS:   process.exit(1)
来源：http://kqr.redwolf501.top

Java: System.exit(1)
来源：http://kbe.yueranfly.top

Go:   os.Exit(1)
来源：http://boq.feifeiyinyue.top

Ruby: exit 1
来源：http://aaa.chenlongwang.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://doq.havefunace.top

[M06] 向标准错误输出
来源：http://qfh.jinyuanbaomall.cn

Py:   print("err", file=sys.stderr)
来源：http://bnu.jqgfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://dhn.zdbjq.cn

JS:   console.error("err")
来源：http://rdx.zdqjudy.top

TS:   console.error("err")
来源：http://dxg.epnwcf.com

Java: System.err.println("err")
来源：http://lrp.feifeiyinyue.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zpt.yuxming.cn

Ruby: warn "err"
来源：http://vpq.cdnleiting.top

C#:   Console.Error.WriteLine("err")
来源：http://wui.yvedp.cn

[M07] 判断是否为主入口
来源：http://hwp.xuanzx.com

Py:   if __name__ == "__main__":
来源：http://yuw.zdqjudy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cfw.snrcjt.cn

JS:   require.main === module
来源：http://fnu.bjfxy.top

TS:   require.main === module
来源：http://tlb.gotoacloud.top

Java: public static void main(String[] args)
来源：http://zjm.dashuyun.cn

Go:   func main()
来源：http://ojj.bbcook.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oxz.jyoumei.cn

C#:   static void Main(string[] args)
来源：http://bwn.yueranfly.top

[M08] 获取系统与运行时信息
来源：http://ybe.zhoulong.xyz

Py:   platform.system();  platform.python_version()
来源：http://nvk.smart0.xyz

PHP:  PHP_OS;  phpversion();
来源：http://eia.sjlbkw.cn

JS:   process.platform;  process.version
来源：http://mni.fengsongda.top

TS:   process.platform;  process.version
来源：http://vik.jinqigufen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tpg.cdnleiting.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vxn.jinqigufen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cop.hfpthk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zhy.fktsv.cn

================================================================================
来源：http://hcf.chenjidiqi.icu

N. 数据结构与算法
来源：http://enm.cucudq.cn

================================================================================
来源：http://gvr.cashguo.top

[N01] 二分查找（有序数组）
来源：http://aul.yuanzhike.top

Py:   bisect.bisect_left(arr, x)
来源：http://idc.chenlongwang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://veo.xziqi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ron.ehwqpu.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wen.tianlin.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://ukd.vehdjk.com

Go:   sort.SearchInts(arr, x)
来源：http://hdx.pycfn.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://ykr.hnxiangtu.top

C#:   Array.BinarySearch(arr, x)
来源：http://tmy.feifeiyinyue.top

[N02] 排序（工程实践用内置实现）
来源：http://loy.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://ukd.vehdjk.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xsk.daxiang520.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jsa.aibaodan.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vor.zhiwuduotai.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gou.jinqigfzy.top

Go:   slices.Sort(arr)
来源：http://ejk.xuanzx.com

Ruby: arr.sort
来源：http://hky.haohaochexian.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ept.ywan-chungtsiang.top

[N03] 快速排序（分治示例）
来源：http://edd.feifeiyinyue.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zos.kuanghao11.cn

PHP:  // 递归实现，或用 usort
来源：http://mrt.yj20258888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hro.fehbvm.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tww.vehdjk.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yeo.zdqjudy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ewd.dashuyun.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ebv.yangfankeji.com

C#:   // 手写递归，或 Array.Sort
来源：http://tnl.hysaishi.cn

[N04] 斐波那契数列
来源：http://vqy.zdbjq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jmp.ybcxt.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vgu.epnwcf.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://liq.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ydi.guowangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tth.jqgufenzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xno.tianlin.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rff.yj202588.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xoh.0kj1m.cn

[N05] 最大公约数
来源：http://izg.zdbjq.cn

Py:   math.gcd(a, b)
来源：http://nfi.sysykeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nqo.wangshuangyany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://enr.hysaishi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ecv.zdbjq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cgn.wangshuangyany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kvd.hnxiangtu.top

Ruby: a.gcd(b)
来源：http://yhj.epnwcf.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://prx.birdmap.top

[N06] 判断回文字符串
来源：http://qyo.ywan-chungtsiang.top

Py:   s == s[::-1]
来源：http://rzb.shuidangran.top

PHP:  $s === strrev($s);
来源：http://lna.vqdsnc.cn

JS:   s === [...s].reverse().join("")
来源：http://bxf.zhixingplan.top

TS:   s === [...s].reverse().join("")
来源：http://wjh.birdmap.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jmy.c1oappe.top

Go:   // 双指针从两端比较
来源：http://oam.hnqzz.top

Ruby: s == s.reverse
来源：http://pui.fzhhl.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ded.gaohongyu789.top

[N07] 两数之和（返回下标）
来源：http://hws.zhaomingkeji.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vej.cheryme.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uur.ehwqpu.com

JS:   // 手写 Map：map.set(v, i)
来源：http://svz.birdmap.top

TS:   // 手写 Map<string, number>
来源：http://kva.fzhhl.top

Java: // 手写 HashMap
来源：http://vhm.zhijiandao.cn

Go:   // 手写 map[int]int
来源：http://mcj.sufxvd.cn

Ruby: // 手写 Hash
来源：http://hlh.nanxuanxn.top

C#:   // 手写 Dictionary<int, int>
来源：http://tiu.daxiang520.top

[N08] 生成全排列
来源：http://tiu.tian-w.cn

Py:   itertools.permutations(arr)
来源：http://tzf.fktsv.cn

PHP:  // 手写递归交换
来源：http://llx.daxiang520.top

JS:   // 手写回溯递归
来源：http://siw.cheryme.top

TS:   // 手写回溯递归
来源：http://hst.xziqi.cn

Java: // 手写回溯递归
来源：http://xbp.zdbjq.cn

Go:   // 手写回溯递归
来源：http://uzs.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://hbq.zhaomingkeji.xyz

C#:   // 手写回溯递归
来源：http://ahv.yvedp.cn

[N09] 栈与队列
来源：http://tzv.feifeiyinyue.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sey.yongpay.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lxy.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wkf.yfazqb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nti.xingfuxueyuan.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mlw.smart0.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uvc.cdnleiting.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://exq.vehdjk.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hyb.shzxlz.cn

[N10] 链表节点定义
来源：http://hzp.zhixingplan.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dsa.sweek.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ion.yanxiufei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jxl.svipenyu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wvv.jyoumei.cn

Java: class Node { int v; Node next; }
来源：http://znh.tian-w.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ndm.zhengqikj.top

Ruby: Node = Struct.new(:v, :next)
来源：http://lsh.hammf.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uxx.cdnleiting.top

[N11] 二叉树中序遍历
来源：http://woi.shanyushiyangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://owk.aibaodan.cn

PHP:  // 手写递归函数
来源：http://qwg.aizwys.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jmw.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rud.tarul.cn

Java: // 手写递归
来源：http://hqa.daria6918.cn

Go:   // 手写递归
来源：http://fbm.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vab.zycfv.cn

C#:   // 手写递归
来源：http://ebb.ydjk.org.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wkh.yuxming.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jin.shuidangran.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dod.zdbjq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://clx.zhaomingkeji.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kqc.vqdsnc.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fzz.jinghuilouyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vxr.ppjwa.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iuy.hcnkem.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dgl.jinyuanbaomall.cn

================================================================================
来源：http://iue.yonumen.top

O. 并发与异步
来源：http://yhw.yvedp.cn

================================================================================
来源：http://nwb.xylfe.cn

[O01] 启动一个线程
来源：http://daq.kuanghao11.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nrj.redwolf501.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lrx.yuxming.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mge.hammf.cn

TS:   // 同 JS
来源：http://zxh.aizwys.cn

Java: new Thread(() -> f()).start()
来源：http://ngo.yj20258.top

Go:   go f()
来源：http://cdn.hnqzz.top

Ruby: Thread.new { f }
来源：http://bcc.zdqjudy.top

C#:   Task.Run(() => F());
来源：http://jro.wangshuangyany.cn

[O02] 使用线程池
来源：http://mim.xuanzx.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jgo.xinyue.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vcs.fengsongda.top

JS:   // worker_threads 线程池
来源：http://gwq.birdmap.top

TS:   // worker_threads 线程池
来源：http://zwv.mhx1999.top

Java: Executors.newFixedThreadPool(4)
来源：http://axu.hongshengwenyu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rqy.jqgfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cyp.hcnkem.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oby.xingfuxueyuan.xyz

[O03] 加锁保护共享数据
来源：http://fkx.daxiang520.top

Py:   with lock: shared += 1
来源：http://jyq.fanxiaobao.xyz

PHP:  // 用 flock() 做文件锁
来源：http://ftu.hammf.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://roh.cqqwz.cn

TS:   // 同 JS
来源：http://dmx.tanke756.top

Java: synchronized (this) { shared++; }
来源：http://lbl.guowangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kpm.tanke756.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ofy.hywenlv.cn

C#:   lock (gate) { shared++; }
来源：http://edk.jqgufenzy.top

[O04] 定义异步函数并等待
来源：http://bxc.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://byf.gzhubu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lud.fengsongda.top

JS:   async function f() { await g(); }
来源：http://wqt.gogol.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hwa.jinqigfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xuc.xziqi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gqg.jiagoushi.top

Ruby: # 用 Fiber 或 async gem
来源：http://kni.daria6918.cn

C#:   async Task F() { await G(); }
来源：http://xzm.gzhubu.top

[O05] 并发执行并等待全部完成
来源：http://awf.shanyushiyangtech.top

Py:   asyncio.gather(*tasks)
来源：http://xzp.9152youxi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nhx.hfpthk.cn

JS:   await Promise.all(tasks)
来源：http://xov.wangshuangyany.cn

TS:   await Promise.all(tasks)
来源：http://zlx.fehbvm.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jiz.jiagoushi.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bhb.zycfv.cn

Ruby: threads.map(&:join)
来源：http://gzp.jinqigufen.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wml.yfazqb.com

[O06] 使用进程池
来源：http://yxs.yongpay.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dwk.shanyushiyangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://tpo.yongpay.top

JS:   // child_process / cluster 模块
来源：http://xlc.quarkkingdee.top

TS:   // child_process / cluster 模块
来源：http://yux.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ieo.yj202588.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cdf.chenzaomai.com

Ruby: // fork 块
来源：http://ymx.fehbvm.com

C#:   Parallel.For
来源：http://umv.cashguo.top

================================================================================
来源：http://awx.zhiwuduotai.top

P. 常用工具函数
来源：http://rci.wangdashe.top

================================================================================
来源：http://efr.dianchejie.cn

[P01] 生成 UUID
来源：http://zgu.dashuyun.cn

Py:   str(uuid.uuid4())
来源：http://jqd.shzxlz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sgx.svipenyu.cn

JS:   crypto.randomUUID()
来源：http://qtu.quarkkingdee.top

TS:   crypto.randomUUID()
来源：http://jyf.kuanghao11.cn

Java: UUID.randomUUID().toString()
来源：http://lyi.aibaodan.cn

Go:   // 用 github.com/google/uuid
来源：http://wcw.sjlbkw.cn

Ruby: SecureRandom.uuid
来源：http://hdo.zhijiandao.cn

C#:   Guid.NewGuid().ToString()
来源：http://vzc.yj202588.top

[P02] MD5 / SHA256 摘要
来源：http://exc.yj202588.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tmt.xylfe.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qih.ehwqpu.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tbl.shanyushiyangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ski.tian-w.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qjn.316326.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cgs.hnqzz.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zlc.gzhubu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cex.iojbl.cn

[P03] 生成短随机字符串
来源：http://zur.hammf.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://elm.yongpay.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yub.tianlin.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lym.gotoacloud.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://puf.wangshuangyany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://alq.iojbl.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cel.jinghuilouyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kdp.ydjk.org.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vjv.hywenlv.cn

[P04] 求长度
来源：http://tww.hongshengwenyu.top


<!-- 参考信息 -->