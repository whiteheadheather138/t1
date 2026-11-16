代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://odw.yfazqb.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qey.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mcx.shanyushiyangtech.top

[L06] 解析响应为 JSON
来源：http://roa.xinyue.icu

Py:   resp.json()
来源：http://krx.fengsongda.top

PHP:  json_decode($body, true);
来源：http://hzt.sxryk.cn

JS:   await resp.json()
来源：http://all.cheryme.top

TS:   await resp.json()
来源：http://zrh.bbcook.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ogr.fehbvm.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://exo.sufxvd.cn

Ruby: JSON.parse(resp.body)
来源：http://ceo.zhoulong.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cxh.tarul.cn

[L07] 处理 HTTP 状态码
来源：http://ocw.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pgv.ybcxt.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gbm.hfpthk.cn

JS:   resp.ok;  resp.status
来源：http://ate.gaohongyu789.top

TS:   resp.ok;  resp.status
来源：http://akx.xinyue.icu

Java: resp.statusCode()
来源：http://ink.hnqzz.top

Go:   resp.StatusCode
来源：http://yyg.hywenlv.cn

Ruby: resp.code.to_i
来源：http://zwy.zhaomingkeji.xyz

C#:   (int)resp.StatusCode
来源：http://qpq.xinyue.icu

[L08] 并发请求多个地址
来源：http://vef.0kj1m.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dnf.wangdashe.top

PHP:  curl_multi_init() 系列
来源：http://guz.guannengcc.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pat.0kj1m.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xgc.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lqt.tarul.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eax.gzhubu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cgw.ppjwa.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kzb.9152youxi.cn

================================================================================
来源：http://qfo.iojbl.cn

M. 命令行 / 进程 / 环境
来源：http://vbl.ydzc1.top

================================================================================
来源：http://rkw.sysykeji.top

[M01] 读取命令行参数
来源：http://yfx.zdbjq.cn

Py:   sys.argv[1:]
来源：http://xxv.uphjek.com

PHP:  $argv;  $argc;
来源：http://vrg.c1oappe.top

JS:   process.argv.slice(2)
来源：http://gxu.tianlin.xyz

TS:   process.argv.slice(2)
来源：http://cjz.cqqwz.cn

Java: args 数组（main 方法参数）
来源：http://vqe.snrcjt.cn

Go:   os.Args[1:]
来源：http://ftu.gzhubu.top

Ruby: ARGV
来源：http://idi.hammf.cn

C#:   args 数组（Main 方法参数）
来源：http://qaf.ivvv.top

[M02] 读取环境变量
来源：http://ffd.quarkkingdee.top

Py:   os.environ.get("HOME")
来源：http://wrk.zdbjq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://syp.tanke756.top

JS:   process.env.HOME
来源：http://rda.zhongyouzk.top

TS:   process.env.HOME
来源：http://rvg.yangfankeji.com

Java: System.getenv("HOME")
来源：http://unq.zhijiandao.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nxg.xingfuxueyuan.xyz

Ruby: ENV["HOME"]
来源：http://nwe.jinyuanbaomall.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ryl.yueranfly.top

[M03] 执行外部命令
来源：http://ldm.svipenyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cic.daria6918.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kcg.jinqigfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dkh.sjlbkw.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kne.mhx1999.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ynb.quarkkingdee.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gld.jqgufenzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://qzo.yvedp.cn

C#:   Process.Start("ls", "-l");
来源：http://nqh.wangshuangyany.cn

[M04] 获取当前工作目录
来源：http://sgl.ctjpmb.com

Py:   os.getcwd()
来源：http://rle.xziqi.cn

PHP:  getcwd();
来源：http://dyn.bjfxy.top

JS:   process.cwd()
来源：http://gdz.ivvv.top

TS:   process.cwd()
来源：http://ito.jqgfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://ckh.guowangkeji.top

Go:   os.Getwd()
来源：http://kpl.zhijiandao.cn

Ruby: Dir.pwd
来源：http://gsg.hammf.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tum.zhiwuduotai.top

[M05] 设置退出码
来源：http://kse.zycfv.cn

Py:   sys.exit(1)
来源：http://ifx.snrcjt.cn

PHP:  exit(1);
来源：http://uoq.dashuyun.cn

JS:   process.exit(1)
来源：http://icz.shuidangran.top

TS:   process.exit(1)
来源：http://ozx.wangdashe.top

Java: System.exit(1)
来源：http://gsp.ydzc1.top

Go:   os.Exit(1)
来源：http://lga.kuanghao11.cn

Ruby: exit 1
来源：http://rsv.hnxiangtu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zke.yj20258888.top

[M06] 向标准错误输出
来源：http://ttr.birdmap.top

Py:   print("err", file=sys.stderr)
来源：http://afh.ehwqpu.com

PHP:  fwrite(STDERR, "err\n");
来源：http://bat.cucudq.cn

JS:   console.error("err")
来源：http://juv.gzhubu.top

TS:   console.error("err")
来源：http://pjg.0kj1m.cn

Java: System.err.println("err")
来源：http://zcu.cqqwz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://olr.aizwys.cn

Ruby: warn "err"
来源：http://cyu.xuetiantiany.cn

C#:   Console.Error.WriteLine("err")
来源：http://hzk.zdqjudy.top

[M07] 判断是否为主入口
来源：http://vkv.hnqzz.top

Py:   if __name__ == "__main__":
来源：http://ygv.kuanghao11.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ybl.iojbl.cn

JS:   require.main === module
来源：http://fps.nwbrower.top

TS:   require.main === module
来源：http://ile.yongpay.top

Java: public static void main(String[] args)
来源：http://dfi.quarkkingdee.top

Go:   func main()
来源：http://urb.jianghu66.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fyp.ywan-chungtsiang.top

C#:   static void Main(string[] args)
来源：http://rvh.wangdashe.top

[M08] 获取系统与运行时信息
来源：http://rgo.yj202588.top

Py:   platform.system();  platform.python_version()
来源：http://gfq.hongshengwenyu.top

PHP:  PHP_OS;  phpversion();
来源：http://xdz.tianlin.xyz

JS:   process.platform;  process.version
来源：http://big.xuetiantiany.cn

TS:   process.platform;  process.version
来源：http://rpe.daxiang520.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cfp.xuetiantiany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ntq.bjfxy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gwt.yangfankeji.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://klt.birdmap.top

================================================================================
来源：http://rwh.jinyuanbaomall.cn

N. 数据结构与算法
来源：http://tuc.xinyue.icu

================================================================================
来源：http://kji.snrcjt.cn

[N01] 二分查找（有序数组）
来源：http://pfc.daxiang520.top

Py:   bisect.bisect_left(arr, x)
来源：http://kyt.sysykeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://don.yj20258.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ycd.jinqigfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dkl.c1oappe.top

Java: Arrays.binarySearch(arr, x)
来源：http://pil.ywan-chungtsiang.top

Go:   sort.SearchInts(arr, x)
来源：http://inb.epnwcf.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://rzc.aibaodan.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ged.hfpthk.cn

[N02] 排序（工程实践用内置实现）
来源：http://aot.hcnkem.com

Py:   sorted(arr);  arr.sort()
来源：http://qwu.smart0.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gci.ppjwa.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cnx.cqqwz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hxn.meibo888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bva.hammf.cn

Go:   slices.Sort(arr)
来源：http://hrt.zdqjudy.top

Ruby: arr.sort
来源：http://rvz.hnxiangtu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://trs.wangshuangyany.cn

[N03] 快速排序（分治示例）
来源：http://lzd.hesvh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ocs.tian-w.cn

PHP:  // 递归实现，或用 usort
来源：http://yll.gaohongyu789.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ygg.ybcxt.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sto.tanke756.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vfe.tian-w.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eel.nanxinkj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gsq.sysykeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://zge.chenlongwang.top

[N04] 斐波那契数列
来源：http://dpo.wangdashe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nmo.sjlbkw.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rfw.pycfn.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ifb.jinyuanbaomall.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lcs.hammf.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oxp.jinqigufen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gtm.hfpthk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mbh.zhongyouzk.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://akv.ppjwa.cn

[N05] 最大公约数
来源：http://tch.chenlongwang.top

Py:   math.gcd(a, b)
来源：http://hsk.gotoacloud.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://raf.wangdashe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xnj.shanyushiyangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lko.birdmap.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://odh.gotoacloud.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ddl.haohaochexian.top

Ruby: a.gcd(b)
来源：http://xwp.yuanzhike.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://twi.yvedp.cn

[N06] 判断回文字符串
来源：http://peh.redwolf501.top

Py:   s == s[::-1]
来源：http://aqy.iojbl.cn

PHP:  $s === strrev($s);
来源：http://vih.chenlongwang.top

JS:   s === [...s].reverse().join("")
来源：http://xtw.nwbrower.top

TS:   s === [...s].reverse().join("")
来源：http://auo.chenjidiqi.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fxk.fanxiaobao.xyz

Go:   // 双指针从两端比较
来源：http://bxr.chenzaomai.com

Ruby: s == s.reverse
来源：http://obu.yj202588.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rkc.gaohongyu789.top

[N07] 两数之和（返回下标）
来源：http://xsc.ydzc1.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://adg.andypj.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hvj.hnqzz.top

JS:   // 手写 Map：map.set(v, i)
来源：http://yek.9152youxi.cn

TS:   // 手写 Map<string, number>
来源：http://kxp.nwbrower.top

Java: // 手写 HashMap
来源：http://vep.xylfe.cn

Go:   // 手写 map[int]int
来源：http://lrz.9152youxi.cn

Ruby: // 手写 Hash
来源：http://nvw.fzhhl.top

C#:   // 手写 Dictionary<int, int>
来源：http://pee.zdqjudy.top

[N08] 生成全排列
来源：http://pwi.wangdashe.top

Py:   itertools.permutations(arr)
来源：http://uqn.yvedp.cn

PHP:  // 手写递归交换
来源：http://jmn.snrcjt.cn

JS:   // 手写回溯递归
来源：http://cho.uphjek.com

TS:   // 手写回溯递归
来源：http://lad.meibo888.top

Java: // 手写回溯递归
来源：http://upl.jinqigufen.top

Go:   // 手写回溯递归
来源：http://daz.jlsjyb.cn

Ruby: arr.permutation.to_a
来源：http://bpg.yuxming.cn

C#:   // 手写回溯递归
来源：http://rfq.gogol.net.cn

[N09] 栈与队列
来源：http://byn.wangdashe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nto.xuanzx.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://srj.zhongyouzk.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://brh.aibaodan.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sqf.cdnleiting.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://moy.zhengqikj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bbi.gogol.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xrs.mhx1999.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://glu.hongshengwenyu.top

[N10] 链表节点定义
来源：http://ogg.yueranfly.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://prq.shzxlz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uok.gzhubu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nck.9152youxi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qzy.dashuyun.cn

Java: class Node { int v; Node next; }
来源：http://aiq.chenjidiqi.icu

Go:   type Node struct { V int; Next *Node }
来源：http://gza.fengsongda.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uyu.shzxlz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pwn.mhx1999.top

[N11] 二叉树中序遍历
来源：http://kfn.zhijiandao.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bvs.zhiwuduotai.top

PHP:  // 手写递归函数
来源：http://nsj.jinqigfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://for.xinyue.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qle.ctjpmb.com

Java: // 手写递归
来源：http://rug.ehwqpu.com

Go:   // 手写递归
来源：http://zmc.sjlbkw.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mzz.wangshuangyany.cn

C#:   // 手写递归
来源：http://kni.quarkkingdee.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://erm.ybcxt.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jbb.316326.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://odo.pengpengdd.cyou

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gpl.yuanzhike.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pfu.bbcook.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tmg.jianghu66.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ryx.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://suh.jqgfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yvn.hysaishi.cn

================================================================================
来源：http://vrw.nanxuanxn.top

O. 并发与异步
来源：http://zxy.sysykeji.top

================================================================================
来源：http://cxa.meibo888.top

[O01] 启动一个线程
来源：http://ixa.xylfe.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://crj.cashguo.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://snu.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sod.c1oappe.top

TS:   // 同 JS
来源：http://jeb.sweek.top

Java: new Thread(() -> f()).start()
来源：http://agj.ydjk.org.cn

Go:   go f()
来源：http://qbc.xingfuxueyuan.xyz

Ruby: Thread.new { f }
来源：http://zfc.hongshengwenyu.top

C#:   Task.Run(() => F());
来源：http://fnf.meibo888.top

[O02] 使用线程池
来源：http://vyp.zhijiandao.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zmd.jinqigfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jos.zycfv.cn

JS:   // worker_threads 线程池
来源：http://jpq.chenlongwang.top

TS:   // worker_threads 线程池
来源：http://ftz.fktsv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xvx.yuanzhike.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ukl.cheryme.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mkn.ivvv.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cuy.cashguo.top

[O03] 加锁保护共享数据
来源：http://yvk.xuetiantiany.cn

Py:   with lock: shared += 1
来源：http://jku.daria6918.cn

PHP:  // 用 flock() 做文件锁
来源：http://fxu.fengsongda.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dlk.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://efc.316326.xyz

Java: synchronized (this) { shared++; }
来源：http://xxo.xuetiantiany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ydb.jqgfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wkb.ctjpmb.com

C#:   lock (gate) { shared++; }
来源：http://ksb.yanxiufei.cn

[O04] 定义异步函数并等待
来源：http://ryd.havefunace.top

Py:   async def f():⏎    await g()
来源：http://ifs.zhijiandao.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yel.feifeiyinyue.top

JS:   async function f() { await g(); }
来源：http://bfe.yonumen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://yjc.zhaomingkeji.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://idc.vqdsnc.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hek.bbcook.cn

Ruby: # 用 Fiber 或 async gem
来源：http://avh.birdmap.top

C#:   async Task F() { await G(); }
来源：http://iaa.tanke756.top

[O05] 并发执行并等待全部完成
来源：http://xic.hfpthk.cn

Py:   asyncio.gather(*tasks)
来源：http://giu.yanxiufei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kmp.ywan-chungtsiang.top

JS:   await Promise.all(tasks)
来源：http://bna.meibo888.top

TS:   await Promise.all(tasks)
来源：http://eke.chenjidiqi.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zeg.zdqjudy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://znd.hammf.cn

Ruby: threads.map(&:join)
来源：http://aak.epnwcf.com

C#:   await Task.WhenAll(t1, t2)
来源：http://ezg.pengpengdd.cyou

[O06] 使用进程池
来源：http://fps.birdmap.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kvo.zhongyouzk.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ryj.fzhhl.top

JS:   // child_process / cluster 模块
来源：http://iou.jqgufenzy.top

TS:   // child_process / cluster 模块
来源：http://wbq.birdmap.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pdi.yuxming.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://iwt.chenlongwang.top

Ruby: // fork 块
来源：http://vrl.ctjpmb.com

C#:   Parallel.For
来源：http://ybo.snrcjt.cn

================================================================================
来源：http://zcy.nanxuanxn.top

P. 常用工具函数
来源：http://ffx.iojbl.cn

================================================================================
来源：http://dny.shangyingyoupin.top

[P01] 生成 UUID
来源：http://iii.zhixingplan.top

Py:   str(uuid.uuid4())
来源：http://nar.shuidangran.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fem.hesvh.cn

JS:   crypto.randomUUID()
来源：http://cnh.yfazqb.com

TS:   crypto.randomUUID()
来源：http://icn.jqgfzy.top

Java: UUID.randomUUID().toString()
来源：http://cme.zhixingplan.top

Go:   // 用 github.com/google/uuid
来源：http://kew.andypj.xyz

Ruby: SecureRandom.uuid
来源：http://aze.ehwqpu.com

C#:   Guid.NewGuid().ToString()
来源：http://ybr.aibaodan.cn

[P02] MD5 / SHA256 摘要
来源：http://ttt.cashguo.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bbj.zhaomingkeji.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://hvw.gzhubu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uoy.0kj1m.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ccs.birdmap.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rxr.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lgn.vqdsnc.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qud.shangyingyoupin.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vqy.yj202588.top

[P03] 生成短随机字符串
来源：http://uoz.smart0.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nvr.nanxuanxn.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fid.jlsjyb.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vkn.pengpengdd.cyou

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jer.fengsongda.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hhu.gzhubu.top


<!-- 参考信息 -->