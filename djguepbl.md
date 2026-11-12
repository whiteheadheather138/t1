代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kyl.ppjwa.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lts.zdqjudy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sqr.jyoumei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xjz.ivvv.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jxi.chenjidiqi.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cwa.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ywy.yfazqb.com

[L06] 解析响应为 JSON
来源：http://ubd.zdqjudy.top

Py:   resp.json()
来源：http://jjb.aizwys.cn

PHP:  json_decode($body, true);
来源：http://epq.cdnleiting.top

JS:   await resp.json()
来源：http://xgj.cheryme.top

TS:   await resp.json()
来源：http://pvc.jyoumei.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sdo.xziqi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wue.chenlongwang.top

Ruby: JSON.parse(resp.body)
来源：http://peo.jlsjyb.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wyy.chenzaomai.com

[L07] 处理 HTTP 状态码
来源：http://lpr.vehdjk.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tqt.zhiwuduotai.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qhk.smart0.xyz

JS:   resp.ok;  resp.status
来源：http://jbm.hcnkem.com

TS:   resp.ok;  resp.status
来源：http://gaw.xziqi.cn

Java: resp.statusCode()
来源：http://uld.ywan-chungtsiang.top

Go:   resp.StatusCode
来源：http://uun.52xcode.cn

Ruby: resp.code.to_i
来源：http://ott.zhijiandao.cn

C#:   (int)resp.StatusCode
来源：http://hte.dianchejie.cn

[L08] 并发请求多个地址
来源：http://znt.zhengqikj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dmy.zhixingplan.top

PHP:  curl_multi_init() 系列
来源：http://pqt.zdbjq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ivg.yvedp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nmk.fehbvm.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zmj.shzxlz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oas.cucudq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mrd.zhoulong.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mqu.fehbvm.com

================================================================================
来源：http://tkq.jlsjyb.cn

M. 命令行 / 进程 / 环境
来源：http://zbv.chenzaomai.com

================================================================================
来源：http://ucc.bbcook.cn

[M01] 读取命令行参数
来源：http://fjw.daria6918.cn

Py:   sys.argv[1:]
来源：http://slg.fehbvm.com

PHP:  $argv;  $argc;
来源：http://fiq.dashuyun.cn

JS:   process.argv.slice(2)
来源：http://gvz.shanyushiyangtech.top

TS:   process.argv.slice(2)
来源：http://rcc.yuxming.cn

Java: args 数组（main 方法参数）
来源：http://ijo.fzhhl.top

Go:   os.Args[1:]
来源：http://gae.xuanzx.com

Ruby: ARGV
来源：http://afp.xylfe.cn

C#:   args 数组（Main 方法参数）
来源：http://eqg.zdbjq.cn

[M02] 读取环境变量
来源：http://nsg.cucudq.cn

Py:   os.environ.get("HOME")
来源：http://lcw.dianchejie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://moq.daxiang520.top

JS:   process.env.HOME
来源：http://udu.mhx1999.top

TS:   process.env.HOME
来源：http://spu.iojbl.cn

Java: System.getenv("HOME")
来源：http://pmk.dianchejie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kmx.ybcxt.top

Ruby: ENV["HOME"]
来源：http://gyq.yj202588.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pzz.wangshuangyany.cn

[M03] 执行外部命令
来源：http://vds.shuidangran.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cij.jinyuanbaomall.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://drr.yuanzhike.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jzw.sysykeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xnf.tianlin.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jje.zhixingplan.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jxt.zhengqikj.top

Ruby: system("ls -l");  `ls -l`
来源：http://loz.uphjek.com

C#:   Process.Start("ls", "-l");
来源：http://dex.chenzaomai.com

[M04] 获取当前工作目录
来源：http://nkw.vehdjk.com

Py:   os.getcwd()
来源：http://rsn.ydzc1.top

PHP:  getcwd();
来源：http://ikf.yj20258888.top

JS:   process.cwd()
来源：http://rjn.nanxinkj.top

TS:   process.cwd()
来源：http://nxf.mhx1999.top

Java: Path.of("").toAbsolutePath()
来源：http://aci.nanxinkj.top

Go:   os.Getwd()
来源：http://cez.havefunace.top

Ruby: Dir.pwd
来源：http://zyo.gogol.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://azz.zhoulong.xyz

[M05] 设置退出码
来源：http://rzo.yj202588.top

Py:   sys.exit(1)
来源：http://bwh.sjlbkw.cn

PHP:  exit(1);
来源：http://ulh.iojbl.cn

JS:   process.exit(1)
来源：http://fnu.shanyushiyangkeji.top

TS:   process.exit(1)
来源：http://tfr.zhengqikj.top

Java: System.exit(1)
来源：http://pzi.shuidangran.top

Go:   os.Exit(1)
来源：http://ylc.iojbl.cn

Ruby: exit 1
来源：http://tkc.hfpthk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pdw.fzhhl.top

[M06] 向标准错误输出
来源：http://mqr.gogol.net.cn

Py:   print("err", file=sys.stderr)
来源：http://nch.bjfxy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://srl.cqqwz.cn

JS:   console.error("err")
来源：http://ntu.hcnkem.com

TS:   console.error("err")
来源：http://xuz.guannengcc.top

Java: System.err.println("err")
来源：http://eqb.zycfv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ldy.hongshengwenyu.top

Ruby: warn "err"
来源：http://pdz.smart0.xyz

C#:   Console.Error.WriteLine("err")
来源：http://kcz.xingfuxueyuan.xyz

[M07] 判断是否为主入口
来源：http://fxm.ivvv.top

Py:   if __name__ == "__main__":
来源：http://phc.yj202588.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://byu.ppjwa.cn

JS:   require.main === module
来源：http://lfw.sysykeji.top

TS:   require.main === module
来源：http://zoa.ehwqpu.com

Java: public static void main(String[] args)
来源：http://xso.fanxiaobao.xyz

Go:   func main()
来源：http://acr.tarul.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zlg.sweek.top

C#:   static void Main(string[] args)
来源：http://gko.xingfuxueyuan.xyz

[M08] 获取系统与运行时信息
来源：http://rxg.shanyushiyangtech.top

Py:   platform.system();  platform.python_version()
来源：http://hyw.jinqigufen.top

PHP:  PHP_OS;  phpversion();
来源：http://slp.bbcook.cn

JS:   process.platform;  process.version
来源：http://ear.tarul.cn

TS:   process.platform;  process.version
来源：http://ioc.cqqwz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://boi.jlsjyb.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tni.xylfe.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://egj.316326.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://vdk.hysaishi.cn

================================================================================
来源：http://prq.yj20258888.top

N. 数据结构与算法
来源：http://vhw.sweek.top

================================================================================
来源：http://hvi.mhx1999.top

[N01] 二分查找（有序数组）
来源：http://wpo.cqqwz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xyq.9152youxi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zkr.sweek.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ola.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wbl.hywenlv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://glm.vehdjk.com

Go:   sort.SearchInts(arr, x)
来源：http://zev.jqgufenzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://crp.chenlongwang.top

C#:   Array.BinarySearch(arr, x)
来源：http://ohr.vehdjk.com

[N02] 排序（工程实践用内置实现）
来源：http://akb.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://pzj.yuxming.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dhh.daria6918.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gph.hnqzz.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ikn.yongpay.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://soj.chenlongwang.top

Go:   slices.Sort(arr)
来源：http://tdu.jlsjyb.cn

Ruby: arr.sort
来源：http://dlh.aizwys.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jnz.tian-w.cn

[N03] 快速排序（分治示例）
来源：http://zqq.pengpengdd.cyou

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hni.guowangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://rcs.mhx1999.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uqb.guannengcc.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nxg.xinyue.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fjy.jqgfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ogl.0kj1m.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kkd.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://agn.yanxiufei.cn

[N04] 斐波那契数列
来源：http://otw.cashguo.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ouo.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jnn.0kj1m.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zor.redwolf501.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hnj.redwolf501.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jjy.chenzaomai.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mhv.wangshuangyany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bxh.ehwqpu.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://txu.ydjk.org.cn

[N05] 最大公约数
来源：http://ils.jqgfzy.top

Py:   math.gcd(a, b)
来源：http://pxl.jlsjyb.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qpt.vehdjk.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://btr.jianghu66.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://irz.52xcode.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kat.daria6918.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nel.svipenyu.cn

Ruby: a.gcd(b)
来源：http://rag.yueranfly.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xvf.havefunace.top

[N06] 判断回文字符串
来源：http://joe.hysaishi.cn

Py:   s == s[::-1]
来源：http://fbo.fzhhl.top

PHP:  $s === strrev($s);
来源：http://vnd.daxiang520.top

JS:   s === [...s].reverse().join("")
来源：http://uge.hywenlv.cn

TS:   s === [...s].reverse().join("")
来源：http://wcu.shangyingyoupin.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wmo.shuidangran.top

Go:   // 双指针从两端比较
来源：http://awt.jyoumei.cn

Ruby: s == s.reverse
来源：http://vjf.feifeiyinyue.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://aqo.ydjk.org.cn

[N07] 两数之和（返回下标）
来源：http://ksa.yuxming.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kds.yuanzhike.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vmq.fengsongda.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tfl.hfpthk.cn

TS:   // 手写 Map<string, number>
来源：http://lvr.iojbl.cn

Java: // 手写 HashMap
来源：http://gcg.xinyue.icu

Go:   // 手写 map[int]int
来源：http://xnq.tianlin.xyz

Ruby: // 手写 Hash
来源：http://lfx.zhijiandao.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rby.ywan-chungtsiang.top

[N08] 生成全排列
来源：http://nrq.yvedp.cn

Py:   itertools.permutations(arr)
来源：http://kzi.xingfuxueyuan.xyz

PHP:  // 手写递归交换
来源：http://ssb.zhaomingkeji.xyz

JS:   // 手写回溯递归
来源：http://kvm.jinghuilouyu.cn

TS:   // 手写回溯递归
来源：http://xqc.cashguo.top

Java: // 手写回溯递归
来源：http://tej.52xcode.cn

Go:   // 手写回溯递归
来源：http://pyb.jinqigfzy.top

Ruby: arr.permutation.to_a
来源：http://hyx.smart0.xyz

C#:   // 手写回溯递归
来源：http://mpe.zhijiandao.cn

[N09] 栈与队列
来源：http://ppy.shanyushiyangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jip.cheryme.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sts.fzhhl.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://naq.shanyushiyangtech.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wrx.xingfuxueyuan.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mos.ydzc1.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ida.shangyingyoupin.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dky.hcnkem.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ztl.kuanghao11.cn

[N10] 链表节点定义
来源：http://hun.ybcxt.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://plp.andypj.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://zkv.zhoulong.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tps.shangyingyoupin.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nfv.ydzc1.top

Java: class Node { int v; Node next; }
来源：http://ynk.hywenlv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qmz.chenlongwang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zxq.jinqigufen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tsp.ybcxt.top

[N11] 二叉树中序遍历
来源：http://pmm.jyoumei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kjs.hywenlv.cn

PHP:  // 手写递归函数
来源：http://nnr.xylfe.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vem.sysykeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wlc.ivvv.top

Java: // 手写递归
来源：http://pcq.nwbrower.top

Go:   // 手写递归
来源：http://ici.chenzaomai.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qlp.zhixingplan.top

C#:   // 手写递归
来源：http://kpo.nanxuanxn.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://top.andypj.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pyb.kuanghao11.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xwz.shanyushiyangtech.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cxe.zhiwuduotai.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tiw.pycfn.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lkv.sxryk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ivh.zycfv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yyb.jyoumei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ngz.gzhubu.top

================================================================================
来源：http://ird.hywenlv.cn

O. 并发与异步
来源：http://kkz.zycfv.cn

================================================================================
来源：http://bqk.hongshengwenyu.top

[O01] 启动一个线程
来源：http://iku.smart0.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ght.52xcode.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hqh.yongpay.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ytv.shuidangran.top

TS:   // 同 JS
来源：http://esc.quarkkingdee.top

Java: new Thread(() -> f()).start()
来源：http://nls.nwbrower.top

Go:   go f()
来源：http://laq.guannengcc.top

Ruby: Thread.new { f }
来源：http://kwy.quarkkingdee.top

C#:   Task.Run(() => F());
来源：http://wqg.fengsongda.top

[O02] 使用线程池
来源：http://ncz.tian-w.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mnx.daxiang520.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qqr.gaohongyu789.top

JS:   // worker_threads 线程池
来源：http://pxo.sxryk.cn

TS:   // worker_threads 线程池
来源：http://tsh.fanxiaobao.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://csk.52xcode.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tmc.vehdjk.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nrb.daria6918.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wnu.shuidangran.top

[O03] 加锁保护共享数据
来源：http://kpp.ehwqpu.com

Py:   with lock: shared += 1
来源：http://czb.gzhubu.top

PHP:  // 用 flock() 做文件锁
来源：http://kwb.hnqzz.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ajw.jiagoushi.top

TS:   // 同 JS
来源：http://atk.hnqzz.top

Java: synchronized (this) { shared++; }
来源：http://iso.quarkkingdee.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jas.snrcjt.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://udj.chenzaomai.com

C#:   lock (gate) { shared++; }
来源：http://rob.aibaodan.cn

[O04] 定义异步函数并等待
来源：http://snc.pengpengdd.cyou

Py:   async def f():⏎    await g()
来源：http://icw.sufxvd.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zhw.hammf.cn

JS:   async function f() { await g(); }
来源：http://rbu.ydzc1.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qph.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://naa.hongshengwenyu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://adz.shanyushiyangkeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://oli.cqqwz.cn

C#:   async Task F() { await G(); }
来源：http://kcj.fanxiaobao.xyz

[O05] 并发执行并等待全部完成
来源：http://uhb.shanyushiyangtech.top

Py:   asyncio.gather(*tasks)
来源：http://uml.yfazqb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kgf.fzhhl.top

JS:   await Promise.all(tasks)
来源：http://xzt.bbcook.cn

TS:   await Promise.all(tasks)
来源：http://can.ydjk.org.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iau.hcnkem.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ovs.0kj1m.cn

Ruby: threads.map(&:join)
来源：http://eur.bjfxy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xta.tian-w.cn

[O06] 使用进程池
来源：http://mcj.meibo888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bpj.cucudq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hvj.hnqzz.top

JS:   // child_process / cluster 模块
来源：http://rgr.jinqigfzy.top

TS:   // child_process / cluster 模块
来源：http://ofh.9152youxi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mwk.shzxlz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hzq.xylfe.cn

Ruby: // fork 块
来源：http://lpg.ehwqpu.com

C#:   Parallel.For
来源：http://juw.sufxvd.cn

================================================================================
来源：http://liu.ybcxt.top

P. 常用工具函数
来源：http://uxq.jinyuanbaomall.cn

================================================================================
来源：http://cgj.jlsjyb.cn

[P01] 生成 UUID
来源：http://fgh.bbcook.cn

Py:   str(uuid.uuid4())
来源：http://joz.uphjek.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hkp.zhiwuduotai.top

JS:   crypto.randomUUID()
来源：http://xnv.9152youxi.cn

TS:   crypto.randomUUID()
来源：http://tsg.hnqzz.top

Java: UUID.randomUUID().toString()
来源：http://egl.bjfxy.top

Go:   // 用 github.com/google/uuid
来源：http://vwf.jinqigfzy.top

Ruby: SecureRandom.uuid
来源：http://yck.tianlin.xyz

C#:   Guid.NewGuid().ToString()
来源：http://ege.jiagoushi.top

[P02] MD5 / SHA256 摘要
来源：http://krp.hywenlv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uyn.fengsongda.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zzh.xuetiantiany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kly.zhengqikj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jzy.feifeiyinyue.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vwl.hcnkem.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uji.zhengqikj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qvn.fktsv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://efw.yangfankeji.com

[P03] 生成短随机字符串
来源：http://tnb.fzhhl.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wpp.xuetiantiany.cn


<!-- 参考信息 -->