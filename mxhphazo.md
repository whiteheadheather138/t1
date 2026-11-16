代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lbp.wangdashe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sil.52xcode.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nao.zhaomingkeji.xyz

[L06] 解析响应为 JSON
来源：http://rsw.guowangkeji.top

Py:   resp.json()
来源：http://pwl.52xcode.cn

PHP:  json_decode($body, true);
来源：http://swc.zhixingplan.top

JS:   await resp.json()
来源：http://imu.cheryme.top

TS:   await resp.json()
来源：http://gmv.cucudq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oun.hysaishi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iul.jinyuanbaomall.cn

Ruby: JSON.parse(resp.body)
来源：http://kwq.kuanghao11.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ndy.yvedp.cn

[L07] 处理 HTTP 状态码
来源：http://fkg.shanyushiyangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uze.0kj1m.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://psm.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://dmy.xziqi.cn

TS:   resp.ok;  resp.status
来源：http://wxz.zdqjudy.top

Java: resp.statusCode()
来源：http://pox.52xcode.cn

Go:   resp.StatusCode
来源：http://tml.hesvh.cn

Ruby: resp.code.to_i
来源：http://osz.jinyuanbaomall.cn

C#:   (int)resp.StatusCode
来源：http://lvf.pengpengdd.cyou

[L08] 并发请求多个地址
来源：http://eyq.hfpthk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sqh.snrcjt.cn

PHP:  curl_multi_init() 系列
来源：http://vui.jlsjyb.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tvr.yj20258.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://soe.jianghu66.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lvw.daxiang520.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ciq.yongpay.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aml.hammf.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wnm.ppjwa.cn

================================================================================
来源：http://auh.yuxming.cn

M. 命令行 / 进程 / 环境
来源：http://fds.sxryk.cn

================================================================================
来源：http://pqn.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://dkm.cdnleiting.top

Py:   sys.argv[1:]
来源：http://gyu.xuetiantiany.cn

PHP:  $argv;  $argc;
来源：http://fod.shzxlz.cn

JS:   process.argv.slice(2)
来源：http://avg.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://fhb.xylfe.cn

Java: args 数组（main 方法参数）
来源：http://uyx.fehbvm.com

Go:   os.Args[1:]
来源：http://zam.cucudq.cn

Ruby: ARGV
来源：http://ddf.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://svv.jinqigufen.top

[M02] 读取环境变量
来源：http://okh.kuanghao11.cn

Py:   os.environ.get("HOME")
来源：http://urh.fzhhl.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yyu.jinqigufen.top

JS:   process.env.HOME
来源：http://ajp.xuanzx.com

TS:   process.env.HOME
来源：http://hjo.daxiang520.top

Java: System.getenv("HOME")
来源：http://zrp.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wmi.yj20258.top

Ruby: ENV["HOME"]
来源：http://wej.gogol.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jpj.sysykeji.top

[M03] 执行外部命令
来源：http://sig.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mem.0kj1m.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kxz.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://axv.shanyushiyangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wfg.yuanzhike.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tnt.xingfuxueyuan.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://jdm.c1oappe.top

Ruby: system("ls -l");  `ls -l`
来源：http://ljs.snrcjt.cn

C#:   Process.Start("ls", "-l");
来源：http://gzb.zhaomingkeji.xyz

[M04] 获取当前工作目录
来源：http://gim.kuanghao11.cn

Py:   os.getcwd()
来源：http://fwi.guowangkeji.top

PHP:  getcwd();
来源：http://mzi.chenzaomai.com

JS:   process.cwd()
来源：http://oqi.9152youxi.cn

TS:   process.cwd()
来源：http://kzy.feifeiyinyue.top

Java: Path.of("").toAbsolutePath()
来源：http://zao.52xcode.cn

Go:   os.Getwd()
来源：http://vkt.nanxuanxn.top

Ruby: Dir.pwd
来源：http://ibg.hongshengwenyu.top

C#:   Directory.GetCurrentDirectory()
来源：http://ggd.sxryk.cn

[M05] 设置退出码
来源：http://ysd.dashuyun.cn

Py:   sys.exit(1)
来源：http://wuj.xinyue.icu

PHP:  exit(1);
来源：http://vye.tanke756.top

JS:   process.exit(1)
来源：http://cbr.zdbjq.cn

TS:   process.exit(1)
来源：http://nqf.cheryme.top

Java: System.exit(1)
来源：http://gsf.0kj1m.cn

Go:   os.Exit(1)
来源：http://vuc.ywan-chungtsiang.top

Ruby: exit 1
来源：http://mdm.bbcook.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fgp.nanxinkj.top

[M06] 向标准错误输出
来源：http://lyf.smart0.xyz

Py:   print("err", file=sys.stderr)
来源：http://gne.bbcook.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ccm.fzhhl.top

JS:   console.error("err")
来源：http://yfc.shuidangran.top

TS:   console.error("err")
来源：http://lcb.sufxvd.cn

Java: System.err.println("err")
来源：http://xxu.nanxuanxn.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gpx.jiagoushi.top

Ruby: warn "err"
来源：http://awe.iojbl.cn

C#:   Console.Error.WriteLine("err")
来源：http://zej.tarul.cn

[M07] 判断是否为主入口
来源：http://nxs.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://wyi.redwolf501.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eid.fzhhl.top

JS:   require.main === module
来源：http://jnt.ivvv.top

TS:   require.main === module
来源：http://xma.chenzaomai.com

Java: public static void main(String[] args)
来源：http://vek.yueranfly.top

Go:   func main()
来源：http://fmk.gaohongyu789.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zwk.yanxiufei.cn

C#:   static void Main(string[] args)
来源：http://sso.yvedp.cn

[M08] 获取系统与运行时信息
来源：http://uzr.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://xep.gotoacloud.top

PHP:  PHP_OS;  phpversion();
来源：http://vno.fktsv.cn

JS:   process.platform;  process.version
来源：http://spi.uphjek.com

TS:   process.platform;  process.version
来源：http://pgp.jinqigufen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lny.sufxvd.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bff.yj202588.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baq.gotoacloud.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bxc.dianchejie.cn

================================================================================
来源：http://nuf.yj20258888.top

N. 数据结构与算法
来源：http://mam.tarul.cn

================================================================================
来源：http://cid.0kj1m.cn

[N01] 二分查找（有序数组）
来源：http://xit.fzhhl.top

Py:   bisect.bisect_left(arr, x)
来源：http://lba.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rem.hysaishi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://thi.ppjwa.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jry.jqgufenzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://njx.52xcode.cn

Go:   sort.SearchInts(arr, x)
来源：http://fqu.xingfuxueyuan.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://bvb.yonumen.top

C#:   Array.BinarySearch(arr, x)
来源：http://wjx.chenlongwang.top

[N02] 排序（工程实践用内置实现）
来源：http://jqv.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://faj.c1oappe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hgy.quarkkingdee.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://wrn.fzhhl.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://frc.haohaochexian.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uks.birdmap.top

Go:   slices.Sort(arr)
来源：http://xoo.ybcxt.top

Ruby: arr.sort
来源：http://dll.fktsv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zjm.hfpthk.cn

[N03] 快速排序（分治示例）
来源：http://swn.fanxiaobao.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nno.tarul.cn

PHP:  // 递归实现，或用 usort
来源：http://azf.chenzaomai.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ecb.yuanzhike.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://out.tian-w.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kua.yfazqb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ncl.shanyushiyangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yxe.zhijiandao.cn

C#:   // 手写递归，或 Array.Sort
来源：http://epw.yj20258.top

[N04] 斐波那契数列
来源：http://gfi.sweek.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qkj.mhx1999.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vrm.xuanzx.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fvh.jinghuilouyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wco.dashuyun.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jxx.xinyue.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eze.hywenlv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ota.ivvv.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zjd.cdnleiting.top

[N05] 最大公约数
来源：http://ney.jinqigufen.top

Py:   math.gcd(a, b)
来源：http://boo.redwolf501.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qnt.ppjwa.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lqo.jinyuanbaomall.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nqk.cashguo.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kfl.jinqigfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ywh.xuetiantiany.cn

Ruby: a.gcd(b)
来源：http://wfy.jianghu66.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jau.aizwys.cn

[N06] 判断回文字符串
来源：http://gxv.shangyingyoupin.top

Py:   s == s[::-1]
来源：http://bss.yuxming.cn

PHP:  $s === strrev($s);
来源：http://owi.cqqwz.cn

JS:   s === [...s].reverse().join("")
来源：http://hqk.hywenlv.cn

TS:   s === [...s].reverse().join("")
来源：http://acm.ppjwa.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xhr.nanxinkj.top

Go:   // 双指针从两端比较
来源：http://lcj.svipenyu.cn

Ruby: s == s.reverse
来源：http://nvo.epnwcf.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://gah.yfazqb.com

[N07] 两数之和（返回下标）
来源：http://eds.shangyingyoupin.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tly.tianlin.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dgj.cheryme.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vkd.guannengcc.top

TS:   // 手写 Map<string, number>
来源：http://aac.hammf.cn

Java: // 手写 HashMap
来源：http://owv.hammf.cn

Go:   // 手写 map[int]int
来源：http://zzd.daxiang520.top

Ruby: // 手写 Hash
来源：http://aso.xylfe.cn

C#:   // 手写 Dictionary<int, int>
来源：http://eou.yueranfly.top

[N08] 生成全排列
来源：http://zbc.ydjk.org.cn

Py:   itertools.permutations(arr)
来源：http://tnq.zhoulong.xyz

PHP:  // 手写递归交换
来源：http://lup.gotoacloud.top

JS:   // 手写回溯递归
来源：http://mnk.tian-w.cn

TS:   // 手写回溯递归
来源：http://pen.jqgufenzy.top

Java: // 手写回溯递归
来源：http://dod.yuxming.cn

Go:   // 手写回溯递归
来源：http://azf.jinyuanbaomall.cn

Ruby: arr.permutation.to_a
来源：http://wvj.gogol.net.cn

C#:   // 手写回溯递归
来源：http://dok.fktsv.cn

[N09] 栈与队列
来源：http://fjs.bbcook.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jrm.xylfe.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jvg.xziqi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lwz.daxiang520.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hkb.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bbs.yangfankeji.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bsv.yuanzhike.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nce.jqgfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wsw.hesvh.cn

[N10] 链表节点定义
来源：http://brg.nwbrower.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lio.c1oappe.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cwl.jiagoushi.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://njf.meibo888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ffr.uphjek.com

Java: class Node { int v; Node next; }
来源：http://psv.hcnkem.com

Go:   type Node struct { V int; Next *Node }
来源：http://scz.dianchejie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://koj.pycfn.com

C#:   class Node { public int V; public Node? Next; }
来源：http://iln.kuanghao11.cn

[N11] 二叉树中序遍历
来源：http://byd.shzxlz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://njp.hnxiangtu.top

PHP:  // 手写递归函数
来源：http://sac.hnqzz.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gnr.aizwys.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ofa.xinyue.icu

Java: // 手写递归
来源：http://axm.zdbjq.cn

Go:   // 手写递归
来源：http://usg.fanxiaobao.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tgw.shanyushiyangkeji.top

C#:   // 手写递归
来源：http://zcc.hysaishi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bsx.hywenlv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mtw.xuanzx.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wzr.cashguo.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xzc.hfpthk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tno.kuanghao11.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zcy.tarul.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xse.dashuyun.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kbz.yuanzhike.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xhy.svipenyu.cn

================================================================================
来源：http://dlq.ywan-chungtsiang.top

O. 并发与异步
来源：http://jxq.316326.xyz

================================================================================
来源：http://zbc.jinyuanbaomall.cn

[O01] 启动一个线程
来源：http://wwp.gaohongyu789.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://grv.zdqjudy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pcr.cdnleiting.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qrp.epnwcf.com

TS:   // 同 JS
来源：http://cvp.zhijiandao.cn

Java: new Thread(() -> f()).start()
来源：http://mrw.sufxvd.cn

Go:   go f()
来源：http://cle.jinghuilouyu.cn

Ruby: Thread.new { f }
来源：http://rdh.yj202588.top

C#:   Task.Run(() => F());
来源：http://pwb.ybcxt.top

[O02] 使用线程池
来源：http://faa.zhoulong.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tdz.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pki.andypj.xyz

JS:   // worker_threads 线程池
来源：http://cdq.hcnkem.com

TS:   // worker_threads 线程池
来源：http://lml.zhengqikj.top

Java: Executors.newFixedThreadPool(4)
来源：http://zfk.iojbl.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://umt.zhijiandao.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://evo.pycfn.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yfn.daria6918.cn

[O03] 加锁保护共享数据
来源：http://egd.cdnleiting.top

Py:   with lock: shared += 1
来源：http://ctx.vehdjk.com

PHP:  // 用 flock() 做文件锁
来源：http://bkx.hfpthk.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yjf.zhiwuduotai.top

TS:   // 同 JS
来源：http://she.dashuyun.cn

Java: synchronized (this) { shared++; }
来源：http://ill.guowangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zsz.wangdashe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zcq.dashuyun.cn

C#:   lock (gate) { shared++; }
来源：http://sad.hnxiangtu.top

[O04] 定义异步函数并等待
来源：http://sfu.hammf.cn

Py:   async def f():⏎    await g()
来源：http://vgh.9152youxi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yyg.zhengqikj.top

JS:   async function f() { await g(); }
来源：http://bcs.yonumen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qwz.ybcxt.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lns.daxiang520.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://prm.guannengcc.top

Ruby: # 用 Fiber 或 async gem
来源：http://kkm.wangdashe.top

C#:   async Task F() { await G(); }
来源：http://irb.c1oappe.top

[O05] 并发执行并等待全部完成
来源：http://rko.fengsongda.top

Py:   asyncio.gather(*tasks)
来源：http://dps.pengpengdd.cyou

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qcl.wangdashe.top

JS:   await Promise.all(tasks)
来源：http://szv.hesvh.cn

TS:   await Promise.all(tasks)
来源：http://gbe.shanyushiyangtech.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mbc.dianchejie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tef.chenzaomai.com

Ruby: threads.map(&:join)
来源：http://qbp.hnqzz.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xju.haohaochexian.top

[O06] 使用进程池
来源：http://ijp.guowangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pfg.wangdashe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jhy.zhongyouzk.top

JS:   // child_process / cluster 模块
来源：http://cmw.yangfankeji.com

TS:   // child_process / cluster 模块
来源：http://bbw.sxryk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mdk.nanxuanxn.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://aml.xuetiantiany.cn

Ruby: // fork 块
来源：http://rip.hfpthk.cn

C#:   Parallel.For
来源：http://pgp.cheryme.top

================================================================================
来源：http://idb.shangyingyoupin.top

P. 常用工具函数
来源：http://xzr.tarul.cn

================================================================================
来源：http://urf.jiagoushi.top

[P01] 生成 UUID
来源：http://yfa.shuidangran.top

Py:   str(uuid.uuid4())
来源：http://sxd.sysykeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rqu.yangfankeji.com

JS:   crypto.randomUUID()
来源：http://lac.cheryme.top

TS:   crypto.randomUUID()
来源：http://muy.sufxvd.cn

Java: UUID.randomUUID().toString()
来源：http://oji.jiagoushi.top

Go:   // 用 github.com/google/uuid
来源：http://vwc.cqqwz.cn

Ruby: SecureRandom.uuid
来源：http://xcc.kuanghao11.cn

C#:   Guid.NewGuid().ToString()
来源：http://ayt.daria6918.cn

[P02] MD5 / SHA256 摘要
来源：http://srz.zhijiandao.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gxa.zhengqikj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://udv.zdqjudy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://djz.zhixingplan.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vni.guannengcc.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kvn.aizwys.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ajy.jiagoushi.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oob.gaohongyu789.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nxt.jinqigufen.top

[P03] 生成短随机字符串
来源：http://auc.jinghuilouyu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zfm.jiagoushi.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oof.jlsjyb.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sjh.cheryme.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://obr.fktsv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jtq.chenzaomai.com


<!-- 参考信息 -->