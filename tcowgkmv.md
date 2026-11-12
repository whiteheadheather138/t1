代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wnk.nanxinkj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gls.sysykeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tum.daxiang520.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fhd.yongpay.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zmc.zdqjudy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rjh.sysykeji.top

[L05] 上传文件（multipart）
来源：http://fav.jianghu66.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ahp.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qfp.ywan-chungtsiang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://boe.gotoacloud.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://upp.birdmap.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://inv.snrcjt.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fxd.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oti.jiagoushi.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jhu.pengpengdd.cyou

[L06] 解析响应为 JSON
来源：http://nxx.jiagoushi.top

Py:   resp.json()
来源：http://yvj.ydzc1.top

PHP:  json_decode($body, true);
来源：http://btt.shanyushiyangtech.top

JS:   await resp.json()
来源：http://agw.nwbrower.top

TS:   await resp.json()
来源：http://ohb.sweek.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hib.shangyingyoupin.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hvt.jqgfzy.top

Ruby: JSON.parse(resp.body)
来源：http://ybh.nanxinkj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dlh.fanxiaobao.xyz

[L07] 处理 HTTP 状态码
来源：http://jmm.cdnleiting.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nge.chenzaomai.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://shj.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://oki.jinqigfzy.top

TS:   resp.ok;  resp.status
来源：http://dhv.shzxlz.cn

Java: resp.statusCode()
来源：http://lcg.zhongyouzk.top

Go:   resp.StatusCode
来源：http://gec.nanxuanxn.top

Ruby: resp.code.to_i
来源：http://cgk.epnwcf.com

C#:   (int)resp.StatusCode
来源：http://wot.fengsongda.top

[L08] 并发请求多个地址
来源：http://npe.shanyushiyangkeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nfs.vehdjk.com

PHP:  curl_multi_init() 系列
来源：http://kxw.jinyuanbaomall.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xgc.xuanzx.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sya.andypj.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wdu.yj20258888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vco.dianchejie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://myt.gaohongyu789.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kky.zhijiandao.cn

================================================================================
来源：http://udz.vqdsnc.cn

M. 命令行 / 进程 / 环境
来源：http://jkx.cdnleiting.top

================================================================================
来源：http://ifi.52xcode.cn

[M01] 读取命令行参数
来源：http://wri.vehdjk.com

Py:   sys.argv[1:]
来源：http://nih.fengsongda.top

PHP:  $argv;  $argc;
来源：http://vbf.0kj1m.cn

JS:   process.argv.slice(2)
来源：http://ide.jqgufenzy.top

TS:   process.argv.slice(2)
来源：http://uaj.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://gab.ctjpmb.com

Go:   os.Args[1:]
来源：http://fkk.wangshuangyany.cn

Ruby: ARGV
来源：http://doo.yj20258888.top

C#:   args 数组（Main 方法参数）
来源：http://pse.yj20258.top

[M02] 读取环境变量
来源：http://eku.jinyuanbaomall.cn

Py:   os.environ.get("HOME")
来源：http://epv.jinqigfzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zhh.xuanzx.com

JS:   process.env.HOME
来源：http://xvs.xuanzx.com

TS:   process.env.HOME
来源：http://wzu.snrcjt.cn

Java: System.getenv("HOME")
来源：http://yba.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kbt.sweek.top

Ruby: ENV["HOME"]
来源：http://emj.pycfn.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mzs.snrcjt.cn

[M03] 执行外部命令
来源：http://tzt.ydzc1.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iqi.aibaodan.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ujy.ydjk.org.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bxu.xingfuxueyuan.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://uww.wangdashe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://csw.yvedp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tdw.guowangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://jcl.cheryme.top

C#:   Process.Start("ls", "-l");
来源：http://fmp.xuetiantiany.cn

[M04] 获取当前工作目录
来源：http://snq.gotoacloud.top

Py:   os.getcwd()
来源：http://hvx.haohaochexian.top

PHP:  getcwd();
来源：http://dlq.jqgufenzy.top

JS:   process.cwd()
来源：http://rnw.yueranfly.top

TS:   process.cwd()
来源：http://pmy.zhengqikj.top

Java: Path.of("").toAbsolutePath()
来源：http://rcd.pycfn.com

Go:   os.Getwd()
来源：http://ilj.zdbjq.cn

Ruby: Dir.pwd
来源：http://vto.cheryme.top

C#:   Directory.GetCurrentDirectory()
来源：http://jwn.zhaomingkeji.xyz

[M05] 设置退出码
来源：http://oaw.nanxinkj.top

Py:   sys.exit(1)
来源：http://puj.guowangkeji.top

PHP:  exit(1);
来源：http://bqz.jianghu66.top

JS:   process.exit(1)
来源：http://mnz.redwolf501.top

TS:   process.exit(1)
来源：http://jar.guannengcc.top

Java: System.exit(1)
来源：http://qrh.shanyushiyangtech.top

Go:   os.Exit(1)
来源：http://jgg.yangfankeji.com

Ruby: exit 1
来源：http://qnp.yanxiufei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bhj.svipenyu.cn

[M06] 向标准错误输出
来源：http://jyz.quarkkingdee.top

Py:   print("err", file=sys.stderr)
来源：http://aqs.tanke756.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gbh.hnqzz.top

JS:   console.error("err")
来源：http://jsf.cheryme.top

TS:   console.error("err")
来源：http://esz.iojbl.cn

Java: System.err.println("err")
来源：http://wgu.sysykeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ksk.wangdashe.top

Ruby: warn "err"
来源：http://asl.tanke756.top

C#:   Console.Error.WriteLine("err")
来源：http://lml.yuanzhike.top

[M07] 判断是否为主入口
来源：http://dek.jianghu66.top

Py:   if __name__ == "__main__":
来源：http://vwf.mhx1999.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kow.sufxvd.cn

JS:   require.main === module
来源：http://btn.bbcook.cn

TS:   require.main === module
来源：http://hpa.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://slx.zdqjudy.top

Go:   func main()
来源：http://gzm.daria6918.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gvc.hesvh.cn

C#:   static void Main(string[] args)
来源：http://aoo.tarul.cn

[M08] 获取系统与运行时信息
来源：http://ekf.chenlongwang.top

Py:   platform.system();  platform.python_version()
来源：http://ykc.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://upw.sufxvd.cn

JS:   process.platform;  process.version
来源：http://tbz.xinyue.icu

TS:   process.platform;  process.version
来源：http://xym.hywenlv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lbu.yongpay.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://agm.tarul.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vpx.gzhubu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://uht.nanxinkj.top

================================================================================
来源：http://wbz.yuxming.cn

N. 数据结构与算法
来源：http://tdc.yongpay.top

================================================================================
来源：http://jzk.hnxiangtu.top

[N01] 二分查找（有序数组）
来源：http://sdc.sysykeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://rjs.yangfankeji.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zes.hnqzz.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://afq.wangdashe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kvt.guowangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://cxo.yanxiufei.cn

Go:   sort.SearchInts(arr, x)
来源：http://nun.meibo888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://kqb.svipenyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rcw.jianghu66.top

[N02] 排序（工程实践用内置实现）
来源：http://bwy.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://qbp.daria6918.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://onz.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://zvf.ehwqpu.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://cdb.vqdsnc.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ieh.shzxlz.cn

Go:   slices.Sort(arr)
来源：http://cog.andypj.xyz

Ruby: arr.sort
来源：http://ymo.snrcjt.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xik.tian-w.cn

[N03] 快速排序（分治示例）
来源：http://jsu.daxiang520.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jpn.zhoulong.xyz

PHP:  // 递归实现，或用 usort
来源：http://fhm.chenlongwang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://teh.chenjidiqi.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ekh.xuetiantiany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xgi.fktsv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ryb.fanxiaobao.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oco.zhaomingkeji.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://iba.gzhubu.top

[N04] 斐波那契数列
来源：http://qut.shanyushiyangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://puo.zhengqikj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pon.shanyushiyangtech.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yxa.quarkkingdee.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cry.sysykeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wlx.yonumen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yym.jiagoushi.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dce.guannengcc.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lsi.jinqigfzy.top

[N05] 最大公约数
来源：http://qko.daxiang520.top

Py:   math.gcd(a, b)
来源：http://wyr.cdnleiting.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rtn.tanke756.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yez.yanxiufei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mzx.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zrc.svipenyu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fny.ydjk.org.cn

Ruby: a.gcd(b)
来源：http://ian.xuetiantiany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zvw.zhijiandao.cn

[N06] 判断回文字符串
来源：http://lxq.jlsjyb.cn

Py:   s == s[::-1]
来源：http://vrm.sjlbkw.cn

PHP:  $s === strrev($s);
来源：http://tlj.0kj1m.cn

JS:   s === [...s].reverse().join("")
来源：http://rum.zhongyouzk.top

TS:   s === [...s].reverse().join("")
来源：http://xvp.xinyue.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://umc.ybcxt.top

Go:   // 双指针从两端比较
来源：http://hqc.havefunace.top

Ruby: s == s.reverse
来源：http://vta.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://zgg.havefunace.top

[N07] 两数之和（返回下标）
来源：http://gvl.yvedp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wzd.hywenlv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tan.yj20258888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://pzi.guowangkeji.top

TS:   // 手写 Map<string, number>
来源：http://axz.ppjwa.cn

Java: // 手写 HashMap
来源：http://dvk.yueranfly.top

Go:   // 手写 map[int]int
来源：http://uql.cheryme.top

Ruby: // 手写 Hash
来源：http://kvj.sweek.top

C#:   // 手写 Dictionary<int, int>
来源：http://yac.jiagoushi.top

[N08] 生成全排列
来源：http://onk.zhixingplan.top

Py:   itertools.permutations(arr)
来源：http://oxt.zhixingplan.top

PHP:  // 手写递归交换
来源：http://dvi.zhengqikj.top

JS:   // 手写回溯递归
来源：http://xul.yfazqb.com

TS:   // 手写回溯递归
来源：http://pgu.xuanzx.com

Java: // 手写回溯递归
来源：http://byr.yuxming.cn

Go:   // 手写回溯递归
来源：http://uqi.yfazqb.com

Ruby: arr.permutation.to_a
来源：http://pbt.nanxinkj.top

C#:   // 手写回溯递归
来源：http://myy.daxiang520.top

[N09] 栈与队列
来源：http://eix.andypj.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fjr.c1oappe.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ybo.zhiwuduotai.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://odb.fengsongda.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nym.0kj1m.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://knf.yj202588.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://knm.zhengqikj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dcv.yangfankeji.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rre.chenlongwang.top

[N10] 链表节点定义
来源：http://unb.aizwys.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ief.xinyue.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://qub.mhx1999.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ppu.dianchejie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mli.kuanghao11.cn

Java: class Node { int v; Node next; }
来源：http://cia.birdmap.top

Go:   type Node struct { V int; Next *Node }
来源：http://hcd.sxryk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dqb.sjlbkw.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sbc.epnwcf.com

[N11] 二叉树中序遍历
来源：http://qyk.haohaochexian.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tdd.sufxvd.cn

PHP:  // 手写递归函数
来源：http://cwq.xziqi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yav.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gcx.hfpthk.cn

Java: // 手写递归
来源：http://niq.xinyue.icu

Go:   // 手写递归
来源：http://ies.ctjpmb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ayy.feifeiyinyue.top

C#:   // 手写递归
来源：http://yof.bjfxy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bif.zhixingplan.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kxg.hysaishi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zjv.sweek.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rhv.yueranfly.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zqi.zhongyouzk.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://goy.yuxming.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://maq.sxryk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dhe.ppjwa.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ttu.316326.xyz

================================================================================
来源：http://hap.gotoacloud.top

O. 并发与异步
来源：http://arw.shzxlz.cn

================================================================================
来源：http://gmf.nwbrower.top

[O01] 启动一个线程
来源：http://blj.havefunace.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aqr.vqdsnc.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bbq.hnxiangtu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pbp.pycfn.com

TS:   // 同 JS
来源：http://ano.cucudq.cn

Java: new Thread(() -> f()).start()
来源：http://faz.xinyue.icu

Go:   go f()
来源：http://xwz.fehbvm.com

Ruby: Thread.new { f }
来源：http://xke.fehbvm.com

C#:   Task.Run(() => F());
来源：http://hdu.gaohongyu789.top

[O02] 使用线程池
来源：http://lkc.ywan-chungtsiang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gyc.nwbrower.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lpw.andypj.xyz

JS:   // worker_threads 线程池
来源：http://uvv.zhixingplan.top

TS:   // worker_threads 线程池
来源：http://kwo.daxiang520.top

Java: Executors.newFixedThreadPool(4)
来源：http://ouu.jlsjyb.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sei.yongpay.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xgy.pycfn.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uad.daxiang520.top

[O03] 加锁保护共享数据
来源：http://hsl.gogol.net.cn

Py:   with lock: shared += 1
来源：http://axl.pycfn.com

PHP:  // 用 flock() 做文件锁
来源：http://ind.c1oappe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jdw.ctjpmb.com

TS:   // 同 JS
来源：http://hfk.hesvh.cn

Java: synchronized (this) { shared++; }
来源：http://eej.hnqzz.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gza.dashuyun.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kro.9152youxi.cn

C#:   lock (gate) { shared++; }
来源：http://jec.svipenyu.cn

[O04] 定义异步函数并等待
来源：http://hvj.tanke756.top

Py:   async def f():⏎    await g()
来源：http://fui.nwbrower.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ewo.0kj1m.cn

JS:   async function f() { await g(); }
来源：http://htc.cdnleiting.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://khz.c1oappe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dgt.svipenyu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xel.xuetiantiany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zav.jinyuanbaomall.cn

C#:   async Task F() { await G(); }
来源：http://sly.xinyue.icu

[O05] 并发执行并等待全部完成
来源：http://juz.ehwqpu.com

Py:   asyncio.gather(*tasks)
来源：http://jga.jinyuanbaomall.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://skt.zdbjq.cn

JS:   await Promise.all(tasks)
来源：http://rtg.c1oappe.top

TS:   await Promise.all(tasks)
来源：http://qgw.fanxiaobao.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dua.cheryme.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fsl.cucudq.cn

Ruby: threads.map(&:join)
来源：http://goq.jinyuanbaomall.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://etp.jinqigfzy.top

[O06] 使用进程池
来源：http://vtp.zycfv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hdr.hnxiangtu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://wds.zhaomingkeji.xyz

JS:   // child_process / cluster 模块
来源：http://oea.fanxiaobao.xyz

TS:   // child_process / cluster 模块
来源：http://tqk.zhengqikj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pto.tian-w.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zdk.vehdjk.com

Ruby: // fork 块
来源：http://puy.hcnkem.com

C#:   Parallel.For
来源：http://lln.zdbjq.cn

================================================================================
来源：http://pzv.zhixingplan.top

P. 常用工具函数
来源：http://qfd.tianlin.xyz

================================================================================
来源：http://ssr.daria6918.cn

[P01] 生成 UUID
来源：http://lki.guannengcc.top

Py:   str(uuid.uuid4())
来源：http://anr.zhiwuduotai.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jyr.tian-w.cn

JS:   crypto.randomUUID()
来源：http://rlu.daxiang520.top

TS:   crypto.randomUUID()
来源：http://glt.xingfuxueyuan.xyz

Java: UUID.randomUUID().toString()
来源：http://gfj.sysykeji.top

Go:   // 用 github.com/google/uuid
来源：http://dbl.hfpthk.cn

Ruby: SecureRandom.uuid
来源：http://nrd.havefunace.top

C#:   Guid.NewGuid().ToString()
来源：http://qcd.mhx1999.top

[P02] MD5 / SHA256 摘要
来源：http://mnb.jlsjyb.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jgt.shanyushiyangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://gvp.redwolf501.top


<!-- 参考信息 -->