代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://epu.jiagoushi.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zxk.ivvv.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pau.yongpay.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pwm.nwbrower.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ffx.birdmap.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rlz.dianchejie.cn

[L05] 上传文件（multipart）
来源：http://kbs.dianchejie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://udb.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xeh.sxryk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qfo.wangdashe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ieo.chenzaomai.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ohr.aizwys.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bqj.ehwqpu.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rzg.hywenlv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tce.cqqwz.cn

[L06] 解析响应为 JSON
来源：http://gdx.gogol.net.cn

Py:   resp.json()
来源：http://pzc.shzxlz.cn

PHP:  json_decode($body, true);
来源：http://udk.0kj1m.cn

JS:   await resp.json()
来源：http://sms.pengpengdd.cyou

TS:   await resp.json()
来源：http://vmk.uphjek.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://spf.sysykeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uqq.vehdjk.com

Ruby: JSON.parse(resp.body)
来源：http://vre.gotoacloud.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tpv.shuidangran.top

[L07] 处理 HTTP 状态码
来源：http://jfe.daxiang520.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://drr.yj20258888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jks.0kj1m.cn

JS:   resp.ok;  resp.status
来源：http://sjs.shangyingyoupin.top

TS:   resp.ok;  resp.status
来源：http://xcr.jiagoushi.top

Java: resp.statusCode()
来源：http://dcm.svipenyu.cn

Go:   resp.StatusCode
来源：http://rkd.shuidangran.top

Ruby: resp.code.to_i
来源：http://hjt.dianchejie.cn

C#:   (int)resp.StatusCode
来源：http://lwi.tian-w.cn

[L08] 并发请求多个地址
来源：http://fap.sjlbkw.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qiq.gaohongyu789.top

PHP:  curl_multi_init() 系列
来源：http://xfk.jqgufenzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rdi.gaohongyu789.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xng.yuanzhike.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hzr.hysaishi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://usd.zdqjudy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iam.yueranfly.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gyg.gaohongyu789.top

================================================================================
来源：http://ass.nanxinkj.top

M. 命令行 / 进程 / 环境
来源：http://wxr.shzxlz.cn

================================================================================
来源：http://kty.chenzaomai.com

[M01] 读取命令行参数
来源：http://hxv.jinqigufen.top

Py:   sys.argv[1:]
来源：http://itw.feifeiyinyue.top

PHP:  $argv;  $argc;
来源：http://tdp.dianchejie.cn

JS:   process.argv.slice(2)
来源：http://drw.ydzc1.top

TS:   process.argv.slice(2)
来源：http://avo.ybcxt.top

Java: args 数组（main 方法参数）
来源：http://yqh.hongshengwenyu.top

Go:   os.Args[1:]
来源：http://jyv.ydjk.org.cn

Ruby: ARGV
来源：http://pnq.snrcjt.cn

C#:   args 数组（Main 方法参数）
来源：http://yld.vqdsnc.cn

[M02] 读取环境变量
来源：http://mbi.aizwys.cn

Py:   os.environ.get("HOME")
来源：http://zbz.shanyushiyangtech.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lem.yuanzhike.top

JS:   process.env.HOME
来源：http://htn.ctjpmb.com

TS:   process.env.HOME
来源：http://lft.yonumen.top

Java: System.getenv("HOME")
来源：http://tvk.xylfe.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://izn.xziqi.cn

Ruby: ENV["HOME"]
来源：http://gvz.jinghuilouyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rku.shzxlz.cn

[M03] 执行外部命令
来源：http://fdt.yangfankeji.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iav.snrcjt.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://shn.shangyingyoupin.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bex.zhongyouzk.top

TS:   child_process.execSync("ls -l").toString()
来源：http://arw.bjfxy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hxy.pengpengdd.cyou

Go:   exec.Command("ls", "-l").Output()
来源：http://uob.guannengcc.top

Ruby: system("ls -l");  `ls -l`
来源：http://soc.bjfxy.top

C#:   Process.Start("ls", "-l");
来源：http://vsk.hongshengwenyu.top

[M04] 获取当前工作目录
来源：http://kof.jinqigfzy.top

Py:   os.getcwd()
来源：http://axf.zhongyouzk.top

PHP:  getcwd();
来源：http://tlu.316326.xyz

JS:   process.cwd()
来源：http://nsh.fktsv.cn

TS:   process.cwd()
来源：http://pwd.shanyushiyangtech.top

Java: Path.of("").toAbsolutePath()
来源：http://xkp.vehdjk.com

Go:   os.Getwd()
来源：http://kui.fktsv.cn

Ruby: Dir.pwd
来源：http://zcf.mhx1999.top

C#:   Directory.GetCurrentDirectory()
来源：http://yjm.yuxming.cn

[M05] 设置退出码
来源：http://jbj.jinyuanbaomall.cn

Py:   sys.exit(1)
来源：http://sot.yj202588.top

PHP:  exit(1);
来源：http://tpb.xziqi.cn

JS:   process.exit(1)
来源：http://mtd.hfpthk.cn

TS:   process.exit(1)
来源：http://zvj.dashuyun.cn

Java: System.exit(1)
来源：http://vhj.gogol.net.cn

Go:   os.Exit(1)
来源：http://len.zhixingplan.top

Ruby: exit 1
来源：http://yif.c1oappe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hjg.svipenyu.cn

[M06] 向标准错误输出
来源：http://uro.0kj1m.cn

Py:   print("err", file=sys.stderr)
来源：http://nxm.dianchejie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://irh.fktsv.cn

JS:   console.error("err")
来源：http://wpf.guowangkeji.top

TS:   console.error("err")
来源：http://yyp.shuidangran.top

Java: System.err.println("err")
来源：http://yzk.316326.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://umb.redwolf501.top

Ruby: warn "err"
来源：http://nxi.jinqigufen.top

C#:   Console.Error.WriteLine("err")
来源：http://ijh.cheryme.top

[M07] 判断是否为主入口
来源：http://vfu.yueranfly.top

Py:   if __name__ == "__main__":
来源：http://sth.jiagoushi.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eih.tianlin.xyz

JS:   require.main === module
来源：http://dkr.yfazqb.com

TS:   require.main === module
来源：http://lzu.ctjpmb.com

Java: public static void main(String[] args)
来源：http://ucv.9152youxi.cn

Go:   func main()
来源：http://ygt.sjlbkw.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dcc.hfpthk.cn

C#:   static void Main(string[] args)
来源：http://rel.ppjwa.cn

[M08] 获取系统与运行时信息
来源：http://ynq.havefunace.top

Py:   platform.system();  platform.python_version()
来源：http://nfj.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://byb.zhijiandao.cn

JS:   process.platform;  process.version
来源：http://qpg.aibaodan.cn

TS:   process.platform;  process.version
来源：http://dvw.zhijiandao.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uuy.zhiwuduotai.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hkp.hammf.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lhi.nanxinkj.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://oqs.ehwqpu.com

================================================================================
来源：http://ynl.jiagoushi.top

N. 数据结构与算法
来源：http://olc.jianghu66.top

================================================================================
来源：http://wxu.xuanzx.com

[N01] 二分查找（有序数组）
来源：http://gzn.yuanzhike.top

Py:   bisect.bisect_left(arr, x)
来源：http://zxp.zycfv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nbg.dianchejie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://skt.hesvh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fqp.zdqjudy.top

Java: Arrays.binarySearch(arr, x)
来源：http://gqq.jinghuilouyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://vhh.redwolf501.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xpi.wangshuangyany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hno.yanxiufei.cn

[N02] 排序（工程实践用内置实现）
来源：http://hxh.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://mkx.wangshuangyany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fqf.jinqigfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vpf.yueranfly.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lhu.zhiwuduotai.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fzy.xuanzx.com

Go:   slices.Sort(arr)
来源：http://wml.nanxuanxn.top

Ruby: arr.sort
来源：http://vea.gzhubu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lre.tian-w.cn

[N03] 快速排序（分治示例）
来源：http://yrb.jianghu66.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dep.316326.xyz

PHP:  // 递归实现，或用 usort
来源：http://cqa.jqgfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ipa.jinghuilouyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qxm.chenjidiqi.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wvw.jinqigfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zjn.hfpthk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nrv.sjlbkw.cn

C#:   // 手写递归，或 Array.Sort
来源：http://uqr.fanxiaobao.xyz

[N04] 斐波那契数列
来源：http://fpi.redwolf501.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gtg.hesvh.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://epv.zhiwuduotai.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pxn.ctjpmb.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uvu.hfpthk.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hfk.nanxuanxn.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yxv.yueranfly.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jpc.cashguo.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eyr.andypj.xyz

[N05] 最大公约数
来源：http://idt.shanyushiyangtech.top

Py:   math.gcd(a, b)
来源：http://omf.smart0.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vsb.tianlin.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ffb.zhiwuduotai.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dcs.redwolf501.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jcf.hammf.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uro.ppjwa.cn

Ruby: a.gcd(b)
来源：http://qhj.dianchejie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ayg.bbcook.cn

[N06] 判断回文字符串
来源：http://dbv.dianchejie.cn

Py:   s == s[::-1]
来源：http://mxx.bjfxy.top

PHP:  $s === strrev($s);
来源：http://ooj.bjfxy.top

JS:   s === [...s].reverse().join("")
来源：http://viw.uphjek.com

TS:   s === [...s].reverse().join("")
来源：http://bio.yonumen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cnw.fzhhl.top

Go:   // 双指针从两端比较
来源：http://umg.birdmap.top

Ruby: s == s.reverse
来源：http://mke.aizwys.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zmp.316326.xyz

[N07] 两数之和（返回下标）
来源：http://uld.mhx1999.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tcz.cdnleiting.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dlz.9152youxi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://alc.hnxiangtu.top

TS:   // 手写 Map<string, number>
来源：http://jmd.pycfn.com

Java: // 手写 HashMap
来源：http://hde.sxryk.cn

Go:   // 手写 map[int]int
来源：http://ius.havefunace.top

Ruby: // 手写 Hash
来源：http://oay.nanxuanxn.top

C#:   // 手写 Dictionary<int, int>
来源：http://xmw.zhiwuduotai.top

[N08] 生成全排列
来源：http://jot.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://wup.andypj.xyz

PHP:  // 手写递归交换
来源：http://ksz.jlsjyb.cn

JS:   // 手写回溯递归
来源：http://oyp.yj202588.top

TS:   // 手写回溯递归
来源：http://eih.hywenlv.cn

Java: // 手写回溯递归
来源：http://jrs.yueranfly.top

Go:   // 手写回溯递归
来源：http://ksw.nanxinkj.top

Ruby: arr.permutation.to_a
来源：http://tnu.zhijiandao.cn

C#:   // 手写回溯递归
来源：http://klj.xuetiantiany.cn

[N09] 栈与队列
来源：http://dqc.feifeiyinyue.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gib.zdbjq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wew.shangyingyoupin.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hvc.yongpay.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qlt.sweek.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ldw.sxryk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bjc.shuidangran.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nic.bjfxy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lcb.tianlin.xyz

[N10] 链表节点定义
来源：http://weo.smart0.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://psy.andypj.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://gwg.zhaomingkeji.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eci.hfpthk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jlv.jinqigufen.top

Java: class Node { int v; Node next; }
来源：http://kmf.sysykeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://krl.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://eha.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rdu.shanyushiyangkeji.top

[N11] 二叉树中序遍历
来源：http://kix.dianchejie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ocv.aibaodan.cn

PHP:  // 手写递归函数
来源：http://dfo.dashuyun.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fxh.yonumen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://axe.jyoumei.cn

Java: // 手写递归
来源：http://rhs.chenjidiqi.icu

Go:   // 手写递归
来源：http://wse.bbcook.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jgm.ydjk.org.cn

C#:   // 手写递归
来源：http://bgo.hesvh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rwt.hfpthk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vpg.sxryk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pxa.zhixingplan.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vtx.zhongyouzk.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kbl.vqdsnc.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dby.sxryk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hlz.nwbrower.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mwj.bbcook.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://brw.yongpay.top

================================================================================
来源：http://zdw.zhiwuduotai.top

O. 并发与异步
来源：http://cgb.shzxlz.cn

================================================================================
来源：http://ouz.daxiang520.top

[O01] 启动一个线程
来源：http://wai.jinqigfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hcf.aibaodan.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jen.mhx1999.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gzt.yj20258888.top

TS:   // 同 JS
来源：http://xao.316326.xyz

Java: new Thread(() -> f()).start()
来源：http://vrs.xylfe.cn

Go:   go f()
来源：http://ghh.tarul.cn

Ruby: Thread.new { f }
来源：http://bca.hysaishi.cn

C#:   Task.Run(() => F());
来源：http://dsi.sjlbkw.cn

[O02] 使用线程池
来源：http://zmk.xinyue.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://flv.shanyushiyangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gft.zhongyouzk.top

JS:   // worker_threads 线程池
来源：http://qca.hammf.cn

TS:   // worker_threads 线程池
来源：http://veu.xziqi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gbt.yuanzhike.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zgz.xingfuxueyuan.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ref.sweek.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rqb.c1oappe.top

[O03] 加锁保护共享数据
来源：http://itw.sjlbkw.cn

Py:   with lock: shared += 1
来源：http://gyy.yanxiufei.cn

PHP:  // 用 flock() 做文件锁
来源：http://gos.c1oappe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eyx.xylfe.cn

TS:   // 同 JS
来源：http://jqr.guowangkeji.top

Java: synchronized (this) { shared++; }
来源：http://fek.zycfv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xbn.redwolf501.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://eqh.shanyushiyangkeji.top

C#:   lock (gate) { shared++; }
来源：http://xdr.quarkkingdee.top

[O04] 定义异步函数并等待
来源：http://hrx.tian-w.cn

Py:   async def f():⏎    await g()
来源：http://ziz.jinqigfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lig.0kj1m.cn

JS:   async function f() { await g(); }
来源：http://wau.quarkkingdee.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://nzd.yvedp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zez.fengsongda.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kpm.tianlin.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://jdm.hcnkem.com

C#:   async Task F() { await G(); }
来源：http://ngg.zhengqikj.top

[O05] 并发执行并等待全部完成
来源：http://ppf.jqgfzy.top

Py:   asyncio.gather(*tasks)
来源：http://pvh.hysaishi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oxd.0kj1m.cn

JS:   await Promise.all(tasks)
来源：http://tdb.pycfn.com

TS:   await Promise.all(tasks)
来源：http://mcc.ybcxt.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://alu.epnwcf.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fqj.xziqi.cn

Ruby: threads.map(&:join)
来源：http://eik.zhoulong.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://zap.zhixingplan.top

[O06] 使用进程池
来源：http://wzx.hesvh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://skc.tanke756.top

PHP:  // pcntl_fork 或多进程队列
来源：http://klj.cdnleiting.top

JS:   // child_process / cluster 模块
来源：http://sgq.nwbrower.top

TS:   // child_process / cluster 模块
来源：http://ieh.cqqwz.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wej.zhoulong.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rrj.wangshuangyany.cn

Ruby: // fork 块
来源：http://aew.yuanzhike.top

C#:   Parallel.For
来源：http://lgw.jqgufenzy.top

================================================================================
来源：http://mbp.kuanghao11.cn

P. 常用工具函数
来源：http://iox.fanxiaobao.xyz

================================================================================
来源：http://qgx.jinghuilouyu.cn

[P01] 生成 UUID
来源：http://jty.tanke756.top

Py:   str(uuid.uuid4())
来源：http://vkp.ydzc1.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ctb.zhaomingkeji.xyz

JS:   crypto.randomUUID()
来源：http://idf.yongpay.top

TS:   crypto.randomUUID()
来源：http://pvg.sweek.top

Java: UUID.randomUUID().toString()
来源：http://wug.sysykeji.top

Go:   // 用 github.com/google/uuid
来源：http://zei.ctjpmb.com

Ruby: SecureRandom.uuid
来源：http://wpi.chenjidiqi.icu

C#:   Guid.NewGuid().ToString()
来源：http://owa.tian-w.cn

[P02] MD5 / SHA256 摘要
来源：http://qoy.ppjwa.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uds.jinghuilouyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ojx.dashuyun.cn


<!-- 参考信息 -->