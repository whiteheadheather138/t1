代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ecc.iojbl.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://slt.c1oappe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rce.dianchejie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xyc.xuanzx.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gmx.zycfv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://svy.quarkkingdee.top

[L05] 上传文件（multipart）
来源：http://egj.jinqigufen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qxp.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ozd.pengpengdd.cyou

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nik.sjlbkw.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dje.zhijiandao.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qtt.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nib.guannengcc.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mct.shuidangran.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rev.jinqigufen.top

[L06] 解析响应为 JSON
来源：http://pmf.cqqwz.cn

Py:   resp.json()
来源：http://cqk.0kj1m.cn

PHP:  json_decode($body, true);
来源：http://out.nanxinkj.top

JS:   await resp.json()
来源：http://rxu.hywenlv.cn

TS:   await resp.json()
来源：http://fvm.nanxinkj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yuf.xuetiantiany.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ufc.yvedp.cn

Ruby: JSON.parse(resp.body)
来源：http://svi.jianghu66.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bim.zhongyouzk.top

[L07] 处理 HTTP 状态码
来源：http://tlb.zdqjudy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jhp.yueranfly.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://moz.yj202588.top

JS:   resp.ok;  resp.status
来源：http://rid.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://imi.shanyushiyangkeji.top

Java: resp.statusCode()
来源：http://kwj.andypj.xyz

Go:   resp.StatusCode
来源：http://hnu.yongpay.top

Ruby: resp.code.to_i
来源：http://qce.xuanzx.com

C#:   (int)resp.StatusCode
来源：http://lnh.zhiwuduotai.top

[L08] 并发请求多个地址
来源：http://ple.0kj1m.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zdi.havefunace.top

PHP:  curl_multi_init() 系列
来源：http://tes.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ckb.zdqjudy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qsn.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cpw.ydjk.org.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://idi.dashuyun.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mzg.vqdsnc.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xwb.shzxlz.cn

================================================================================
来源：http://cid.jiagoushi.top

M. 命令行 / 进程 / 环境
来源：http://kwv.jqgufenzy.top

================================================================================
来源：http://afi.cashguo.top

[M01] 读取命令行参数
来源：http://wcx.aizwys.cn

Py:   sys.argv[1:]
来源：http://ada.hywenlv.cn

PHP:  $argv;  $argc;
来源：http://ekx.vehdjk.com

JS:   process.argv.slice(2)
来源：http://yhf.ydzc1.top

TS:   process.argv.slice(2)
来源：http://qyd.chenjidiqi.icu

Java: args 数组（main 方法参数）
来源：http://kyb.meibo888.top

Go:   os.Args[1:]
来源：http://wjf.hnxiangtu.top

Ruby: ARGV
来源：http://ova.jiagoushi.top

C#:   args 数组（Main 方法参数）
来源：http://xsr.jyoumei.cn

[M02] 读取环境变量
来源：http://bnz.yfazqb.com

Py:   os.environ.get("HOME")
来源：http://oyq.zhixingplan.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ken.pycfn.com

JS:   process.env.HOME
来源：http://zqx.shzxlz.cn

TS:   process.env.HOME
来源：http://wau.vqdsnc.cn

Java: System.getenv("HOME")
来源：http://mvk.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kqq.vehdjk.com

Ruby: ENV["HOME"]
来源：http://dur.xziqi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://myr.guowangkeji.top

[M03] 执行外部命令
来源：http://wtv.fzhhl.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ixb.yonumen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://onu.xylfe.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ycn.cqqwz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mln.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ppt.xingfuxueyuan.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://tqt.feifeiyinyue.top

Ruby: system("ls -l");  `ls -l`
来源：http://igy.aizwys.cn

C#:   Process.Start("ls", "-l");
来源：http://bbt.smart0.xyz

[M04] 获取当前工作目录
来源：http://fwz.vehdjk.com

Py:   os.getcwd()
来源：http://gsz.52xcode.cn

PHP:  getcwd();
来源：http://iqb.yvedp.cn

JS:   process.cwd()
来源：http://axp.snrcjt.cn

TS:   process.cwd()
来源：http://puc.shuidangran.top

Java: Path.of("").toAbsolutePath()
来源：http://fwd.tanke756.top

Go:   os.Getwd()
来源：http://tta.chenjidiqi.icu

Ruby: Dir.pwd
来源：http://pdo.vqdsnc.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mcc.zdqjudy.top

[M05] 设置退出码
来源：http://igg.hfpthk.cn

Py:   sys.exit(1)
来源：http://khb.chenzaomai.com

PHP:  exit(1);
来源：http://idr.iojbl.cn

JS:   process.exit(1)
来源：http://vfs.ywan-chungtsiang.top

TS:   process.exit(1)
来源：http://uqy.aibaodan.cn

Java: System.exit(1)
来源：http://kcx.cqqwz.cn

Go:   os.Exit(1)
来源：http://vsg.cheryme.top

Ruby: exit 1
来源：http://dzy.ppjwa.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rog.cashguo.top

[M06] 向标准错误输出
来源：http://bia.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://car.wangshuangyany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://opo.gaohongyu789.top

JS:   console.error("err")
来源：http://xrm.ehwqpu.com

TS:   console.error("err")
来源：http://igf.tarul.cn

Java: System.err.println("err")
来源：http://rey.fzhhl.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xuf.jinqigfzy.top

Ruby: warn "err"
来源：http://svg.hammf.cn

C#:   Console.Error.WriteLine("err")
来源：http://oeq.yvedp.cn

[M07] 判断是否为主入口
来源：http://bls.xuanzx.com

Py:   if __name__ == "__main__":
来源：http://cre.meibo888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://knc.sysykeji.top

JS:   require.main === module
来源：http://vse.wangshuangyany.cn

TS:   require.main === module
来源：http://srt.redwolf501.top

Java: public static void main(String[] args)
来源：http://yos.yanxiufei.cn

Go:   func main()
来源：http://sou.xingfuxueyuan.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uub.ehwqpu.com

C#:   static void Main(string[] args)
来源：http://txk.epnwcf.com

[M08] 获取系统与运行时信息
来源：http://kvi.ydjk.org.cn

Py:   platform.system();  platform.python_version()
来源：http://ozp.kuanghao11.cn

PHP:  PHP_OS;  phpversion();
来源：http://okx.tianlin.xyz

JS:   process.platform;  process.version
来源：http://rpc.fehbvm.com

TS:   process.platform;  process.version
来源：http://sqf.ydzc1.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rml.jlsjyb.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gyj.ivvv.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zeg.hammf.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hyi.zhijiandao.cn

================================================================================
来源：http://rwn.yonumen.top

N. 数据结构与算法
来源：http://san.sweek.top

================================================================================
来源：http://gbe.vehdjk.com

[N01] 二分查找（有序数组）
来源：http://rdl.pengpengdd.cyou

Py:   bisect.bisect_left(arr, x)
来源：http://ddx.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://unq.jinghuilouyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://etc.gotoacloud.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fos.jlsjyb.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hoo.bjfxy.top

Go:   sort.SearchInts(arr, x)
来源：http://nmm.fehbvm.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://jbe.pengpengdd.cyou

C#:   Array.BinarySearch(arr, x)
来源：http://qyp.jqgufenzy.top

[N02] 排序（工程实践用内置实现）
来源：http://mhb.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://qum.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pwa.daria6918.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zgu.yonumen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://iwu.zhiwuduotai.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pqm.mhx1999.top

Go:   slices.Sort(arr)
来源：http://rmi.gzhubu.top

Ruby: arr.sort
来源：http://fyz.cheryme.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pmj.yuanzhike.top

[N03] 快速排序（分治示例）
来源：http://pbj.jinqigufen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lql.c1oappe.top

PHP:  // 递归实现，或用 usort
来源：http://lwt.hesvh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gdt.ydjk.org.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aji.guowangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xuj.316326.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zhj.meibo888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kfa.andypj.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://pnz.0kj1m.cn

[N04] 斐波那契数列
来源：http://yjm.zdbjq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ovs.gogol.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sew.cashguo.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://krq.chenjidiqi.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bft.jinqigfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uoz.jinqigfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vxi.yuxming.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fzb.nwbrower.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rvv.xingfuxueyuan.xyz

[N05] 最大公约数
来源：http://wgi.yonumen.top

Py:   math.gcd(a, b)
来源：http://fff.sjlbkw.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gjr.hywenlv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://crx.zdqjudy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oym.sysykeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xza.daxiang520.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zxg.shuidangran.top

Ruby: a.gcd(b)
来源：http://glg.chenlongwang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sou.sufxvd.cn

[N06] 判断回文字符串
来源：http://nuy.zhengqikj.top

Py:   s == s[::-1]
来源：http://exh.hfpthk.cn

PHP:  $s === strrev($s);
来源：http://hit.ctjpmb.com

JS:   s === [...s].reverse().join("")
来源：http://xwn.jlsjyb.cn

TS:   s === [...s].reverse().join("")
来源：http://ils.jinyuanbaomall.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xuh.hcnkem.com

Go:   // 双指针从两端比较
来源：http://crk.jianghu66.top

Ruby: s == s.reverse
来源：http://byp.jinqigfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dvh.52xcode.cn

[N07] 两数之和（返回下标）
来源：http://qwr.aibaodan.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rhy.zhixingplan.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cyn.meibo888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mos.guowangkeji.top

TS:   // 手写 Map<string, number>
来源：http://cds.tanke756.top

Java: // 手写 HashMap
来源：http://cwj.yj202588.top

Go:   // 手写 map[int]int
来源：http://ohd.guowangkeji.top

Ruby: // 手写 Hash
来源：http://vud.yongpay.top

C#:   // 手写 Dictionary<int, int>
来源：http://cta.redwolf501.top

[N08] 生成全排列
来源：http://pzu.zhijiandao.cn

Py:   itertools.permutations(arr)
来源：http://jpb.gogol.net.cn

PHP:  // 手写递归交换
来源：http://nkc.yanxiufei.cn

JS:   // 手写回溯递归
来源：http://hck.mhx1999.top

TS:   // 手写回溯递归
来源：http://wuf.zhixingplan.top

Java: // 手写回溯递归
来源：http://ryd.yj20258888.top

Go:   // 手写回溯递归
来源：http://aod.xuanzx.com

Ruby: arr.permutation.to_a
来源：http://ado.hesvh.cn

C#:   // 手写回溯递归
来源：http://esx.sweek.top

[N09] 栈与队列
来源：http://vcn.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://spe.cqqwz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vtw.hammf.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wno.shanyushiyangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ojw.cdnleiting.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cat.cqqwz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xmk.chenlongwang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zbv.yonumen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dvp.zycfv.cn

[N10] 链表节点定义
来源：http://tsp.hnxiangtu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uka.zhaomingkeji.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://djy.aibaodan.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fxg.nanxuanxn.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xli.xziqi.cn

Java: class Node { int v; Node next; }
来源：http://prj.uphjek.com

Go:   type Node struct { V int; Next *Node }
来源：http://sut.c1oappe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://cbw.zhixingplan.top

C#:   class Node { public int V; public Node? Next; }
来源：http://uzk.ydjk.org.cn

[N11] 二叉树中序遍历
来源：http://gvb.ywan-chungtsiang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mmq.yj20258.top

PHP:  // 手写递归函数
来源：http://ymb.cashguo.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mii.iojbl.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mfk.shanyushiyangkeji.top

Java: // 手写递归
来源：http://rnj.hcnkem.com

Go:   // 手写递归
来源：http://ctl.tianlin.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ndz.cucudq.cn

C#:   // 手写递归
来源：http://cpk.c1oappe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kpn.wangshuangyany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iwy.vqdsnc.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://niw.chenlongwang.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gbr.sysykeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tqf.cqqwz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cum.redwolf501.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://obd.dashuyun.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://new.yj20258888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wly.tarul.cn

================================================================================
来源：http://kix.hesvh.cn

O. 并发与异步
来源：http://gcu.tarul.cn

================================================================================
来源：http://jow.ywan-chungtsiang.top

[O01] 启动一个线程
来源：http://shv.fanxiaobao.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ahk.52xcode.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tjv.zhaomingkeji.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ylh.pycfn.com

TS:   // 同 JS
来源：http://ufz.hywenlv.cn

Java: new Thread(() -> f()).start()
来源：http://rqc.yangfankeji.com

Go:   go f()
来源：http://axk.fengsongda.top

Ruby: Thread.new { f }
来源：http://yli.hongshengwenyu.top

C#:   Task.Run(() => F());
来源：http://kpz.xuanzx.com

[O02] 使用线程池
来源：http://npl.cdnleiting.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lhu.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kww.sweek.top

JS:   // worker_threads 线程池
来源：http://pwt.zdqjudy.top

TS:   // worker_threads 线程池
来源：http://fdv.yueranfly.top

Java: Executors.newFixedThreadPool(4)
来源：http://qpo.cashguo.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pym.xziqi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dwm.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pbd.yj20258.top

[O03] 加锁保护共享数据
来源：http://tme.smart0.xyz

Py:   with lock: shared += 1
来源：http://mes.yj20258.top

PHP:  // 用 flock() 做文件锁
来源：http://vdw.jinyuanbaomall.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mra.svipenyu.cn

TS:   // 同 JS
来源：http://air.daxiang520.top

Java: synchronized (this) { shared++; }
来源：http://bqi.zhiwuduotai.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gqf.jinqigufen.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lax.smart0.xyz

C#:   lock (gate) { shared++; }
来源：http://gqa.9152youxi.cn

[O04] 定义异步函数并等待
来源：http://prq.hnqzz.top

Py:   async def f():⏎    await g()
来源：http://mzh.sysykeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mci.zdqjudy.top

JS:   async function f() { await g(); }
来源：http://vmz.jinyuanbaomall.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yii.sxryk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gxy.pengpengdd.cyou

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hux.ybcxt.top

Ruby: # 用 Fiber 或 async gem
来源：http://dwp.gogol.net.cn

C#:   async Task F() { await G(); }
来源：http://dyt.hongshengwenyu.top

[O05] 并发执行并等待全部完成
来源：http://eap.shuidangran.top

Py:   asyncio.gather(*tasks)
来源：http://rbr.nwbrower.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wxe.bbcook.cn

JS:   await Promise.all(tasks)
来源：http://mqw.cqqwz.cn

TS:   await Promise.all(tasks)
来源：http://lli.nwbrower.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://buw.yongpay.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://otp.sufxvd.cn

Ruby: threads.map(&:join)
来源：http://yvv.shzxlz.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ltz.hysaishi.cn

[O06] 使用进程池
来源：http://jik.jinyuanbaomall.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jne.epnwcf.com

PHP:  // pcntl_fork 或多进程队列
来源：http://ybu.ehwqpu.com

JS:   // child_process / cluster 模块
来源：http://vbs.hammf.cn

TS:   // child_process / cluster 模块
来源：http://bhu.fanxiaobao.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wov.xuetiantiany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xay.aibaodan.cn

Ruby: // fork 块
来源：http://gbc.yuxming.cn

C#:   Parallel.For
来源：http://lii.xinyue.icu

================================================================================
来源：http://ihn.xingfuxueyuan.xyz

P. 常用工具函数
来源：http://nnv.zhengqikj.top

================================================================================
来源：http://ewm.9152youxi.cn

[P01] 生成 UUID
来源：http://vby.cashguo.top

Py:   str(uuid.uuid4())
来源：http://amu.ppjwa.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cvj.sjlbkw.cn

JS:   crypto.randomUUID()
来源：http://urf.gaohongyu789.top

TS:   crypto.randomUUID()
来源：http://oid.jinqigufen.top

Java: UUID.randomUUID().toString()
来源：http://xfl.yonumen.top

Go:   // 用 github.com/google/uuid
来源：http://vse.fzhhl.top

Ruby: SecureRandom.uuid
来源：http://jlq.sysykeji.top

C#:   Guid.NewGuid().ToString()
来源：http://crh.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://uuf.feifeiyinyue.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dce.hnqzz.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://sjl.cdnleiting.top


<!-- 参考信息 -->