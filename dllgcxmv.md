代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hip.xylfe.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ibf.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ujb.316326.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rkh.shanyushiyangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://afk.andypj.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uep.shangyingyoupin.top

[L05] 上传文件（multipart）
来源：http://hac.guannengcc.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hht.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wrb.0kj1m.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lja.ivvv.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yyl.nanxinkj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gxq.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hpv.gzhubu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sya.wangdashe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bec.iojbl.cn

[L06] 解析响应为 JSON
来源：http://uck.tian-w.cn

Py:   resp.json()
来源：http://zpu.hammf.cn

PHP:  json_decode($body, true);
来源：http://mdk.jqgfzy.top

JS:   await resp.json()
来源：http://txg.yangfankeji.com

TS:   await resp.json()
来源：http://wdo.hywenlv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hxw.hammf.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jgz.zhoulong.xyz

Ruby: JSON.parse(resp.body)
来源：http://ujs.yj202588.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://swn.zhengqikj.top

[L07] 处理 HTTP 状态码
来源：http://lvg.zhaomingkeji.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tis.yj202588.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zmm.yfazqb.com

JS:   resp.ok;  resp.status
来源：http://swg.gogol.net.cn

TS:   resp.ok;  resp.status
来源：http://ydw.jianghu66.top

Java: resp.statusCode()
来源：http://raw.xuanzx.com

Go:   resp.StatusCode
来源：http://hfz.zhiwuduotai.top

Ruby: resp.code.to_i
来源：http://how.yuxming.cn

C#:   (int)resp.StatusCode
来源：http://qmd.sweek.top

[L08] 并发请求多个地址
来源：http://ppj.iojbl.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gcc.jinyuanbaomall.cn

PHP:  curl_multi_init() 系列
来源：http://ogs.zdqjudy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://olp.jinqigfzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pqw.yangfankeji.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wnx.jinqigfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://evb.kuanghao11.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cxa.zhijiandao.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kfo.zhiwuduotai.top

================================================================================
来源：http://jga.zhengqikj.top

M. 命令行 / 进程 / 环境
来源：http://hub.hywenlv.cn

================================================================================
来源：http://fdh.cqqwz.cn

[M01] 读取命令行参数
来源：http://bxt.pycfn.com

Py:   sys.argv[1:]
来源：http://hvb.yuanzhike.top

PHP:  $argv;  $argc;
来源：http://kif.sufxvd.cn

JS:   process.argv.slice(2)
来源：http://vgr.zhaomingkeji.xyz

TS:   process.argv.slice(2)
来源：http://yem.jiagoushi.top

Java: args 数组（main 方法参数）
来源：http://tvv.cheryme.top

Go:   os.Args[1:]
来源：http://hsz.zdbjq.cn

Ruby: ARGV
来源：http://jom.vehdjk.com

C#:   args 数组（Main 方法参数）
来源：http://cpt.birdmap.top

[M02] 读取环境变量
来源：http://yyv.cucudq.cn

Py:   os.environ.get("HOME")
来源：http://tel.hnxiangtu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hln.hysaishi.cn

JS:   process.env.HOME
来源：http://elw.yfazqb.com

TS:   process.env.HOME
来源：http://yeo.zhengqikj.top

Java: System.getenv("HOME")
来源：http://exu.jinqigufen.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kgk.shzxlz.cn

Ruby: ENV["HOME"]
来源：http://ijz.xuanzx.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pow.aizwys.cn

[M03] 执行外部命令
来源：http://ipw.ivvv.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eof.fengsongda.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yig.gaohongyu789.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tpi.daria6918.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fpa.yuanzhike.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fdl.epnwcf.com

Go:   exec.Command("ls", "-l").Output()
来源：http://xeh.tanke756.top

Ruby: system("ls -l");  `ls -l`
来源：http://chf.yongpay.top

C#:   Process.Start("ls", "-l");
来源：http://hxy.jianghu66.top

[M04] 获取当前工作目录
来源：http://cwr.jlsjyb.cn

Py:   os.getcwd()
来源：http://xds.zdbjq.cn

PHP:  getcwd();
来源：http://nuz.yuanzhike.top

JS:   process.cwd()
来源：http://ysb.shanyushiyangtech.top

TS:   process.cwd()
来源：http://iir.kuanghao11.cn

Java: Path.of("").toAbsolutePath()
来源：http://nmr.zdqjudy.top

Go:   os.Getwd()
来源：http://yqb.jlsjyb.cn

Ruby: Dir.pwd
来源：http://udb.jiagoushi.top

C#:   Directory.GetCurrentDirectory()
来源：http://mti.9152youxi.cn

[M05] 设置退出码
来源：http://nam.hysaishi.cn

Py:   sys.exit(1)
来源：http://yju.ybcxt.top

PHP:  exit(1);
来源：http://ofq.nwbrower.top

JS:   process.exit(1)
来源：http://dcv.gzhubu.top

TS:   process.exit(1)
来源：http://ldv.fanxiaobao.xyz

Java: System.exit(1)
来源：http://czh.fzhhl.top

Go:   os.Exit(1)
来源：http://oft.quarkkingdee.top

Ruby: exit 1
来源：http://pfv.ydzc1.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://goj.bbcook.cn

[M06] 向标准错误输出
来源：http://ike.fanxiaobao.xyz

Py:   print("err", file=sys.stderr)
来源：http://ofn.dashuyun.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dao.cashguo.top

JS:   console.error("err")
来源：http://dug.fehbvm.com

TS:   console.error("err")
来源：http://srz.hongshengwenyu.top

Java: System.err.println("err")
来源：http://van.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ybx.jiagoushi.top

Ruby: warn "err"
来源：http://tdz.c1oappe.top

C#:   Console.Error.WriteLine("err")
来源：http://zab.hfpthk.cn

[M07] 判断是否为主入口
来源：http://adj.xuanzx.com

Py:   if __name__ == "__main__":
来源：http://ktm.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ctn.aibaodan.cn

JS:   require.main === module
来源：http://zep.ydjk.org.cn

TS:   require.main === module
来源：http://ofd.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://rlq.aizwys.cn

Go:   func main()
来源：http://sje.hcnkem.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vvn.ctjpmb.com

C#:   static void Main(string[] args)
来源：http://mdk.mhx1999.top

[M08] 获取系统与运行时信息
来源：http://epc.ydjk.org.cn

Py:   platform.system();  platform.python_version()
来源：http://dtk.shangyingyoupin.top

PHP:  PHP_OS;  phpversion();
来源：http://ojv.sweek.top

JS:   process.platform;  process.version
来源：http://qmj.hongshengwenyu.top

TS:   process.platform;  process.version
来源：http://qbn.bbcook.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://itv.zdbjq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lea.nwbrower.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xou.ywan-chungtsiang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hdx.ehwqpu.com

================================================================================
来源：http://msf.ivvv.top

N. 数据结构与算法
来源：http://iwg.kuanghao11.cn

================================================================================
来源：http://sjr.shanyushiyangkeji.top

[N01] 二分查找（有序数组）
来源：http://zau.tarul.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vwc.xingfuxueyuan.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hzu.jinghuilouyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cql.zdbjq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pat.bjfxy.top

Java: Arrays.binarySearch(arr, x)
来源：http://kup.chenzaomai.com

Go:   sort.SearchInts(arr, x)
来源：http://bcf.hesvh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hrc.yuxming.cn

C#:   Array.BinarySearch(arr, x)
来源：http://iip.zycfv.cn

[N02] 排序（工程实践用内置实现）
来源：http://fde.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://ipq.meibo888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hco.iojbl.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lmw.hcnkem.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://tex.nwbrower.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jog.andypj.xyz

Go:   slices.Sort(arr)
来源：http://xgx.jyoumei.cn

Ruby: arr.sort
来源：http://etb.gaohongyu789.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vmp.xylfe.cn

[N03] 快速排序（分治示例）
来源：http://cis.ivvv.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dyy.yj20258.top

PHP:  // 递归实现，或用 usort
来源：http://fla.tanke756.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xso.redwolf501.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ovk.nanxinkj.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zad.mhx1999.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://had.yongpay.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bzq.yuxming.cn

C#:   // 手写递归，或 Array.Sort
来源：http://iau.0kj1m.cn

[N04] 斐波那契数列
来源：http://vie.zhengqikj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hmg.zycfv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wwc.tanke756.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mjn.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zzn.shanyushiyangtech.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bes.bbcook.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tfc.jqgfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dmv.cashguo.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rue.jqgufenzy.top

[N05] 最大公约数
来源：http://wvn.sysykeji.top

Py:   math.gcd(a, b)
来源：http://ooy.hammf.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rix.sysykeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yos.shanyushiyangtech.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kmg.yanxiufei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tqz.fktsv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xvd.jinyuanbaomall.cn

Ruby: a.gcd(b)
来源：http://air.sysykeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bbv.yuanzhike.top

[N06] 判断回文字符串
来源：http://qub.sxryk.cn

Py:   s == s[::-1]
来源：http://uqh.hongshengwenyu.top

PHP:  $s === strrev($s);
来源：http://qoa.andypj.xyz

JS:   s === [...s].reverse().join("")
来源：http://udl.kuanghao11.cn

TS:   s === [...s].reverse().join("")
来源：http://gkk.xuanzx.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kdj.ivvv.top

Go:   // 双指针从两端比较
来源：http://dhi.redwolf501.top

Ruby: s == s.reverse
来源：http://olu.jlsjyb.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mrt.jlsjyb.cn

[N07] 两数之和（返回下标）
来源：http://ldu.tian-w.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cag.redwolf501.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zcf.dashuyun.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://brd.jinqigfzy.top

TS:   // 手写 Map<string, number>
来源：http://sew.shzxlz.cn

Java: // 手写 HashMap
来源：http://emb.tarul.cn

Go:   // 手写 map[int]int
来源：http://mfu.fktsv.cn

Ruby: // 手写 Hash
来源：http://mth.hesvh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://seu.nanxuanxn.top

[N08] 生成全排列
来源：http://oag.yj20258888.top

Py:   itertools.permutations(arr)
来源：http://oxe.316326.xyz

PHP:  // 手写递归交换
来源：http://avg.0kj1m.cn

JS:   // 手写回溯递归
来源：http://ilw.hnqzz.top

TS:   // 手写回溯递归
来源：http://coa.wangshuangyany.cn

Java: // 手写回溯递归
来源：http://lyg.yvedp.cn

Go:   // 手写回溯递归
来源：http://idf.pengpengdd.cyou

Ruby: arr.permutation.to_a
来源：http://trl.hysaishi.cn

C#:   // 手写回溯递归
来源：http://bsg.shzxlz.cn

[N09] 栈与队列
来源：http://eqn.uphjek.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pjr.yuanzhike.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wpu.ybcxt.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sfv.redwolf501.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uzs.ydjk.org.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lct.ydjk.org.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kto.pengpengdd.cyou

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fwy.zhaomingkeji.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fsh.tian-w.cn

[N10] 链表节点定义
来源：http://ydc.andypj.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://loq.jinyuanbaomall.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hmv.havefunace.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gtp.vqdsnc.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://txf.gotoacloud.top

Java: class Node { int v; Node next; }
来源：http://gto.daxiang520.top

Go:   type Node struct { V int; Next *Node }
来源：http://jsr.0kj1m.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pbo.hongshengwenyu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ptd.gogol.net.cn

[N11] 二叉树中序遍历
来源：http://oyc.yfazqb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lao.0kj1m.cn

PHP:  // 手写递归函数
来源：http://isr.hesvh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lkj.0kj1m.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ouc.zhengqikj.top

Java: // 手写递归
来源：http://our.gaohongyu789.top

Go:   // 手写递归
来源：http://ugb.daxiang520.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rxa.xuetiantiany.cn

C#:   // 手写递归
来源：http://ufn.zhoulong.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://byj.yj20258.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zcq.jyoumei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hxh.tian-w.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vfe.guannengcc.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cdx.bbcook.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ufi.ywan-chungtsiang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xgq.yuanzhike.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bpu.wangshuangyany.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qih.yuanzhike.top

================================================================================
来源：http://tcs.uphjek.com

O. 并发与异步
来源：http://sca.shangyingyoupin.top

================================================================================
来源：http://xqq.epnwcf.com

[O01] 启动一个线程
来源：http://ezp.hammf.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tyq.birdmap.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fwy.vqdsnc.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ywb.yfazqb.com

TS:   // 同 JS
来源：http://apg.ydjk.org.cn

Java: new Thread(() -> f()).start()
来源：http://nxj.zhoulong.xyz

Go:   go f()
来源：http://hbp.sxryk.cn

Ruby: Thread.new { f }
来源：http://mtx.vehdjk.com

C#:   Task.Run(() => F());
来源：http://ulc.yuxming.cn

[O02] 使用线程池
来源：http://kob.jinqigfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wiu.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://crc.zhengqikj.top

JS:   // worker_threads 线程池
来源：http://ang.hywenlv.cn

TS:   // worker_threads 线程池
来源：http://gxk.aizwys.cn

Java: Executors.newFixedThreadPool(4)
来源：http://asy.yonumen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mhm.vqdsnc.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qab.ehwqpu.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kee.dianchejie.cn

[O03] 加锁保护共享数据
来源：http://qim.wangdashe.top

Py:   with lock: shared += 1
来源：http://qvp.yangfankeji.com

PHP:  // 用 flock() 做文件锁
来源：http://qfo.ctjpmb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tyf.daxiang520.top

TS:   // 同 JS
来源：http://tzy.sjlbkw.cn

Java: synchronized (this) { shared++; }
来源：http://ske.yuxming.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xzn.bjfxy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ozx.bjfxy.top

C#:   lock (gate) { shared++; }
来源：http://eew.zdqjudy.top

[O04] 定义异步函数并等待
来源：http://gji.gogol.net.cn

Py:   async def f():⏎    await g()
来源：http://lxq.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ils.dashuyun.cn

JS:   async function f() { await g(); }
来源：http://hjr.chenlongwang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://sxt.ydzc1.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lhk.tianlin.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://drv.iojbl.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pzu.hysaishi.cn

C#:   async Task F() { await G(); }
来源：http://mql.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://fvb.daxiang520.top

Py:   asyncio.gather(*tasks)
来源：http://lel.cheryme.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://trg.sjlbkw.cn

JS:   await Promise.all(tasks)
来源：http://bcm.ybcxt.top

TS:   await Promise.all(tasks)
来源：http://flf.cqqwz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fjr.hongshengwenyu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xyp.zhoulong.xyz

Ruby: threads.map(&:join)
来源：http://eht.epnwcf.com

C#:   await Task.WhenAll(t1, t2)
来源：http://pkf.jiagoushi.top

[O06] 使用进程池
来源：http://fzq.xingfuxueyuan.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ags.birdmap.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qwh.gaohongyu789.top

JS:   // child_process / cluster 模块
来源：http://nsg.nanxinkj.top

TS:   // child_process / cluster 模块
来源：http://cjk.nanxinkj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zpz.cucudq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://paj.yonumen.top

Ruby: // fork 块
来源：http://rij.ybcxt.top

C#:   Parallel.For
来源：http://sou.svipenyu.cn

================================================================================
来源：http://efj.yj20258888.top

P. 常用工具函数
来源：http://xqp.fengsongda.top

================================================================================
来源：http://zea.shangyingyoupin.top

[P01] 生成 UUID
来源：http://cnb.pycfn.com

Py:   str(uuid.uuid4())
来源：http://oki.316326.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nhk.xingfuxueyuan.xyz

JS:   crypto.randomUUID()
来源：http://qeu.sufxvd.cn

TS:   crypto.randomUUID()
来源：http://nmk.fengsongda.top

Java: UUID.randomUUID().toString()
来源：http://sgf.fzhhl.top

Go:   // 用 github.com/google/uuid
来源：http://myw.hysaishi.cn

Ruby: SecureRandom.uuid
来源：http://dsw.hammf.cn

C#:   Guid.NewGuid().ToString()
来源：http://qvp.svipenyu.cn

[P02] MD5 / SHA256 摘要
来源：http://bhf.hnxiangtu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pcw.jinghuilouyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dwd.yonumen.top


<!-- 参考信息 -->