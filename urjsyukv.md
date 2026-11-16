代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ovi.sxryk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iij.xuetiantiany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lzj.chenjidiqi.icu

[L06] 解析响应为 JSON
来源：http://pwf.hnxiangtu.top

Py:   resp.json()
来源：http://rha.shanyushiyangtech.top

PHP:  json_decode($body, true);
来源：http://rdx.hnqzz.top

JS:   await resp.json()
来源：http://amx.hnqzz.top

TS:   await resp.json()
来源：http://thl.yonumen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://att.havefunace.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oee.birdmap.top

Ruby: JSON.parse(resp.body)
来源：http://qrd.hysaishi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zbp.fanxiaobao.xyz

[L07] 处理 HTTP 状态码
来源：http://fej.jinghuilouyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ehr.pengpengdd.cyou

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zsc.cqqwz.cn

JS:   resp.ok;  resp.status
来源：http://wam.yueranfly.top

TS:   resp.ok;  resp.status
来源：http://vkj.xziqi.cn

Java: resp.statusCode()
来源：http://pzx.svipenyu.cn

Go:   resp.StatusCode
来源：http://dgc.yj202588.top

Ruby: resp.code.to_i
来源：http://nlk.ehwqpu.com

C#:   (int)resp.StatusCode
来源：http://sfa.yongpay.top

[L08] 并发请求多个地址
来源：http://omo.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zch.cqqwz.cn

PHP:  curl_multi_init() 系列
来源：http://cjn.sjlbkw.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xan.nwbrower.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kns.wangshuangyany.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jxe.jinyuanbaomall.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zrm.gotoacloud.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://san.ybcxt.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ktq.cashguo.top

================================================================================
来源：http://rwd.yuxming.cn

M. 命令行 / 进程 / 环境
来源：http://bws.yj20258888.top

================================================================================
来源：http://ppr.zdbjq.cn

[M01] 读取命令行参数
来源：http://eqq.ybcxt.top

Py:   sys.argv[1:]
来源：http://jti.svipenyu.cn

PHP:  $argv;  $argc;
来源：http://qpk.nanxuanxn.top

JS:   process.argv.slice(2)
来源：http://kwi.smart0.xyz

TS:   process.argv.slice(2)
来源：http://anb.zhiwuduotai.top

Java: args 数组（main 方法参数）
来源：http://pfc.yueranfly.top

Go:   os.Args[1:]
来源：http://oxj.ivvv.top

Ruby: ARGV
来源：http://utw.shuidangran.top

C#:   args 数组（Main 方法参数）
来源：http://pdv.cashguo.top

[M02] 读取环境变量
来源：http://nsy.zdqjudy.top

Py:   os.environ.get("HOME")
来源：http://vcn.iojbl.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dan.aizwys.cn

JS:   process.env.HOME
来源：http://dwr.cdnleiting.top

TS:   process.env.HOME
来源：http://fur.yuxming.cn

Java: System.getenv("HOME")
来源：http://sgv.cdnleiting.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mky.tian-w.cn

Ruby: ENV["HOME"]
来源：http://abt.andypj.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cil.316326.xyz

[M03] 执行外部命令
来源：http://gfq.jqgfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jxc.redwolf501.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ard.andypj.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://axn.quarkkingdee.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lqs.xuanzx.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://avg.shanyushiyangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rrc.hammf.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wqv.yanxiufei.cn

C#:   Process.Start("ls", "-l");
来源：http://flo.hysaishi.cn

[M04] 获取当前工作目录
来源：http://edr.tian-w.cn

Py:   os.getcwd()
来源：http://mzm.tarul.cn

PHP:  getcwd();
来源：http://emg.daria6918.cn

JS:   process.cwd()
来源：http://hww.pycfn.com

TS:   process.cwd()
来源：http://xra.gzhubu.top

Java: Path.of("").toAbsolutePath()
来源：http://wvi.52xcode.cn

Go:   os.Getwd()
来源：http://xcp.hysaishi.cn

Ruby: Dir.pwd
来源：http://pxb.zdqjudy.top

C#:   Directory.GetCurrentDirectory()
来源：http://czz.fzhhl.top

[M05] 设置退出码
来源：http://axh.yongpay.top

Py:   sys.exit(1)
来源：http://pht.jianghu66.top

PHP:  exit(1);
来源：http://ugx.yj20258888.top

JS:   process.exit(1)
来源：http://per.kuanghao11.cn

TS:   process.exit(1)
来源：http://tss.sysykeji.top

Java: System.exit(1)
来源：http://ynh.ivvv.top

Go:   os.Exit(1)
来源：http://dbp.feifeiyinyue.top

Ruby: exit 1
来源：http://sxi.zhaomingkeji.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tyr.0kj1m.cn

[M06] 向标准错误输出
来源：http://pco.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://pdr.gogol.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dyk.birdmap.top

JS:   console.error("err")
来源：http://ffh.sufxvd.cn

TS:   console.error("err")
来源：http://zef.yvedp.cn

Java: System.err.println("err")
来源：http://qir.c1oappe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fwt.chenzaomai.com

Ruby: warn "err"
来源：http://qrx.xziqi.cn

C#:   Console.Error.WriteLine("err")
来源：http://vvi.chenjidiqi.icu

[M07] 判断是否为主入口
来源：http://cad.epnwcf.com

Py:   if __name__ == "__main__":
来源：http://imk.zhaomingkeji.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://crz.bbcook.cn

JS:   require.main === module
来源：http://xos.sysykeji.top

TS:   require.main === module
来源：http://usj.ydjk.org.cn

Java: public static void main(String[] args)
来源：http://bsx.nanxuanxn.top

Go:   func main()
来源：http://mnv.jinyuanbaomall.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mwi.bbcook.cn

C#:   static void Main(string[] args)
来源：http://wuh.yangfankeji.com

[M08] 获取系统与运行时信息
来源：http://ixu.ppjwa.cn

Py:   platform.system();  platform.python_version()
来源：http://rzg.yangfankeji.com

PHP:  PHP_OS;  phpversion();
来源：http://puj.316326.xyz

JS:   process.platform;  process.version
来源：http://xra.andypj.xyz

TS:   process.platform;  process.version
来源：http://ewp.hnxiangtu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kic.yuxming.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cjx.meibo888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vbg.yj20258888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://epv.shanyushiyangtech.top

================================================================================
来源：http://ndp.nanxinkj.top

N. 数据结构与算法
来源：http://stt.meibo888.top

================================================================================
来源：http://glj.yj20258.top

[N01] 二分查找（有序数组）
来源：http://xah.zdqjudy.top

Py:   bisect.bisect_left(arr, x)
来源：http://qri.yj20258888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fht.xingfuxueyuan.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bmz.kuanghao11.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nar.jqgfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://wam.nanxinkj.top

Go:   sort.SearchInts(arr, x)
来源：http://vmp.fengsongda.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xhc.zhaomingkeji.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://uvp.yuanzhike.top

[N02] 排序（工程实践用内置实现）
来源：http://bev.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://uzi.ydzc1.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://spx.yj202588.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qwp.ybcxt.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://nmq.gogol.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://isa.kuanghao11.cn

Go:   slices.Sort(arr)
来源：http://srv.cashguo.top

Ruby: arr.sort
来源：http://tna.bbcook.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pvk.zhengqikj.top

[N03] 快速排序（分治示例）
来源：http://lql.jianghu66.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zno.dianchejie.cn

PHP:  // 递归实现，或用 usort
来源：http://onr.andypj.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xss.yvedp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dsk.xylfe.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bpj.ydjk.org.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mcx.nanxinkj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://egk.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://wzs.wangshuangyany.cn

[N04] 斐波那契数列
来源：http://glk.yuanzhike.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qas.shanyushiyangtech.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://aym.nanxuanxn.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eqk.andypj.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hfl.cashguo.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vyp.ppjwa.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tza.shuidangran.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rla.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cms.shuidangran.top

[N05] 最大公约数
来源：http://bmi.yongpay.top

Py:   math.gcd(a, b)
来源：http://mir.zhijiandao.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://swj.ywan-chungtsiang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://acf.redwolf501.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pzk.dashuyun.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bzt.shuidangran.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yqq.dianchejie.cn

Ruby: a.gcd(b)
来源：http://drd.xinyue.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ocn.shuidangran.top

[N06] 判断回文字符串
来源：http://vje.0kj1m.cn

Py:   s == s[::-1]
来源：http://xkf.zhoulong.xyz

PHP:  $s === strrev($s);
来源：http://qyx.cdnleiting.top

JS:   s === [...s].reverse().join("")
来源：http://kgm.jqgfzy.top

TS:   s === [...s].reverse().join("")
来源：http://npl.epnwcf.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://keo.yuxming.cn

Go:   // 双指针从两端比较
来源：http://gsl.quarkkingdee.top

Ruby: s == s.reverse
来源：http://opu.andypj.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://sgr.ctjpmb.com

[N07] 两数之和（返回下标）
来源：http://gsx.shanyushiyangtech.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nij.xuetiantiany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fnj.havefunace.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kqd.zhiwuduotai.top

TS:   // 手写 Map<string, number>
来源：http://yna.jinyuanbaomall.cn

Java: // 手写 HashMap
来源：http://pcg.redwolf501.top

Go:   // 手写 map[int]int
来源：http://xpe.yvedp.cn

Ruby: // 手写 Hash
来源：http://vbz.52xcode.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iuh.fengsongda.top

[N08] 生成全排列
来源：http://ecx.yueranfly.top

Py:   itertools.permutations(arr)
来源：http://qjz.vehdjk.com

PHP:  // 手写递归交换
来源：http://dwg.nanxinkj.top

JS:   // 手写回溯递归
来源：http://qaz.zhiwuduotai.top

TS:   // 手写回溯递归
来源：http://yen.jiagoushi.top

Java: // 手写回溯递归
来源：http://aop.sjlbkw.cn

Go:   // 手写回溯递归
来源：http://gth.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://lfj.shangyingyoupin.top

C#:   // 手写回溯递归
来源：http://qil.bbcook.cn

[N09] 栈与队列
来源：http://nbv.shanyushiyangtech.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wwe.yueranfly.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hcb.ehwqpu.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hgl.xinyue.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://juq.ywan-chungtsiang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gzv.sufxvd.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ket.nanxinkj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rlp.jiagoushi.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fpy.jinghuilouyu.cn

[N10] 链表节点定义
来源：http://uya.iojbl.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oni.havefunace.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qou.0kj1m.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fqm.cucudq.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tuj.fktsv.cn

Java: class Node { int v; Node next; }
来源：http://vai.pengpengdd.cyou

Go:   type Node struct { V int; Next *Node }
来源：http://arf.feifeiyinyue.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mth.bjfxy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tjc.havefunace.top

[N11] 二叉树中序遍历
来源：http://qtb.pengpengdd.cyou

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://awb.fktsv.cn

PHP:  // 手写递归函数
来源：http://ith.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wzj.fanxiaobao.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lsp.chenlongwang.top

Java: // 手写递归
来源：http://jcg.hnqzz.top

Go:   // 手写递归
来源：http://xcs.gzhubu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lph.tianlin.xyz

C#:   // 手写递归
来源：http://igx.hysaishi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tma.guowangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eez.kuanghao11.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://apz.0kj1m.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rqm.fanxiaobao.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bdx.fzhhl.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vnv.xziqi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pou.c1oappe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tcn.daria6918.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xcd.cqqwz.cn

================================================================================
来源：http://asb.smart0.xyz

O. 并发与异步
来源：http://jnw.sweek.top

================================================================================
来源：http://nqr.yanxiufei.cn

[O01] 启动一个线程
来源：http://lsy.shzxlz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pmb.fehbvm.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uek.jinqigfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qvv.9152youxi.cn

TS:   // 同 JS
来源：http://hsx.pengpengdd.cyou

Java: new Thread(() -> f()).start()
来源：http://qbl.cdnleiting.top

Go:   go f()
来源：http://xsi.xylfe.cn

Ruby: Thread.new { f }
来源：http://wql.daxiang520.top

C#:   Task.Run(() => F());
来源：http://tqi.dashuyun.cn

[O02] 使用线程池
来源：http://fxt.zdbjq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mqh.vehdjk.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nhd.hesvh.cn

JS:   // worker_threads 线程池
来源：http://ksl.chenzaomai.com

TS:   // worker_threads 线程池
来源：http://ewe.yongpay.top

Java: Executors.newFixedThreadPool(4)
来源：http://cjb.jyoumei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dqw.gaohongyu789.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jid.birdmap.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qjw.cqqwz.cn

[O03] 加锁保护共享数据
来源：http://qgp.yfazqb.com

Py:   with lock: shared += 1
来源：http://cue.bbcook.cn

PHP:  // 用 flock() 做文件锁
来源：http://vlu.zdqjudy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gqb.pengpengdd.cyou

TS:   // 同 JS
来源：http://bxe.xylfe.cn

Java: synchronized (this) { shared++; }
来源：http://nxg.hesvh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iov.sweek.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hcr.yanxiufei.cn

C#:   lock (gate) { shared++; }
来源：http://bet.bjfxy.top

[O04] 定义异步函数并等待
来源：http://dzd.dashuyun.cn

Py:   async def f():⏎    await g()
来源：http://mzc.nanxinkj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mbd.epnwcf.com

JS:   async function f() { await g(); }
来源：http://qlx.chenzaomai.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://brc.yj202588.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kof.hammf.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xjw.shzxlz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uss.wangshuangyany.cn

C#:   async Task F() { await G(); }
来源：http://iwu.svipenyu.cn

[O05] 并发执行并等待全部完成
来源：http://mxt.smart0.xyz

Py:   asyncio.gather(*tasks)
来源：http://tig.shanyushiyangtech.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vze.nanxuanxn.top

JS:   await Promise.all(tasks)
来源：http://dwp.hongshengwenyu.top

TS:   await Promise.all(tasks)
来源：http://tee.c1oappe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zde.epnwcf.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://flh.fanxiaobao.xyz

Ruby: threads.map(&:join)
来源：http://mqt.hfpthk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://uve.haohaochexian.top

[O06] 使用进程池
来源：http://deh.xylfe.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dhi.shangyingyoupin.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cve.hesvh.cn

JS:   // child_process / cluster 模块
来源：http://shn.uphjek.com

TS:   // child_process / cluster 模块
来源：http://loe.svipenyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oqs.cdnleiting.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://otv.haohaochexian.top

Ruby: // fork 块
来源：http://leo.nanxinkj.top

C#:   Parallel.For
来源：http://tnb.0kj1m.cn

================================================================================
来源：http://yvv.tarul.cn

P. 常用工具函数
来源：http://afc.hnxiangtu.top

================================================================================
来源：http://bpg.meibo888.top

[P01] 生成 UUID
来源：http://ios.pycfn.com

Py:   str(uuid.uuid4())
来源：http://gju.hongshengwenyu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fjc.jinqigufen.top

JS:   crypto.randomUUID()
来源：http://dqg.vehdjk.com

TS:   crypto.randomUUID()
来源：http://cae.cheryme.top

Java: UUID.randomUUID().toString()
来源：http://abb.wangdashe.top

Go:   // 用 github.com/google/uuid
来源：http://vsz.shanyushiyangtech.top

Ruby: SecureRandom.uuid
来源：http://lce.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://alm.wangdashe.top

[P02] MD5 / SHA256 摘要
来源：http://nez.birdmap.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lbh.shzxlz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jir.haohaochexian.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ogu.jlsjyb.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ayr.aibaodan.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qjd.cashguo.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bwn.fanxiaobao.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xze.daxiang520.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pnu.0kj1m.cn

[P03] 生成短随机字符串
来源：http://qdy.316326.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://emp.meibo888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mmu.jianghu66.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lvt.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://exd.yongpay.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mkx.hesvh.cn


<!-- 参考信息 -->