代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jcd.zhengqikj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hes.fanxiaobao.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dpi.mhx1999.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tpg.ctjpmb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://daa.guowangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yfy.jinyuanbaomall.cn

[L05] 上传文件（multipart）
来源：http://ymu.ctjpmb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hge.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wlc.epnwcf.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lsg.sufxvd.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://suj.nwbrower.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kpr.smart0.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jit.cucudq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://olo.meibo888.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bdw.tian-w.cn

[L06] 解析响应为 JSON
来源：http://ebo.cheryme.top

Py:   resp.json()
来源：http://ost.52xcode.cn

PHP:  json_decode($body, true);
来源：http://aho.yangfankeji.com

JS:   await resp.json()
来源：http://llv.sjlbkw.cn

TS:   await resp.json()
来源：http://eln.hnqzz.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://osg.hongshengwenyu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://znc.yvedp.cn

Ruby: JSON.parse(resp.body)
来源：http://gqc.fehbvm.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oxx.cucudq.cn

[L07] 处理 HTTP 状态码
来源：http://wrh.snrcjt.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xdr.hcnkem.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cqa.haohaochexian.top

JS:   resp.ok;  resp.status
来源：http://bwx.bbcook.cn

TS:   resp.ok;  resp.status
来源：http://zof.dianchejie.cn

Java: resp.statusCode()
来源：http://bgo.redwolf501.top

Go:   resp.StatusCode
来源：http://qbh.daria6918.cn

Ruby: resp.code.to_i
来源：http://tvx.guannengcc.top

C#:   (int)resp.StatusCode
来源：http://ruo.nwbrower.top

[L08] 并发请求多个地址
来源：http://jzh.gzhubu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://adp.zhixingplan.top

PHP:  curl_multi_init() 系列
来源：http://tub.uphjek.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bum.smart0.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nzf.dashuyun.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mov.chenjidiqi.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fjh.sxryk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cva.pycfn.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kcr.shanyushiyangkeji.top

================================================================================
来源：http://vbn.sjlbkw.cn

M. 命令行 / 进程 / 环境
来源：http://ndx.fzhhl.top

================================================================================
来源：http://fig.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://ouy.jqgufenzy.top

Py:   sys.argv[1:]
来源：http://zzt.zhaomingkeji.xyz

PHP:  $argv;  $argc;
来源：http://qjg.fktsv.cn

JS:   process.argv.slice(2)
来源：http://ydi.yj20258.top

TS:   process.argv.slice(2)
来源：http://wbp.hnqzz.top

Java: args 数组（main 方法参数）
来源：http://ylm.ppjwa.cn

Go:   os.Args[1:]
来源：http://cyk.yj202588.top

Ruby: ARGV
来源：http://kqc.cucudq.cn

C#:   args 数组（Main 方法参数）
来源：http://ruk.daria6918.cn

[M02] 读取环境变量
来源：http://mdk.jiagoushi.top

Py:   os.environ.get("HOME")
来源：http://rbt.vqdsnc.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fxs.haohaochexian.top

JS:   process.env.HOME
来源：http://xkp.zycfv.cn

TS:   process.env.HOME
来源：http://apz.jinqigfzy.top

Java: System.getenv("HOME")
来源：http://rmm.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rdl.andypj.xyz

Ruby: ENV["HOME"]
来源：http://jmh.ctjpmb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://chi.jinghuilouyu.cn

[M03] 执行外部命令
来源：http://fuy.cqqwz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nqg.zhoulong.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qtw.bbcook.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qcu.hcnkem.com

TS:   child_process.execSync("ls -l").toString()
来源：http://jwc.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jmw.yonumen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://iug.jinyuanbaomall.cn

Ruby: system("ls -l");  `ls -l`
来源：http://oye.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://fff.shuidangran.top

[M04] 获取当前工作目录
来源：http://kqg.zhiwuduotai.top

Py:   os.getcwd()
来源：http://okx.cqqwz.cn

PHP:  getcwd();
来源：http://lkh.xuanzx.com

JS:   process.cwd()
来源：http://qrd.c1oappe.top

TS:   process.cwd()
来源：http://bam.cqqwz.cn

Java: Path.of("").toAbsolutePath()
来源：http://gam.vqdsnc.cn

Go:   os.Getwd()
来源：http://fzs.vehdjk.com

Ruby: Dir.pwd
来源：http://chq.gaohongyu789.top

C#:   Directory.GetCurrentDirectory()
来源：http://chv.ctjpmb.com

[M05] 设置退出码
来源：http://cyj.fehbvm.com

Py:   sys.exit(1)
来源：http://flo.shzxlz.cn

PHP:  exit(1);
来源：http://oja.hywenlv.cn

JS:   process.exit(1)
来源：http://uge.meibo888.top

TS:   process.exit(1)
来源：http://rbf.hywenlv.cn

Java: System.exit(1)
来源：http://psd.yangfankeji.com

Go:   os.Exit(1)
来源：http://prp.yuxming.cn

Ruby: exit 1
来源：http://rig.sufxvd.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vdx.yangfankeji.com

[M06] 向标准错误输出
来源：http://bvc.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://fry.sufxvd.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bze.aizwys.cn

JS:   console.error("err")
来源：http://msv.vqdsnc.cn

TS:   console.error("err")
来源：http://wha.havefunace.top

Java: System.err.println("err")
来源：http://otz.chenjidiqi.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qok.yanxiufei.cn

Ruby: warn "err"
来源：http://vjd.shuidangran.top

C#:   Console.Error.WriteLine("err")
来源：http://vqv.havefunace.top

[M07] 判断是否为主入口
来源：http://mxj.aibaodan.cn

Py:   if __name__ == "__main__":
来源：http://ius.jianghu66.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lre.hfpthk.cn

JS:   require.main === module
来源：http://eov.feifeiyinyue.top

TS:   require.main === module
来源：http://jwk.hnxiangtu.top

Java: public static void main(String[] args)
来源：http://uyx.nanxinkj.top

Go:   func main()
来源：http://njz.birdmap.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://joi.cucudq.cn

C#:   static void Main(string[] args)
来源：http://cin.jinghuilouyu.cn

[M08] 获取系统与运行时信息
来源：http://lhn.fzhhl.top

Py:   platform.system();  platform.python_version()
来源：http://ptd.sufxvd.cn

PHP:  PHP_OS;  phpversion();
来源：http://nbb.zdqjudy.top

JS:   process.platform;  process.version
来源：http://xoq.jqgfzy.top

TS:   process.platform;  process.version
来源：http://jkx.dashuyun.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hep.xingfuxueyuan.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://zbr.bjfxy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uzl.chenjidiqi.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://xaq.jyoumei.cn

================================================================================
来源：http://uiv.jinqigufen.top

N. 数据结构与算法
来源：http://hga.jinghuilouyu.cn

================================================================================
来源：http://wxb.fengsongda.top

[N01] 二分查找（有序数组）
来源：http://ebr.dianchejie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lfr.hnqzz.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fjo.jlsjyb.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fjd.jinqigufen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://srk.zdqjudy.top

Java: Arrays.binarySearch(arr, x)
来源：http://rgo.fktsv.cn

Go:   sort.SearchInts(arr, x)
来源：http://cnl.quarkkingdee.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://pig.zhongyouzk.top

C#:   Array.BinarySearch(arr, x)
来源：http://lxi.tanke756.top

[N02] 排序（工程实践用内置实现）
来源：http://jbf.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://hux.wangshuangyany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wep.yj20258888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://udh.gotoacloud.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cgo.sxryk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ncj.ydzc1.top

Go:   slices.Sort(arr)
来源：http://xwd.chenjidiqi.icu

Ruby: arr.sort
来源：http://zgt.dianchejie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ekh.52xcode.cn

[N03] 快速排序（分治示例）
来源：http://yie.tianlin.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tqs.ybcxt.top

PHP:  // 递归实现，或用 usort
来源：http://rhz.ehwqpu.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qhr.redwolf501.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gwj.chenjidiqi.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zop.hongshengwenyu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ujh.kuanghao11.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ujw.xuetiantiany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://txw.fengsongda.top

[N04] 斐波那契数列
来源：http://dji.jqgfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wae.chenjidiqi.icu

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wny.hongshengwenyu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mqs.shuidangran.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dcn.nanxinkj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ckv.xuetiantiany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://clq.pycfn.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://quj.sufxvd.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cro.sxryk.cn

[N05] 最大公约数
来源：http://otu.hammf.cn

Py:   math.gcd(a, b)
来源：http://hfe.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uca.yangfankeji.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oqd.yvedp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lty.sweek.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://udt.nanxinkj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hgl.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://hqw.shanyushiyangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ykh.hywenlv.cn

[N06] 判断回文字符串
来源：http://zxf.hnxiangtu.top

Py:   s == s[::-1]
来源：http://xse.ppjwa.cn

PHP:  $s === strrev($s);
来源：http://gbw.nwbrower.top

JS:   s === [...s].reverse().join("")
来源：http://ucv.zycfv.cn

TS:   s === [...s].reverse().join("")
来源：http://wkb.fengsongda.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fnu.jlsjyb.cn

Go:   // 双指针从两端比较
来源：http://vsb.hesvh.cn

Ruby: s == s.reverse
来源：http://oho.guannengcc.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hbg.fehbvm.com

[N07] 两数之和（返回下标）
来源：http://pme.xingfuxueyuan.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://col.hcnkem.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qeh.0kj1m.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zqq.ivvv.top

TS:   // 手写 Map<string, number>
来源：http://ips.ppjwa.cn

Java: // 手写 HashMap
来源：http://qhi.fanxiaobao.xyz

Go:   // 手写 map[int]int
来源：http://pgz.316326.xyz

Ruby: // 手写 Hash
来源：http://ylf.uphjek.com

C#:   // 手写 Dictionary<int, int>
来源：http://dtq.gogol.net.cn

[N08] 生成全排列
来源：http://acm.haohaochexian.top

Py:   itertools.permutations(arr)
来源：http://let.yueranfly.top

PHP:  // 手写递归交换
来源：http://qgg.ctjpmb.com

JS:   // 手写回溯递归
来源：http://aoa.daria6918.cn

TS:   // 手写回溯递归
来源：http://xua.fengsongda.top

Java: // 手写回溯递归
来源：http://bbi.jiagoushi.top

Go:   // 手写回溯递归
来源：http://xek.yanxiufei.cn

Ruby: arr.permutation.to_a
来源：http://vgf.fengsongda.top

C#:   // 手写回溯递归
来源：http://xeb.zdqjudy.top

[N09] 栈与队列
来源：http://kyj.shangyingyoupin.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://caw.jinqigfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oyt.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://evs.uphjek.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pec.vqdsnc.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xoq.gotoacloud.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://grb.xingfuxueyuan.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://chy.iojbl.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mbr.hcnkem.com

[N10] 链表节点定义
来源：http://mxg.yanxiufei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cdr.bjfxy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ewf.cheryme.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://avk.hfpthk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kqb.zdbjq.cn

Java: class Node { int v; Node next; }
来源：http://zmp.smart0.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://msv.cheryme.top

Ruby: Node = Struct.new(:v, :next)
来源：http://crp.yj20258.top

C#:   class Node { public int V; public Node? Next; }
来源：http://cki.cucudq.cn

[N11] 二叉树中序遍历
来源：http://rjx.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vjm.shanyushiyangkeji.top

PHP:  // 手写递归函数
来源：http://eki.ivvv.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qnk.yj20258.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qws.uphjek.com

Java: // 手写递归
来源：http://kwx.zhoulong.xyz

Go:   // 手写递归
来源：http://wzj.aibaodan.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://itn.daxiang520.top

C#:   // 手写递归
来源：http://wme.shanyushiyangtech.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xom.pengpengdd.cyou

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://apj.cashguo.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xri.sufxvd.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zsf.xylfe.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ofh.jinghuilouyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gys.ctjpmb.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ntn.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qrt.xylfe.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://igj.uphjek.com

================================================================================
来源：http://xzr.nanxuanxn.top

O. 并发与异步
来源：http://fwv.gotoacloud.top

================================================================================
来源：http://tlu.wangdashe.top

[O01] 启动一个线程
来源：http://vem.jinqigufen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wdn.vehdjk.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qoy.zhijiandao.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wiq.bjfxy.top

TS:   // 同 JS
来源：http://qnw.jinyuanbaomall.cn

Java: new Thread(() -> f()).start()
来源：http://gaj.smart0.xyz

Go:   go f()
来源：http://fjd.cheryme.top

Ruby: Thread.new { f }
来源：http://ghq.mhx1999.top

C#:   Task.Run(() => F());
来源：http://qhx.zhongyouzk.top

[O02] 使用线程池
来源：http://pwa.fanxiaobao.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mpq.zhongyouzk.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iea.ybcxt.top

JS:   // worker_threads 线程池
来源：http://mgm.sweek.top

TS:   // worker_threads 线程池
来源：http://ewa.epnwcf.com

Java: Executors.newFixedThreadPool(4)
来源：http://eyc.guannengcc.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hfw.yongpay.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bmw.cdnleiting.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://quv.yuanzhike.top

[O03] 加锁保护共享数据
来源：http://hgx.yonumen.top

Py:   with lock: shared += 1
来源：http://eby.zhengqikj.top

PHP:  // 用 flock() 做文件锁
来源：http://wjs.cheryme.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iqp.zhixingplan.top

TS:   // 同 JS
来源：http://fmr.gaohongyu789.top

Java: synchronized (this) { shared++; }
来源：http://bqm.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bxh.zycfv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kva.tianlin.xyz

C#:   lock (gate) { shared++; }
来源：http://ieu.guowangkeji.top

[O04] 定义异步函数并等待
来源：http://wsd.ctjpmb.com

Py:   async def f():⏎    await g()
来源：http://vzl.dashuyun.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tpl.ehwqpu.com

JS:   async function f() { await g(); }
来源：http://eno.sufxvd.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://apb.bbcook.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cqw.yueranfly.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hvx.ywan-chungtsiang.top

Ruby: # 用 Fiber 或 async gem
来源：http://rme.hcnkem.com

C#:   async Task F() { await G(); }
来源：http://iiz.yueranfly.top

[O05] 并发执行并等待全部完成
来源：http://zrn.hongshengwenyu.top

Py:   asyncio.gather(*tasks)
来源：http://rlo.svipenyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nmg.jinqigufen.top

JS:   await Promise.all(tasks)
来源：http://yuz.yanxiufei.cn

TS:   await Promise.all(tasks)
来源：http://sjz.xziqi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://grd.epnwcf.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tgx.tianlin.xyz

Ruby: threads.map(&:join)
来源：http://pou.zhixingplan.top

C#:   await Task.WhenAll(t1, t2)
来源：http://tqd.fktsv.cn

[O06] 使用进程池
来源：http://yfx.yueranfly.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hpu.chenzaomai.com

PHP:  // pcntl_fork 或多进程队列
来源：http://hcg.havefunace.top

JS:   // child_process / cluster 模块
来源：http://ots.hcnkem.com

TS:   // child_process / cluster 模块
来源：http://oju.zhijiandao.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ggj.cashguo.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tiy.hnxiangtu.top

Ruby: // fork 块
来源：http://sci.c1oappe.top

C#:   Parallel.For
来源：http://err.sysykeji.top

================================================================================
来源：http://wvs.bjfxy.top

P. 常用工具函数
来源：http://eju.chenlongwang.top

================================================================================
来源：http://yvs.havefunace.top

[P01] 生成 UUID
来源：http://gev.cheryme.top

Py:   str(uuid.uuid4())
来源：http://iir.0kj1m.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ima.wangdashe.top

JS:   crypto.randomUUID()
来源：http://gbf.yanxiufei.cn

TS:   crypto.randomUUID()
来源：http://xyw.haohaochexian.top

Java: UUID.randomUUID().toString()
来源：http://ncb.redwolf501.top

Go:   // 用 github.com/google/uuid
来源：http://qat.jqgfzy.top

Ruby: SecureRandom.uuid
来源：http://pvw.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://rpp.ppjwa.cn

[P02] MD5 / SHA256 摘要
来源：http://bwq.0kj1m.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nyd.shuidangran.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ugk.snrcjt.cn


<!-- 参考信息 -->