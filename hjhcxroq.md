代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tfm.nanxuanxn.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tbu.havefunace.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xiu.havefunace.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gxw.andypj.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eeg.yonumen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zxg.sjlbkw.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jlx.iojbl.cn

[L06] 解析响应为 JSON
来源：http://zai.xinyue.icu

Py:   resp.json()
来源：http://kyj.pycfn.com

PHP:  json_decode($body, true);
来源：http://qnf.gaohongyu789.top

JS:   await resp.json()
来源：http://bjf.havefunace.top

TS:   await resp.json()
来源：http://oon.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wdk.hongshengwenyu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xnl.zdqjudy.top

Ruby: JSON.parse(resp.body)
来源：http://xrj.yj20258.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jgi.jinqigufen.top

[L07] 处理 HTTP 状态码
来源：http://gyj.yangfankeji.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vur.cheryme.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nzt.fehbvm.com

JS:   resp.ok;  resp.status
来源：http://nmm.nwbrower.top

TS:   resp.ok;  resp.status
来源：http://cal.xinyue.icu

Java: resp.statusCode()
来源：http://fsf.hesvh.cn

Go:   resp.StatusCode
来源：http://owg.quarkkingdee.top

Ruby: resp.code.to_i
来源：http://tov.hnxiangtu.top

C#:   (int)resp.StatusCode
来源：http://ihz.shzxlz.cn

[L08] 并发请求多个地址
来源：http://kgv.vehdjk.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kdp.shuidangran.top

PHP:  curl_multi_init() 系列
来源：http://djv.9152youxi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lti.shzxlz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dlv.fengsongda.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dny.9152youxi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oqi.jinyuanbaomall.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ndw.zhongyouzk.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sgk.pycfn.com

================================================================================
来源：http://gjd.zhaomingkeji.xyz

M. 命令行 / 进程 / 环境
来源：http://uwz.jiagoushi.top

================================================================================
来源：http://tam.0kj1m.cn

[M01] 读取命令行参数
来源：http://alg.pengpengdd.cyou

Py:   sys.argv[1:]
来源：http://dwr.jqgufenzy.top

PHP:  $argv;  $argc;
来源：http://czf.yj20258888.top

JS:   process.argv.slice(2)
来源：http://nno.shanyushiyangkeji.top

TS:   process.argv.slice(2)
来源：http://wte.daria6918.cn

Java: args 数组（main 方法参数）
来源：http://gmk.iojbl.cn

Go:   os.Args[1:]
来源：http://soa.jinyuanbaomall.cn

Ruby: ARGV
来源：http://dav.vehdjk.com

C#:   args 数组（Main 方法参数）
来源：http://opn.yueranfly.top

[M02] 读取环境变量
来源：http://hya.jinqigufen.top

Py:   os.environ.get("HOME")
来源：http://iai.yfazqb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iri.zhiwuduotai.top

JS:   process.env.HOME
来源：http://aid.zdqjudy.top

TS:   process.env.HOME
来源：http://unm.fktsv.cn

Java: System.getenv("HOME")
来源：http://xhj.svipenyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dco.nanxuanxn.top

Ruby: ENV["HOME"]
来源：http://bbx.iojbl.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pew.gogol.net.cn

[M03] 执行外部命令
来源：http://rmf.redwolf501.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kvn.zhaomingkeji.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qnj.hammf.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cpe.yangfankeji.com

TS:   child_process.execSync("ls -l").toString()
来源：http://lsq.zhijiandao.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rlk.yuxming.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vbo.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://quv.yonumen.top

C#:   Process.Start("ls", "-l");
来源：http://lyh.epnwcf.com

[M04] 获取当前工作目录
来源：http://amo.ctjpmb.com

Py:   os.getcwd()
来源：http://uht.xinyue.icu

PHP:  getcwd();
来源：http://dqz.hnxiangtu.top

JS:   process.cwd()
来源：http://tcq.vqdsnc.cn

TS:   process.cwd()
来源：http://jcp.yueranfly.top

Java: Path.of("").toAbsolutePath()
来源：http://dlk.hcnkem.com

Go:   os.Getwd()
来源：http://rnj.fehbvm.com

Ruby: Dir.pwd
来源：http://azr.ydjk.org.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zbg.redwolf501.top

[M05] 设置退出码
来源：http://uxy.chenzaomai.com

Py:   sys.exit(1)
来源：http://ujo.jlsjyb.cn

PHP:  exit(1);
来源：http://bcc.hesvh.cn

JS:   process.exit(1)
来源：http://xgw.tianlin.xyz

TS:   process.exit(1)
来源：http://pmz.yj20258.top

Java: System.exit(1)
来源：http://cwr.hfpthk.cn

Go:   os.Exit(1)
来源：http://tax.svipenyu.cn

Ruby: exit 1
来源：http://ixr.c1oappe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jkm.cashguo.top

[M06] 向标准错误输出
来源：http://uaq.jqgufenzy.top

Py:   print("err", file=sys.stderr)
来源：http://qmp.jianghu66.top

PHP:  fwrite(STDERR, "err\n");
来源：http://jia.316326.xyz

JS:   console.error("err")
来源：http://osi.cashguo.top

TS:   console.error("err")
来源：http://zvt.yanxiufei.cn

Java: System.err.println("err")
来源：http://ahv.zhongyouzk.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://myx.wangshuangyany.cn

Ruby: warn "err"
来源：http://yok.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://rbt.yanxiufei.cn

[M07] 判断是否为主入口
来源：http://fbv.yvedp.cn

Py:   if __name__ == "__main__":
来源：http://tdd.jinghuilouyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vqf.xylfe.cn

JS:   require.main === module
来源：http://nry.haohaochexian.top

TS:   require.main === module
来源：http://yzg.jinqigfzy.top

Java: public static void main(String[] args)
来源：http://dvf.sufxvd.cn

Go:   func main()
来源：http://alf.gzhubu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://klp.sjlbkw.cn

C#:   static void Main(string[] args)
来源：http://yfa.xziqi.cn

[M08] 获取系统与运行时信息
来源：http://osr.wangdashe.top

Py:   platform.system();  platform.python_version()
来源：http://qtv.tian-w.cn

PHP:  PHP_OS;  phpversion();
来源：http://ovl.hongshengwenyu.top

JS:   process.platform;  process.version
来源：http://hmv.jinqigfzy.top

TS:   process.platform;  process.version
来源：http://yrv.xuetiantiany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ndi.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zyx.ivvv.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fum.dianchejie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rls.yj20258888.top

================================================================================
来源：http://qln.pengpengdd.cyou

N. 数据结构与算法
来源：http://dub.yangfankeji.com

================================================================================
来源：http://hfo.aibaodan.cn

[N01] 二分查找（有序数组）
来源：http://okz.tian-w.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mzc.guannengcc.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kdk.jiagoushi.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://obl.gaohongyu789.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bfj.kuanghao11.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wah.hnxiangtu.top

Go:   sort.SearchInts(arr, x)
来源：http://frg.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mcc.zhijiandao.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jeo.hesvh.cn

[N02] 排序（工程实践用内置实现）
来源：http://ruz.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://gny.quarkkingdee.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bax.shuidangran.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tkx.daxiang520.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://gym.cqqwz.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wzp.zhiwuduotai.top

Go:   slices.Sort(arr)
来源：http://man.sxryk.cn

Ruby: arr.sort
来源：http://jvq.dashuyun.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jqj.fanxiaobao.xyz

[N03] 快速排序（分治示例）
来源：http://cbn.fengsongda.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gmh.hfpthk.cn

PHP:  // 递归实现，或用 usort
来源：http://cuj.nwbrower.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dyb.hywenlv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ikm.zycfv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jtd.9152youxi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vyo.ydjk.org.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mcf.xylfe.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xpw.sxryk.cn

[N04] 斐波那契数列
来源：http://rou.hongshengwenyu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fud.epnwcf.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xwp.jinqigufen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wgv.chenjidiqi.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dow.cheryme.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uai.fktsv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xoh.daxiang520.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cyt.fktsv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zep.cdnleiting.top

[N05] 最大公约数
来源：http://lyj.cqqwz.cn

Py:   math.gcd(a, b)
来源：http://gye.yuanzhike.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fdy.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ozr.dianchejie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oye.yj20258.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bkb.hnqzz.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tqz.jlsjyb.cn

Ruby: a.gcd(b)
来源：http://rik.guannengcc.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sdw.dianchejie.cn

[N06] 判断回文字符串
来源：http://wmf.sxryk.cn

Py:   s == s[::-1]
来源：http://jvp.yvedp.cn

PHP:  $s === strrev($s);
来源：http://uit.snrcjt.cn

JS:   s === [...s].reverse().join("")
来源：http://yvh.sufxvd.cn

TS:   s === [...s].reverse().join("")
来源：http://qrk.yongpay.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tec.ppjwa.cn

Go:   // 双指针从两端比较
来源：http://pot.nanxinkj.top

Ruby: s == s.reverse
来源：http://byl.guowangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://oco.mhx1999.top

[N07] 两数之和（返回下标）
来源：http://dvp.fktsv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vir.sjlbkw.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cbg.cheryme.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ojr.zhoulong.xyz

TS:   // 手写 Map<string, number>
来源：http://byx.chenjidiqi.icu

Java: // 手写 HashMap
来源：http://klf.jinghuilouyu.cn

Go:   // 手写 map[int]int
来源：http://sth.shangyingyoupin.top

Ruby: // 手写 Hash
来源：http://wnk.sysykeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://cre.hnxiangtu.top

[N08] 生成全排列
来源：http://bll.shanyushiyangkeji.top

Py:   itertools.permutations(arr)
来源：http://dus.jqgufenzy.top

PHP:  // 手写递归交换
来源：http://tzc.sjlbkw.cn

JS:   // 手写回溯递归
来源：http://jge.ywan-chungtsiang.top

TS:   // 手写回溯递归
来源：http://ciq.jinghuilouyu.cn

Java: // 手写回溯递归
来源：http://lec.xziqi.cn

Go:   // 手写回溯递归
来源：http://pww.tianlin.xyz

Ruby: arr.permutation.to_a
来源：http://aqx.nanxinkj.top

C#:   // 手写回溯递归
来源：http://nnz.0kj1m.cn

[N09] 栈与队列
来源：http://qnq.9152youxi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pah.jqgfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vwi.shzxlz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gek.yanxiufei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nrk.gogol.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ztj.quarkkingdee.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rsd.nanxinkj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hlz.zhiwuduotai.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://egn.redwolf501.top

[N10] 链表节点定义
来源：http://hnq.hesvh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qoc.yfazqb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://rcs.iojbl.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yxu.fzhhl.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xsh.fanxiaobao.xyz

Java: class Node { int v; Node next; }
来源：http://pbu.dashuyun.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nil.fehbvm.com

Ruby: Node = Struct.new(:v, :next)
来源：http://byb.wangdashe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://emo.jqgufenzy.top

[N11] 二叉树中序遍历
来源：http://nsl.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uyv.fengsongda.top

PHP:  // 手写递归函数
来源：http://kei.hesvh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uik.wangshuangyany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://upe.yonumen.top

Java: // 手写递归
来源：http://dmv.snrcjt.cn

Go:   // 手写递归
来源：http://mja.bbcook.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bes.mhx1999.top

C#:   // 手写递归
来源：http://lcv.jqgfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baf.smart0.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ity.shanyushiyangtech.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vsw.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yht.havefunace.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lbs.tian-w.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tqe.316326.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://scy.zhijiandao.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cdf.wangdashe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vau.yfazqb.com

================================================================================
来源：http://zyd.jlsjyb.cn

O. 并发与异步
来源：http://ukr.hysaishi.cn

================================================================================
来源：http://bpl.hfpthk.cn

[O01] 启动一个线程
来源：http://ycc.tian-w.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://avn.jinqigufen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tdw.yfazqb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://izo.316326.xyz

TS:   // 同 JS
来源：http://cuw.ctjpmb.com

Java: new Thread(() -> f()).start()
来源：http://zxk.hnxiangtu.top

Go:   go f()
来源：http://cog.jinyuanbaomall.cn

Ruby: Thread.new { f }
来源：http://vmi.zhaomingkeji.xyz

C#:   Task.Run(() => F());
来源：http://lmt.yj20258.top

[O02] 使用线程池
来源：http://avy.nwbrower.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ehm.aizwys.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cps.jqgufenzy.top

JS:   // worker_threads 线程池
来源：http://fdy.zdbjq.cn

TS:   // worker_threads 线程池
来源：http://lmn.xingfuxueyuan.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://npc.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pyn.hfpthk.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jwx.hesvh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tjl.birdmap.top

[O03] 加锁保护共享数据
来源：http://hlq.jyoumei.cn

Py:   with lock: shared += 1
来源：http://ubq.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://ntn.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://onk.ctjpmb.com

TS:   // 同 JS
来源：http://xno.zhaomingkeji.xyz

Java: synchronized (this) { shared++; }
来源：http://hxc.xziqi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dpc.jiagoushi.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://geu.yueranfly.top

C#:   lock (gate) { shared++; }
来源：http://jdb.vqdsnc.cn

[O04] 定义异步函数并等待
来源：http://fuw.ctjpmb.com

Py:   async def f():⏎    await g()
来源：http://blb.aibaodan.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eqr.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://rsu.svipenyu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ore.kuanghao11.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fre.smart0.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://afh.jinghuilouyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gjk.redwolf501.top

C#:   async Task F() { await G(); }
来源：http://zrc.dianchejie.cn

[O05] 并发执行并等待全部完成
来源：http://yqg.zhiwuduotai.top

Py:   asyncio.gather(*tasks)
来源：http://dpe.sweek.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://brc.zhijiandao.cn

JS:   await Promise.all(tasks)
来源：http://tnr.chenjidiqi.icu

TS:   await Promise.all(tasks)
来源：http://xfl.chenjidiqi.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rlu.zycfv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fip.tian-w.cn

Ruby: threads.map(&:join)
来源：http://tkb.chenjidiqi.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://oze.tanke756.top

[O06] 使用进程池
来源：http://qod.hywenlv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iju.ppjwa.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rmr.shanyushiyangtech.top

JS:   // child_process / cluster 模块
来源：http://snn.dashuyun.cn

TS:   // child_process / cluster 模块
来源：http://tdm.nanxuanxn.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gki.fzhhl.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fek.shangyingyoupin.top

Ruby: // fork 块
来源：http://ylt.shangyingyoupin.top

C#:   Parallel.For
来源：http://zxb.jinghuilouyu.cn

================================================================================
来源：http://bjh.quarkkingdee.top

P. 常用工具函数
来源：http://dxp.bbcook.cn

================================================================================
来源：http://svm.zhaomingkeji.xyz

[P01] 生成 UUID
来源：http://doc.sufxvd.cn

Py:   str(uuid.uuid4())
来源：http://mvj.xziqi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jzd.daxiang520.top

JS:   crypto.randomUUID()
来源：http://rsh.pengpengdd.cyou

TS:   crypto.randomUUID()
来源：http://ecc.fanxiaobao.xyz

Java: UUID.randomUUID().toString()
来源：http://jll.yonumen.top

Go:   // 用 github.com/google/uuid
来源：http://htu.haohaochexian.top

Ruby: SecureRandom.uuid
来源：http://xev.bjfxy.top

C#:   Guid.NewGuid().ToString()
来源：http://prh.fktsv.cn

[P02] MD5 / SHA256 摘要
来源：http://vel.xinyue.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tgl.cqqwz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ync.zhoulong.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hif.haohaochexian.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uql.xuanzx.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sfj.bjfxy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hni.sjlbkw.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sbm.ivvv.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aaw.jinqigfzy.top

[P03] 生成短随机字符串
来源：http://gtc.9152youxi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sni.jiagoushi.top


<!-- 参考信息 -->