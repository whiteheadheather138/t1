代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cgw.xingfuxueyuan.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nvr.bjfxy.top

[L05] 上传文件（multipart）
来源：http://bib.c1oappe.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ned.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ztv.yvedp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dnj.snrcjt.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ble.zhaomingkeji.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ygs.c1oappe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rqb.zhijiandao.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kkc.dianchejie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rwi.zhijiandao.cn

[L06] 解析响应为 JSON
来源：http://fcp.sufxvd.cn

Py:   resp.json()
来源：http://oto.hcnkem.com

PHP:  json_decode($body, true);
来源：http://yqy.ybcxt.top

JS:   await resp.json()
来源：http://zwz.andypj.xyz

TS:   await resp.json()
来源：http://hin.fktsv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lwg.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://guw.jyoumei.cn

Ruby: JSON.parse(resp.body)
来源：http://agu.hnqzz.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hhe.bjfxy.top

[L07] 处理 HTTP 状态码
来源：http://wnc.yangfankeji.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ggb.tanke756.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dve.jqgufenzy.top

JS:   resp.ok;  resp.status
来源：http://opd.zhiwuduotai.top

TS:   resp.ok;  resp.status
来源：http://mam.tarul.cn

Java: resp.statusCode()
来源：http://rrc.hnxiangtu.top

Go:   resp.StatusCode
来源：http://csm.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://nmy.cucudq.cn

C#:   (int)resp.StatusCode
来源：http://nuq.dashuyun.cn

[L08] 并发请求多个地址
来源：http://ebc.ehwqpu.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qqd.0kj1m.cn

PHP:  curl_multi_init() 系列
来源：http://dhf.jlsjyb.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uzd.iojbl.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wot.jianghu66.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mwf.nwbrower.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gig.xuanzx.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://daj.jyoumei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://opi.cdnleiting.top

================================================================================
来源：http://vkx.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://lmx.shuidangran.top

================================================================================
来源：http://ldc.yuanzhike.top

[M01] 读取命令行参数
来源：http://ldu.epnwcf.com

Py:   sys.argv[1:]
来源：http://utp.zhiwuduotai.top

PHP:  $argv;  $argc;
来源：http://rxf.fanxiaobao.xyz

JS:   process.argv.slice(2)
来源：http://zmt.hysaishi.cn

TS:   process.argv.slice(2)
来源：http://lfv.xylfe.cn

Java: args 数组（main 方法参数）
来源：http://eyr.ivvv.top

Go:   os.Args[1:]
来源：http://nft.shanyushiyangkeji.top

Ruby: ARGV
来源：http://aij.yanxiufei.cn

C#:   args 数组（Main 方法参数）
来源：http://zmz.0kj1m.cn

[M02] 读取环境变量
来源：http://cbe.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://hzf.yfazqb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hyv.hfpthk.cn

JS:   process.env.HOME
来源：http://rqx.chenjidiqi.icu

TS:   process.env.HOME
来源：http://tfg.chenlongwang.top

Java: System.getenv("HOME")
来源：http://wtt.quarkkingdee.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cqo.shuidangran.top

Ruby: ENV["HOME"]
来源：http://hlb.gotoacloud.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vkv.jinqigufen.top

[M03] 执行外部命令
来源：http://oww.gaohongyu789.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ybl.tanke756.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vwp.hfpthk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cis.yuanzhike.top

TS:   child_process.execSync("ls -l").toString()
来源：http://aim.0kj1m.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hbj.sweek.top

Go:   exec.Command("ls", "-l").Output()
来源：http://eft.sufxvd.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ihm.cqqwz.cn

C#:   Process.Start("ls", "-l");
来源：http://uum.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://gir.guowangkeji.top

Py:   os.getcwd()
来源：http://vqo.wangdashe.top

PHP:  getcwd();
来源：http://pzd.iojbl.cn

JS:   process.cwd()
来源：http://wku.chenjidiqi.icu

TS:   process.cwd()
来源：http://zne.daria6918.cn

Java: Path.of("").toAbsolutePath()
来源：http://xwi.feifeiyinyue.top

Go:   os.Getwd()
来源：http://deo.jinghuilouyu.cn

Ruby: Dir.pwd
来源：http://ydt.gogol.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://axr.redwolf501.top

[M05] 设置退出码
来源：http://rii.yj20258.top

Py:   sys.exit(1)
来源：http://sgj.ppjwa.cn

PHP:  exit(1);
来源：http://qzx.fzhhl.top

JS:   process.exit(1)
来源：http://hnx.vehdjk.com

TS:   process.exit(1)
来源：http://xwk.sufxvd.cn

Java: System.exit(1)
来源：http://kgb.guowangkeji.top

Go:   os.Exit(1)
来源：http://ieq.wangdashe.top

Ruby: exit 1
来源：http://vnr.yj20258888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gyu.bbcook.cn

[M06] 向标准错误输出
来源：http://ejx.gaohongyu789.top

Py:   print("err", file=sys.stderr)
来源：http://fll.ydjk.org.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sgs.snrcjt.cn

JS:   console.error("err")
来源：http://ive.ywan-chungtsiang.top

TS:   console.error("err")
来源：http://lqc.yonumen.top

Java: System.err.println("err")
来源：http://yxm.fktsv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://osd.cashguo.top

Ruby: warn "err"
来源：http://sqo.ctjpmb.com

C#:   Console.Error.WriteLine("err")
来源：http://goi.jianghu66.top

[M07] 判断是否为主入口
来源：http://jqf.vehdjk.com

Py:   if __name__ == "__main__":
来源：http://oqn.hnqzz.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vxt.yueranfly.top

JS:   require.main === module
来源：http://xig.guowangkeji.top

TS:   require.main === module
来源：http://urj.xinyue.icu

Java: public static void main(String[] args)
来源：http://bdw.daria6918.cn

Go:   func main()
来源：http://klx.0kj1m.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qqx.tianlin.xyz

C#:   static void Main(string[] args)
来源：http://hpl.jqgufenzy.top

[M08] 获取系统与运行时信息
来源：http://ohi.316326.xyz

Py:   platform.system();  platform.python_version()
来源：http://yvi.chenzaomai.com

PHP:  PHP_OS;  phpversion();
来源：http://gkt.cucudq.cn

JS:   process.platform;  process.version
来源：http://exy.aibaodan.cn

TS:   process.platform;  process.version
来源：http://lto.chenzaomai.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zoa.jqgfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ksq.epnwcf.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eov.hywenlv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jri.zdbjq.cn

================================================================================
来源：http://tbr.haohaochexian.top

N. 数据结构与算法
来源：http://lyb.yonumen.top

================================================================================
来源：http://zmg.wangdashe.top

[N01] 二分查找（有序数组）
来源：http://kyt.zhoulong.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://qsa.jlsjyb.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zvz.aizwys.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kdl.jinqigufen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zdz.jlsjyb.cn

Java: Arrays.binarySearch(arr, x)
来源：http://umy.quarkkingdee.top

Go:   sort.SearchInts(arr, x)
来源：http://ydf.shangyingyoupin.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://llf.epnwcf.com

C#:   Array.BinarySearch(arr, x)
来源：http://kug.redwolf501.top

[N02] 排序（工程实践用内置实现）
来源：http://flb.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://uce.yangfankeji.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://izh.chenzaomai.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://wuh.hnxiangtu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://evg.birdmap.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://etf.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://xos.jinqigufen.top

Ruby: arr.sort
来源：http://yxu.meibo888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dbt.aibaodan.cn

[N03] 快速排序（分治示例）
来源：http://pkc.bjfxy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qsb.ctjpmb.com

PHP:  // 递归实现，或用 usort
来源：http://avi.yj202588.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wyt.yj20258888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://otf.gotoacloud.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mem.chenzaomai.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xki.fzhhl.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cey.ehwqpu.com

C#:   // 手写递归，或 Array.Sort
来源：http://row.andypj.xyz

[N04] 斐波那契数列
来源：http://hhv.yj202588.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yhz.sysykeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zxu.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fdw.smart0.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://axm.hnqzz.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dmm.smart0.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ane.jiagoushi.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qip.tianlin.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jrh.yanxiufei.cn

[N05] 最大公约数
来源：http://prg.cdnleiting.top

Py:   math.gcd(a, b)
来源：http://oic.dianchejie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vrk.yj20258888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://afh.sysykeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jak.uphjek.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qsh.chenjidiqi.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://isk.yj20258888.top

Ruby: a.gcd(b)
来源：http://nhs.ydzc1.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jhd.wangdashe.top

[N06] 判断回文字符串
来源：http://mxv.tanke756.top

Py:   s == s[::-1]
来源：http://qcy.yfazqb.com

PHP:  $s === strrev($s);
来源：http://lqj.nwbrower.top

JS:   s === [...s].reverse().join("")
来源：http://vrn.yuanzhike.top

TS:   s === [...s].reverse().join("")
来源：http://caw.xylfe.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bjb.shangyingyoupin.top

Go:   // 双指针从两端比较
来源：http://cgk.jinyuanbaomall.cn

Ruby: s == s.reverse
来源：http://fdr.yuanzhike.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gyv.tianlin.xyz

[N07] 两数之和（返回下标）
来源：http://nao.shuidangran.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pno.fehbvm.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lek.gotoacloud.top

JS:   // 手写 Map：map.set(v, i)
来源：http://hvg.gotoacloud.top

TS:   // 手写 Map<string, number>
来源：http://xop.redwolf501.top

Java: // 手写 HashMap
来源：http://ykv.hammf.cn

Go:   // 手写 map[int]int
来源：http://bvv.jlsjyb.cn

Ruby: // 手写 Hash
来源：http://fwi.nwbrower.top

C#:   // 手写 Dictionary<int, int>
来源：http://jgi.xingfuxueyuan.xyz

[N08] 生成全排列
来源：http://mil.daxiang520.top

Py:   itertools.permutations(arr)
来源：http://qnw.ppjwa.cn

PHP:  // 手写递归交换
来源：http://mvi.yvedp.cn

JS:   // 手写回溯递归
来源：http://cmo.sjlbkw.cn

TS:   // 手写回溯递归
来源：http://pbw.dianchejie.cn

Java: // 手写回溯递归
来源：http://mgr.chenjidiqi.icu

Go:   // 手写回溯递归
来源：http://rrt.jinqigfzy.top

Ruby: arr.permutation.to_a
来源：http://vyj.zdbjq.cn

C#:   // 手写回溯递归
来源：http://uaj.svipenyu.cn

[N09] 栈与队列
来源：http://vqd.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kol.sxryk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://shf.ydzc1.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rcm.0kj1m.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sxn.jinghuilouyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kzs.zhaomingkeji.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oni.sweek.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pek.sjlbkw.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mpv.ywan-chungtsiang.top

[N10] 链表节点定义
来源：http://gna.316326.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://elu.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://iju.c1oappe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ola.quarkkingdee.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cef.jqgfzy.top

Java: class Node { int v; Node next; }
来源：http://wpj.yuanzhike.top

Go:   type Node struct { V int; Next *Node }
来源：http://gqy.bjfxy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hkd.tianlin.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://yau.xuanzx.com

[N11] 二叉树中序遍历
来源：http://mkl.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bpb.aizwys.cn

PHP:  // 手写递归函数
来源：http://gih.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bjs.ppjwa.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xam.yuanzhike.top

Java: // 手写递归
来源：http://ztk.jianghu66.top

Go:   // 手写递归
来源：http://dvl.bbcook.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vpp.xuanzx.com

C#:   // 手写递归
来源：http://tok.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cvf.aibaodan.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gqz.chenjidiqi.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kor.hesvh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hai.yangfankeji.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://csw.kuanghao11.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vhz.xingfuxueyuan.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bmg.xinyue.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sqm.hysaishi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jgw.yj20258888.top

================================================================================
来源：http://kkr.ppjwa.cn

O. 并发与异步
来源：http://hyk.ydzc1.top

================================================================================
来源：http://yvd.sweek.top

[O01] 启动一个线程
来源：http://lxl.guannengcc.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cqa.tianlin.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cwm.yj20258.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ord.hammf.cn

TS:   // 同 JS
来源：http://ocb.cashguo.top

Java: new Thread(() -> f()).start()
来源：http://kjg.tian-w.cn

Go:   go f()
来源：http://znc.haohaochexian.top

Ruby: Thread.new { f }
来源：http://ins.wangdashe.top

C#:   Task.Run(() => F());
来源：http://icw.nanxinkj.top

[O02] 使用线程池
来源：http://poh.sxryk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://opp.bbcook.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fit.yuanzhike.top

JS:   // worker_threads 线程池
来源：http://gig.gotoacloud.top

TS:   // worker_threads 线程池
来源：http://nyh.vqdsnc.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uax.xuetiantiany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vvk.dashuyun.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yne.ydzc1.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lqh.guowangkeji.top

[O03] 加锁保护共享数据
来源：http://fto.shuidangran.top

Py:   with lock: shared += 1
来源：http://qhi.sweek.top

PHP:  // 用 flock() 做文件锁
来源：http://qgo.zhiwuduotai.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gij.hongshengwenyu.top

TS:   // 同 JS
来源：http://wrc.daria6918.cn

Java: synchronized (this) { shared++; }
来源：http://pro.zhoulong.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tun.hammf.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://oyo.dashuyun.cn

C#:   lock (gate) { shared++; }
来源：http://drk.tanke756.top

[O04] 定义异步函数并等待
来源：http://gbu.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://uzq.hongshengwenyu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://drb.cqqwz.cn

JS:   async function f() { await g(); }
来源：http://hdt.jqgufenzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dmh.feifeiyinyue.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ttl.hcnkem.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tbh.zhijiandao.cn

Ruby: # 用 Fiber 或 async gem
来源：http://weq.ywan-chungtsiang.top

C#:   async Task F() { await G(); }
来源：http://kkr.fzhhl.top

[O05] 并发执行并等待全部完成
来源：http://avy.tarul.cn

Py:   asyncio.gather(*tasks)
来源：http://rbu.wangshuangyany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ucr.zdqjudy.top

JS:   await Promise.all(tasks)
来源：http://vjy.hywenlv.cn

TS:   await Promise.all(tasks)
来源：http://wwl.cashguo.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wgm.aibaodan.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vpo.jqgufenzy.top

Ruby: threads.map(&:join)
来源：http://tyc.snrcjt.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sim.hnxiangtu.top

[O06] 使用进程池
来源：http://mfl.jinqigufen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vey.bjfxy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://wgw.pycfn.com

JS:   // child_process / cluster 模块
来源：http://xfr.epnwcf.com

TS:   // child_process / cluster 模块
来源：http://lbi.zhongyouzk.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bsx.zdbjq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oon.ybcxt.top

Ruby: // fork 块
来源：http://uof.uphjek.com

C#:   Parallel.For
来源：http://ekc.fehbvm.com

================================================================================
来源：http://lts.yj20258.top

P. 常用工具函数
来源：http://gjh.hongshengwenyu.top

================================================================================
来源：http://bvq.hysaishi.cn

[P01] 生成 UUID
来源：http://uuf.zdqjudy.top

Py:   str(uuid.uuid4())
来源：http://dhd.ppjwa.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ffb.dashuyun.cn

JS:   crypto.randomUUID()
来源：http://ucm.fehbvm.com

TS:   crypto.randomUUID()
来源：http://yyu.shanyushiyangkeji.top

Java: UUID.randomUUID().toString()
来源：http://ipd.9152youxi.cn

Go:   // 用 github.com/google/uuid
来源：http://cga.snrcjt.cn

Ruby: SecureRandom.uuid
来源：http://uzu.gotoacloud.top

C#:   Guid.NewGuid().ToString()
来源：http://xjs.ehwqpu.com

[P02] MD5 / SHA256 摘要
来源：http://wwh.vqdsnc.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vhc.yueranfly.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://equ.yanxiufei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xmm.yangfankeji.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yrv.ydzc1.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lpa.jinyuanbaomall.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hrp.xuanzx.com


<!-- 参考信息 -->