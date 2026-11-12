代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jgd.dianchejie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gjz.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tsq.ehwqpu.com

[L06] 解析响应为 JSON
来源：http://hpt.hfpthk.cn

Py:   resp.json()
来源：http://fym.aizwys.cn

PHP:  json_decode($body, true);
来源：http://cca.chenlongwang.top

JS:   await resp.json()
来源：http://nkm.tanke756.top

TS:   await resp.json()
来源：http://lfw.zhiwuduotai.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zgc.ctjpmb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hvc.redwolf501.top

Ruby: JSON.parse(resp.body)
来源：http://gmo.tianlin.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wvo.gogol.net.cn

[L07] 处理 HTTP 状态码
来源：http://stw.guowangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hjq.zdqjudy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mrd.chenjidiqi.icu

JS:   resp.ok;  resp.status
来源：http://zel.xziqi.cn

TS:   resp.ok;  resp.status
来源：http://bad.dianchejie.cn

Java: resp.statusCode()
来源：http://vuk.zhongyouzk.top

Go:   resp.StatusCode
来源：http://dag.xuanzx.com

Ruby: resp.code.to_i
来源：http://zfc.zhongyouzk.top

C#:   (int)resp.StatusCode
来源：http://lip.cqqwz.cn

[L08] 并发请求多个地址
来源：http://ewp.9152youxi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nno.jinqigfzy.top

PHP:  curl_multi_init() 系列
来源：http://fat.quarkkingdee.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rdn.yueranfly.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qzb.jiagoushi.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rzi.tarul.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zix.yvedp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ocj.uphjek.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://epv.meibo888.top

================================================================================
来源：http://syr.jyoumei.cn

M. 命令行 / 进程 / 环境
来源：http://xym.gogol.net.cn

================================================================================
来源：http://rns.tian-w.cn

[M01] 读取命令行参数
来源：http://yzm.nanxuanxn.top

Py:   sys.argv[1:]
来源：http://qow.xuetiantiany.cn

PHP:  $argv;  $argc;
来源：http://jza.xinyue.icu

JS:   process.argv.slice(2)
来源：http://wgf.jqgfzy.top

TS:   process.argv.slice(2)
来源：http://zyy.gzhubu.top

Java: args 数组（main 方法参数）
来源：http://nlx.nanxinkj.top

Go:   os.Args[1:]
来源：http://oyc.yuanzhike.top

Ruby: ARGV
来源：http://tgv.zhixingplan.top

C#:   args 数组（Main 方法参数）
来源：http://avr.jianghu66.top

[M02] 读取环境变量
来源：http://hlm.uphjek.com

Py:   os.environ.get("HOME")
来源：http://mjd.hywenlv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ylm.jinqigfzy.top

JS:   process.env.HOME
来源：http://fis.cdnleiting.top

TS:   process.env.HOME
来源：http://ted.shangyingyoupin.top

Java: System.getenv("HOME")
来源：http://ncz.xziqi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gfd.jinqigfzy.top

Ruby: ENV["HOME"]
来源：http://qxx.birdmap.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uhj.fengsongda.top

[M03] 执行外部命令
来源：http://hfy.daxiang520.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zkf.daxiang520.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xcr.uphjek.com

JS:   child_process.execSync("ls -l").toString()
来源：http://moi.zhoulong.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://pwz.shuidangran.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://btz.zhijiandao.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pcz.yuanzhike.top

Ruby: system("ls -l");  `ls -l`
来源：http://tmx.jqgufenzy.top

C#:   Process.Start("ls", "-l");
来源：http://ydc.jinyuanbaomall.cn

[M04] 获取当前工作目录
来源：http://fto.ehwqpu.com

Py:   os.getcwd()
来源：http://gll.cdnleiting.top

PHP:  getcwd();
来源：http://fhy.sufxvd.cn

JS:   process.cwd()
来源：http://nyg.tanke756.top

TS:   process.cwd()
来源：http://zxg.hnxiangtu.top

Java: Path.of("").toAbsolutePath()
来源：http://prg.zhaomingkeji.xyz

Go:   os.Getwd()
来源：http://yzb.guowangkeji.top

Ruby: Dir.pwd
来源：http://sln.wangdashe.top

C#:   Directory.GetCurrentDirectory()
来源：http://awp.cdnleiting.top

[M05] 设置退出码
来源：http://zxb.hammf.cn

Py:   sys.exit(1)
来源：http://fns.cdnleiting.top

PHP:  exit(1);
来源：http://jrh.yfazqb.com

JS:   process.exit(1)
来源：http://cfo.uphjek.com

TS:   process.exit(1)
来源：http://yit.epnwcf.com

Java: System.exit(1)
来源：http://lrm.redwolf501.top

Go:   os.Exit(1)
来源：http://nrq.c1oappe.top

Ruby: exit 1
来源：http://odl.jianghu66.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nuw.xziqi.cn

[M06] 向标准错误输出
来源：http://qkf.uphjek.com

Py:   print("err", file=sys.stderr)
来源：http://ckq.smart0.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://xaq.guowangkeji.top

JS:   console.error("err")
来源：http://tll.epnwcf.com

TS:   console.error("err")
来源：http://fzn.nanxuanxn.top

Java: System.err.println("err")
来源：http://hoy.hcnkem.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kdj.mhx1999.top

Ruby: warn "err"
来源：http://gnr.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://erh.ybcxt.top

[M07] 判断是否为主入口
来源：http://nfe.yonumen.top

Py:   if __name__ == "__main__":
来源：http://xzn.gzhubu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rgf.nwbrower.top

JS:   require.main === module
来源：http://qic.jqgfzy.top

TS:   require.main === module
来源：http://bza.jqgufenzy.top

Java: public static void main(String[] args)
来源：http://vbs.epnwcf.com

Go:   func main()
来源：http://jrf.zhongyouzk.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vzc.cashguo.top

C#:   static void Main(string[] args)
来源：http://trm.daria6918.cn

[M08] 获取系统与运行时信息
来源：http://yrj.sufxvd.cn

Py:   platform.system();  platform.python_version()
来源：http://hia.52xcode.cn

PHP:  PHP_OS;  phpversion();
来源：http://mke.52xcode.cn

JS:   process.platform;  process.version
来源：http://yii.gotoacloud.top

TS:   process.platform;  process.version
来源：http://afb.ctjpmb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lve.wangshuangyany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zfd.cashguo.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rjz.gaohongyu789.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lin.ehwqpu.com

================================================================================
来源：http://enm.zhixingplan.top

N. 数据结构与算法
来源：http://lpe.hesvh.cn

================================================================================
来源：http://lyg.birdmap.top

[N01] 二分查找（有序数组）
来源：http://nju.jianghu66.top

Py:   bisect.bisect_left(arr, x)
来源：http://vnf.zycfv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kaa.meibo888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fag.tarul.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://egq.yangfankeji.com

Java: Arrays.binarySearch(arr, x)
来源：http://trh.yj20258.top

Go:   sort.SearchInts(arr, x)
来源：http://lrt.hywenlv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hzx.xuetiantiany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mlb.jinqigfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://boc.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://qmb.mhx1999.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cko.zycfv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hdm.svipenyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xhh.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://puf.jinqigufen.top

Go:   slices.Sort(arr)
来源：http://yxk.sufxvd.cn

Ruby: arr.sort
来源：http://bmt.jianghu66.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://evk.daxiang520.top

[N03] 快速排序（分治示例）
来源：http://qqw.yuxming.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://udy.bjfxy.top

PHP:  // 递归实现，或用 usort
来源：http://wji.gaohongyu789.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ujx.jqgufenzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wih.hesvh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xud.gaohongyu789.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pcg.0kj1m.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ooy.ybcxt.top

C#:   // 手写递归，或 Array.Sort
来源：http://dvf.daxiang520.top

[N04] 斐波那契数列
来源：http://kyv.chenlongwang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ehk.tian-w.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://owk.hnxiangtu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zhx.jyoumei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hou.shangyingyoupin.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ylg.bjfxy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://emr.tian-w.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vur.guowangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jdy.shangyingyoupin.top

[N05] 最大公约数
来源：http://ouy.tarul.cn

Py:   math.gcd(a, b)
来源：http://doe.zhixingplan.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gsb.daxiang520.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dvq.yj20258.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://csh.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eed.aibaodan.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kxt.vehdjk.com

Ruby: a.gcd(b)
来源：http://nrs.yj20258.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wum.jinyuanbaomall.cn

[N06] 判断回文字符串
来源：http://tvf.0kj1m.cn

Py:   s == s[::-1]
来源：http://xxh.ydjk.org.cn

PHP:  $s === strrev($s);
来源：http://jmh.yanxiufei.cn

JS:   s === [...s].reverse().join("")
来源：http://xan.0kj1m.cn

TS:   s === [...s].reverse().join("")
来源：http://hqo.c1oappe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gfw.xylfe.cn

Go:   // 双指针从两端比较
来源：http://ytb.316326.xyz

Ruby: s == s.reverse
来源：http://jax.yuxming.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ujb.sxryk.cn

[N07] 两数之和（返回下标）
来源：http://unz.yfazqb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rzg.yj20258.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ijc.gaohongyu789.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jvd.xuanzx.com

TS:   // 手写 Map<string, number>
来源：http://rdu.sweek.top

Java: // 手写 HashMap
来源：http://iug.yuanzhike.top

Go:   // 手写 map[int]int
来源：http://naf.nanxuanxn.top

Ruby: // 手写 Hash
来源：http://gvy.meibo888.top

C#:   // 手写 Dictionary<int, int>
来源：http://ini.zhiwuduotai.top

[N08] 生成全排列
来源：http://fhy.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://mhb.gzhubu.top

PHP:  // 手写递归交换
来源：http://sag.gotoacloud.top

JS:   // 手写回溯递归
来源：http://ggj.bjfxy.top

TS:   // 手写回溯递归
来源：http://oxa.guannengcc.top

Java: // 手写回溯递归
来源：http://ygb.svipenyu.cn

Go:   // 手写回溯递归
来源：http://jph.daria6918.cn

Ruby: arr.permutation.to_a
来源：http://zsw.bbcook.cn

C#:   // 手写回溯递归
来源：http://sik.redwolf501.top

[N09] 栈与队列
来源：http://nug.cdnleiting.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nsv.shanyushiyangkeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kuw.hcnkem.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mpq.yj202588.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oaq.yueranfly.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ivj.cqqwz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dlc.cashguo.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zrb.yj202588.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://twr.xinyue.icu

[N10] 链表节点定义
来源：http://txm.epnwcf.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tmn.feifeiyinyue.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kti.tianlin.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://suy.jiagoushi.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bkf.chenzaomai.com

Java: class Node { int v; Node next; }
来源：http://xjp.gogol.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zfa.dashuyun.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kyb.quarkkingdee.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lrq.aizwys.cn

[N11] 二叉树中序遍历
来源：http://rmr.ydjk.org.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ybx.aizwys.cn

PHP:  // 手写递归函数
来源：http://bfi.zhiwuduotai.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rub.snrcjt.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hhy.uphjek.com

Java: // 手写递归
来源：http://epp.316326.xyz

Go:   // 手写递归
来源：http://war.sufxvd.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qpa.redwolf501.top

C#:   // 手写递归
来源：http://fwb.zhengqikj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://klw.sweek.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ajg.jinqigfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kka.yvedp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://snz.yueranfly.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dgi.pycfn.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vsr.yangfankeji.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jex.nanxuanxn.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eid.ywan-chungtsiang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bqo.xinyue.icu

================================================================================
来源：http://qfh.xuetiantiany.cn

O. 并发与异步
来源：http://tnz.cqqwz.cn

================================================================================
来源：http://ozw.dianchejie.cn

[O01] 启动一个线程
来源：http://wzp.dashuyun.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vuv.hesvh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xnz.xziqi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tru.jiagoushi.top

TS:   // 同 JS
来源：http://xic.guowangkeji.top

Java: new Thread(() -> f()).start()
来源：http://mzl.zdqjudy.top

Go:   go f()
来源：http://hod.sxryk.cn

Ruby: Thread.new { f }
来源：http://uls.kuanghao11.cn

C#:   Task.Run(() => F());
来源：http://oaq.pengpengdd.cyou

[O02] 使用线程池
来源：http://gnu.vehdjk.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vlt.0kj1m.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vph.guannengcc.top

JS:   // worker_threads 线程池
来源：http://eqx.dashuyun.cn

TS:   // worker_threads 线程池
来源：http://fcp.snrcjt.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oil.jinyuanbaomall.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dam.guannengcc.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://naw.mhx1999.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zpm.quarkkingdee.top

[O03] 加锁保护共享数据
来源：http://ufl.zhixingplan.top

Py:   with lock: shared += 1
来源：http://okh.jqgfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://bnl.jqgufenzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mlk.quarkkingdee.top

TS:   // 同 JS
来源：http://upf.yonumen.top

Java: synchronized (this) { shared++; }
来源：http://dyl.jianghu66.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vup.ctjpmb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://lyt.hnxiangtu.top

C#:   lock (gate) { shared++; }
来源：http://jmw.yangfankeji.com

[O04] 定义异步函数并等待
来源：http://dzm.xziqi.cn

Py:   async def f():⏎    await g()
来源：http://ntl.mhx1999.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ige.zycfv.cn

JS:   async function f() { await g(); }
来源：http://vvq.hysaishi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bss.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fmd.nwbrower.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rha.shangyingyoupin.top

Ruby: # 用 Fiber 或 async gem
来源：http://bjz.jiagoushi.top

C#:   async Task F() { await G(); }
来源：http://nux.tianlin.xyz

[O05] 并发执行并等待全部完成
来源：http://xav.ybcxt.top

Py:   asyncio.gather(*tasks)
来源：http://qrq.cdnleiting.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sxo.hfpthk.cn

JS:   await Promise.all(tasks)
来源：http://fyg.yuxming.cn

TS:   await Promise.all(tasks)
来源：http://vep.nanxinkj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wvu.ehwqpu.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lio.jinyuanbaomall.cn

Ruby: threads.map(&:join)
来源：http://ybu.aizwys.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wpz.jinqigufen.top

[O06] 使用进程池
来源：http://ljo.jqgfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fbz.guannengcc.top

PHP:  // pcntl_fork 或多进程队列
来源：http://npt.zhijiandao.cn

JS:   // child_process / cluster 模块
来源：http://jho.shanyushiyangkeji.top

TS:   // child_process / cluster 模块
来源：http://tgk.snrcjt.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://msa.zdbjq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://guc.sysykeji.top

Ruby: // fork 块
来源：http://wzh.svipenyu.cn

C#:   Parallel.For
来源：http://nsf.yangfankeji.com

================================================================================
来源：http://vbb.zhengqikj.top

P. 常用工具函数
来源：http://zhd.fzhhl.top

================================================================================
来源：http://jij.gogol.net.cn

[P01] 生成 UUID
来源：http://wqh.quarkkingdee.top

Py:   str(uuid.uuid4())
来源：http://uld.vehdjk.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yrc.jiagoushi.top

JS:   crypto.randomUUID()
来源：http://mho.fanxiaobao.xyz

TS:   crypto.randomUUID()
来源：http://ifp.yangfankeji.com

Java: UUID.randomUUID().toString()
来源：http://qzk.fanxiaobao.xyz

Go:   // 用 github.com/google/uuid
来源：http://lyl.xinyue.icu

Ruby: SecureRandom.uuid
来源：http://yyu.xziqi.cn

C#:   Guid.NewGuid().ToString()
来源：http://mky.zhijiandao.cn

[P02] MD5 / SHA256 摘要
来源：http://wts.c1oappe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mvo.wangshuangyany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ssh.fanxiaobao.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fgz.ybcxt.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jek.wangdashe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yyq.haohaochexian.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yum.yanxiufei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mws.nanxuanxn.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qge.shanyushiyangtech.top

[P03] 生成短随机字符串
来源：http://dlc.nwbrower.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rjg.hnqzz.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bmn.jinyuanbaomall.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vwo.yuxming.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xrr.dianchejie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ldu.zdqjudy.top


<!-- 参考信息 -->