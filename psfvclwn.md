代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bgi.cqqwz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kaq.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ehy.snrcjt.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ppn.uphjek.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tgt.iojbl.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ixe.sjlbkw.cn

[L05] 上传文件（multipart）
来源：http://ysa.hywenlv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zaf.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lkr.hesvh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bjx.yj20258888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fwe.zdbjq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tei.jinqigufen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dhg.xinyue.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ugd.guannengcc.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rbn.guowangkeji.top

[L06] 解析响应为 JSON
来源：http://vjf.dianchejie.cn

Py:   resp.json()
来源：http://ork.yj202588.top

PHP:  json_decode($body, true);
来源：http://zxh.nwbrower.top

JS:   await resp.json()
来源：http://nzw.daria6918.cn

TS:   await resp.json()
来源：http://mor.yanxiufei.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hxy.yangfankeji.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://skz.sxryk.cn

Ruby: JSON.parse(resp.body)
来源：http://hbn.kuanghao11.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rym.wangdashe.top

[L07] 处理 HTTP 状态码
来源：http://bsf.hongshengwenyu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zqu.sysykeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uen.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://odx.yj202588.top

TS:   resp.ok;  resp.status
来源：http://unf.hnxiangtu.top

Java: resp.statusCode()
来源：http://ita.fanxiaobao.xyz

Go:   resp.StatusCode
来源：http://cqt.haohaochexian.top

Ruby: resp.code.to_i
来源：http://vup.9152youxi.cn

C#:   (int)resp.StatusCode
来源：http://nfd.hongshengwenyu.top

[L08] 并发请求多个地址
来源：http://yvb.quarkkingdee.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ufk.zycfv.cn

PHP:  curl_multi_init() 系列
来源：http://qte.hesvh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://huo.yangfankeji.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tfp.sysykeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sqm.tian-w.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://clz.hnqzz.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://swg.yvedp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oli.mhx1999.top

================================================================================
来源：http://dph.hnxiangtu.top

M. 命令行 / 进程 / 环境
来源：http://ymq.ppjwa.cn

================================================================================
来源：http://jwc.hywenlv.cn

[M01] 读取命令行参数
来源：http://pdz.ywan-chungtsiang.top

Py:   sys.argv[1:]
来源：http://zbz.iojbl.cn

PHP:  $argv;  $argc;
来源：http://sif.guannengcc.top

JS:   process.argv.slice(2)
来源：http://hgl.wangdashe.top

TS:   process.argv.slice(2)
来源：http://mbn.cqqwz.cn

Java: args 数组（main 方法参数）
来源：http://yud.xuetiantiany.cn

Go:   os.Args[1:]
来源：http://wte.yvedp.cn

Ruby: ARGV
来源：http://bne.wangdashe.top

C#:   args 数组（Main 方法参数）
来源：http://piw.aibaodan.cn

[M02] 读取环境变量
来源：http://wqp.ydjk.org.cn

Py:   os.environ.get("HOME")
来源：http://bud.gzhubu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yxi.hfpthk.cn

JS:   process.env.HOME
来源：http://vuw.yuanzhike.top

TS:   process.env.HOME
来源：http://zjs.bbcook.cn

Java: System.getenv("HOME")
来源：http://uyk.yvedp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://chb.ydjk.org.cn

Ruby: ENV["HOME"]
来源：http://gtv.cheryme.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mov.chenlongwang.top

[M03] 执行外部命令
来源：http://oup.cqqwz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xii.wangshuangyany.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xwc.cucudq.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ium.yanxiufei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dxf.hnxiangtu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dtf.birdmap.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xfx.jlsjyb.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wuy.316326.xyz

C#:   Process.Start("ls", "-l");
来源：http://wow.haohaochexian.top

[M04] 获取当前工作目录
来源：http://str.fehbvm.com

Py:   os.getcwd()
来源：http://vui.shzxlz.cn

PHP:  getcwd();
来源：http://tpl.jinyuanbaomall.cn

JS:   process.cwd()
来源：http://mse.chenjidiqi.icu

TS:   process.cwd()
来源：http://svx.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://gif.shanyushiyangkeji.top

Go:   os.Getwd()
来源：http://wzg.c1oappe.top

Ruby: Dir.pwd
来源：http://glx.9152youxi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zkl.tarul.cn

[M05] 设置退出码
来源：http://ciw.cashguo.top

Py:   sys.exit(1)
来源：http://gnl.chenzaomai.com

PHP:  exit(1);
来源：http://ivb.meibo888.top

JS:   process.exit(1)
来源：http://snj.jqgfzy.top

TS:   process.exit(1)
来源：http://jpx.iojbl.cn

Java: System.exit(1)
来源：http://hog.zhengqikj.top

Go:   os.Exit(1)
来源：http://wus.yuanzhike.top

Ruby: exit 1
来源：http://ogc.kuanghao11.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ehl.chenjidiqi.icu

[M06] 向标准错误输出
来源：http://xzg.9152youxi.cn

Py:   print("err", file=sys.stderr)
来源：http://xde.316326.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://vbb.ydzc1.top

JS:   console.error("err")
来源：http://chp.nanxuanxn.top

TS:   console.error("err")
来源：http://kzk.hongshengwenyu.top

Java: System.err.println("err")
来源：http://fgt.jqgufenzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://res.jinqigufen.top

Ruby: warn "err"
来源：http://ntb.zhiwuduotai.top

C#:   Console.Error.WriteLine("err")
来源：http://eio.xziqi.cn

[M07] 判断是否为主入口
来源：http://ulk.yueranfly.top

Py:   if __name__ == "__main__":
来源：http://ucj.cashguo.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vdt.fktsv.cn

JS:   require.main === module
来源：http://rtd.zhijiandao.cn

TS:   require.main === module
来源：http://kko.birdmap.top

Java: public static void main(String[] args)
来源：http://ebe.hysaishi.cn

Go:   func main()
来源：http://tkc.pycfn.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mia.ydzc1.top

C#:   static void Main(string[] args)
来源：http://tql.hysaishi.cn

[M08] 获取系统与运行时信息
来源：http://pzv.pycfn.com

Py:   platform.system();  platform.python_version()
来源：http://vwl.gzhubu.top

PHP:  PHP_OS;  phpversion();
来源：http://qxl.zhixingplan.top

JS:   process.platform;  process.version
来源：http://mnd.yonumen.top

TS:   process.platform;  process.version
来源：http://znt.jlsjyb.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ngd.meibo888.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wuj.xziqi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://izq.smart0.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://mfl.xuanzx.com

================================================================================
来源：http://sdk.bbcook.cn

N. 数据结构与算法
来源：http://dzk.zhaomingkeji.xyz

================================================================================
来源：http://vwc.xziqi.cn

[N01] 二分查找（有序数组）
来源：http://ens.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://vmu.yuanzhike.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gsj.chenzaomai.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qkj.meibo888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cqm.tian-w.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xsg.havefunace.top

Go:   sort.SearchInts(arr, x)
来源：http://vkm.hnqzz.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jgd.xziqi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dxg.yuanzhike.top

[N02] 排序（工程实践用内置实现）
来源：http://zvj.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://jsv.shanyushiyangtech.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cgg.ctjpmb.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://rzj.wangshuangyany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zuv.xingfuxueyuan.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://der.nanxinkj.top

Go:   slices.Sort(arr)
来源：http://rvi.aibaodan.cn

Ruby: arr.sort
来源：http://amr.epnwcf.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://brk.hfpthk.cn

[N03] 快速排序（分治示例）
来源：http://olw.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ywo.uphjek.com

PHP:  // 递归实现，或用 usort
来源：http://kii.ehwqpu.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cbd.aibaodan.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nnv.guannengcc.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zdf.zhongyouzk.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ere.xuanzx.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bbz.ivvv.top

C#:   // 手写递归，或 Array.Sort
来源：http://syq.cqqwz.cn

[N04] 斐波那契数列
来源：http://hfm.xingfuxueyuan.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://thw.vqdsnc.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kkl.fengsongda.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sfm.ywan-chungtsiang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fts.yonumen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nor.ehwqpu.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aik.zhongyouzk.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hde.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://npl.yangfankeji.com

[N05] 最大公约数
来源：http://wqx.cucudq.cn

Py:   math.gcd(a, b)
来源：http://hry.svipenyu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nba.shanyushiyangtech.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aiz.zhiwuduotai.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ywu.zhoulong.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ppp.hcnkem.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hcc.hongshengwenyu.top

Ruby: a.gcd(b)
来源：http://ccc.guannengcc.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://iol.meibo888.top

[N06] 判断回文字符串
来源：http://ugd.yj202588.top

Py:   s == s[::-1]
来源：http://vol.bbcook.cn

PHP:  $s === strrev($s);
来源：http://rqb.zhiwuduotai.top

JS:   s === [...s].reverse().join("")
来源：http://iml.ybcxt.top

TS:   s === [...s].reverse().join("")
来源：http://vgk.chenjidiqi.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://isr.havefunace.top

Go:   // 双指针从两端比较
来源：http://jvk.fengsongda.top

Ruby: s == s.reverse
来源：http://was.zdbjq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://thi.pycfn.com

[N07] 两数之和（返回下标）
来源：http://geo.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cbc.yongpay.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gda.hesvh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ehz.52xcode.cn

TS:   // 手写 Map<string, number>
来源：http://phi.ivvv.top

Java: // 手写 HashMap
来源：http://vgg.zhiwuduotai.top

Go:   // 手写 map[int]int
来源：http://hmp.quarkkingdee.top

Ruby: // 手写 Hash
来源：http://zrh.gzhubu.top

C#:   // 手写 Dictionary<int, int>
来源：http://chb.sysykeji.top

[N08] 生成全排列
来源：http://wxu.cashguo.top

Py:   itertools.permutations(arr)
来源：http://rzx.zycfv.cn

PHP:  // 手写递归交换
来源：http://sav.cucudq.cn

JS:   // 手写回溯递归
来源：http://voj.ppjwa.cn

TS:   // 手写回溯递归
来源：http://hzt.jinyuanbaomall.cn

Java: // 手写回溯递归
来源：http://mol.hnqzz.top

Go:   // 手写回溯递归
来源：http://ymj.hysaishi.cn

Ruby: arr.permutation.to_a
来源：http://ovr.zhengqikj.top

C#:   // 手写回溯递归
来源：http://nek.fzhhl.top

[N09] 栈与队列
来源：http://tsv.shanyushiyangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qzz.cheryme.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mny.vqdsnc.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aem.jqgfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gxi.hnqzz.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mte.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vni.shanyushiyangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pum.tianlin.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qvq.hcnkem.com

[N10] 链表节点定义
来源：http://ehj.xinyue.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wrs.cucudq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wnt.yuxming.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://laq.cqqwz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ixg.tanke756.top

Java: class Node { int v; Node next; }
来源：http://dsx.fktsv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ayi.gogol.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zfn.316326.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://sld.hywenlv.cn

[N11] 二叉树中序遍历
来源：http://mwy.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gzd.wangdashe.top

PHP:  // 手写递归函数
来源：http://ifq.pengpengdd.cyou

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yin.shanyushiyangtech.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://heb.feifeiyinyue.top

Java: // 手写递归
来源：http://euj.redwolf501.top

Go:   // 手写递归
来源：http://iap.hnqzz.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xms.meibo888.top

C#:   // 手写递归
来源：http://mff.yj202588.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kkx.ctjpmb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lfz.fktsv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xap.fanxiaobao.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cnv.snrcjt.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ghs.daxiang520.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dwf.ppjwa.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pbb.zhaomingkeji.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iph.vqdsnc.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tpx.uphjek.com

================================================================================
来源：http://fwy.xinyue.icu

O. 并发与异步
来源：http://nzb.ehwqpu.com

================================================================================
来源：http://jze.andypj.xyz

[O01] 启动一个线程
来源：http://ydn.sjlbkw.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://urq.uphjek.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lrl.52xcode.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zzu.zhiwuduotai.top

TS:   // 同 JS
来源：http://jnk.daxiang520.top

Java: new Thread(() -> f()).start()
来源：http://luw.havefunace.top

Go:   go f()
来源：http://cep.xziqi.cn

Ruby: Thread.new { f }
来源：http://ilh.zhijiandao.cn

C#:   Task.Run(() => F());
来源：http://fiq.fengsongda.top

[O02] 使用线程池
来源：http://bmd.316326.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xxo.nwbrower.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qmn.quarkkingdee.top

JS:   // worker_threads 线程池
来源：http://bhl.zhongyouzk.top

TS:   // worker_threads 线程池
来源：http://snt.snrcjt.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kda.sjlbkw.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cto.sjlbkw.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fbh.jqgfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lay.jqgfzy.top

[O03] 加锁保护共享数据
来源：http://vmn.shanyushiyangkeji.top

Py:   with lock: shared += 1
来源：http://cnz.xylfe.cn

PHP:  // 用 flock() 做文件锁
来源：http://rqg.chenjidiqi.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bya.gogol.net.cn

TS:   // 同 JS
来源：http://czf.c1oappe.top

Java: synchronized (this) { shared++; }
来源：http://lfu.zhixingplan.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rlh.yongpay.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://sgg.ywan-chungtsiang.top

C#:   lock (gate) { shared++; }
来源：http://waw.jiagoushi.top

[O04] 定义异步函数并等待
来源：http://cjw.52xcode.cn

Py:   async def f():⏎    await g()
来源：http://ffn.gogol.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lvz.feifeiyinyue.top

JS:   async function f() { await g(); }
来源：http://mjq.gotoacloud.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://uvr.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pcm.aibaodan.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lyu.nanxuanxn.top

Ruby: # 用 Fiber 或 async gem
来源：http://fzt.gaohongyu789.top

C#:   async Task F() { await G(); }
来源：http://cxa.redwolf501.top

[O05] 并发执行并等待全部完成
来源：http://siy.jqgufenzy.top

Py:   asyncio.gather(*tasks)
来源：http://ggw.wangshuangyany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oif.gogol.net.cn

JS:   await Promise.all(tasks)
来源：http://xli.bbcook.cn

TS:   await Promise.all(tasks)
来源：http://qme.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ymw.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xlc.daxiang520.top

Ruby: threads.map(&:join)
来源：http://fjd.xingfuxueyuan.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://qev.vehdjk.com

[O06] 使用进程池
来源：http://knz.tanke756.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sog.chenlongwang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nqc.zhiwuduotai.top

JS:   // child_process / cluster 模块
来源：http://xim.vqdsnc.cn

TS:   // child_process / cluster 模块
来源：http://jnw.ywan-chungtsiang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bmz.jinqigufen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rjc.jinqigufen.top

Ruby: // fork 块
来源：http://qrc.quarkkingdee.top

C#:   Parallel.For
来源：http://ghg.sxryk.cn

================================================================================
来源：http://toa.uphjek.com

P. 常用工具函数
来源：http://nxm.ehwqpu.com

================================================================================
来源：http://vqd.zhiwuduotai.top

[P01] 生成 UUID
来源：http://bru.nanxuanxn.top

Py:   str(uuid.uuid4())
来源：http://uuz.ydjk.org.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jon.nanxuanxn.top

JS:   crypto.randomUUID()
来源：http://eip.svipenyu.cn

TS:   crypto.randomUUID()
来源：http://kjr.hywenlv.cn

Java: UUID.randomUUID().toString()
来源：http://ulz.tianlin.xyz

Go:   // 用 github.com/google/uuid
来源：http://wrb.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://fpa.daria6918.cn

C#:   Guid.NewGuid().ToString()
来源：http://zbm.yj20258888.top

[P02] MD5 / SHA256 摘要
来源：http://kgl.shzxlz.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://byl.yvedp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ldz.yuanzhike.top


<!-- 参考信息 -->