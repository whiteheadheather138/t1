代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dwe.jyoumei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ier.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kfv.chenzaomai.com

[L06] 解析响应为 JSON
来源：http://hue.tarul.cn

Py:   resp.json()
来源：http://epl.aizwys.cn

PHP:  json_decode($body, true);
来源：http://hpg.yfazqb.com

JS:   await resp.json()
来源：http://gik.jlsjyb.cn

TS:   await resp.json()
来源：http://arz.cheryme.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rph.yonumen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://auc.tianlin.xyz

Ruby: JSON.parse(resp.body)
来源：http://xbn.zhixingplan.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ynt.havefunace.top

[L07] 处理 HTTP 状态码
来源：http://lpy.yonumen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qzi.hywenlv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sbr.ybcxt.top

JS:   resp.ok;  resp.status
来源：http://uyx.9152youxi.cn

TS:   resp.ok;  resp.status
来源：http://vyy.tarul.cn

Java: resp.statusCode()
来源：http://htg.tianlin.xyz

Go:   resp.StatusCode
来源：http://wxp.snrcjt.cn

Ruby: resp.code.to_i
来源：http://ewh.zhijiandao.cn

C#:   (int)resp.StatusCode
来源：http://tft.hfpthk.cn

[L08] 并发请求多个地址
来源：http://ndj.kuanghao11.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hll.zhiwuduotai.top

PHP:  curl_multi_init() 系列
来源：http://ovv.cdnleiting.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zwv.meibo888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://flz.yuanzhike.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hle.redwolf501.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jne.zhoulong.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ogi.vqdsnc.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hpz.xuetiantiany.cn

================================================================================
来源：http://tlh.redwolf501.top

M. 命令行 / 进程 / 环境
来源：http://lci.zhiwuduotai.top

================================================================================
来源：http://xgo.hcnkem.com

[M01] 读取命令行参数
来源：http://vug.yangfankeji.com

Py:   sys.argv[1:]
来源：http://qwl.feifeiyinyue.top

PHP:  $argv;  $argc;
来源：http://jpg.zhaomingkeji.xyz

JS:   process.argv.slice(2)
来源：http://rpm.gogol.net.cn

TS:   process.argv.slice(2)
来源：http://klc.chenzaomai.com

Java: args 数组（main 方法参数）
来源：http://wrf.yuxming.cn

Go:   os.Args[1:]
来源：http://rcu.shuidangran.top

Ruby: ARGV
来源：http://alk.xziqi.cn

C#:   args 数组（Main 方法参数）
来源：http://wlr.uphjek.com

[M02] 读取环境变量
来源：http://dsx.ybcxt.top

Py:   os.environ.get("HOME")
来源：http://hrd.aibaodan.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rgl.zdqjudy.top

JS:   process.env.HOME
来源：http://evo.fengsongda.top

TS:   process.env.HOME
来源：http://ulf.0kj1m.cn

Java: System.getenv("HOME")
来源：http://xks.bbcook.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bin.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://fvi.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lkh.ehwqpu.com

[M03] 执行外部命令
来源：http://hxp.gotoacloud.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qgv.ehwqpu.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yme.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fcl.yj202588.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jmq.tian-w.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fzv.fehbvm.com

Go:   exec.Command("ls", "-l").Output()
来源：http://akj.gotoacloud.top

Ruby: system("ls -l");  `ls -l`
来源：http://gix.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://dre.hesvh.cn

[M04] 获取当前工作目录
来源：http://szo.vqdsnc.cn

Py:   os.getcwd()
来源：http://wht.hongshengwenyu.top

PHP:  getcwd();
来源：http://tll.ybcxt.top

JS:   process.cwd()
来源：http://xwp.iojbl.cn

TS:   process.cwd()
来源：http://xhw.fehbvm.com

Java: Path.of("").toAbsolutePath()
来源：http://vny.smart0.xyz

Go:   os.Getwd()
来源：http://ujz.nanxinkj.top

Ruby: Dir.pwd
来源：http://roq.shanyushiyangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://yio.shanyushiyangkeji.top

[M05] 设置退出码
来源：http://nje.cdnleiting.top

Py:   sys.exit(1)
来源：http://llx.chenzaomai.com

PHP:  exit(1);
来源：http://fwp.yuxming.cn

JS:   process.exit(1)
来源：http://rtd.gogol.net.cn

TS:   process.exit(1)
来源：http://rni.guowangkeji.top

Java: System.exit(1)
来源：http://hbu.fanxiaobao.xyz

Go:   os.Exit(1)
来源：http://umq.zycfv.cn

Ruby: exit 1
来源：http://nrm.316326.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://anh.zhixingplan.top

[M06] 向标准错误输出
来源：http://jwp.jinyuanbaomall.cn

Py:   print("err", file=sys.stderr)
来源：http://dke.snrcjt.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dcy.52xcode.cn

JS:   console.error("err")
来源：http://gjr.fengsongda.top

TS:   console.error("err")
来源：http://tdj.tarul.cn

Java: System.err.println("err")
来源：http://myp.bjfxy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fsx.cdnleiting.top

Ruby: warn "err"
来源：http://mru.bbcook.cn

C#:   Console.Error.WriteLine("err")
来源：http://knw.yanxiufei.cn

[M07] 判断是否为主入口
来源：http://oxx.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://xko.hnqzz.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ebd.jyoumei.cn

JS:   require.main === module
来源：http://pre.hfpthk.cn

TS:   require.main === module
来源：http://rcd.ppjwa.cn

Java: public static void main(String[] args)
来源：http://vpk.52xcode.cn

Go:   func main()
来源：http://fig.yfazqb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://anm.316326.xyz

C#:   static void Main(string[] args)
来源：http://pxv.ydjk.org.cn

[M08] 获取系统与运行时信息
来源：http://unu.hnqzz.top

Py:   platform.system();  platform.python_version()
来源：http://yku.jinqigufen.top

PHP:  PHP_OS;  phpversion();
来源：http://chi.yvedp.cn

JS:   process.platform;  process.version
来源：http://gry.jianghu66.top

TS:   process.platform;  process.version
来源：http://zcs.zycfv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vha.aibaodan.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xmy.yvedp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://loh.hfpthk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kfk.xylfe.cn

================================================================================
来源：http://hiv.haohaochexian.top

N. 数据结构与算法
来源：http://dbx.jqgfzy.top

================================================================================
来源：http://igf.nanxuanxn.top

[N01] 二分查找（有序数组）
来源：http://fqj.gaohongyu789.top

Py:   bisect.bisect_left(arr, x)
来源：http://rgj.svipenyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lnw.hesvh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://quh.yangfankeji.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bmi.ehwqpu.com

Java: Arrays.binarySearch(arr, x)
来源：http://cfq.yonumen.top

Go:   sort.SearchInts(arr, x)
来源：http://kxq.redwolf501.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://nei.bjfxy.top

C#:   Array.BinarySearch(arr, x)
来源：http://odu.yangfankeji.com

[N02] 排序（工程实践用内置实现）
来源：http://rbz.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://eyf.zhijiandao.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ksk.mhx1999.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://let.jinqigfzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vrq.yangfankeji.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ctk.yuxming.cn

Go:   slices.Sort(arr)
来源：http://axu.haohaochexian.top

Ruby: arr.sort
来源：http://eyj.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kzs.andypj.xyz

[N03] 快速排序（分治示例）
来源：http://kwu.sxryk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://smw.pycfn.com

PHP:  // 递归实现，或用 usort
来源：http://zlm.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tdf.aibaodan.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ngb.wangdashe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yci.uphjek.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://agw.guowangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kiy.sxryk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tfl.yj20258888.top

[N04] 斐波那契数列
来源：http://bzc.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uvi.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ylw.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dlk.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zhe.ybcxt.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lgk.yj20258888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zjh.yuanzhike.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cim.jqgufenzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gfc.jinqigufen.top

[N05] 最大公约数
来源：http://ndv.zhengqikj.top

Py:   math.gcd(a, b)
来源：http://hzk.jinghuilouyu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fkw.zdqjudy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lip.jlsjyb.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fgd.xingfuxueyuan.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zcq.hywenlv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uie.quarkkingdee.top

Ruby: a.gcd(b)
来源：http://yfy.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mvl.jinghuilouyu.cn

[N06] 判断回文字符串
来源：http://ppk.xinyue.icu

Py:   s == s[::-1]
来源：http://zkd.jqgufenzy.top

PHP:  $s === strrev($s);
来源：http://fwx.bbcook.cn

JS:   s === [...s].reverse().join("")
来源：http://rlp.c1oappe.top

TS:   s === [...s].reverse().join("")
来源：http://apk.cqqwz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qul.haohaochexian.top

Go:   // 双指针从两端比较
来源：http://eji.cdnleiting.top

Ruby: s == s.reverse
来源：http://bdh.daxiang520.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ahb.vehdjk.com

[N07] 两数之和（返回下标）
来源：http://ubb.xingfuxueyuan.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qbl.yangfankeji.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yuq.zhongyouzk.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dtq.daria6918.cn

TS:   // 手写 Map<string, number>
来源：http://npa.yfazqb.com

Java: // 手写 HashMap
来源：http://jne.ybcxt.top

Go:   // 手写 map[int]int
来源：http://heg.wangdashe.top

Ruby: // 手写 Hash
来源：http://zes.daxiang520.top

C#:   // 手写 Dictionary<int, int>
来源：http://ytz.fengsongda.top

[N08] 生成全排列
来源：http://vcu.chenzaomai.com

Py:   itertools.permutations(arr)
来源：http://qdl.mhx1999.top

PHP:  // 手写递归交换
来源：http://tlu.yueranfly.top

JS:   // 手写回溯递归
来源：http://kuj.bjfxy.top

TS:   // 手写回溯递归
来源：http://myq.fehbvm.com

Java: // 手写回溯递归
来源：http://xvk.c1oappe.top

Go:   // 手写回溯递归
来源：http://xjc.jqgufenzy.top

Ruby: arr.permutation.to_a
来源：http://hje.gaohongyu789.top

C#:   // 手写回溯递归
来源：http://beo.smart0.xyz

[N09] 栈与队列
来源：http://wxx.xingfuxueyuan.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dbb.tarul.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rqp.sjlbkw.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ogr.tianlin.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mks.hfpthk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fpc.yj20258.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ehy.nwbrower.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bkp.sufxvd.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oah.zhiwuduotai.top

[N10] 链表节点定义
来源：http://nyw.kuanghao11.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fpf.jqgufenzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://sdr.hnqzz.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xxp.gogol.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eqi.zhengqikj.top

Java: class Node { int v; Node next; }
来源：http://euo.ybcxt.top

Go:   type Node struct { V int; Next *Node }
来源：http://xeg.fanxiaobao.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://plb.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cby.xinyue.icu

[N11] 二叉树中序遍历
来源：http://uvg.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rkq.yuxming.cn

PHP:  // 手写递归函数
来源：http://ysx.hnqzz.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qcq.cashguo.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hab.zhaomingkeji.xyz

Java: // 手写递归
来源：http://tvl.xinyue.icu

Go:   // 手写递归
来源：http://wic.xuetiantiany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zif.316326.xyz

C#:   // 手写递归
来源：http://lwo.9152youxi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xvp.aizwys.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://drw.shangyingyoupin.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ojv.jianghu66.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dnr.daria6918.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wrz.aizwys.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ena.dianchejie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mme.yangfankeji.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zfc.shzxlz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wgw.cashguo.top

================================================================================
来源：http://vbi.quarkkingdee.top

O. 并发与异步
来源：http://ruq.jinyuanbaomall.cn

================================================================================
来源：http://ezb.hfpthk.cn

[O01] 启动一个线程
来源：http://opw.jqgfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hej.chenjidiqi.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://snl.svipenyu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nmc.zhiwuduotai.top

TS:   // 同 JS
来源：http://jwd.xuetiantiany.cn

Java: new Thread(() -> f()).start()
来源：http://zhl.ehwqpu.com

Go:   go f()
来源：http://tng.c1oappe.top

Ruby: Thread.new { f }
来源：http://ttr.nwbrower.top

C#:   Task.Run(() => F());
来源：http://afp.birdmap.top

[O02] 使用线程池
来源：http://fmg.xylfe.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://quz.xuetiantiany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://swc.xingfuxueyuan.xyz

JS:   // worker_threads 线程池
来源：http://fuz.hysaishi.cn

TS:   // worker_threads 线程池
来源：http://roa.tian-w.cn

Java: Executors.newFixedThreadPool(4)
来源：http://iid.guannengcc.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://izh.andypj.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bqt.jinyuanbaomall.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cmv.uphjek.com

[O03] 加锁保护共享数据
来源：http://ugk.meibo888.top

Py:   with lock: shared += 1
来源：http://hin.c1oappe.top

PHP:  // 用 flock() 做文件锁
来源：http://bgr.yanxiufei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://joe.zycfv.cn

TS:   // 同 JS
来源：http://lgk.yangfankeji.com

Java: synchronized (this) { shared++; }
来源：http://zjl.hammf.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bfp.zdbjq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nqs.tanke756.top

C#:   lock (gate) { shared++; }
来源：http://jqz.epnwcf.com

[O04] 定义异步函数并等待
来源：http://tlj.nanxinkj.top

Py:   async def f():⏎    await g()
来源：http://yhg.bjfxy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://chr.aizwys.cn

JS:   async function f() { await g(); }
来源：http://ivi.yuxming.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://aef.jinyuanbaomall.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hlq.sweek.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jql.dashuyun.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qgs.jiagoushi.top

C#:   async Task F() { await G(); }
来源：http://sau.nwbrower.top

[O05] 并发执行并等待全部完成
来源：http://laa.zdbjq.cn

Py:   asyncio.gather(*tasks)
来源：http://qjv.hcnkem.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lbd.gzhubu.top

JS:   await Promise.all(tasks)
来源：http://ayi.hnxiangtu.top

TS:   await Promise.all(tasks)
来源：http://yrd.zdbjq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tpp.zhaomingkeji.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jdb.hysaishi.cn

Ruby: threads.map(&:join)
来源：http://wtd.tian-w.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zfa.gogol.net.cn

[O06] 使用进程池
来源：http://lry.xinyue.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zpf.hcnkem.com

PHP:  // pcntl_fork 或多进程队列
来源：http://rsu.zhoulong.xyz

JS:   // child_process / cluster 模块
来源：http://eis.wangshuangyany.cn

TS:   // child_process / cluster 模块
来源：http://ifn.yj20258.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uzz.fengsongda.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wpo.yonumen.top

Ruby: // fork 块
来源：http://zyo.feifeiyinyue.top

C#:   Parallel.For
来源：http://lks.tianlin.xyz

================================================================================
来源：http://cdr.fanxiaobao.xyz

P. 常用工具函数
来源：http://iwk.xuanzx.com

================================================================================
来源：http://lce.hnxiangtu.top

[P01] 生成 UUID
来源：http://bmh.shangyingyoupin.top

Py:   str(uuid.uuid4())
来源：http://nia.52xcode.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mnz.jiagoushi.top

JS:   crypto.randomUUID()
来源：http://jbu.gotoacloud.top

TS:   crypto.randomUUID()
来源：http://dhq.tarul.cn

Java: UUID.randomUUID().toString()
来源：http://oqp.xinyue.icu

Go:   // 用 github.com/google/uuid
来源：http://ssl.hongshengwenyu.top

Ruby: SecureRandom.uuid
来源：http://uab.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://guq.ctjpmb.com

[P02] MD5 / SHA256 摘要
来源：http://eka.andypj.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://iez.meibo888.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://byk.hnqzz.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://okr.dashuyun.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kze.epnwcf.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://krb.shanyushiyangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vpw.xylfe.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jmn.shanyushiyangkeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lbh.pengpengdd.cyou

[P03] 生成短随机字符串
来源：http://mbp.yj20258888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ueu.zhixingplan.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://joi.c1oappe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://agh.tarul.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mxx.zycfv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ist.jinyuanbaomall.cn


<!-- 参考信息 -->