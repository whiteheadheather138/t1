代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bsf.andypj.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xyi.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://isq.wangshuangyany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vsx.jinqigfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vnb.cqqwz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kdd.hcnkem.com

[L05] 上传文件（multipart）
来源：http://cxd.hammf.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pjz.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cqv.uphjek.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nvh.jyoumei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ynr.haohaochexian.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://viw.shuidangran.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://psr.9152youxi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mmo.zhiwuduotai.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fkw.mhx1999.top

[L06] 解析响应为 JSON
来源：http://vpe.cdnleiting.top

Py:   resp.json()
来源：http://bbh.pengpengdd.cyou

PHP:  json_decode($body, true);
来源：http://sif.cheryme.top

JS:   await resp.json()
来源：http://ddz.gogol.net.cn

TS:   await resp.json()
来源：http://kgj.yonumen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://elz.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qcj.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://ios.tarul.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uds.meibo888.top

[L07] 处理 HTTP 状态码
来源：http://osd.jlsjyb.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ewi.fehbvm.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ade.guannengcc.top

JS:   resp.ok;  resp.status
来源：http://ghq.fehbvm.com

TS:   resp.ok;  resp.status
来源：http://jxh.kuanghao11.cn

Java: resp.statusCode()
来源：http://rfl.shanyushiyangtech.top

Go:   resp.StatusCode
来源：http://fhj.ydzc1.top

Ruby: resp.code.to_i
来源：http://jru.mhx1999.top

C#:   (int)resp.StatusCode
来源：http://otg.aizwys.cn

[L08] 并发请求多个地址
来源：http://kid.xuetiantiany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://scx.jianghu66.top

PHP:  curl_multi_init() 系列
来源：http://adk.daria6918.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ohp.xziqi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fxv.ybcxt.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xho.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gag.meibo888.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gkz.redwolf501.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qht.mhx1999.top

================================================================================
来源：http://omz.shangyingyoupin.top

M. 命令行 / 进程 / 环境
来源：http://ltc.chenjidiqi.icu

================================================================================
来源：http://zmp.cdnleiting.top

[M01] 读取命令行参数
来源：http://wik.bbcook.cn

Py:   sys.argv[1:]
来源：http://cpf.hfpthk.cn

PHP:  $argv;  $argc;
来源：http://egh.shzxlz.cn

JS:   process.argv.slice(2)
来源：http://jvg.havefunace.top

TS:   process.argv.slice(2)
来源：http://omd.uphjek.com

Java: args 数组（main 方法参数）
来源：http://ouw.kuanghao11.cn

Go:   os.Args[1:]
来源：http://dif.jqgufenzy.top

Ruby: ARGV
来源：http://mkn.jyoumei.cn

C#:   args 数组（Main 方法参数）
来源：http://ere.iojbl.cn

[M02] 读取环境变量
来源：http://dgp.pycfn.com

Py:   os.environ.get("HOME")
来源：http://nho.uphjek.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://syb.yonumen.top

JS:   process.env.HOME
来源：http://yey.jqgfzy.top

TS:   process.env.HOME
来源：http://bxi.sysykeji.top

Java: System.getenv("HOME")
来源：http://ryk.xylfe.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zjb.zhengqikj.top

Ruby: ENV["HOME"]
来源：http://lkw.dianchejie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tyc.yfazqb.com

[M03] 执行外部命令
来源：http://lsd.zdqjudy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vdw.xylfe.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ufx.fzhhl.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hjo.zycfv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bas.zhiwuduotai.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ldd.yuxming.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ivy.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://znz.tian-w.cn

C#:   Process.Start("ls", "-l");
来源：http://qzg.gogol.net.cn

[M04] 获取当前工作目录
来源：http://rwj.xinyue.icu

Py:   os.getcwd()
来源：http://hro.fehbvm.com

PHP:  getcwd();
来源：http://wli.gaohongyu789.top

JS:   process.cwd()
来源：http://xem.pengpengdd.cyou

TS:   process.cwd()
来源：http://mik.xuanzx.com

Java: Path.of("").toAbsolutePath()
来源：http://uhq.dianchejie.cn

Go:   os.Getwd()
来源：http://unc.tanke756.top

Ruby: Dir.pwd
来源：http://kin.gogol.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://eqr.wangshuangyany.cn

[M05] 设置退出码
来源：http://dcb.havefunace.top

Py:   sys.exit(1)
来源：http://jhf.gaohongyu789.top

PHP:  exit(1);
来源：http://ttw.smart0.xyz

JS:   process.exit(1)
来源：http://nuh.ydjk.org.cn

TS:   process.exit(1)
来源：http://orx.yuanzhike.top

Java: System.exit(1)
来源：http://vit.zhaomingkeji.xyz

Go:   os.Exit(1)
来源：http://rqw.daxiang520.top

Ruby: exit 1
来源：http://ddj.hesvh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wxd.bbcook.cn

[M06] 向标准错误输出
来源：http://bya.aizwys.cn

Py:   print("err", file=sys.stderr)
来源：http://fbc.yanxiufei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bpp.jianghu66.top

JS:   console.error("err")
来源：http://sul.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://dcb.yfazqb.com

Java: System.err.println("err")
来源：http://fhp.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tjn.yueranfly.top

Ruby: warn "err"
来源：http://mtj.yj20258888.top

C#:   Console.Error.WriteLine("err")
来源：http://lxz.aizwys.cn

[M07] 判断是否为主入口
来源：http://kgo.xuetiantiany.cn

Py:   if __name__ == "__main__":
来源：http://fzb.mhx1999.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bue.shanyushiyangkeji.top

JS:   require.main === module
来源：http://fph.shangyingyoupin.top

TS:   require.main === module
来源：http://wee.birdmap.top

Java: public static void main(String[] args)
来源：http://qee.xinyue.icu

Go:   func main()
来源：http://nro.gogol.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oae.shanyushiyangtech.top

C#:   static void Main(string[] args)
来源：http://vdi.jianghu66.top

[M08] 获取系统与运行时信息
来源：http://qqb.yanxiufei.cn

Py:   platform.system();  platform.python_version()
来源：http://qwn.yuanzhike.top

PHP:  PHP_OS;  phpversion();
来源：http://avu.bjfxy.top

JS:   process.platform;  process.version
来源：http://kie.zhixingplan.top

TS:   process.platform;  process.version
来源：http://oqm.ehwqpu.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ovv.jyoumei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fkr.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qkb.c1oappe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://odo.shzxlz.cn

================================================================================
来源：http://ntc.pengpengdd.cyou

N. 数据结构与算法
来源：http://kik.c1oappe.top

================================================================================
来源：http://chx.gzhubu.top

[N01] 二分查找（有序数组）
来源：http://fxz.yvedp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wae.guowangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://doy.jinqigufen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fdg.xinyue.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yah.snrcjt.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xrh.cheryme.top

Go:   sort.SearchInts(arr, x)
来源：http://isf.hesvh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jsj.ybcxt.top

C#:   Array.BinarySearch(arr, x)
来源：http://pzb.fehbvm.com

[N02] 排序（工程实践用内置实现）
来源：http://kdv.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://ptp.tian-w.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lib.hcnkem.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://dif.zdqjudy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ech.tian-w.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gjx.wangdashe.top

Go:   slices.Sort(arr)
来源：http://drp.gzhubu.top

Ruby: arr.sort
来源：http://xyq.hongshengwenyu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ydf.shanyushiyangkeji.top

[N03] 快速排序（分治示例）
来源：http://vbr.havefunace.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hno.yj20258.top

PHP:  // 递归实现，或用 usort
来源：http://uqy.yuxming.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mah.0kj1m.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ehj.zhixingplan.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lyn.pengpengdd.cyou

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rik.shanyushiyangtech.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bru.uphjek.com

C#:   // 手写递归，或 Array.Sort
来源：http://zoe.fengsongda.top

[N04] 斐波那契数列
来源：http://vwi.jlsjyb.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wyh.yongpay.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lyc.smart0.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ssx.yuanzhike.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hic.xziqi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yiw.wangdashe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iyw.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jjp.zhaomingkeji.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uld.cashguo.top

[N05] 最大公约数
来源：http://yih.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://uaf.ppjwa.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xhe.shanyushiyangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fxa.yfazqb.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cxz.birdmap.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wbm.jinqigufen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ejb.yj20258888.top

Ruby: a.gcd(b)
来源：http://ned.sufxvd.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://scx.yongpay.top

[N06] 判断回文字符串
来源：http://hzh.zhijiandao.cn

Py:   s == s[::-1]
来源：http://xnl.yj20258.top

PHP:  $s === strrev($s);
来源：http://isz.sweek.top

JS:   s === [...s].reverse().join("")
来源：http://kun.shanyushiyangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://vfe.daxiang520.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uwc.hywenlv.cn

Go:   // 双指针从两端比较
来源：http://okc.316326.xyz

Ruby: s == s.reverse
来源：http://lzf.uphjek.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://zjp.c1oappe.top

[N07] 两数之和（返回下标）
来源：http://der.hnxiangtu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bgy.kuanghao11.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yoh.daria6918.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://reu.guowangkeji.top

TS:   // 手写 Map<string, number>
来源：http://qew.yuxming.cn

Java: // 手写 HashMap
来源：http://xwt.hysaishi.cn

Go:   // 手写 map[int]int
来源：http://jdk.cheryme.top

Ruby: // 手写 Hash
来源：http://ysg.yvedp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iwl.aibaodan.cn

[N08] 生成全排列
来源：http://izk.yj20258888.top

Py:   itertools.permutations(arr)
来源：http://qda.pycfn.com

PHP:  // 手写递归交换
来源：http://hxp.dianchejie.cn

JS:   // 手写回溯递归
来源：http://kol.dashuyun.cn

TS:   // 手写回溯递归
来源：http://czw.snrcjt.cn

Java: // 手写回溯递归
来源：http://mcq.gzhubu.top

Go:   // 手写回溯递归
来源：http://qbd.ywan-chungtsiang.top

Ruby: arr.permutation.to_a
来源：http://qwv.zhengqikj.top

C#:   // 手写回溯递归
来源：http://slq.daria6918.cn

[N09] 栈与队列
来源：http://jup.daria6918.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xks.ywan-chungtsiang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wdk.bjfxy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fgm.kuanghao11.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dfo.yueranfly.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://liy.ivvv.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hzi.ydjk.org.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://utt.redwolf501.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tkz.tarul.cn

[N10] 链表节点定义
来源：http://xws.xylfe.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bne.jiagoushi.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zio.yj20258.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://khu.jlsjyb.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xaa.sxryk.cn

Java: class Node { int v; Node next; }
来源：http://tgx.haohaochexian.top

Go:   type Node struct { V int; Next *Node }
来源：http://yuy.jqgufenzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://pik.ehwqpu.com

C#:   class Node { public int V; public Node? Next; }
来源：http://few.smart0.xyz

[N11] 二叉树中序遍历
来源：http://wav.nwbrower.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tev.ivvv.top

PHP:  // 手写递归函数
来源：http://hmf.316326.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tne.52xcode.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jkn.zhongyouzk.top

Java: // 手写递归
来源：http://rhd.yanxiufei.cn

Go:   // 手写递归
来源：http://wib.chenzaomai.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vzu.jiagoushi.top

C#:   // 手写递归
来源：http://gfq.yongpay.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vtx.zhengqikj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ipg.shanyushiyangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rsm.havefunace.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://abt.yonumen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jld.wangdashe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pql.fengsongda.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jfi.uphjek.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gon.yj20258.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tcm.pycfn.com

================================================================================
来源：http://uok.vehdjk.com

O. 并发与异步
来源：http://hlh.zhaomingkeji.xyz

================================================================================
来源：http://owk.sysykeji.top

[O01] 启动一个线程
来源：http://xud.jinyuanbaomall.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dlw.tarul.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oeb.hcnkem.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zqr.fengsongda.top

TS:   // 同 JS
来源：http://jdh.jqgfzy.top

Java: new Thread(() -> f()).start()
来源：http://wgm.svipenyu.cn

Go:   go f()
来源：http://jqx.kuanghao11.cn

Ruby: Thread.new { f }
来源：http://ixm.sweek.top

C#:   Task.Run(() => F());
来源：http://xuu.c1oappe.top

[O02] 使用线程池
来源：http://nmt.bbcook.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://feq.ivvv.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zhv.guowangkeji.top

JS:   // worker_threads 线程池
来源：http://pzz.sjlbkw.cn

TS:   // worker_threads 线程池
来源：http://agy.cheryme.top

Java: Executors.newFixedThreadPool(4)
来源：http://kce.zdqjudy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cyb.daxiang520.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pvk.yuxming.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cwb.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://aid.nanxinkj.top

Py:   with lock: shared += 1
来源：http://ion.cashguo.top

PHP:  // 用 flock() 做文件锁
来源：http://bcj.yuanzhike.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yop.316326.xyz

TS:   // 同 JS
来源：http://bfk.zycfv.cn

Java: synchronized (this) { shared++; }
来源：http://zca.xziqi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wkk.pengpengdd.cyou

Ruby: mutex.synchronize { shared += 1 }
来源：http://ytb.tarul.cn

C#:   lock (gate) { shared++; }
来源：http://cza.cdnleiting.top

[O04] 定义异步函数并等待
来源：http://niy.gaohongyu789.top

Py:   async def f():⏎    await g()
来源：http://olf.xylfe.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ruy.quarkkingdee.top

JS:   async function f() { await g(); }
来源：http://mrd.xingfuxueyuan.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://kff.hesvh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ihf.ybcxt.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zag.shuidangran.top

Ruby: # 用 Fiber 或 async gem
来源：http://mvx.yongpay.top

C#:   async Task F() { await G(); }
来源：http://jmj.vehdjk.com

[O05] 并发执行并等待全部完成
来源：http://dwk.aibaodan.cn

Py:   asyncio.gather(*tasks)
来源：http://gyp.ivvv.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dae.epnwcf.com

JS:   await Promise.all(tasks)
来源：http://cet.vehdjk.com

TS:   await Promise.all(tasks)
来源：http://fgu.ydjk.org.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oyn.fzhhl.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oqc.fanxiaobao.xyz

Ruby: threads.map(&:join)
来源：http://qcm.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qtv.zhongyouzk.top

[O06] 使用进程池
来源：http://xfz.jqgufenzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://meu.aibaodan.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jyd.ehwqpu.com

JS:   // child_process / cluster 模块
来源：http://kun.yj20258888.top

TS:   // child_process / cluster 模块
来源：http://zak.chenzaomai.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fol.zhixingplan.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://syz.c1oappe.top

Ruby: // fork 块
来源：http://qwm.yj20258.top

C#:   Parallel.For
来源：http://opc.sufxvd.cn

================================================================================
来源：http://eqx.ctjpmb.com

P. 常用工具函数
来源：http://yht.dashuyun.cn

================================================================================
来源：http://fov.sjlbkw.cn

[P01] 生成 UUID
来源：http://vng.fengsongda.top

Py:   str(uuid.uuid4())
来源：http://oam.guannengcc.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ltg.yj202588.top

JS:   crypto.randomUUID()
来源：http://ftf.zhijiandao.cn

TS:   crypto.randomUUID()
来源：http://dvh.jinghuilouyu.cn

Java: UUID.randomUUID().toString()
来源：http://irg.wangshuangyany.cn

Go:   // 用 github.com/google/uuid
来源：http://zvb.fzhhl.top

Ruby: SecureRandom.uuid
来源：http://qzm.sjlbkw.cn

C#:   Guid.NewGuid().ToString()
来源：http://zis.xingfuxueyuan.xyz

[P02] MD5 / SHA256 摘要
来源：http://jlf.c1oappe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kfi.nwbrower.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://gez.kuanghao11.cn


<!-- 参考信息 -->