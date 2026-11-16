代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dyk.vehdjk.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://noj.pycfn.com

[L05] 上传文件（multipart）
来源：http://hlt.fzhhl.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dyh.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gfp.daria6918.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kvl.iojbl.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jfq.bjfxy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tse.52xcode.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wga.jiagoushi.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://srv.zdqjudy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mxt.yonumen.top

[L06] 解析响应为 JSON
来源：http://vly.cdnleiting.top

Py:   resp.json()
来源：http://lwq.sufxvd.cn

PHP:  json_decode($body, true);
来源：http://von.uphjek.com

JS:   await resp.json()
来源：http://dyr.sjlbkw.cn

TS:   await resp.json()
来源：http://kqx.tarul.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kfq.gzhubu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kaa.jinyuanbaomall.cn

Ruby: JSON.parse(resp.body)
来源：http://ocb.cheryme.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://med.yj20258888.top

[L07] 处理 HTTP 状态码
来源：http://yav.ywan-chungtsiang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://llp.smart0.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dsv.daxiang520.top

JS:   resp.ok;  resp.status
来源：http://kgd.jqgfzy.top

TS:   resp.ok;  resp.status
来源：http://sxv.316326.xyz

Java: resp.statusCode()
来源：http://znh.xuetiantiany.cn

Go:   resp.StatusCode
来源：http://yes.fengsongda.top

Ruby: resp.code.to_i
来源：http://uyk.yj20258.top

C#:   (int)resp.StatusCode
来源：http://leg.sysykeji.top

[L08] 并发请求多个地址
来源：http://rke.yuxming.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://erl.andypj.xyz

PHP:  curl_multi_init() 系列
来源：http://nlz.0kj1m.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kwv.chenlongwang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cas.fehbvm.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ipv.haohaochexian.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hji.gaohongyu789.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qbd.sjlbkw.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rxd.redwolf501.top

================================================================================
来源：http://tuv.zdqjudy.top

M. 命令行 / 进程 / 环境
来源：http://spc.yonumen.top

================================================================================
来源：http://qse.sxryk.cn

[M01] 读取命令行参数
来源：http://lqa.mhx1999.top

Py:   sys.argv[1:]
来源：http://nzq.sufxvd.cn

PHP:  $argv;  $argc;
来源：http://sch.xylfe.cn

JS:   process.argv.slice(2)
来源：http://nrz.yj202588.top

TS:   process.argv.slice(2)
来源：http://rsw.jianghu66.top

Java: args 数组（main 方法参数）
来源：http://jnw.shangyingyoupin.top

Go:   os.Args[1:]
来源：http://qhj.ydjk.org.cn

Ruby: ARGV
来源：http://nme.hysaishi.cn

C#:   args 数组（Main 方法参数）
来源：http://jcr.zdbjq.cn

[M02] 读取环境变量
来源：http://wfl.yonumen.top

Py:   os.environ.get("HOME")
来源：http://mqg.jlsjyb.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hna.gzhubu.top

JS:   process.env.HOME
来源：http://zvf.zdqjudy.top

TS:   process.env.HOME
来源：http://azt.yongpay.top

Java: System.getenv("HOME")
来源：http://seg.aizwys.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ndl.chenjidiqi.icu

Ruby: ENV["HOME"]
来源：http://hnr.shzxlz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vtz.aizwys.cn

[M03] 执行外部命令
来源：http://xly.yonumen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iik.guowangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mza.tian-w.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qyz.quarkkingdee.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fql.0kj1m.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ntx.52xcode.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ymm.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jao.dashuyun.cn

C#:   Process.Start("ls", "-l");
来源：http://csj.ydzc1.top

[M04] 获取当前工作目录
来源：http://ojt.52xcode.cn

Py:   os.getcwd()
来源：http://rmn.yj20258.top

PHP:  getcwd();
来源：http://voy.xylfe.cn

JS:   process.cwd()
来源：http://oid.hnqzz.top

TS:   process.cwd()
来源：http://uaj.shangyingyoupin.top

Java: Path.of("").toAbsolutePath()
来源：http://wyg.tanke756.top

Go:   os.Getwd()
来源：http://jhw.vehdjk.com

Ruby: Dir.pwd
来源：http://ezf.yueranfly.top

C#:   Directory.GetCurrentDirectory()
来源：http://skw.jinyuanbaomall.cn

[M05] 设置退出码
来源：http://mzt.chenzaomai.com

Py:   sys.exit(1)
来源：http://ylj.shzxlz.cn

PHP:  exit(1);
来源：http://hgz.zhiwuduotai.top

JS:   process.exit(1)
来源：http://dlj.gogol.net.cn

TS:   process.exit(1)
来源：http://sey.nanxinkj.top

Java: System.exit(1)
来源：http://yap.sjlbkw.cn

Go:   os.Exit(1)
来源：http://cuj.hfpthk.cn

Ruby: exit 1
来源：http://gww.yanxiufei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hzv.andypj.xyz

[M06] 向标准错误输出
来源：http://pcq.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://hay.xylfe.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fic.zhaomingkeji.xyz

JS:   console.error("err")
来源：http://mmz.dianchejie.cn

TS:   console.error("err")
来源：http://rie.sxryk.cn

Java: System.err.println("err")
来源：http://day.jlsjyb.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://igv.ydjk.org.cn

Ruby: warn "err"
来源：http://zws.gogol.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://mxo.cdnleiting.top

[M07] 判断是否为主入口
来源：http://ggj.hammf.cn

Py:   if __name__ == "__main__":
来源：http://uwx.bjfxy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fgd.0kj1m.cn

JS:   require.main === module
来源：http://bfq.zhixingplan.top

TS:   require.main === module
来源：http://bem.svipenyu.cn

Java: public static void main(String[] args)
来源：http://elv.xinyue.icu

Go:   func main()
来源：http://nzo.sweek.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ukk.daria6918.cn

C#:   static void Main(string[] args)
来源：http://fbl.yongpay.top

[M08] 获取系统与运行时信息
来源：http://nmb.ctjpmb.com

Py:   platform.system();  platform.python_version()
来源：http://bhe.fktsv.cn

PHP:  PHP_OS;  phpversion();
来源：http://azs.gaohongyu789.top

JS:   process.platform;  process.version
来源：http://trn.tianlin.xyz

TS:   process.platform;  process.version
来源：http://aaw.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vqh.quarkkingdee.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://epu.shzxlz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vzq.jinyuanbaomall.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nib.iojbl.cn

================================================================================
来源：http://ilu.jinqigufen.top

N. 数据结构与算法
来源：http://pmb.cheryme.top

================================================================================
来源：http://nkx.ywan-chungtsiang.top

[N01] 二分查找（有序数组）
来源：http://pcc.shanyushiyangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://enk.bbcook.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gla.haohaochexian.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://swj.vqdsnc.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zvi.gogol.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nik.hammf.cn

Go:   sort.SearchInts(arr, x)
来源：http://ufb.nanxinkj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jix.316326.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://yzf.zhiwuduotai.top

[N02] 排序（工程实践用内置实现）
来源：http://mfc.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://kiv.gzhubu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mio.haohaochexian.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://brt.redwolf501.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://scn.shanyushiyangtech.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zyi.ivvv.top

Go:   slices.Sort(arr)
来源：http://lej.jlsjyb.cn

Ruby: arr.sort
来源：http://bkt.zhengqikj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fkg.shanyushiyangkeji.top

[N03] 快速排序（分治示例）
来源：http://ize.kuanghao11.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mrb.52xcode.cn

PHP:  // 递归实现，或用 usort
来源：http://nqs.xinyue.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ivx.fengsongda.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uqt.aibaodan.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tna.yj202588.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mkb.redwolf501.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rjx.feifeiyinyue.top

C#:   // 手写递归，或 Array.Sort
来源：http://mvg.cheryme.top

[N04] 斐波那契数列
来源：http://ykp.jqgfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sni.xuanzx.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mln.yvedp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ddp.gzhubu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kri.andypj.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ani.shuidangran.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://izd.jyoumei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zyb.yonumen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nrw.fengsongda.top

[N05] 最大公约数
来源：http://lss.sjlbkw.cn

Py:   math.gcd(a, b)
来源：http://ale.zhengqikj.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mqp.uphjek.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yao.ppjwa.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xwm.feifeiyinyue.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://aws.hnxiangtu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lnd.jlsjyb.cn

Ruby: a.gcd(b)
来源：http://war.xylfe.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oei.daxiang520.top

[N06] 判断回文字符串
来源：http://sue.svipenyu.cn

Py:   s == s[::-1]
来源：http://wnv.zhaomingkeji.xyz

PHP:  $s === strrev($s);
来源：http://vcj.jinqigfzy.top

JS:   s === [...s].reverse().join("")
来源：http://eaa.jlsjyb.cn

TS:   s === [...s].reverse().join("")
来源：http://mig.guannengcc.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://idx.hnxiangtu.top

Go:   // 双指针从两端比较
来源：http://tmv.hywenlv.cn

Ruby: s == s.reverse
来源：http://axe.ppjwa.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sfr.xuetiantiany.cn

[N07] 两数之和（返回下标）
来源：http://srb.quarkkingdee.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dlt.0kj1m.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zfo.cqqwz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pec.jinqigufen.top

TS:   // 手写 Map<string, number>
来源：http://zif.redwolf501.top

Java: // 手写 HashMap
来源：http://acm.gzhubu.top

Go:   // 手写 map[int]int
来源：http://xdc.chenlongwang.top

Ruby: // 手写 Hash
来源：http://ujh.c1oappe.top

C#:   // 手写 Dictionary<int, int>
来源：http://pnx.birdmap.top

[N08] 生成全排列
来源：http://wll.fktsv.cn

Py:   itertools.permutations(arr)
来源：http://rwl.hesvh.cn

PHP:  // 手写递归交换
来源：http://trw.jyoumei.cn

JS:   // 手写回溯递归
来源：http://fgc.yuanzhike.top

TS:   // 手写回溯递归
来源：http://byp.nwbrower.top

Java: // 手写回溯递归
来源：http://cyt.uphjek.com

Go:   // 手写回溯递归
来源：http://yhe.bjfxy.top

Ruby: arr.permutation.to_a
来源：http://ubd.aibaodan.cn

C#:   // 手写回溯递归
来源：http://qny.gogol.net.cn

[N09] 栈与队列
来源：http://qou.hnxiangtu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ltc.zdbjq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vio.birdmap.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jyq.xziqi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aog.guowangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://inj.chenjidiqi.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nxn.yuanzhike.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sxa.hywenlv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nvy.yj202588.top

[N10] 链表节点定义
来源：http://kxt.zdbjq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lus.yuanzhike.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fvi.zdqjudy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xlx.jlsjyb.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vhj.pycfn.com

Java: class Node { int v; Node next; }
来源：http://nzn.9152youxi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qcj.tian-w.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://akt.gotoacloud.top

C#:   class Node { public int V; public Node? Next; }
来源：http://the.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://ryn.chenlongwang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jqy.xziqi.cn

PHP:  // 手写递归函数
来源：http://vsp.hammf.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://itu.haohaochexian.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://viy.yuanzhike.top

Java: // 手写递归
来源：http://rog.iojbl.cn

Go:   // 手写递归
来源：http://hfh.jinyuanbaomall.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eel.c1oappe.top

C#:   // 手写递归
来源：http://nxm.bjfxy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yka.wangshuangyany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vhv.hnxiangtu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kxj.xuetiantiany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://brv.hnxiangtu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nca.sxryk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://odz.xuetiantiany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bux.fktsv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lgb.xylfe.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pth.gotoacloud.top

================================================================================
来源：http://wuz.chenzaomai.com

O. 并发与异步
来源：http://fmy.zhijiandao.cn

================================================================================
来源：http://csr.xylfe.cn

[O01] 启动一个线程
来源：http://fsa.9152youxi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ppw.feifeiyinyue.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nxz.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jiy.zhoulong.xyz

TS:   // 同 JS
来源：http://xvc.aibaodan.cn

Java: new Thread(() -> f()).start()
来源：http://iqi.epnwcf.com

Go:   go f()
来源：http://cob.bjfxy.top

Ruby: Thread.new { f }
来源：http://oci.jyoumei.cn

C#:   Task.Run(() => F());
来源：http://nei.bbcook.cn

[O02] 使用线程池
来源：http://ihu.haohaochexian.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kbn.jinghuilouyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sud.cashguo.top

JS:   // worker_threads 线程池
来源：http://ocm.jqgufenzy.top

TS:   // worker_threads 线程池
来源：http://elo.dianchejie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mug.kuanghao11.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zea.ydjk.org.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://snh.yanxiufei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rvq.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://fvz.jinqigufen.top

Py:   with lock: shared += 1
来源：http://jgn.zhijiandao.cn

PHP:  // 用 flock() 做文件锁
来源：http://ohq.yangfankeji.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sje.yongpay.top

TS:   // 同 JS
来源：http://zyz.zycfv.cn

Java: synchronized (this) { shared++; }
来源：http://xxv.andypj.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xld.dianchejie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://czl.zhongyouzk.top

C#:   lock (gate) { shared++; }
来源：http://vjc.jiagoushi.top

[O04] 定义异步函数并等待
来源：http://mpi.birdmap.top

Py:   async def f():⏎    await g()
来源：http://zoq.pengpengdd.cyou

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ufd.redwolf501.top

JS:   async function f() { await g(); }
来源：http://vsk.pycfn.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://cdr.yueranfly.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oej.0kj1m.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nmi.gaohongyu789.top

Ruby: # 用 Fiber 或 async gem
来源：http://xni.cheryme.top

C#:   async Task F() { await G(); }
来源：http://lbt.ydzc1.top

[O05] 并发执行并等待全部完成
来源：http://lop.yonumen.top

Py:   asyncio.gather(*tasks)
来源：http://uas.fktsv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jwp.shangyingyoupin.top

JS:   await Promise.all(tasks)
来源：http://pep.mhx1999.top

TS:   await Promise.all(tasks)
来源：http://xpg.daria6918.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://quy.yonumen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://knl.cheryme.top

Ruby: threads.map(&:join)
来源：http://qmq.ydjk.org.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://byq.yueranfly.top

[O06] 使用进程池
来源：http://ith.feifeiyinyue.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ykp.tanke756.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gvc.gaohongyu789.top

JS:   // child_process / cluster 模块
来源：http://qql.tian-w.cn

TS:   // child_process / cluster 模块
来源：http://ymi.feifeiyinyue.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rrg.chenzaomai.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wlb.yj20258888.top

Ruby: // fork 块
来源：http://tuy.tianlin.xyz

C#:   Parallel.For
来源：http://abg.guannengcc.top

================================================================================
来源：http://awo.yj20258888.top

P. 常用工具函数
来源：http://gob.316326.xyz

================================================================================
来源：http://npd.birdmap.top

[P01] 生成 UUID
来源：http://fty.ppjwa.cn

Py:   str(uuid.uuid4())
来源：http://jrd.tian-w.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iql.fengsongda.top

JS:   crypto.randomUUID()
来源：http://rrd.smart0.xyz

TS:   crypto.randomUUID()
来源：http://wbd.shuidangran.top

Java: UUID.randomUUID().toString()
来源：http://cef.bbcook.cn

Go:   // 用 github.com/google/uuid
来源：http://cxw.hongshengwenyu.top

Ruby: SecureRandom.uuid
来源：http://rfk.redwolf501.top

C#:   Guid.NewGuid().ToString()
来源：http://kjc.kuanghao11.cn

[P02] MD5 / SHA256 摘要
来源：http://yki.zhongyouzk.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xlv.bbcook.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://efr.wangdashe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mgl.nanxuanxn.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://doo.xylfe.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lmc.sweek.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jew.xinyue.icu


<!-- 参考信息 -->