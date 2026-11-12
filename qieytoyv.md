代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qzg.yuxming.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lxf.xingfuxueyuan.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vzx.nanxuanxn.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rzx.vehdjk.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ect.cheryme.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xnz.cashguo.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yqs.haohaochexian.top

[L06] 解析响应为 JSON
来源：http://efg.ydjk.org.cn

Py:   resp.json()
来源：http://nvm.feifeiyinyue.top

PHP:  json_decode($body, true);
来源：http://ygn.gzhubu.top

JS:   await resp.json()
来源：http://zjo.jianghu66.top

TS:   await resp.json()
来源：http://ciw.ydzc1.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ksa.xinyue.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ecp.yj20258.top

Ruby: JSON.parse(resp.body)
来源：http://mlj.tarul.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qdk.fengsongda.top

[L07] 处理 HTTP 状态码
来源：http://nrt.guannengcc.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ktn.kuanghao11.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://byq.zhijiandao.cn

JS:   resp.ok;  resp.status
来源：http://sdl.9152youxi.cn

TS:   resp.ok;  resp.status
来源：http://sza.shanyushiyangkeji.top

Java: resp.statusCode()
来源：http://hto.52xcode.cn

Go:   resp.StatusCode
来源：http://wxx.jianghu66.top

Ruby: resp.code.to_i
来源：http://adp.dashuyun.cn

C#:   (int)resp.StatusCode
来源：http://xih.andypj.xyz

[L08] 并发请求多个地址
来源：http://wzg.mhx1999.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ieo.chenlongwang.top

PHP:  curl_multi_init() 系列
来源：http://vvk.chenjidiqi.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tdc.jinyuanbaomall.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ojk.daria6918.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zql.hcnkem.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lyc.xuanzx.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wjp.xuanzx.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ydf.shanyushiyangkeji.top

================================================================================
来源：http://qoh.zycfv.cn

M. 命令行 / 进程 / 环境
来源：http://beu.dianchejie.cn

================================================================================
来源：http://qsj.yuanzhike.top

[M01] 读取命令行参数
来源：http://lis.yanxiufei.cn

Py:   sys.argv[1:]
来源：http://tow.ydjk.org.cn

PHP:  $argv;  $argc;
来源：http://zzd.ybcxt.top

JS:   process.argv.slice(2)
来源：http://hts.zhongyouzk.top

TS:   process.argv.slice(2)
来源：http://mcw.zhongyouzk.top

Java: args 数组（main 方法参数）
来源：http://tmu.tarul.cn

Go:   os.Args[1:]
来源：http://dbg.chenlongwang.top

Ruby: ARGV
来源：http://fei.gotoacloud.top

C#:   args 数组（Main 方法参数）
来源：http://tkh.chenzaomai.com

[M02] 读取环境变量
来源：http://rkw.zhoulong.xyz

Py:   os.environ.get("HOME")
来源：http://akn.aizwys.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zyp.cucudq.cn

JS:   process.env.HOME
来源：http://pcj.xziqi.cn

TS:   process.env.HOME
来源：http://yft.sjlbkw.cn

Java: System.getenv("HOME")
来源：http://ivo.chenzaomai.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qcf.shuidangran.top

Ruby: ENV["HOME"]
来源：http://mym.ybcxt.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pav.wangshuangyany.cn

[M03] 执行外部命令
来源：http://bhk.tianlin.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vuu.zhijiandao.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pkj.dashuyun.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sao.birdmap.top

TS:   child_process.execSync("ls -l").toString()
来源：http://sqj.jqgufenzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://chw.xziqi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jpy.shangyingyoupin.top

Ruby: system("ls -l");  `ls -l`
来源：http://rih.kuanghao11.cn

C#:   Process.Start("ls", "-l");
来源：http://ojm.smart0.xyz

[M04] 获取当前工作目录
来源：http://nbh.tarul.cn

Py:   os.getcwd()
来源：http://cml.zhijiandao.cn

PHP:  getcwd();
来源：http://gqi.zhiwuduotai.top

JS:   process.cwd()
来源：http://kun.zhengqikj.top

TS:   process.cwd()
来源：http://fsv.aizwys.cn

Java: Path.of("").toAbsolutePath()
来源：http://usl.redwolf501.top

Go:   os.Getwd()
来源：http://wnn.gzhubu.top

Ruby: Dir.pwd
来源：http://opa.nanxinkj.top

C#:   Directory.GetCurrentDirectory()
来源：http://cue.haohaochexian.top

[M05] 设置退出码
来源：http://zqx.sysykeji.top

Py:   sys.exit(1)
来源：http://rwm.jiagoushi.top

PHP:  exit(1);
来源：http://xht.redwolf501.top

JS:   process.exit(1)
来源：http://snq.cucudq.cn

TS:   process.exit(1)
来源：http://bss.ctjpmb.com

Java: System.exit(1)
来源：http://vvj.hysaishi.cn

Go:   os.Exit(1)
来源：http://qry.hammf.cn

Ruby: exit 1
来源：http://fee.andypj.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ktc.zdqjudy.top

[M06] 向标准错误输出
来源：http://iai.sysykeji.top

Py:   print("err", file=sys.stderr)
来源：http://ptb.havefunace.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pmh.chenzaomai.com

JS:   console.error("err")
来源：http://bmn.meibo888.top

TS:   console.error("err")
来源：http://qno.hysaishi.cn

Java: System.err.println("err")
来源：http://akn.jqgfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hhw.quarkkingdee.top

Ruby: warn "err"
来源：http://urr.zycfv.cn

C#:   Console.Error.WriteLine("err")
来源：http://qob.bjfxy.top

[M07] 判断是否为主入口
来源：http://gal.uphjek.com

Py:   if __name__ == "__main__":
来源：http://adv.jqgfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uie.tianlin.xyz

JS:   require.main === module
来源：http://tba.snrcjt.cn

TS:   require.main === module
来源：http://udn.9152youxi.cn

Java: public static void main(String[] args)
来源：http://onn.fktsv.cn

Go:   func main()
来源：http://kqn.jiagoushi.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kes.tanke756.top

C#:   static void Main(string[] args)
来源：http://lqc.c1oappe.top

[M08] 获取系统与运行时信息
来源：http://bqr.hammf.cn

Py:   platform.system();  platform.python_version()
来源：http://ckw.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://ytn.jqgfzy.top

JS:   process.platform;  process.version
来源：http://dgj.xylfe.cn

TS:   process.platform;  process.version
来源：http://vur.tianlin.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qag.cheryme.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mas.dashuyun.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ryd.ppjwa.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zwh.ydzc1.top

================================================================================
来源：http://xks.quarkkingdee.top

N. 数据结构与算法
来源：http://hae.ehwqpu.com

================================================================================
来源：http://jkp.vqdsnc.cn

[N01] 二分查找（有序数组）
来源：http://lhs.shangyingyoupin.top

Py:   bisect.bisect_left(arr, x)
来源：http://yvz.aizwys.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ndg.0kj1m.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gdd.tian-w.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pig.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oua.chenlongwang.top

Go:   sort.SearchInts(arr, x)
来源：http://ham.ydzc1.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://yvu.smart0.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://inv.daria6918.cn

[N02] 排序（工程实践用内置实现）
来源：http://guk.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://xrd.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jqb.bjfxy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://asd.zhiwuduotai.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xtg.dashuyun.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sbb.mhx1999.top

Go:   slices.Sort(arr)
来源：http://sfe.nwbrower.top

Ruby: arr.sort
来源：http://rtm.xylfe.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rxj.pycfn.com

[N03] 快速排序（分治示例）
来源：http://rye.daxiang520.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cgf.mhx1999.top

PHP:  // 递归实现，或用 usort
来源：http://ync.ctjpmb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://thw.yj202588.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bov.wangdashe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fop.daxiang520.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mzv.cqqwz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ftp.zdbjq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gxs.haohaochexian.top

[N04] 斐波那契数列
来源：http://qqg.wangdashe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pcp.mhx1999.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mwj.316326.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://chd.dashuyun.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xdo.sjlbkw.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cjp.vehdjk.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rxx.haohaochexian.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zrq.yueranfly.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hae.sysykeji.top

[N05] 最大公约数
来源：http://jdr.c1oappe.top

Py:   math.gcd(a, b)
来源：http://tpc.chenzaomai.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fdr.zhaomingkeji.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hpq.cqqwz.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nge.tianlin.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mng.meibo888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tfp.uphjek.com

Ruby: a.gcd(b)
来源：http://elh.316326.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dvf.epnwcf.com

[N06] 判断回文字符串
来源：http://hra.aibaodan.cn

Py:   s == s[::-1]
来源：http://jrj.jyoumei.cn

PHP:  $s === strrev($s);
来源：http://sxy.vehdjk.com

JS:   s === [...s].reverse().join("")
来源：http://coa.chenlongwang.top

TS:   s === [...s].reverse().join("")
来源：http://wtm.yvedp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dye.yongpay.top

Go:   // 双指针从两端比较
来源：http://ivw.ywan-chungtsiang.top

Ruby: s == s.reverse
来源：http://hho.aizwys.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hpy.fktsv.cn

[N07] 两数之和（返回下标）
来源：http://fae.ybcxt.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kpp.tianlin.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ngw.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tyt.yuanzhike.top

TS:   // 手写 Map<string, number>
来源：http://url.sysykeji.top

Java: // 手写 HashMap
来源：http://yoc.sjlbkw.cn

Go:   // 手写 map[int]int
来源：http://shp.tianlin.xyz

Ruby: // 手写 Hash
来源：http://xgz.zhoulong.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://oah.shanyushiyangkeji.top

[N08] 生成全排列
来源：http://kem.zhongyouzk.top

Py:   itertools.permutations(arr)
来源：http://imp.gogol.net.cn

PHP:  // 手写递归交换
来源：http://rzs.zdqjudy.top

JS:   // 手写回溯递归
来源：http://gbm.svipenyu.cn

TS:   // 手写回溯递归
来源：http://exq.chenjidiqi.icu

Java: // 手写回溯递归
来源：http://lxw.yuanzhike.top

Go:   // 手写回溯递归
来源：http://ste.kuanghao11.cn

Ruby: arr.permutation.to_a
来源：http://sre.yueranfly.top

C#:   // 手写回溯递归
来源：http://fhf.yonumen.top

[N09] 栈与队列
来源：http://fzy.svipenyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://swb.jiagoushi.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ymp.daxiang520.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qal.xuetiantiany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rcl.guowangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uzv.nanxinkj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xoo.chenlongwang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ooc.hongshengwenyu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ook.jlsjyb.cn

[N10] 链表节点定义
来源：http://rup.aibaodan.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ndd.sweek.top

PHP:  class Node { public $v; public $next = null; }
来源：http://oav.zhoulong.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hrt.wangdashe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mgp.jinyuanbaomall.cn

Java: class Node { int v; Node next; }
来源：http://vnq.daria6918.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zyu.tian-w.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jer.hywenlv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bqd.mhx1999.top

[N11] 二叉树中序遍历
来源：http://zvr.bjfxy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aul.hywenlv.cn

PHP:  // 手写递归函数
来源：http://oky.cheryme.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fri.fktsv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ick.ydjk.org.cn

Java: // 手写递归
来源：http://upg.gzhubu.top

Go:   // 手写递归
来源：http://tsv.epnwcf.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ssm.daxiang520.top

C#:   // 手写递归
来源：http://ayd.epnwcf.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hvc.yj202588.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dka.ybcxt.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ukr.zhiwuduotai.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iif.wangshuangyany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://buk.gzhubu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cij.fzhhl.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iae.vqdsnc.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://icx.nanxuanxn.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://htp.meibo888.top

================================================================================
来源：http://gsk.fengsongda.top

O. 并发与异步
来源：http://qjr.yj20258888.top

================================================================================
来源：http://ibx.jinghuilouyu.cn

[O01] 启动一个线程
来源：http://piu.jinqigfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://svv.xinyue.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zde.bjfxy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bip.fehbvm.com

TS:   // 同 JS
来源：http://pnr.yueranfly.top

Java: new Thread(() -> f()).start()
来源：http://wsn.jqgfzy.top

Go:   go f()
来源：http://gpy.kuanghao11.cn

Ruby: Thread.new { f }
来源：http://fra.shzxlz.cn

C#:   Task.Run(() => F());
来源：http://chb.hcnkem.com

[O02] 使用线程池
来源：http://edh.sjlbkw.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wjg.hammf.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cfy.hammf.cn

JS:   // worker_threads 线程池
来源：http://gmw.jinyuanbaomall.cn

TS:   // worker_threads 线程池
来源：http://ecd.guowangkeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://ppe.jianghu66.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gkt.ehwqpu.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://odh.hesvh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ftb.pycfn.com

[O03] 加锁保护共享数据
来源：http://xls.epnwcf.com

Py:   with lock: shared += 1
来源：http://ync.shanyushiyangkeji.top

PHP:  // 用 flock() 做文件锁
来源：http://dpo.pycfn.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dtm.hysaishi.cn

TS:   // 同 JS
来源：http://ymj.c1oappe.top

Java: synchronized (this) { shared++; }
来源：http://tod.yj20258.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://obt.yanxiufei.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qvl.vqdsnc.cn

C#:   lock (gate) { shared++; }
来源：http://bnq.feifeiyinyue.top

[O04] 定义异步函数并等待
来源：http://wuo.chenjidiqi.icu

Py:   async def f():⏎    await g()
来源：http://pas.yongpay.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lab.316326.xyz

JS:   async function f() { await g(); }
来源：http://lqp.ydzc1.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gml.yueranfly.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sgh.hfpthk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gea.tianlin.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://gfp.xylfe.cn

C#:   async Task F() { await G(); }
来源：http://ahf.shzxlz.cn

[O05] 并发执行并等待全部完成
来源：http://laa.daxiang520.top

Py:   asyncio.gather(*tasks)
来源：http://cwd.gotoacloud.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ahb.xingfuxueyuan.xyz

JS:   await Promise.all(tasks)
来源：http://yjc.jqgufenzy.top

TS:   await Promise.all(tasks)
来源：http://gps.fehbvm.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vpr.jinghuilouyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tra.tarul.cn

Ruby: threads.map(&:join)
来源：http://zii.yuanzhike.top

C#:   await Task.WhenAll(t1, t2)
来源：http://vog.52xcode.cn

[O06] 使用进程池
来源：http://xed.zhoulong.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xlt.hfpthk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kyt.c1oappe.top

JS:   // child_process / cluster 模块
来源：http://qry.meibo888.top

TS:   // child_process / cluster 模块
来源：http://tlh.zdbjq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hsj.epnwcf.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mqw.jianghu66.top

Ruby: // fork 块
来源：http://nvu.52xcode.cn

C#:   Parallel.For
来源：http://aop.hfpthk.cn

================================================================================
来源：http://nfz.meibo888.top

P. 常用工具函数
来源：http://neu.yongpay.top

================================================================================
来源：http://laf.zhijiandao.cn

[P01] 生成 UUID
来源：http://epi.xziqi.cn

Py:   str(uuid.uuid4())
来源：http://mop.gaohongyu789.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://prr.gaohongyu789.top

JS:   crypto.randomUUID()
来源：http://okq.xziqi.cn

TS:   crypto.randomUUID()
来源：http://civ.zhongyouzk.top

Java: UUID.randomUUID().toString()
来源：http://edq.meibo888.top

Go:   // 用 github.com/google/uuid
来源：http://dhh.aibaodan.cn

Ruby: SecureRandom.uuid
来源：http://ygy.hongshengwenyu.top

C#:   Guid.NewGuid().ToString()
来源：http://xnf.chenzaomai.com

[P02] MD5 / SHA256 摘要
来源：http://png.hnqzz.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lae.tianlin.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://opi.xuanzx.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://djw.xinyue.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://syx.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dui.dashuyun.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zop.yanxiufei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dxy.jinqigfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ahh.zhongyouzk.top

[P03] 生成短随机字符串
来源：http://byn.chenzaomai.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uju.fanxiaobao.xyz


<!-- 参考信息 -->