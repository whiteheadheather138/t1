代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gsh.fehbvm.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iqq.jinghuilouyu.cn

[L05] 上传文件（multipart）
来源：http://tfw.shzxlz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ftm.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vqe.fzhhl.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fdu.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ati.jyoumei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://urm.ydzc1.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lag.wangshuangyany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yvd.ivvv.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iqh.jinqigufen.top

[L06] 解析响应为 JSON
来源：http://oye.jqgfzy.top

Py:   resp.json()
来源：http://uvh.daxiang520.top

PHP:  json_decode($body, true);
来源：http://tcg.chenzaomai.com

JS:   await resp.json()
来源：http://uma.jianghu66.top

TS:   await resp.json()
来源：http://zlx.yonumen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kuh.pengpengdd.cyou

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lnr.ppjwa.cn

Ruby: JSON.parse(resp.body)
来源：http://ysk.yfazqb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zad.gzhubu.top

[L07] 处理 HTTP 状态码
来源：http://wbd.hnxiangtu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://waq.kuanghao11.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nma.shanyushiyangtech.top

JS:   resp.ok;  resp.status
来源：http://bih.zhaomingkeji.xyz

TS:   resp.ok;  resp.status
来源：http://hbn.nanxuanxn.top

Java: resp.statusCode()
来源：http://kxj.sweek.top

Go:   resp.StatusCode
来源：http://mls.zdbjq.cn

Ruby: resp.code.to_i
来源：http://rpe.shzxlz.cn

C#:   (int)resp.StatusCode
来源：http://dfg.xinyue.icu

[L08] 并发请求多个地址
来源：http://goc.jlsjyb.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iwq.yj202588.top

PHP:  curl_multi_init() 系列
来源：http://lff.ybcxt.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ddy.jqgfzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pxz.jinqigufen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wgo.aibaodan.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kxw.52xcode.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ofo.yj202588.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bao.guannengcc.top

================================================================================
来源：http://noi.chenzaomai.com

M. 命令行 / 进程 / 环境
来源：http://wqr.haohaochexian.top

================================================================================
来源：http://tqq.yj20258.top

[M01] 读取命令行参数
来源：http://fkj.dashuyun.cn

Py:   sys.argv[1:]
来源：http://kej.jqgufenzy.top

PHP:  $argv;  $argc;
来源：http://qjl.sweek.top

JS:   process.argv.slice(2)
来源：http://ucq.hcnkem.com

TS:   process.argv.slice(2)
来源：http://wft.andypj.xyz

Java: args 数组（main 方法参数）
来源：http://egb.fengsongda.top

Go:   os.Args[1:]
来源：http://hek.hnxiangtu.top

Ruby: ARGV
来源：http://ohj.meibo888.top

C#:   args 数组（Main 方法参数）
来源：http://wsb.tarul.cn

[M02] 读取环境变量
来源：http://vzv.quarkkingdee.top

Py:   os.environ.get("HOME")
来源：http://nxc.dianchejie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://axn.mhx1999.top

JS:   process.env.HOME
来源：http://wom.hnqzz.top

TS:   process.env.HOME
来源：http://qos.tanke756.top

Java: System.getenv("HOME")
来源：http://tun.tanke756.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sqe.zdbjq.cn

Ruby: ENV["HOME"]
来源：http://xab.zhiwuduotai.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fqj.mhx1999.top

[M03] 执行外部命令
来源：http://xlh.yanxiufei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://naj.tanke756.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nhl.daria6918.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sps.feifeiyinyue.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ofq.xingfuxueyuan.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yao.hammf.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nda.meibo888.top

Ruby: system("ls -l");  `ls -l`
来源：http://llt.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://lhx.hammf.cn

[M04] 获取当前工作目录
来源：http://ypz.epnwcf.com

Py:   os.getcwd()
来源：http://gjh.yanxiufei.cn

PHP:  getcwd();
来源：http://apa.ctjpmb.com

JS:   process.cwd()
来源：http://sux.nwbrower.top

TS:   process.cwd()
来源：http://usj.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://gwo.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://orq.feifeiyinyue.top

Ruby: Dir.pwd
来源：http://pgw.hnxiangtu.top

C#:   Directory.GetCurrentDirectory()
来源：http://tyh.vqdsnc.cn

[M05] 设置退出码
来源：http://nit.zhijiandao.cn

Py:   sys.exit(1)
来源：http://hzj.bbcook.cn

PHP:  exit(1);
来源：http://njy.ivvv.top

JS:   process.exit(1)
来源：http://exm.chenjidiqi.icu

TS:   process.exit(1)
来源：http://pgh.pengpengdd.cyou

Java: System.exit(1)
来源：http://aim.ctjpmb.com

Go:   os.Exit(1)
来源：http://vwb.gogol.net.cn

Ruby: exit 1
来源：http://ziy.svipenyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hmc.jyoumei.cn

[M06] 向标准错误输出
来源：http://ajf.fengsongda.top

Py:   print("err", file=sys.stderr)
来源：http://fkz.cdnleiting.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tgy.hnxiangtu.top

JS:   console.error("err")
来源：http://cmd.jqgfzy.top

TS:   console.error("err")
来源：http://oeg.fktsv.cn

Java: System.err.println("err")
来源：http://pkn.ehwqpu.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qri.yanxiufei.cn

Ruby: warn "err"
来源：http://wax.jyoumei.cn

C#:   Console.Error.WriteLine("err")
来源：http://gdf.aizwys.cn

[M07] 判断是否为主入口
来源：http://lvp.cheryme.top

Py:   if __name__ == "__main__":
来源：http://cdw.havefunace.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jhn.jqgufenzy.top

JS:   require.main === module
来源：http://vld.shzxlz.cn

TS:   require.main === module
来源：http://psb.chenjidiqi.icu

Java: public static void main(String[] args)
来源：http://phx.0kj1m.cn

Go:   func main()
来源：http://gmz.fktsv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jzs.52xcode.cn

C#:   static void Main(string[] args)
来源：http://ini.zhixingplan.top

[M08] 获取系统与运行时信息
来源：http://eah.hnxiangtu.top

Py:   platform.system();  platform.python_version()
来源：http://qda.bjfxy.top

PHP:  PHP_OS;  phpversion();
来源：http://jtm.meibo888.top

JS:   process.platform;  process.version
来源：http://flb.aizwys.cn

TS:   process.platform;  process.version
来源：http://pjw.daxiang520.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nuv.yonumen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ung.zhengqikj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dpo.nanxuanxn.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nry.ydzc1.top

================================================================================
来源：http://kpp.cdnleiting.top

N. 数据结构与算法
来源：http://sbx.jinghuilouyu.cn

================================================================================
来源：http://ydt.zhixingplan.top

[N01] 二分查找（有序数组）
来源：http://dwp.snrcjt.cn

Py:   bisect.bisect_left(arr, x)
来源：http://juk.daxiang520.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aiz.hywenlv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jax.ctjpmb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lfg.xingfuxueyuan.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://zcu.fzhhl.top

Go:   sort.SearchInts(arr, x)
来源：http://mqe.zhengqikj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://fgo.yangfankeji.com

C#:   Array.BinarySearch(arr, x)
来源：http://rzo.ivvv.top

[N02] 排序（工程实践用内置实现）
来源：http://fax.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://gbp.xuanzx.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bis.aibaodan.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://apg.fzhhl.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://gay.hammf.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jlq.c1oappe.top

Go:   slices.Sort(arr)
来源：http://pzs.pycfn.com

Ruby: arr.sort
来源：http://tbe.xingfuxueyuan.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://ojp.kuanghao11.cn

[N03] 快速排序（分治示例）
来源：http://bqx.jinqigufen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://veg.meibo888.top

PHP:  // 递归实现，或用 usort
来源：http://wbo.gogol.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uhp.yuxming.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lvb.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mud.zdbjq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sqa.tianlin.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lxb.yueranfly.top

C#:   // 手写递归，或 Array.Sort
来源：http://nzd.jinqigufen.top

[N04] 斐波那契数列
来源：http://juy.pengpengdd.cyou

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dnv.yueranfly.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cbz.redwolf501.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://odb.hnxiangtu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://czi.gaohongyu789.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qfn.mhx1999.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mfq.dashuyun.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lot.hnqzz.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ppw.yuxming.cn

[N05] 最大公约数
来源：http://dkj.gaohongyu789.top

Py:   math.gcd(a, b)
来源：http://ptf.hnxiangtu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oey.jlsjyb.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dnw.dianchejie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xqy.kuanghao11.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fjy.chenlongwang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wrm.pycfn.com

Ruby: a.gcd(b)
来源：http://kpm.sxryk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ugw.zhengqikj.top

[N06] 判断回文字符串
来源：http://lyr.ydzc1.top

Py:   s == s[::-1]
来源：http://mxc.xylfe.cn

PHP:  $s === strrev($s);
来源：http://vpm.ivvv.top

JS:   s === [...s].reverse().join("")
来源：http://zsz.jinyuanbaomall.cn

TS:   s === [...s].reverse().join("")
来源：http://zzw.c1oappe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vvf.wangdashe.top

Go:   // 双指针从两端比较
来源：http://bso.9152youxi.cn

Ruby: s == s.reverse
来源：http://inf.meibo888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pta.zhixingplan.top

[N07] 两数之和（返回下标）
来源：http://gsm.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cew.hnxiangtu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://olh.svipenyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wrt.daxiang520.top

TS:   // 手写 Map<string, number>
来源：http://igv.jianghu66.top

Java: // 手写 HashMap
来源：http://lwf.aibaodan.cn

Go:   // 手写 map[int]int
来源：http://vso.daria6918.cn

Ruby: // 手写 Hash
来源：http://kes.iojbl.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hdy.tianlin.xyz

[N08] 生成全排列
来源：http://zpj.dashuyun.cn

Py:   itertools.permutations(arr)
来源：http://mxm.uphjek.com

PHP:  // 手写递归交换
来源：http://mje.fktsv.cn

JS:   // 手写回溯递归
来源：http://rxw.sufxvd.cn

TS:   // 手写回溯递归
来源：http://ckk.jinqigfzy.top

Java: // 手写回溯递归
来源：http://zya.guannengcc.top

Go:   // 手写回溯递归
来源：http://oej.0kj1m.cn

Ruby: arr.permutation.to_a
来源：http://sdc.cashguo.top

C#:   // 手写回溯递归
来源：http://ptf.redwolf501.top

[N09] 栈与队列
来源：http://cda.cdnleiting.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dib.gotoacloud.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yop.gzhubu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aeo.0kj1m.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://orp.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ivi.aizwys.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wye.yfazqb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zmj.fktsv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://piv.hcnkem.com

[N10] 链表节点定义
来源：http://xsr.xziqi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hnh.hfpthk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zxx.yanxiufei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rdz.haohaochexian.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wtd.ydzc1.top

Java: class Node { int v; Node next; }
来源：http://myi.bjfxy.top

Go:   type Node struct { V int; Next *Node }
来源：http://ydn.yj202588.top

Ruby: Node = Struct.new(:v, :next)
来源：http://grl.shuidangran.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bmh.9152youxi.cn

[N11] 二叉树中序遍历
来源：http://txr.zycfv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://scz.wangdashe.top

PHP:  // 手写递归函数
来源：http://thz.jqgfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wzr.quarkkingdee.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gvd.yj20258.top

Java: // 手写递归
来源：http://eoe.zhijiandao.cn

Go:   // 手写递归
来源：http://gib.xziqi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://npt.sweek.top

C#:   // 手写递归
来源：http://ccs.zycfv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nmp.smart0.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yly.hammf.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bne.meibo888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fkr.tian-w.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fey.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hbd.zhaomingkeji.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ufd.smart0.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mdy.ybcxt.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ygj.cqqwz.cn

================================================================================
来源：http://agy.yanxiufei.cn

O. 并发与异步
来源：http://wcn.jianghu66.top

================================================================================
来源：http://uzz.jyoumei.cn

[O01] 启动一个线程
来源：http://xwc.316326.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://awg.sjlbkw.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lwt.yj202588.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ria.shuidangran.top

TS:   // 同 JS
来源：http://jjo.ywan-chungtsiang.top

Java: new Thread(() -> f()).start()
来源：http://xyw.jlsjyb.cn

Go:   go f()
来源：http://lun.xuetiantiany.cn

Ruby: Thread.new { f }
来源：http://piq.jinghuilouyu.cn

C#:   Task.Run(() => F());
来源：http://vjv.ctjpmb.com

[O02] 使用线程池
来源：http://udt.sjlbkw.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ghy.gotoacloud.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hsp.quarkkingdee.top

JS:   // worker_threads 线程池
来源：http://lzu.cdnleiting.top

TS:   // worker_threads 线程池
来源：http://hmp.hnqzz.top

Java: Executors.newFixedThreadPool(4)
来源：http://qjn.hywenlv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fzo.hnqzz.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://whc.nwbrower.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wsd.zhoulong.xyz

[O03] 加锁保护共享数据
来源：http://ssl.hysaishi.cn

Py:   with lock: shared += 1
来源：http://wwz.zhijiandao.cn

PHP:  // 用 flock() 做文件锁
来源：http://dmd.chenlongwang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hfv.smart0.xyz

TS:   // 同 JS
来源：http://jkb.ivvv.top

Java: synchronized (this) { shared++; }
来源：http://uwf.tarul.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://itz.sxryk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pxc.wangshuangyany.cn

C#:   lock (gate) { shared++; }
来源：http://sfv.epnwcf.com

[O04] 定义异步函数并等待
来源：http://hkn.yueranfly.top

Py:   async def f():⏎    await g()
来源：http://bxm.ydjk.org.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yqv.svipenyu.cn

JS:   async function f() { await g(); }
来源：http://iyj.hongshengwenyu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://yqg.mhx1999.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yxu.jqgfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ggz.xingfuxueyuan.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://hom.yuxming.cn

C#:   async Task F() { await G(); }
来源：http://kxl.gogol.net.cn

[O05] 并发执行并等待全部完成
来源：http://uff.tanke756.top

Py:   asyncio.gather(*tasks)
来源：http://ttv.ctjpmb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://upn.ybcxt.top

JS:   await Promise.all(tasks)
来源：http://rph.jqgfzy.top

TS:   await Promise.all(tasks)
来源：http://tuc.chenzaomai.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qss.52xcode.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fwt.hywenlv.cn

Ruby: threads.map(&:join)
来源：http://xzj.pycfn.com

C#:   await Task.WhenAll(t1, t2)
来源：http://gdl.chenzaomai.com

[O06] 使用进程池
来源：http://twg.bjfxy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iak.jiagoushi.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kga.chenzaomai.com

JS:   // child_process / cluster 模块
来源：http://bso.guannengcc.top

TS:   // child_process / cluster 模块
来源：http://lcv.nwbrower.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iha.tarul.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ouu.tanke756.top

Ruby: // fork 块
来源：http://fye.tanke756.top

C#:   Parallel.For
来源：http://tju.birdmap.top

================================================================================
来源：http://gzw.hfpthk.cn

P. 常用工具函数
来源：http://mze.yanxiufei.cn

================================================================================
来源：http://oik.havefunace.top

[P01] 生成 UUID
来源：http://quh.jinyuanbaomall.cn

Py:   str(uuid.uuid4())
来源：http://nyw.yonumen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lli.yvedp.cn

JS:   crypto.randomUUID()
来源：http://mol.svipenyu.cn

TS:   crypto.randomUUID()
来源：http://cuz.sufxvd.cn

Java: UUID.randomUUID().toString()
来源：http://pif.hcnkem.com

Go:   // 用 github.com/google/uuid
来源：http://bko.dashuyun.cn

Ruby: SecureRandom.uuid
来源：http://yqu.xingfuxueyuan.xyz

C#:   Guid.NewGuid().ToString()
来源：http://hmy.feifeiyinyue.top

[P02] MD5 / SHA256 摘要
来源：http://zdt.hammf.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ios.tian-w.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yva.jianghu66.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ohn.yfazqb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ksw.mhx1999.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://plm.zhongyouzk.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jaf.shuidangran.top


<!-- 参考信息 -->