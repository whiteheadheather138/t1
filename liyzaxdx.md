代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fms.zhengqikj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oos.feifeiyinyue.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pql.9152youxi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iwm.yueranfly.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rdi.xylfe.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zwz.hongshengwenyu.top

[L05] 上传文件（multipart）
来源：http://nis.c1oappe.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tby.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mrd.cqqwz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pme.fzhhl.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eyv.gzhubu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fsj.meibo888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://prx.gaohongyu789.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zut.cheryme.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tgg.sjlbkw.cn

[L06] 解析响应为 JSON
来源：http://hqf.hammf.cn

Py:   resp.json()
来源：http://vqc.gaohongyu789.top

PHP:  json_decode($body, true);
来源：http://zte.zhijiandao.cn

JS:   await resp.json()
来源：http://hhn.yanxiufei.cn

TS:   await resp.json()
来源：http://blj.jlsjyb.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jcr.zhixingplan.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cso.nanxinkj.top

Ruby: JSON.parse(resp.body)
来源：http://thx.yonumen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vyi.cheryme.top

[L07] 处理 HTTP 状态码
来源：http://bot.pycfn.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pyl.hysaishi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ans.tianlin.xyz

JS:   resp.ok;  resp.status
来源：http://pao.xylfe.cn

TS:   resp.ok;  resp.status
来源：http://hxz.pengpengdd.cyou

Java: resp.statusCode()
来源：http://agr.zhijiandao.cn

Go:   resp.StatusCode
来源：http://nrm.wangdashe.top

Ruby: resp.code.to_i
来源：http://gxo.chenlongwang.top

C#:   (int)resp.StatusCode
来源：http://ran.ywan-chungtsiang.top

[L08] 并发请求多个地址
来源：http://klm.yanxiufei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ezt.yuanzhike.top

PHP:  curl_multi_init() 系列
来源：http://drz.ydjk.org.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rqz.hysaishi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oxh.dashuyun.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uib.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://peo.zhaomingkeji.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cyw.tanke756.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qvl.ctjpmb.com

================================================================================
来源：http://zke.jqgfzy.top

M. 命令行 / 进程 / 环境
来源：http://rhp.aizwys.cn

================================================================================
来源：http://cyv.yfazqb.com

[M01] 读取命令行参数
来源：http://qpq.hfpthk.cn

Py:   sys.argv[1:]
来源：http://nsi.epnwcf.com

PHP:  $argv;  $argc;
来源：http://mrh.dashuyun.cn

JS:   process.argv.slice(2)
来源：http://emi.fehbvm.com

TS:   process.argv.slice(2)
来源：http://wjq.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://eoy.daxiang520.top

Go:   os.Args[1:]
来源：http://yol.tanke756.top

Ruby: ARGV
来源：http://vcu.fktsv.cn

C#:   args 数组（Main 方法参数）
来源：http://zjf.zhixingplan.top

[M02] 读取环境变量
来源：http://mdm.cqqwz.cn

Py:   os.environ.get("HOME")
来源：http://wcn.jqgufenzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pcc.zdqjudy.top

JS:   process.env.HOME
来源：http://wma.hongshengwenyu.top

TS:   process.env.HOME
来源：http://cvk.sysykeji.top

Java: System.getenv("HOME")
来源：http://wlf.ydjk.org.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cvn.ehwqpu.com

Ruby: ENV["HOME"]
来源：http://vli.birdmap.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uis.xziqi.cn

[M03] 执行外部命令
来源：http://wrx.xuetiantiany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://abe.quarkkingdee.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ezz.jinyuanbaomall.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://klc.mhx1999.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nsq.bbcook.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tof.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jxr.ydzc1.top

Ruby: system("ls -l");  `ls -l`
来源：http://qrb.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://ttg.wangshuangyany.cn

[M04] 获取当前工作目录
来源：http://dkg.jinyuanbaomall.cn

Py:   os.getcwd()
来源：http://asr.ywan-chungtsiang.top

PHP:  getcwd();
来源：http://uyc.uphjek.com

JS:   process.cwd()
来源：http://ule.52xcode.cn

TS:   process.cwd()
来源：http://xyw.jinqigufen.top

Java: Path.of("").toAbsolutePath()
来源：http://agh.zdbjq.cn

Go:   os.Getwd()
来源：http://lhf.ctjpmb.com

Ruby: Dir.pwd
来源：http://mak.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://osf.jyoumei.cn

[M05] 设置退出码
来源：http://xnd.wangshuangyany.cn

Py:   sys.exit(1)
来源：http://hwt.andypj.xyz

PHP:  exit(1);
来源：http://kwc.hcnkem.com

JS:   process.exit(1)
来源：http://njl.jinyuanbaomall.cn

TS:   process.exit(1)
来源：http://qew.zhengqikj.top

Java: System.exit(1)
来源：http://ybg.feifeiyinyue.top

Go:   os.Exit(1)
来源：http://jkp.mhx1999.top

Ruby: exit 1
来源：http://hxt.birdmap.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rua.fengsongda.top

[M06] 向标准错误输出
来源：http://vam.shzxlz.cn

Py:   print("err", file=sys.stderr)
来源：http://ghb.yj202588.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ygr.bbcook.cn

JS:   console.error("err")
来源：http://qul.mhx1999.top

TS:   console.error("err")
来源：http://hnx.mhx1999.top

Java: System.err.println("err")
来源：http://vee.iojbl.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jlv.yj20258888.top

Ruby: warn "err"
来源：http://ffg.feifeiyinyue.top

C#:   Console.Error.WriteLine("err")
来源：http://hpi.hongshengwenyu.top

[M07] 判断是否为主入口
来源：http://qcw.vqdsnc.cn

Py:   if __name__ == "__main__":
来源：http://ijh.hnqzz.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vra.bbcook.cn

JS:   require.main === module
来源：http://swx.ywan-chungtsiang.top

TS:   require.main === module
来源：http://qdx.quarkkingdee.top

Java: public static void main(String[] args)
来源：http://hzd.meibo888.top

Go:   func main()
来源：http://guq.yvedp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xxe.sjlbkw.cn

C#:   static void Main(string[] args)
来源：http://byw.yuanzhike.top

[M08] 获取系统与运行时信息
来源：http://bdk.zhongyouzk.top

Py:   platform.system();  platform.python_version()
来源：http://wbj.havefunace.top

PHP:  PHP_OS;  phpversion();
来源：http://zsa.ywan-chungtsiang.top

JS:   process.platform;  process.version
来源：http://spz.vqdsnc.cn

TS:   process.platform;  process.version
来源：http://rvw.chenjidiqi.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://arc.pengpengdd.cyou

Go:   runtime.GOOS;  runtime.Version()
来源：http://vip.jiagoushi.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pzi.0kj1m.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xre.cashguo.top

================================================================================
来源：http://pkg.zhiwuduotai.top

N. 数据结构与算法
来源：http://ypr.chenlongwang.top

================================================================================
来源：http://wxx.jiagoushi.top

[N01] 二分查找（有序数组）
来源：http://ctx.epnwcf.com

Py:   bisect.bisect_left(arr, x)
来源：http://uvy.cdnleiting.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aoa.andypj.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eex.chenlongwang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ibg.yangfankeji.com

Java: Arrays.binarySearch(arr, x)
来源：http://ojp.yongpay.top

Go:   sort.SearchInts(arr, x)
来源：http://ygt.gaohongyu789.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://idj.xziqi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dcp.yuxming.cn

[N02] 排序（工程实践用内置实现）
来源：http://oft.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://vcd.yj20258888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://apn.feifeiyinyue.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jmv.zhaomingkeji.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://wrz.zhijiandao.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ovh.fengsongda.top

Go:   slices.Sort(arr)
来源：http://viv.zdqjudy.top

Ruby: arr.sort
来源：http://nam.hysaishi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zwu.shanyushiyangtech.top

[N03] 快速排序（分治示例）
来源：http://lta.bbcook.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vhv.jyoumei.cn

PHP:  // 递归实现，或用 usort
来源：http://nzg.jinqigfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ixu.gzhubu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ras.zycfv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eqz.ydjk.org.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ioy.sufxvd.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rxv.aizwys.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bsy.52xcode.cn

[N04] 斐波那契数列
来源：http://kjy.xziqi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nup.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uun.sysykeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hiq.haohaochexian.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gjb.shuidangran.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rhq.jinyuanbaomall.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cxl.sjlbkw.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rbz.chenzaomai.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://knz.tarul.cn

[N05] 最大公约数
来源：http://mea.chenzaomai.com

Py:   math.gcd(a, b)
来源：http://iuv.wangshuangyany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lrq.ppjwa.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://chj.zdqjudy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fcp.ydjk.org.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jhy.gotoacloud.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ixa.yuanzhike.top

Ruby: a.gcd(b)
来源：http://slv.fzhhl.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hjs.ybcxt.top

[N06] 判断回文字符串
来源：http://yul.ydzc1.top

Py:   s == s[::-1]
来源：http://xrp.0kj1m.cn

PHP:  $s === strrev($s);
来源：http://qbe.jiagoushi.top

JS:   s === [...s].reverse().join("")
来源：http://dgm.feifeiyinyue.top

TS:   s === [...s].reverse().join("")
来源：http://ljd.jinghuilouyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gef.zycfv.cn

Go:   // 双指针从两端比较
来源：http://jem.vehdjk.com

Ruby: s == s.reverse
来源：http://cdu.ydjk.org.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yxj.cdnleiting.top

[N07] 两数之和（返回下标）
来源：http://vle.gogol.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kky.xinyue.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rwb.yuxming.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ysk.zhijiandao.cn

TS:   // 手写 Map<string, number>
来源：http://smu.pycfn.com

Java: // 手写 HashMap
来源：http://ocn.sweek.top

Go:   // 手写 map[int]int
来源：http://ofm.xuetiantiany.cn

Ruby: // 手写 Hash
来源：http://pgv.svipenyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rqf.nanxuanxn.top

[N08] 生成全排列
来源：http://bxt.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://mhj.zhoulong.xyz

PHP:  // 手写递归交换
来源：http://gpj.nanxuanxn.top

JS:   // 手写回溯递归
来源：http://hkp.haohaochexian.top

TS:   // 手写回溯递归
来源：http://emc.jinqigfzy.top

Java: // 手写回溯递归
来源：http://zvk.zhengqikj.top

Go:   // 手写回溯递归
来源：http://bqd.jyoumei.cn

Ruby: arr.permutation.to_a
来源：http://tcm.daria6918.cn

C#:   // 手写回溯递归
来源：http://sgv.zhijiandao.cn

[N09] 栈与队列
来源：http://pjo.jiagoushi.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://axc.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sbd.aibaodan.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xdw.zhixingplan.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sbh.hcnkem.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lpq.jinqigfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xiz.smart0.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ciy.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xpo.zhengqikj.top

[N10] 链表节点定义
来源：http://ndv.bbcook.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qzu.feifeiyinyue.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wid.yueranfly.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bhk.yongpay.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ubm.shangyingyoupin.top

Java: class Node { int v; Node next; }
来源：http://kbj.sweek.top

Go:   type Node struct { V int; Next *Node }
来源：http://uub.sufxvd.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rsd.chenlongwang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hyy.fzhhl.top

[N11] 二叉树中序遍历
来源：http://fvu.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ilt.cheryme.top

PHP:  // 手写递归函数
来源：http://oao.shanyushiyangtech.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pkg.xylfe.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hwb.hfpthk.cn

Java: // 手写递归
来源：http://njc.bjfxy.top

Go:   // 手写递归
来源：http://opz.guannengcc.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jkj.xuetiantiany.cn

C#:   // 手写递归
来源：http://lkw.chenzaomai.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vms.daria6918.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vgl.c1oappe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lmn.yj20258888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lge.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qwq.aizwys.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://egz.epnwcf.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dwi.shzxlz.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://esy.zdbjq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tde.feifeiyinyue.top

================================================================================
来源：http://hdf.fehbvm.com

O. 并发与异步
来源：http://opc.jinyuanbaomall.cn

================================================================================
来源：http://ksx.kuanghao11.cn

[O01] 启动一个线程
来源：http://mpm.sjlbkw.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vaw.ehwqpu.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pkq.wangdashe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://awz.uphjek.com

TS:   // 同 JS
来源：http://wud.dianchejie.cn

Java: new Thread(() -> f()).start()
来源：http://kja.yvedp.cn

Go:   go f()
来源：http://yqo.jqgfzy.top

Ruby: Thread.new { f }
来源：http://yzo.zycfv.cn

C#:   Task.Run(() => F());
来源：http://sar.jqgufenzy.top

[O02] 使用线程池
来源：http://uyt.ivvv.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gub.fengsongda.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ceb.feifeiyinyue.top

JS:   // worker_threads 线程池
来源：http://nxy.xinyue.icu

TS:   // worker_threads 线程池
来源：http://jqn.yj20258.top

Java: Executors.newFixedThreadPool(4)
来源：http://xsu.yj202588.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://adb.hfpthk.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vdl.bjfxy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://efq.uphjek.com

[O03] 加锁保护共享数据
来源：http://alh.nanxuanxn.top

Py:   with lock: shared += 1
来源：http://nyh.jinqigfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://hle.vqdsnc.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fcc.shzxlz.cn

TS:   // 同 JS
来源：http://cxs.c1oappe.top

Java: synchronized (this) { shared++; }
来源：http://yrc.yvedp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://esh.zhaomingkeji.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://cpe.hcnkem.com

C#:   lock (gate) { shared++; }
来源：http://jwn.hywenlv.cn

[O04] 定义异步函数并等待
来源：http://tqr.dashuyun.cn

Py:   async def f():⏎    await g()
来源：http://bgc.guowangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kch.yangfankeji.com

JS:   async function f() { await g(); }
来源：http://fja.chenjidiqi.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://scq.iojbl.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nqm.hcnkem.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yze.fehbvm.com

Ruby: # 用 Fiber 或 async gem
来源：http://fdz.daria6918.cn

C#:   async Task F() { await G(); }
来源：http://god.tianlin.xyz

[O05] 并发执行并等待全部完成
来源：http://dxd.zhiwuduotai.top

Py:   asyncio.gather(*tasks)
来源：http://erl.yuxming.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nkk.shuidangran.top

JS:   await Promise.all(tasks)
来源：http://mmy.jinghuilouyu.cn

TS:   await Promise.all(tasks)
来源：http://xwc.yueranfly.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vkq.uphjek.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xmm.yangfankeji.com

Ruby: threads.map(&:join)
来源：http://tog.pycfn.com

C#:   await Task.WhenAll(t1, t2)
来源：http://nzm.xuanzx.com

[O06] 使用进程池
来源：http://npl.guannengcc.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://eqk.feifeiyinyue.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xhs.ywan-chungtsiang.top

JS:   // child_process / cluster 模块
来源：http://hhk.shzxlz.cn

TS:   // child_process / cluster 模块
来源：http://akh.sweek.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oyf.mhx1999.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cio.tarul.cn

Ruby: // fork 块
来源：http://wnt.shangyingyoupin.top

C#:   Parallel.For
来源：http://qlq.daxiang520.top

================================================================================
来源：http://rwm.xingfuxueyuan.xyz

P. 常用工具函数
来源：http://ouh.yonumen.top

================================================================================
来源：http://cdu.chenjidiqi.icu

[P01] 生成 UUID
来源：http://mcq.yfazqb.com

Py:   str(uuid.uuid4())
来源：http://hmq.shuidangran.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://eqb.mhx1999.top

JS:   crypto.randomUUID()
来源：http://bin.guannengcc.top

TS:   crypto.randomUUID()
来源：http://lfl.guowangkeji.top

Java: UUID.randomUUID().toString()
来源：http://qum.uphjek.com

Go:   // 用 github.com/google/uuid
来源：http://wpj.yj20258888.top

Ruby: SecureRandom.uuid
来源：http://veu.fengsongda.top

C#:   Guid.NewGuid().ToString()
来源：http://krm.zhoulong.xyz

[P02] MD5 / SHA256 摘要
来源：http://jot.chenlongwang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bmu.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vhc.vqdsnc.cn


<!-- 参考信息 -->