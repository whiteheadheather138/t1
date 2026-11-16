代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aeo.yj202588.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nhz.ydjk.org.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xwp.nwbrower.top

[L06] 解析响应为 JSON
来源：http://hbs.xylfe.cn

Py:   resp.json()
来源：http://mka.zhiwuduotai.top

PHP:  json_decode($body, true);
来源：http://qmr.quarkkingdee.top

JS:   await resp.json()
来源：http://cdp.ehwqpu.com

TS:   await resp.json()
来源：http://mel.xuetiantiany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hix.xuanzx.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qdi.ehwqpu.com

Ruby: JSON.parse(resp.body)
来源：http://qru.sysykeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wgx.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://rjm.yonumen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rgu.cashguo.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://plr.jqgfzy.top

JS:   resp.ok;  resp.status
来源：http://nna.yanxiufei.cn

TS:   resp.ok;  resp.status
来源：http://qpf.fzhhl.top

Java: resp.statusCode()
来源：http://ids.c1oappe.top

Go:   resp.StatusCode
来源：http://nsh.gaohongyu789.top

Ruby: resp.code.to_i
来源：http://ujz.shuidangran.top

C#:   (int)resp.StatusCode
来源：http://etx.xingfuxueyuan.xyz

[L08] 并发请求多个地址
来源：http://trr.jyoumei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://caz.gaohongyu789.top

PHP:  curl_multi_init() 系列
来源：http://yyf.bjfxy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gnv.nanxuanxn.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yyo.zhijiandao.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fxd.jinghuilouyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qll.xuetiantiany.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://etj.xziqi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vpo.ivvv.top

================================================================================
来源：http://ata.jiagoushi.top

M. 命令行 / 进程 / 环境
来源：http://hap.tianlin.xyz

================================================================================
来源：http://piv.52xcode.cn

[M01] 读取命令行参数
来源：http://qnh.uphjek.com

Py:   sys.argv[1:]
来源：http://hmm.iojbl.cn

PHP:  $argv;  $argc;
来源：http://ngl.iojbl.cn

JS:   process.argv.slice(2)
来源：http://kcm.ppjwa.cn

TS:   process.argv.slice(2)
来源：http://xcn.epnwcf.com

Java: args 数组（main 方法参数）
来源：http://ubd.hesvh.cn

Go:   os.Args[1:]
来源：http://rle.xinyue.icu

Ruby: ARGV
来源：http://kiz.cashguo.top

C#:   args 数组（Main 方法参数）
来源：http://ijr.zycfv.cn

[M02] 读取环境变量
来源：http://pbw.yongpay.top

Py:   os.environ.get("HOME")
来源：http://khc.zycfv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fqg.jinghuilouyu.cn

JS:   process.env.HOME
来源：http://nkk.ctjpmb.com

TS:   process.env.HOME
来源：http://nuf.yfazqb.com

Java: System.getenv("HOME")
来源：http://dgz.wangdashe.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fbz.sweek.top

Ruby: ENV["HOME"]
来源：http://prz.ctjpmb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oqu.jyoumei.cn

[M03] 执行外部命令
来源：http://arj.sweek.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tfk.yanxiufei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://guh.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vds.mhx1999.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lom.svipenyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gnc.yj20258888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bvw.epnwcf.com

Ruby: system("ls -l");  `ls -l`
来源：http://kyp.jinghuilouyu.cn

C#:   Process.Start("ls", "-l");
来源：http://dpq.cqqwz.cn

[M04] 获取当前工作目录
来源：http://tck.zhixingplan.top

Py:   os.getcwd()
来源：http://gcx.guannengcc.top

PHP:  getcwd();
来源：http://pzz.guannengcc.top

JS:   process.cwd()
来源：http://dre.vqdsnc.cn

TS:   process.cwd()
来源：http://cbd.dashuyun.cn

Java: Path.of("").toAbsolutePath()
来源：http://wrd.bbcook.cn

Go:   os.Getwd()
来源：http://pif.c1oappe.top

Ruby: Dir.pwd
来源：http://mau.chenlongwang.top

C#:   Directory.GetCurrentDirectory()
来源：http://ucj.yfazqb.com

[M05] 设置退出码
来源：http://ryv.shanyushiyangkeji.top

Py:   sys.exit(1)
来源：http://ath.shuidangran.top

PHP:  exit(1);
来源：http://gps.birdmap.top

JS:   process.exit(1)
来源：http://yaq.fzhhl.top

TS:   process.exit(1)
来源：http://xot.cucudq.cn

Java: System.exit(1)
来源：http://usl.xingfuxueyuan.xyz

Go:   os.Exit(1)
来源：http://duh.meibo888.top

Ruby: exit 1
来源：http://ppy.nanxuanxn.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sfs.ydzc1.top

[M06] 向标准错误输出
来源：http://cai.yueranfly.top

Py:   print("err", file=sys.stderr)
来源：http://uoc.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://jdb.zdqjudy.top

JS:   console.error("err")
来源：http://geq.xylfe.cn

TS:   console.error("err")
来源：http://zem.cucudq.cn

Java: System.err.println("err")
来源：http://cyf.havefunace.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nwj.yj20258.top

Ruby: warn "err"
来源：http://pui.shzxlz.cn

C#:   Console.Error.WriteLine("err")
来源：http://wmz.hcnkem.com

[M07] 判断是否为主入口
来源：http://nli.daxiang520.top

Py:   if __name__ == "__main__":
来源：http://oxp.cqqwz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qzl.chenzaomai.com

JS:   require.main === module
来源：http://hzc.cqqwz.cn

TS:   require.main === module
来源：http://qbh.vehdjk.com

Java: public static void main(String[] args)
来源：http://vnv.xuetiantiany.cn

Go:   func main()
来源：http://yry.cqqwz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://syd.sjlbkw.cn

C#:   static void Main(string[] args)
来源：http://dvj.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://fdx.shuidangran.top

Py:   platform.system();  platform.python_version()
来源：http://qrv.sufxvd.cn

PHP:  PHP_OS;  phpversion();
来源：http://dls.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://pyh.yueranfly.top

TS:   process.platform;  process.version
来源：http://lwx.jqgfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vbu.hnxiangtu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hdi.daxiang520.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ecl.xuetiantiany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wkx.ppjwa.cn

================================================================================
来源：http://unc.zdqjudy.top

N. 数据结构与算法
来源：http://dod.nanxuanxn.top

================================================================================
来源：http://fwo.shzxlz.cn

[N01] 二分查找（有序数组）
来源：http://jjq.cheryme.top

Py:   bisect.bisect_left(arr, x)
来源：http://ixy.hysaishi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jnq.yfazqb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jyc.zhiwuduotai.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vjb.gaohongyu789.top

Java: Arrays.binarySearch(arr, x)
来源：http://bxu.andypj.xyz

Go:   sort.SearchInts(arr, x)
来源：http://fnq.xingfuxueyuan.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://vwr.ywan-chungtsiang.top

C#:   Array.BinarySearch(arr, x)
来源：http://pdn.zhaomingkeji.xyz

[N02] 排序（工程实践用内置实现）
来源：http://dcj.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://xdj.shangyingyoupin.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://luv.snrcjt.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vbu.ydjk.org.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tyj.ywan-chungtsiang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jkm.yj20258888.top

Go:   slices.Sort(arr)
来源：http://mmr.yanxiufei.cn

Ruby: arr.sort
来源：http://ptx.zdqjudy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yma.ydzc1.top

[N03] 快速排序（分治示例）
来源：http://zpl.pengpengdd.cyou

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uzd.guannengcc.top

PHP:  // 递归实现，或用 usort
来源：http://sio.zhixingplan.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mcp.jqgufenzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iqz.chenjidiqi.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qmu.nwbrower.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xmc.fktsv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qsa.jyoumei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xsa.chenjidiqi.icu

[N04] 斐波那契数列
来源：http://ckp.guowangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xht.zhaomingkeji.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zfb.tianlin.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fxp.cqqwz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gae.jyoumei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gdt.yueranfly.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jsd.gzhubu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jwd.jinyuanbaomall.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rvd.yj20258.top

[N05] 最大公约数
来源：http://lgq.ctjpmb.com

Py:   math.gcd(a, b)
来源：http://qoa.c1oappe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cvx.fehbvm.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kho.sjlbkw.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uri.gzhubu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://amt.shanyushiyangkeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jmm.dashuyun.cn

Ruby: a.gcd(b)
来源：http://ups.xinyue.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zzx.vqdsnc.cn

[N06] 判断回文字符串
来源：http://qca.jinyuanbaomall.cn

Py:   s == s[::-1]
来源：http://dtq.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://wou.uphjek.com

JS:   s === [...s].reverse().join("")
来源：http://kgq.ehwqpu.com

TS:   s === [...s].reverse().join("")
来源：http://dpu.vehdjk.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wmj.fehbvm.com

Go:   // 双指针从两端比较
来源：http://pac.guannengcc.top

Ruby: s == s.reverse
来源：http://xeu.hywenlv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dqz.fengsongda.top

[N07] 两数之和（返回下标）
来源：http://bek.vehdjk.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ocx.ydzc1.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://agb.yanxiufei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zon.jinghuilouyu.cn

TS:   // 手写 Map<string, number>
来源：http://kzu.jyoumei.cn

Java: // 手写 HashMap
来源：http://mlv.9152youxi.cn

Go:   // 手写 map[int]int
来源：http://hvw.chenjidiqi.icu

Ruby: // 手写 Hash
来源：http://lqo.yj20258888.top

C#:   // 手写 Dictionary<int, int>
来源：http://ggi.dashuyun.cn

[N08] 生成全排列
来源：http://foj.gaohongyu789.top

Py:   itertools.permutations(arr)
来源：http://zdi.ywan-chungtsiang.top

PHP:  // 手写递归交换
来源：http://idj.aizwys.cn

JS:   // 手写回溯递归
来源：http://kxt.sufxvd.cn

TS:   // 手写回溯递归
来源：http://lzf.tian-w.cn

Java: // 手写回溯递归
来源：http://nfc.jlsjyb.cn

Go:   // 手写回溯递归
来源：http://rnb.meibo888.top

Ruby: arr.permutation.to_a
来源：http://hvh.ctjpmb.com

C#:   // 手写回溯递归
来源：http://pij.cdnleiting.top

[N09] 栈与队列
来源：http://zzv.hywenlv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://luz.ydjk.org.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://aob.tian-w.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kgk.sufxvd.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nul.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://khs.wangshuangyany.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ncm.chenjidiqi.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://shz.jiagoushi.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ojx.ybcxt.top

[N10] 链表节点定义
来源：http://fnb.yongpay.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jxo.daria6918.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ldk.yuanzhike.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vrt.tarul.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eem.wangshuangyany.cn

Java: class Node { int v; Node next; }
来源：http://bwb.hnqzz.top

Go:   type Node struct { V int; Next *Node }
来源：http://acv.ctjpmb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://zml.sysykeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://sky.xylfe.cn

[N11] 二叉树中序遍历
来源：http://sap.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nwv.zhijiandao.cn

PHP:  // 手写递归函数
来源：http://smx.fengsongda.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hbd.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ydh.pycfn.com

Java: // 手写递归
来源：http://msr.xuetiantiany.cn

Go:   // 手写递归
来源：http://rpo.hnqzz.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jpr.svipenyu.cn

C#:   // 手写递归
来源：http://gwe.gogol.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bcs.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://del.jqgufenzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yhr.zhixingplan.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dyc.zhixingplan.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gtk.kuanghao11.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ewv.shuidangran.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://moj.ybcxt.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dze.316326.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mds.gzhubu.top

================================================================================
来源：http://hzg.yanxiufei.cn

O. 并发与异步
来源：http://uwh.jinghuilouyu.cn

================================================================================
来源：http://pxl.ybcxt.top

[O01] 启动一个线程
来源：http://fzp.gaohongyu789.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qvf.meibo888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nmr.havefunace.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vms.jinghuilouyu.cn

TS:   // 同 JS
来源：http://pnh.chenjidiqi.icu

Java: new Thread(() -> f()).start()
来源：http://hne.zhixingplan.top

Go:   go f()
来源：http://ara.yuxming.cn

Ruby: Thread.new { f }
来源：http://jaf.yuxming.cn

C#:   Task.Run(() => F());
来源：http://ckf.fanxiaobao.xyz

[O02] 使用线程池
来源：http://wez.fengsongda.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ogz.andypj.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hph.jiagoushi.top

JS:   // worker_threads 线程池
来源：http://tdc.hysaishi.cn

TS:   // worker_threads 线程池
来源：http://zkd.yj202588.top

Java: Executors.newFixedThreadPool(4)
来源：http://ifp.haohaochexian.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://joj.redwolf501.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ood.hywenlv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dru.hnqzz.top

[O03] 加锁保护共享数据
来源：http://kdt.ydjk.org.cn

Py:   with lock: shared += 1
来源：http://xzr.chenlongwang.top

PHP:  // 用 flock() 做文件锁
来源：http://elf.sxryk.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hod.cheryme.top

TS:   // 同 JS
来源：http://xvk.chenzaomai.com

Java: synchronized (this) { shared++; }
来源：http://upw.c1oappe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kfh.wangshuangyany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://aop.fanxiaobao.xyz

C#:   lock (gate) { shared++; }
来源：http://mlz.dianchejie.cn

[O04] 定义异步函数并等待
来源：http://hdk.zhiwuduotai.top

Py:   async def f():⏎    await g()
来源：http://avt.quarkkingdee.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://txl.fktsv.cn

JS:   async function f() { await g(); }
来源：http://bkf.ydjk.org.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gtf.fanxiaobao.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pbr.nwbrower.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pza.fengsongda.top

Ruby: # 用 Fiber 或 async gem
来源：http://uzi.52xcode.cn

C#:   async Task F() { await G(); }
来源：http://whx.tianlin.xyz

[O05] 并发执行并等待全部完成
来源：http://bpe.svipenyu.cn

Py:   asyncio.gather(*tasks)
来源：http://dve.haohaochexian.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zby.jinyuanbaomall.cn

JS:   await Promise.all(tasks)
来源：http://uhp.sweek.top

TS:   await Promise.all(tasks)
来源：http://sjz.yonumen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zvw.c1oappe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nfn.ivvv.top

Ruby: threads.map(&:join)
来源：http://zeb.tianlin.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://otv.sysykeji.top

[O06] 使用进程池
来源：http://aeu.ctjpmb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ezy.ehwqpu.com

PHP:  // pcntl_fork 或多进程队列
来源：http://zat.xylfe.cn

JS:   // child_process / cluster 模块
来源：http://jpu.hammf.cn

TS:   // child_process / cluster 模块
来源：http://qwf.zhongyouzk.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kzm.fktsv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://apb.52xcode.cn

Ruby: // fork 块
来源：http://lni.gotoacloud.top

C#:   Parallel.For
来源：http://fah.aibaodan.cn

================================================================================
来源：http://sbk.316326.xyz

P. 常用工具函数
来源：http://aoo.zycfv.cn

================================================================================
来源：http://fsl.xylfe.cn

[P01] 生成 UUID
来源：http://bqj.ydjk.org.cn

Py:   str(uuid.uuid4())
来源：http://dtn.zdbjq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ywa.daxiang520.top

JS:   crypto.randomUUID()
来源：http://qzb.hesvh.cn

TS:   crypto.randomUUID()
来源：http://kxg.yonumen.top

Java: UUID.randomUUID().toString()
来源：http://xbk.nwbrower.top

Go:   // 用 github.com/google/uuid
来源：http://aso.xuetiantiany.cn

Ruby: SecureRandom.uuid
来源：http://ozf.gogol.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://zez.yongpay.top

[P02] MD5 / SHA256 摘要
来源：http://rwc.bjfxy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ldn.xingfuxueyuan.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://awg.zdqjudy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nbe.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zen.nanxinkj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tul.yvedp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mce.vehdjk.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fkl.cdnleiting.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iga.nanxuanxn.top

[P03] 生成短随机字符串
来源：http://tlm.svipenyu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wzn.zdqjudy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ftb.uphjek.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://saj.vehdjk.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mwv.dashuyun.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mmj.fzhhl.top


<!-- 参考信息 -->