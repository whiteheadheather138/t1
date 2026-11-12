代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hxk.ydzc1.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bnl.gotoacloud.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lpx.jlsjyb.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wsc.fengsongda.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fzy.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rfu.pycfn.com

[L05] 上传文件（multipart）
来源：http://kzy.hnxiangtu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hwo.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kkj.uphjek.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rbo.andypj.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://igh.ydjk.org.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://npp.tianlin.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yyl.cucudq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jvr.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wjq.jianghu66.top

[L06] 解析响应为 JSON
来源：http://xeo.hammf.cn

Py:   resp.json()
来源：http://fkv.zycfv.cn

PHP:  json_decode($body, true);
来源：http://dtr.meibo888.top

JS:   await resp.json()
来源：http://dxj.shangyingyoupin.top

TS:   await resp.json()
来源：http://qmc.ivvv.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dzq.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ena.gogol.net.cn

Ruby: JSON.parse(resp.body)
来源：http://obo.ehwqpu.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://epc.xuanzx.com

[L07] 处理 HTTP 状态码
来源：http://nor.feifeiyinyue.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://neg.xingfuxueyuan.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hov.nwbrower.top

JS:   resp.ok;  resp.status
来源：http://ban.gzhubu.top

TS:   resp.ok;  resp.status
来源：http://qtp.zycfv.cn

Java: resp.statusCode()
来源：http://ylm.yanxiufei.cn

Go:   resp.StatusCode
来源：http://ayd.chenlongwang.top

Ruby: resp.code.to_i
来源：http://wzh.cashguo.top

C#:   (int)resp.StatusCode
来源：http://lqm.shzxlz.cn

[L08] 并发请求多个地址
来源：http://gzq.hysaishi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lhl.zhongyouzk.top

PHP:  curl_multi_init() 系列
来源：http://iho.fehbvm.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://slc.shanyushiyangtech.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pfu.mhx1999.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://efw.hysaishi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://guc.0kj1m.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cov.zhengqikj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sbm.shanyushiyangtech.top

================================================================================
来源：http://tnn.cqqwz.cn

M. 命令行 / 进程 / 环境
来源：http://vtl.ybcxt.top

================================================================================
来源：http://xpn.fehbvm.com

[M01] 读取命令行参数
来源：http://pat.xziqi.cn

Py:   sys.argv[1:]
来源：http://nxt.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://fql.jlsjyb.cn

JS:   process.argv.slice(2)
来源：http://fgq.jinyuanbaomall.cn

TS:   process.argv.slice(2)
来源：http://jar.sweek.top

Java: args 数组（main 方法参数）
来源：http://ijb.hongshengwenyu.top

Go:   os.Args[1:]
来源：http://ufc.fzhhl.top

Ruby: ARGV
来源：http://urn.yfazqb.com

C#:   args 数组（Main 方法参数）
来源：http://ctp.jlsjyb.cn

[M02] 读取环境变量
来源：http://ryi.hcnkem.com

Py:   os.environ.get("HOME")
来源：http://yft.fktsv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yzc.zhongyouzk.top

JS:   process.env.HOME
来源：http://nwf.yueranfly.top

TS:   process.env.HOME
来源：http://ecw.hnqzz.top

Java: System.getenv("HOME")
来源：http://fxd.nanxinkj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://quo.hesvh.cn

Ruby: ENV["HOME"]
来源：http://iig.svipenyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bnc.tanke756.top

[M03] 执行外部命令
来源：http://rvs.9152youxi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mwg.shanyushiyangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://izp.pengpengdd.cyou

JS:   child_process.execSync("ls -l").toString()
来源：http://xwl.haohaochexian.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zpp.dashuyun.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://egj.ydjk.org.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://udk.jiagoushi.top

Ruby: system("ls -l");  `ls -l`
来源：http://zwt.hongshengwenyu.top

C#:   Process.Start("ls", "-l");
来源：http://zax.jinqigufen.top

[M04] 获取当前工作目录
来源：http://jyr.dashuyun.cn

Py:   os.getcwd()
来源：http://qvd.xuetiantiany.cn

PHP:  getcwd();
来源：http://elm.fzhhl.top

JS:   process.cwd()
来源：http://ttv.sjlbkw.cn

TS:   process.cwd()
来源：http://miu.cucudq.cn

Java: Path.of("").toAbsolutePath()
来源：http://dne.snrcjt.cn

Go:   os.Getwd()
来源：http://kdt.nwbrower.top

Ruby: Dir.pwd
来源：http://anr.zhoulong.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://bgb.hnxiangtu.top

[M05] 设置退出码
来源：http://hgb.hysaishi.cn

Py:   sys.exit(1)
来源：http://vse.sufxvd.cn

PHP:  exit(1);
来源：http://bsm.epnwcf.com

JS:   process.exit(1)
来源：http://sun.redwolf501.top

TS:   process.exit(1)
来源：http://iie.vqdsnc.cn

Java: System.exit(1)
来源：http://qqi.ctjpmb.com

Go:   os.Exit(1)
来源：http://mnl.smart0.xyz

Ruby: exit 1
来源：http://ycs.xylfe.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ipi.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://fva.xylfe.cn

Py:   print("err", file=sys.stderr)
来源：http://dzb.xuanzx.com

PHP:  fwrite(STDERR, "err\n");
来源：http://yvt.dashuyun.cn

JS:   console.error("err")
来源：http://lzq.hfpthk.cn

TS:   console.error("err")
来源：http://pna.andypj.xyz

Java: System.err.println("err")
来源：http://dov.ctjpmb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eoz.feifeiyinyue.top

Ruby: warn "err"
来源：http://uuu.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://ejt.ctjpmb.com

[M07] 判断是否为主入口
来源：http://whx.ydzc1.top

Py:   if __name__ == "__main__":
来源：http://otr.sweek.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://end.nwbrower.top

JS:   require.main === module
来源：http://rmx.zhixingplan.top

TS:   require.main === module
来源：http://zka.zhoulong.xyz

Java: public static void main(String[] args)
来源：http://dij.zhaomingkeji.xyz

Go:   func main()
来源：http://zsp.yangfankeji.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://usl.zdqjudy.top

C#:   static void Main(string[] args)
来源：http://sbq.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://zds.wangshuangyany.cn

Py:   platform.system();  platform.python_version()
来源：http://efa.sjlbkw.cn

PHP:  PHP_OS;  phpversion();
来源：http://kkp.hesvh.cn

JS:   process.platform;  process.version
来源：http://tde.ywan-chungtsiang.top

TS:   process.platform;  process.version
来源：http://gug.hnqzz.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zrv.dianchejie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vae.cheryme.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ykv.hcnkem.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://nah.hongshengwenyu.top

================================================================================
来源：http://iap.c1oappe.top

N. 数据结构与算法
来源：http://upo.feifeiyinyue.top

================================================================================
来源：http://jag.bjfxy.top

[N01] 二分查找（有序数组）
来源：http://spo.bjfxy.top

Py:   bisect.bisect_left(arr, x)
来源：http://ejj.hfpthk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hqd.ydzc1.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bsb.smart0.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ndo.yonumen.top

Java: Arrays.binarySearch(arr, x)
来源：http://jyn.yongpay.top

Go:   sort.SearchInts(arr, x)
来源：http://ukp.sxryk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vkg.zdbjq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cug.bjfxy.top

[N02] 排序（工程实践用内置实现）
来源：http://liu.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://vwp.jqgfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://daj.fzhhl.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://dwx.jiagoushi.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ptn.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gtj.jiagoushi.top

Go:   slices.Sort(arr)
来源：http://lgc.wangshuangyany.cn

Ruby: arr.sort
来源：http://pra.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vnd.xziqi.cn

[N03] 快速排序（分治示例）
来源：http://rql.tianlin.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://owt.tianlin.xyz

PHP:  // 递归实现，或用 usort
来源：http://cmj.jinqigfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yao.chenlongwang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kva.hesvh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kpn.vqdsnc.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eek.yj202588.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ebd.aizwys.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vul.zhixingplan.top

[N04] 斐波那契数列
来源：http://nxn.fengsongda.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xcm.hammf.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ymg.sysykeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kbn.haohaochexian.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ozm.ivvv.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://akw.tian-w.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zno.shuidangran.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jve.xziqi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pix.zhixingplan.top

[N05] 最大公约数
来源：http://xix.feifeiyinyue.top

Py:   math.gcd(a, b)
来源：http://gci.yj20258888.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ufb.daxiang520.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fsh.gzhubu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kky.tarul.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://egx.316326.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pcu.xuanzx.com

Ruby: a.gcd(b)
来源：http://kmt.birdmap.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qtn.gogol.net.cn

[N06] 判断回文字符串
来源：http://iwr.c1oappe.top

Py:   s == s[::-1]
来源：http://brw.hnqzz.top

PHP:  $s === strrev($s);
来源：http://tka.aizwys.cn

JS:   s === [...s].reverse().join("")
来源：http://muf.ybcxt.top

TS:   s === [...s].reverse().join("")
来源：http://vvo.bjfxy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://foh.zhengqikj.top

Go:   // 双指针从两端比较
来源：http://ftv.tianlin.xyz

Ruby: s == s.reverse
来源：http://xqi.dianchejie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://img.fanxiaobao.xyz

[N07] 两数之和（返回下标）
来源：http://nae.yj202588.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://eup.epnwcf.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ity.yuanzhike.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jbk.snrcjt.cn

TS:   // 手写 Map<string, number>
来源：http://zqf.uphjek.com

Java: // 手写 HashMap
来源：http://obr.yj20258.top

Go:   // 手写 map[int]int
来源：http://txs.zhoulong.xyz

Ruby: // 手写 Hash
来源：http://ktq.feifeiyinyue.top

C#:   // 手写 Dictionary<int, int>
来源：http://kfl.yj20258.top

[N08] 生成全排列
来源：http://fxf.vehdjk.com

Py:   itertools.permutations(arr)
来源：http://vql.tarul.cn

PHP:  // 手写递归交换
来源：http://gfk.wangdashe.top

JS:   // 手写回溯递归
来源：http://xyr.cashguo.top

TS:   // 手写回溯递归
来源：http://fpp.andypj.xyz

Java: // 手写回溯递归
来源：http://bju.aibaodan.cn

Go:   // 手写回溯递归
来源：http://zrp.fanxiaobao.xyz

Ruby: arr.permutation.to_a
来源：http://wtx.hesvh.cn

C#:   // 手写回溯递归
来源：http://hom.hysaishi.cn

[N09] 栈与队列
来源：http://gno.iojbl.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ftw.redwolf501.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hol.tianlin.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pao.nwbrower.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gwf.fzhhl.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lal.daxiang520.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xlk.fehbvm.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jru.yanxiufei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://byd.xinyue.icu

[N10] 链表节点定义
来源：http://cbi.svipenyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dpv.hywenlv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fwa.cucudq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://glg.chenjidiqi.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cdn.hywenlv.cn

Java: class Node { int v; Node next; }
来源：http://dcd.tian-w.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pgp.ehwqpu.com

Ruby: Node = Struct.new(:v, :next)
来源：http://ysq.meibo888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://omx.hesvh.cn

[N11] 二叉树中序遍历
来源：http://ddk.zhiwuduotai.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ion.yonumen.top

PHP:  // 手写递归函数
来源：http://tli.jqgufenzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zkk.52xcode.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pbz.epnwcf.com

Java: // 手写递归
来源：http://rji.tarul.cn

Go:   // 手写递归
来源：http://hqw.ydzc1.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tey.yongpay.top

C#:   // 手写递归
来源：http://rdy.chenjidiqi.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ndx.9152youxi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://omt.cucudq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dca.yuanzhike.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ady.zdbjq.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wpl.epnwcf.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lev.dashuyun.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uef.jinqigufen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://leu.epnwcf.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dyc.chenjidiqi.icu

================================================================================
来源：http://ryv.jinqigufen.top

O. 并发与异步
来源：http://xej.jqgufenzy.top

================================================================================
来源：http://sht.316326.xyz

[O01] 启动一个线程
来源：http://cng.dashuyun.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ohz.shzxlz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nsx.dashuyun.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vtw.iojbl.cn

TS:   // 同 JS
来源：http://miz.zhiwuduotai.top

Java: new Thread(() -> f()).start()
来源：http://ayk.yuxming.cn

Go:   go f()
来源：http://kin.uphjek.com

Ruby: Thread.new { f }
来源：http://jln.havefunace.top

C#:   Task.Run(() => F());
来源：http://tgt.svipenyu.cn

[O02] 使用线程池
来源：http://wbu.chenzaomai.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xiu.daxiang520.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kao.redwolf501.top

JS:   // worker_threads 线程池
来源：http://oji.yonumen.top

TS:   // worker_threads 线程池
来源：http://mxg.redwolf501.top

Java: Executors.newFixedThreadPool(4)
来源：http://mrd.jinyuanbaomall.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lyr.zhengqikj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ppt.snrcjt.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://trb.hammf.cn

[O03] 加锁保护共享数据
来源：http://arb.zhijiandao.cn

Py:   with lock: shared += 1
来源：http://xyp.316326.xyz

PHP:  // 用 flock() 做文件锁
来源：http://fax.zycfv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lqa.xuetiantiany.cn

TS:   // 同 JS
来源：http://vzq.sysykeji.top

Java: synchronized (this) { shared++; }
来源：http://uvy.haohaochexian.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://juv.smart0.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://pfo.shzxlz.cn

C#:   lock (gate) { shared++; }
来源：http://szp.wangshuangyany.cn

[O04] 定义异步函数并等待
来源：http://vad.sxryk.cn

Py:   async def f():⏎    await g()
来源：http://edo.gotoacloud.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ksy.ivvv.top

JS:   async function f() { await g(); }
来源：http://tty.epnwcf.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://kxg.9152youxi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vpf.52xcode.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fte.daxiang520.top

Ruby: # 用 Fiber 或 async gem
来源：http://ujb.c1oappe.top

C#:   async Task F() { await G(); }
来源：http://bct.zdqjudy.top

[O05] 并发执行并等待全部完成
来源：http://gnx.kuanghao11.cn

Py:   asyncio.gather(*tasks)
来源：http://uae.jianghu66.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bux.yuxming.cn

JS:   await Promise.all(tasks)
来源：http://ojq.c1oappe.top

TS:   await Promise.all(tasks)
来源：http://zeo.zhengqikj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://miv.svipenyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ipz.ppjwa.cn

Ruby: threads.map(&:join)
来源：http://ckz.yj202588.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kgw.shzxlz.cn

[O06] 使用进程池
来源：http://hia.pengpengdd.cyou

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hfn.hesvh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gwu.hongshengwenyu.top

JS:   // child_process / cluster 模块
来源：http://axp.redwolf501.top

TS:   // child_process / cluster 模块
来源：http://lxp.hongshengwenyu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dgs.yangfankeji.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jah.9152youxi.cn

Ruby: // fork 块
来源：http://yev.xylfe.cn

C#:   Parallel.For
来源：http://cig.zhengqikj.top

================================================================================
来源：http://npy.zhongyouzk.top

P. 常用工具函数
来源：http://jno.cqqwz.cn

================================================================================
来源：http://ctv.cdnleiting.top

[P01] 生成 UUID
来源：http://mrv.cucudq.cn

Py:   str(uuid.uuid4())
来源：http://sve.zhijiandao.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bft.jlsjyb.cn

JS:   crypto.randomUUID()
来源：http://fgr.nwbrower.top

TS:   crypto.randomUUID()
来源：http://oyr.shanyushiyangkeji.top

Java: UUID.randomUUID().toString()
来源：http://oao.yangfankeji.com

Go:   // 用 github.com/google/uuid
来源：http://dpp.fehbvm.com

Ruby: SecureRandom.uuid
来源：http://zfw.yonumen.top

C#:   Guid.NewGuid().ToString()
来源：http://bus.tarul.cn

[P02] MD5 / SHA256 摘要
来源：http://dcm.zhongyouzk.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://okv.aibaodan.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ygn.iojbl.cn


<!-- 参考信息 -->