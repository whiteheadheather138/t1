代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://agf.fanxiaobao.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zge.dianchejie.cn

[L05] 上传文件（multipart）
来源：http://kvb.zdqjudy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oia.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fao.hywenlv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bnq.yanxiufei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://die.shzxlz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://atx.zhaomingkeji.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cre.fanxiaobao.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uvc.dianchejie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dow.nwbrower.top

[L06] 解析响应为 JSON
来源：http://tby.chenlongwang.top

Py:   resp.json()
来源：http://ltp.aizwys.cn

PHP:  json_decode($body, true);
来源：http://spe.snrcjt.cn

JS:   await resp.json()
来源：http://izf.jiagoushi.top

TS:   await resp.json()
来源：http://ovr.ppjwa.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xeu.sjlbkw.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sms.yj20258888.top

Ruby: JSON.parse(resp.body)
来源：http://xqg.yj20258888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zom.zdbjq.cn

[L07] 处理 HTTP 状态码
来源：http://kbw.hnxiangtu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://srm.hnxiangtu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fyx.jiagoushi.top

JS:   resp.ok;  resp.status
来源：http://cvv.sysykeji.top

TS:   resp.ok;  resp.status
来源：http://vlo.pycfn.com

Java: resp.statusCode()
来源：http://tww.yuanzhike.top

Go:   resp.StatusCode
来源：http://akd.hnqzz.top

Ruby: resp.code.to_i
来源：http://bmr.zhiwuduotai.top

C#:   (int)resp.StatusCode
来源：http://yex.fehbvm.com

[L08] 并发请求多个地址
来源：http://vki.zhongyouzk.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://frv.hfpthk.cn

PHP:  curl_multi_init() 系列
来源：http://gkv.havefunace.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://snl.fehbvm.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qjd.aizwys.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wgs.mhx1999.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://krw.chenjidiqi.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ibe.yj202588.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kek.fehbvm.com

================================================================================
来源：http://rel.yuxming.cn

M. 命令行 / 进程 / 环境
来源：http://rvr.shangyingyoupin.top

================================================================================
来源：http://zwy.yueranfly.top

[M01] 读取命令行参数
来源：http://cur.cucudq.cn

Py:   sys.argv[1:]
来源：http://lxb.cashguo.top

PHP:  $argv;  $argc;
来源：http://ndh.jinghuilouyu.cn

JS:   process.argv.slice(2)
来源：http://ugs.xinyue.icu

TS:   process.argv.slice(2)
来源：http://bfz.ybcxt.top

Java: args 数组（main 方法参数）
来源：http://zal.zdqjudy.top

Go:   os.Args[1:]
来源：http://ads.daria6918.cn

Ruby: ARGV
来源：http://gmu.zdqjudy.top

C#:   args 数组（Main 方法参数）
来源：http://jll.fengsongda.top

[M02] 读取环境变量
来源：http://ftf.zdbjq.cn

Py:   os.environ.get("HOME")
来源：http://kpc.haohaochexian.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tna.hnqzz.top

JS:   process.env.HOME
来源：http://gsj.52xcode.cn

TS:   process.env.HOME
来源：http://hfy.yj20258888.top

Java: System.getenv("HOME")
来源：http://cmc.bbcook.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lwd.52xcode.cn

Ruby: ENV["HOME"]
来源：http://rxh.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ptg.zdqjudy.top

[M03] 执行外部命令
来源：http://tdt.hammf.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vdj.yueranfly.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dnx.zhixingplan.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pnv.jyoumei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pqo.jinyuanbaomall.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mdj.cucudq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://evs.zycfv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ccd.hnxiangtu.top

C#:   Process.Start("ls", "-l");
来源：http://fje.chenzaomai.com

[M04] 获取当前工作目录
来源：http://qrp.hnqzz.top

Py:   os.getcwd()
来源：http://pzz.zhengqikj.top

PHP:  getcwd();
来源：http://aqz.yuanzhike.top

JS:   process.cwd()
来源：http://wnp.jqgfzy.top

TS:   process.cwd()
来源：http://jmh.fengsongda.top

Java: Path.of("").toAbsolutePath()
来源：http://cwr.hywenlv.cn

Go:   os.Getwd()
来源：http://psr.chenzaomai.com

Ruby: Dir.pwd
来源：http://fjw.gogol.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zpv.cdnleiting.top

[M05] 设置退出码
来源：http://vvj.uphjek.com

Py:   sys.exit(1)
来源：http://viz.shanyushiyangtech.top

PHP:  exit(1);
来源：http://rwl.daria6918.cn

JS:   process.exit(1)
来源：http://ngm.jqgfzy.top

TS:   process.exit(1)
来源：http://trs.fanxiaobao.xyz

Java: System.exit(1)
来源：http://xpc.vehdjk.com

Go:   os.Exit(1)
来源：http://ekj.yvedp.cn

Ruby: exit 1
来源：http://ocp.hnxiangtu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rsv.yueranfly.top

[M06] 向标准错误输出
来源：http://gkh.tian-w.cn

Py:   print("err", file=sys.stderr)
来源：http://pgw.jinghuilouyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yem.yj20258888.top

JS:   console.error("err")
来源：http://afp.tanke756.top

TS:   console.error("err")
来源：http://yru.jinghuilouyu.cn

Java: System.err.println("err")
来源：http://ltf.vehdjk.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://srj.nanxinkj.top

Ruby: warn "err"
来源：http://lth.jianghu66.top

C#:   Console.Error.WriteLine("err")
来源：http://boj.vqdsnc.cn

[M07] 判断是否为主入口
来源：http://ryz.yfazqb.com

Py:   if __name__ == "__main__":
来源：http://xbo.sysykeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yvl.yj20258888.top

JS:   require.main === module
来源：http://elb.xingfuxueyuan.xyz

TS:   require.main === module
来源：http://zuw.dianchejie.cn

Java: public static void main(String[] args)
来源：http://ntx.nanxuanxn.top

Go:   func main()
来源：http://fql.hnxiangtu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fic.zhengqikj.top

C#:   static void Main(string[] args)
来源：http://gyl.xziqi.cn

[M08] 获取系统与运行时信息
来源：http://dcc.shanyushiyangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://hyn.zhixingplan.top

PHP:  PHP_OS;  phpversion();
来源：http://isw.daria6918.cn

JS:   process.platform;  process.version
来源：http://hmf.gaohongyu789.top

TS:   process.platform;  process.version
来源：http://zys.zdbjq.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://alm.gotoacloud.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://bao.gaohongyu789.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wwl.jinqigfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mxp.svipenyu.cn

================================================================================
来源：http://azo.gaohongyu789.top

N. 数据结构与算法
来源：http://dyo.zhoulong.xyz

================================================================================
来源：http://rrk.xziqi.cn

[N01] 二分查找（有序数组）
来源：http://yak.jinqigfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://yaw.ywan-chungtsiang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://esp.jianghu66.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cwh.fengsongda.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://caa.pycfn.com

Java: Arrays.binarySearch(arr, x)
来源：http://nmt.shuidangran.top

Go:   sort.SearchInts(arr, x)
来源：http://sgn.chenzaomai.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://auo.shanyushiyangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://buz.quarkkingdee.top

[N02] 排序（工程实践用内置实现）
来源：http://nbn.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://ncw.smart0.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rgf.tanke756.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://hsl.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oet.yangfankeji.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yaj.hnxiangtu.top

Go:   slices.Sort(arr)
来源：http://shi.vqdsnc.cn

Ruby: arr.sort
来源：http://qpp.c1oappe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://val.ehwqpu.com

[N03] 快速排序（分治示例）
来源：http://mcx.sysykeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xlq.ehwqpu.com

PHP:  // 递归实现，或用 usort
来源：http://nls.guowangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qma.sjlbkw.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ruo.fengsongda.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mxl.c1oappe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wbm.zhoulong.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ggu.hammf.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yqx.guowangkeji.top

[N04] 斐波那契数列
来源：http://ago.yvedp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://smy.jyoumei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tjs.pycfn.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rdh.52xcode.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ika.bjfxy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://viq.sufxvd.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sfl.cqqwz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hpl.wangdashe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hkm.fzhhl.top

[N05] 最大公约数
来源：http://psa.tianlin.xyz

Py:   math.gcd(a, b)
来源：http://nvn.yj20258888.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://squ.shuidangran.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lzv.chenlongwang.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nol.shanyushiyangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dwl.52xcode.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jqv.yj20258888.top

Ruby: a.gcd(b)
来源：http://nip.svipenyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xic.xylfe.cn

[N06] 判断回文字符串
来源：http://rnj.jinyuanbaomall.cn

Py:   s == s[::-1]
来源：http://iqv.9152youxi.cn

PHP:  $s === strrev($s);
来源：http://ztc.yonumen.top

JS:   s === [...s].reverse().join("")
来源：http://fgh.uphjek.com

TS:   s === [...s].reverse().join("")
来源：http://qoj.jinghuilouyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rhb.redwolf501.top

Go:   // 双指针从两端比较
来源：http://hnu.pycfn.com

Ruby: s == s.reverse
来源：http://rnp.bjfxy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nfs.hcnkem.com

[N07] 两数之和（返回下标）
来源：http://pwf.jqgfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hox.jqgufenzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wpr.iojbl.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://etl.uphjek.com

TS:   // 手写 Map<string, number>
来源：http://duz.aibaodan.cn

Java: // 手写 HashMap
来源：http://uzf.zdbjq.cn

Go:   // 手写 map[int]int
来源：http://jdb.yueranfly.top

Ruby: // 手写 Hash
来源：http://xer.tian-w.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lzd.ctjpmb.com

[N08] 生成全排列
来源：http://kqx.ivvv.top

Py:   itertools.permutations(arr)
来源：http://uff.cdnleiting.top

PHP:  // 手写递归交换
来源：http://ohh.shanyushiyangkeji.top

JS:   // 手写回溯递归
来源：http://qrx.redwolf501.top

TS:   // 手写回溯递归
来源：http://xnd.ydjk.org.cn

Java: // 手写回溯递归
来源：http://kme.sysykeji.top

Go:   // 手写回溯递归
来源：http://xag.kuanghao11.cn

Ruby: arr.permutation.to_a
来源：http://ibd.hysaishi.cn

C#:   // 手写回溯递归
来源：http://nnr.fanxiaobao.xyz

[N09] 栈与队列
来源：http://xrx.jinqigfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bju.xuanzx.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vlg.sysykeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fnb.gzhubu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zek.ywan-chungtsiang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://srj.hfpthk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ewh.hesvh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tqt.haohaochexian.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zfs.zhengqikj.top

[N10] 链表节点定义
来源：http://iqd.jqgfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mqi.yfazqb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://hkh.c1oappe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://htb.hongshengwenyu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://osg.jlsjyb.cn

Java: class Node { int v; Node next; }
来源：http://vjw.jianghu66.top

Go:   type Node struct { V int; Next *Node }
来源：http://dji.daxiang520.top

Ruby: Node = Struct.new(:v, :next)
来源：http://weu.yj20258.top

C#:   class Node { public int V; public Node? Next; }
来源：http://nyo.hywenlv.cn

[N11] 二叉树中序遍历
来源：http://isr.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ogw.hammf.cn

PHP:  // 手写递归函数
来源：http://ofs.tanke756.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://evg.meibo888.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pct.yuanzhike.top

Java: // 手写递归
来源：http://aiu.52xcode.cn

Go:   // 手写递归
来源：http://pxa.shuidangran.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yeq.zhaomingkeji.xyz

C#:   // 手写递归
来源：http://nle.aibaodan.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gkn.ppjwa.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kqa.yongpay.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yzu.shangyingyoupin.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lab.xingfuxueyuan.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lpm.hongshengwenyu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lxt.cheryme.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qlz.tianlin.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yhi.shangyingyoupin.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hgi.fanxiaobao.xyz

================================================================================
来源：http://zqj.nanxinkj.top

O. 并发与异步
来源：http://ftb.andypj.xyz

================================================================================
来源：http://iak.yvedp.cn

[O01] 启动一个线程
来源：http://jhl.meibo888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ymn.bbcook.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mee.yongpay.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hgz.hnqzz.top

TS:   // 同 JS
来源：http://phy.hysaishi.cn

Java: new Thread(() -> f()).start()
来源：http://wck.cheryme.top

Go:   go f()
来源：http://muk.hnqzz.top

Ruby: Thread.new { f }
来源：http://dfy.hcnkem.com

C#:   Task.Run(() => F());
来源：http://gmc.yueranfly.top

[O02] 使用线程池
来源：http://dfs.chenjidiqi.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fkl.hysaishi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ryf.jinqigufen.top

JS:   // worker_threads 线程池
来源：http://oyb.aibaodan.cn

TS:   // worker_threads 线程池
来源：http://zwn.xylfe.cn

Java: Executors.newFixedThreadPool(4)
来源：http://btf.haohaochexian.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bsm.cashguo.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tpo.ehwqpu.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hgq.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://tcm.zhixingplan.top

Py:   with lock: shared += 1
来源：http://sny.yj20258.top

PHP:  // 用 flock() 做文件锁
来源：http://jsk.shanyushiyangtech.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kjr.316326.xyz

TS:   // 同 JS
来源：http://thy.tian-w.cn

Java: synchronized (this) { shared++; }
来源：http://umk.xylfe.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pyv.zdbjq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://joz.wangdashe.top

C#:   lock (gate) { shared++; }
来源：http://uio.vqdsnc.cn

[O04] 定义异步函数并等待
来源：http://mgm.ctjpmb.com

Py:   async def f():⏎    await g()
来源：http://hfj.yueranfly.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fyq.sysykeji.top

JS:   async function f() { await g(); }
来源：http://sjw.hysaishi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dzv.fengsongda.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://onr.shanyushiyangkeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fld.ehwqpu.com

Ruby: # 用 Fiber 或 async gem
来源：http://yjb.dashuyun.cn

C#:   async Task F() { await G(); }
来源：http://ddw.bbcook.cn

[O05] 并发执行并等待全部完成
来源：http://iqe.hammf.cn

Py:   asyncio.gather(*tasks)
来源：http://pro.yj202588.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wkv.mhx1999.top

JS:   await Promise.all(tasks)
来源：http://obx.tian-w.cn

TS:   await Promise.all(tasks)
来源：http://cdb.xinyue.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qsx.xingfuxueyuan.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://itd.ppjwa.cn

Ruby: threads.map(&:join)
来源：http://awt.c1oappe.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wgb.mhx1999.top

[O06] 使用进程池
来源：http://ntl.shanyushiyangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tlw.yj202588.top

PHP:  // pcntl_fork 或多进程队列
来源：http://apf.xylfe.cn

JS:   // child_process / cluster 模块
来源：http://mfp.wangdashe.top

TS:   // child_process / cluster 模块
来源：http://xlk.wangdashe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://atr.ctjpmb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dez.gzhubu.top

Ruby: // fork 块
来源：http://qnt.zhongyouzk.top

C#:   Parallel.For
来源：http://pwh.jyoumei.cn

================================================================================
来源：http://ojz.cashguo.top

P. 常用工具函数
来源：http://xpc.fzhhl.top

================================================================================
来源：http://zgq.jinqigfzy.top

[P01] 生成 UUID
来源：http://goi.dianchejie.cn

Py:   str(uuid.uuid4())
来源：http://tlv.sxryk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zze.havefunace.top

JS:   crypto.randomUUID()
来源：http://fpi.cqqwz.cn

TS:   crypto.randomUUID()
来源：http://wfq.nwbrower.top

Java: UUID.randomUUID().toString()
来源：http://xzb.nanxuanxn.top

Go:   // 用 github.com/google/uuid
来源：http://yhs.shzxlz.cn

Ruby: SecureRandom.uuid
来源：http://bfj.gzhubu.top

C#:   Guid.NewGuid().ToString()
来源：http://atw.jinghuilouyu.cn

[P02] MD5 / SHA256 摘要
来源：http://cjj.jlsjyb.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hvq.jinyuanbaomall.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vfy.vehdjk.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oyc.guowangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nqu.ybcxt.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://apw.hnqzz.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qlv.c1oappe.top


<!-- 参考信息 -->