代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cej.snrcjt.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jpv.gotoacloud.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wmp.cdnleiting.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kru.gogol.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wor.hnxiangtu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wmq.sjlbkw.cn

[L05] 上传文件（multipart）
来源：http://uuw.sysykeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eje.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ulo.zhijiandao.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eli.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cwe.shanyushiyangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://stl.dianchejie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://elk.birdmap.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sin.hammf.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iay.gaohongyu789.top

[L06] 解析响应为 JSON
来源：http://tcb.xylfe.cn

Py:   resp.json()
来源：http://bjb.yj20258.top

PHP:  json_decode($body, true);
来源：http://uyc.tarul.cn

JS:   await resp.json()
来源：http://gjg.wangdashe.top

TS:   await resp.json()
来源：http://ugy.cucudq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tps.feifeiyinyue.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hni.yangfankeji.com

Ruby: JSON.parse(resp.body)
来源：http://akn.yj20258.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kgx.vehdjk.com

[L07] 处理 HTTP 状态码
来源：http://cov.xylfe.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mhc.uphjek.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wli.mhx1999.top

JS:   resp.ok;  resp.status
来源：http://hzx.gogol.net.cn

TS:   resp.ok;  resp.status
来源：http://zjb.kuanghao11.cn

Java: resp.statusCode()
来源：http://ldw.hesvh.cn

Go:   resp.StatusCode
来源：http://frs.mhx1999.top

Ruby: resp.code.to_i
来源：http://oug.ywan-chungtsiang.top

C#:   (int)resp.StatusCode
来源：http://huz.vehdjk.com

[L08] 并发请求多个地址
来源：http://vun.yonumen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jsf.zhaomingkeji.xyz

PHP:  curl_multi_init() 系列
来源：http://dgn.wangshuangyany.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ved.hcnkem.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tjc.ivvv.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bsv.chenlongwang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://whl.xingfuxueyuan.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gsv.andypj.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://doa.sxryk.cn

================================================================================
来源：http://ozl.daria6918.cn

M. 命令行 / 进程 / 环境
来源：http://aml.nanxuanxn.top

================================================================================
来源：http://xla.jqgufenzy.top

[M01] 读取命令行参数
来源：http://zpt.pycfn.com

Py:   sys.argv[1:]
来源：http://zlu.xingfuxueyuan.xyz

PHP:  $argv;  $argc;
来源：http://jof.daxiang520.top

JS:   process.argv.slice(2)
来源：http://biu.shangyingyoupin.top

TS:   process.argv.slice(2)
来源：http://tzq.cdnleiting.top

Java: args 数组（main 方法参数）
来源：http://gmf.hcnkem.com

Go:   os.Args[1:]
来源：http://ita.hfpthk.cn

Ruby: ARGV
来源：http://bfq.chenjidiqi.icu

C#:   args 数组（Main 方法参数）
来源：http://joo.bjfxy.top

[M02] 读取环境变量
来源：http://pel.xingfuxueyuan.xyz

Py:   os.environ.get("HOME")
来源：http://sxv.yonumen.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jkq.gogol.net.cn

JS:   process.env.HOME
来源：http://wid.fehbvm.com

TS:   process.env.HOME
来源：http://bcy.9152youxi.cn

Java: System.getenv("HOME")
来源：http://dll.ybcxt.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yoz.redwolf501.top

Ruby: ENV["HOME"]
来源：http://drf.nanxuanxn.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://knr.hysaishi.cn

[M03] 执行外部命令
来源：http://ckr.zhoulong.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mkn.hcnkem.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gbq.ehwqpu.com

JS:   child_process.execSync("ls -l").toString()
来源：http://emo.jiagoushi.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gxw.hongshengwenyu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wna.ybcxt.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ytv.yangfankeji.com

Ruby: system("ls -l");  `ls -l`
来源：http://bpg.zhiwuduotai.top

C#:   Process.Start("ls", "-l");
来源：http://iyg.sjlbkw.cn

[M04] 获取当前工作目录
来源：http://ruy.shanyushiyangkeji.top

Py:   os.getcwd()
来源：http://usa.tian-w.cn

PHP:  getcwd();
来源：http://yki.jinyuanbaomall.cn

JS:   process.cwd()
来源：http://baj.jqgfzy.top

TS:   process.cwd()
来源：http://vbu.gzhubu.top

Java: Path.of("").toAbsolutePath()
来源：http://cld.redwolf501.top

Go:   os.Getwd()
来源：http://xxt.ydjk.org.cn

Ruby: Dir.pwd
来源：http://uph.shangyingyoupin.top

C#:   Directory.GetCurrentDirectory()
来源：http://mrn.redwolf501.top

[M05] 设置退出码
来源：http://mds.sysykeji.top

Py:   sys.exit(1)
来源：http://gdp.ctjpmb.com

PHP:  exit(1);
来源：http://uct.hesvh.cn

JS:   process.exit(1)
来源：http://uig.jlsjyb.cn

TS:   process.exit(1)
来源：http://hit.fanxiaobao.xyz

Java: System.exit(1)
来源：http://qsp.dianchejie.cn

Go:   os.Exit(1)
来源：http://qpi.shzxlz.cn

Ruby: exit 1
来源：http://xml.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tsm.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://gpc.zhixingplan.top

Py:   print("err", file=sys.stderr)
来源：http://tdr.9152youxi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vfr.fzhhl.top

JS:   console.error("err")
来源：http://epi.jinqigufen.top

TS:   console.error("err")
来源：http://acs.nanxuanxn.top

Java: System.err.println("err")
来源：http://enx.havefunace.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wqx.cdnleiting.top

Ruby: warn "err"
来源：http://uwv.andypj.xyz

C#:   Console.Error.WriteLine("err")
来源：http://xjf.xziqi.cn

[M07] 判断是否为主入口
来源：http://qbe.vehdjk.com

Py:   if __name__ == "__main__":
来源：http://ywf.snrcjt.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nah.jiagoushi.top

JS:   require.main === module
来源：http://qzc.fanxiaobao.xyz

TS:   require.main === module
来源：http://auq.gaohongyu789.top

Java: public static void main(String[] args)
来源：http://rbp.hammf.cn

Go:   func main()
来源：http://ekj.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ooo.tarul.cn

C#:   static void Main(string[] args)
来源：http://bcp.zhiwuduotai.top

[M08] 获取系统与运行时信息
来源：http://qcw.yj20258888.top

Py:   platform.system();  platform.python_version()
来源：http://jsf.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://hbv.smart0.xyz

JS:   process.platform;  process.version
来源：http://xxk.guowangkeji.top

TS:   process.platform;  process.version
来源：http://gxu.yongpay.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bkl.hysaishi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://aqw.aizwys.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fpl.yueranfly.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bxs.nwbrower.top

================================================================================
来源：http://dqx.316326.xyz

N. 数据结构与算法
来源：http://efk.chenlongwang.top

================================================================================
来源：http://qci.jinqigufen.top

[N01] 二分查找（有序数组）
来源：http://dut.ywan-chungtsiang.top

Py:   bisect.bisect_left(arr, x)
来源：http://tqo.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yzg.redwolf501.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zzc.gzhubu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vdg.zhoulong.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://eti.sxryk.cn

Go:   sort.SearchInts(arr, x)
来源：http://nvj.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vvm.zhiwuduotai.top

C#:   Array.BinarySearch(arr, x)
来源：http://acn.jianghu66.top

[N02] 排序（工程实践用内置实现）
来源：http://ewu.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://ktr.guowangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nvg.ywan-chungtsiang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lki.birdmap.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cqc.feifeiyinyue.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ppw.xylfe.cn

Go:   slices.Sort(arr)
来源：http://awb.hfpthk.cn

Ruby: arr.sort
来源：http://cvp.fzhhl.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rga.shanyushiyangkeji.top

[N03] 快速排序（分治示例）
来源：http://paf.hongshengwenyu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vby.hammf.cn

PHP:  // 递归实现，或用 usort
来源：http://ibu.havefunace.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rgk.ydzc1.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zvy.redwolf501.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zhm.fengsongda.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://npz.zhaomingkeji.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bny.yongpay.top

C#:   // 手写递归，或 Array.Sort
来源：http://yvp.fanxiaobao.xyz

[N04] 斐波那契数列
来源：http://vlh.zhongyouzk.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dhu.cashguo.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mat.ppjwa.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oat.cashguo.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dia.quarkkingdee.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tyq.yongpay.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bpb.ydzc1.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fod.yfazqb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cou.uphjek.com

[N05] 最大公约数
来源：http://wol.jqgfzy.top

Py:   math.gcd(a, b)
来源：http://tiy.gzhubu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://umg.smart0.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bjv.xuanzx.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fzl.jianghu66.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bjx.shzxlz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ppu.fehbvm.com

Ruby: a.gcd(b)
来源：http://uzl.hongshengwenyu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nzl.hnqzz.top

[N06] 判断回文字符串
来源：http://igt.meibo888.top

Py:   s == s[::-1]
来源：http://bli.0kj1m.cn

PHP:  $s === strrev($s);
来源：http://htf.tanke756.top

JS:   s === [...s].reverse().join("")
来源：http://ubj.gzhubu.top

TS:   s === [...s].reverse().join("")
来源：http://owj.zhijiandao.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bsa.ybcxt.top

Go:   // 双指针从两端比较
来源：http://yyz.xinyue.icu

Ruby: s == s.reverse
来源：http://lzg.zhixingplan.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cqd.guannengcc.top

[N07] 两数之和（返回下标）
来源：http://xki.tarul.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wrs.cashguo.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vwf.wangdashe.top

JS:   // 手写 Map：map.set(v, i)
来源：http://plv.cqqwz.cn

TS:   // 手写 Map<string, number>
来源：http://rng.redwolf501.top

Java: // 手写 HashMap
来源：http://mww.yongpay.top

Go:   // 手写 map[int]int
来源：http://vnj.fehbvm.com

Ruby: // 手写 Hash
来源：http://lhg.wangdashe.top

C#:   // 手写 Dictionary<int, int>
来源：http://lkp.tian-w.cn

[N08] 生成全排列
来源：http://ixu.zdbjq.cn

Py:   itertools.permutations(arr)
来源：http://dec.svipenyu.cn

PHP:  // 手写递归交换
来源：http://raa.ydzc1.top

JS:   // 手写回溯递归
来源：http://ztt.birdmap.top

TS:   // 手写回溯递归
来源：http://gci.aibaodan.cn

Java: // 手写回溯递归
来源：http://czp.shuidangran.top

Go:   // 手写回溯递归
来源：http://kmr.tianlin.xyz

Ruby: arr.permutation.to_a
来源：http://pfj.zycfv.cn

C#:   // 手写回溯递归
来源：http://vqb.sxryk.cn

[N09] 栈与队列
来源：http://duu.gogol.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://egv.hfpthk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nwg.yfazqb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zyq.hysaishi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tlb.gaohongyu789.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pzt.xingfuxueyuan.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ujn.zdbjq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lin.gzhubu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nyc.yongpay.top

[N10] 链表节点定义
来源：http://qau.vehdjk.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mba.ivvv.top

PHP:  class Node { public $v; public $next = null; }
来源：http://veq.zhoulong.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bua.xuanzx.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://elq.yongpay.top

Java: class Node { int v; Node next; }
来源：http://dsp.nanxinkj.top

Go:   type Node struct { V int; Next *Node }
来源：http://svf.ehwqpu.com

Ruby: Node = Struct.new(:v, :next)
来源：http://xle.iojbl.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nxv.aibaodan.cn

[N11] 二叉树中序遍历
来源：http://sqx.vehdjk.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xfu.hcnkem.com

PHP:  // 手写递归函数
来源：http://zil.meibo888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kwc.cqqwz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tfj.sxryk.cn

Java: // 手写递归
来源：http://ohk.jlsjyb.cn

Go:   // 手写递归
来源：http://bix.jinyuanbaomall.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sfx.gotoacloud.top

C#:   // 手写递归
来源：http://dbm.hysaishi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ekg.redwolf501.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://edu.bjfxy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hjg.shangyingyoupin.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ctd.zhixingplan.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bcp.hywenlv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nwd.jianghu66.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hif.snrcjt.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ucz.xinyue.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://obo.guowangkeji.top

================================================================================
来源：http://xfe.ywan-chungtsiang.top

O. 并发与异步
来源：http://rhg.zhongyouzk.top

================================================================================
来源：http://omt.sjlbkw.cn

[O01] 启动一个线程
来源：http://lnm.jianghu66.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://epq.pengpengdd.cyou

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yzr.birdmap.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hfs.zhiwuduotai.top

TS:   // 同 JS
来源：http://pdb.vehdjk.com

Java: new Thread(() -> f()).start()
来源：http://bet.fehbvm.com

Go:   go f()
来源：http://qkn.nanxuanxn.top

Ruby: Thread.new { f }
来源：http://kbe.wangdashe.top

C#:   Task.Run(() => F());
来源：http://hsc.feifeiyinyue.top

[O02] 使用线程池
来源：http://lyj.cqqwz.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zdk.xziqi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zoe.yonumen.top

JS:   // worker_threads 线程池
来源：http://jgw.gogol.net.cn

TS:   // worker_threads 线程池
来源：http://cgr.sufxvd.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xmd.dianchejie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fky.pycfn.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jbg.cqqwz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pfb.wangdashe.top

[O03] 加锁保护共享数据
来源：http://znf.aibaodan.cn

Py:   with lock: shared += 1
来源：http://eht.hesvh.cn

PHP:  // 用 flock() 做文件锁
来源：http://eul.hongshengwenyu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vmk.chenjidiqi.icu

TS:   // 同 JS
来源：http://rdf.zhiwuduotai.top

Java: synchronized (this) { shared++; }
来源：http://mxb.yueranfly.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kpe.hongshengwenyu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://yva.nanxuanxn.top

C#:   lock (gate) { shared++; }
来源：http://wyl.ybcxt.top

[O04] 定义异步函数并等待
来源：http://yml.sufxvd.cn

Py:   async def f():⏎    await g()
来源：http://lfi.fktsv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iou.yueranfly.top

JS:   async function f() { await g(); }
来源：http://nsn.zhixingplan.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://mdn.nwbrower.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fau.tarul.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://box.cashguo.top

Ruby: # 用 Fiber 或 async gem
来源：http://dzg.yj202588.top

C#:   async Task F() { await G(); }
来源：http://sqi.gzhubu.top

[O05] 并发执行并等待全部完成
来源：http://jia.daria6918.cn

Py:   asyncio.gather(*tasks)
来源：http://vcj.zdbjq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lfd.xylfe.cn

JS:   await Promise.all(tasks)
来源：http://qip.jqgfzy.top

TS:   await Promise.all(tasks)
来源：http://ktp.ydjk.org.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fmk.xinyue.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lhe.0kj1m.cn

Ruby: threads.map(&:join)
来源：http://tqh.52xcode.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vjz.ivvv.top

[O06] 使用进程池
来源：http://zkm.yonumen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cyy.xingfuxueyuan.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://eue.gogol.net.cn

JS:   // child_process / cluster 模块
来源：http://bpz.jqgfzy.top

TS:   // child_process / cluster 模块
来源：http://uls.quarkkingdee.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://imu.hywenlv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gbc.shangyingyoupin.top

Ruby: // fork 块
来源：http://dyj.zhongyouzk.top

C#:   Parallel.For
来源：http://bao.nanxuanxn.top

================================================================================
来源：http://glh.hcnkem.com

P. 常用工具函数
来源：http://ywk.cheryme.top

================================================================================
来源：http://gzp.zhengqikj.top

[P01] 生成 UUID
来源：http://qhs.hfpthk.cn

Py:   str(uuid.uuid4())
来源：http://pmv.smart0.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://voc.birdmap.top

JS:   crypto.randomUUID()
来源：http://sik.bjfxy.top

TS:   crypto.randomUUID()
来源：http://jbs.zhaomingkeji.xyz

Java: UUID.randomUUID().toString()
来源：http://pqm.shuidangran.top

Go:   // 用 github.com/google/uuid
来源：http://nlk.yj202588.top

Ruby: SecureRandom.uuid
来源：http://ycz.shanyushiyangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://ubl.sweek.top

[P02] MD5 / SHA256 摘要
来源：http://diw.sweek.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lmn.redwolf501.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hem.andypj.xyz


<!-- 参考信息 -->