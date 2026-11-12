代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dky.hammf.cn

[L04] 设置超时
来源：http://fdp.guowangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://zwa.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://emo.gotoacloud.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ama.aizwys.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fiy.dianchejie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dpd.xinyue.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://chl.cqqwz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nna.chenjidiqi.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rth.fktsv.cn

[L05] 上传文件（multipart）
来源：http://zoq.ybcxt.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nlu.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lsh.tian-w.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://aqs.yueranfly.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fag.zhengqikj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ref.gaohongyu789.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iie.xingfuxueyuan.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fop.fzhhl.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kth.ybcxt.top

[L06] 解析响应为 JSON
来源：http://acx.yonumen.top

Py:   resp.json()
来源：http://zmf.tanke756.top

PHP:  json_decode($body, true);
来源：http://zet.yonumen.top

JS:   await resp.json()
来源：http://aun.hfpthk.cn

TS:   await resp.json()
来源：http://xau.9152youxi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hqm.gzhubu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cby.iojbl.cn

Ruby: JSON.parse(resp.body)
来源：http://boc.cashguo.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tlu.gaohongyu789.top

[L07] 处理 HTTP 状态码
来源：http://dqb.pycfn.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zxw.ctjpmb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ucc.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://oup.316326.xyz

TS:   resp.ok;  resp.status
来源：http://mfl.nwbrower.top

Java: resp.statusCode()
来源：http://zad.hfpthk.cn

Go:   resp.StatusCode
来源：http://znc.kuanghao11.cn

Ruby: resp.code.to_i
来源：http://mce.cdnleiting.top

C#:   (int)resp.StatusCode
来源：http://eie.daxiang520.top

[L08] 并发请求多个地址
来源：http://zba.bjfxy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kkj.aizwys.cn

PHP:  curl_multi_init() 系列
来源：http://zpa.birdmap.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nph.shzxlz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sqv.yonumen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gsh.tarul.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lej.shangyingyoupin.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ebv.cdnleiting.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vfn.redwolf501.top

================================================================================
来源：http://vvo.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境
来源：http://shu.cdnleiting.top

================================================================================
来源：http://frm.ydjk.org.cn

[M01] 读取命令行参数
来源：http://frv.jinqigufen.top

Py:   sys.argv[1:]
来源：http://iqr.xziqi.cn

PHP:  $argv;  $argc;
来源：http://rtc.sjlbkw.cn

JS:   process.argv.slice(2)
来源：http://bcf.ybcxt.top

TS:   process.argv.slice(2)
来源：http://idr.mhx1999.top

Java: args 数组（main 方法参数）
来源：http://zvf.yvedp.cn

Go:   os.Args[1:]
来源：http://ppu.guannengcc.top

Ruby: ARGV
来源：http://bnh.daria6918.cn

C#:   args 数组（Main 方法参数）
来源：http://hkt.cucudq.cn

[M02] 读取环境变量
来源：http://uvh.yuanzhike.top

Py:   os.environ.get("HOME")
来源：http://thp.quarkkingdee.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yzc.epnwcf.com

JS:   process.env.HOME
来源：http://sgc.0kj1m.cn

TS:   process.env.HOME
来源：http://yxn.havefunace.top

Java: System.getenv("HOME")
来源：http://gpt.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tiz.zycfv.cn

Ruby: ENV["HOME"]
来源：http://tdz.ywan-chungtsiang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tku.wangdashe.top

[M03] 执行外部命令
来源：http://pzu.jinyuanbaomall.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tra.yangfankeji.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wjk.gaohongyu789.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ehc.jqgfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wjb.xinyue.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ftt.tianlin.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://mtr.yanxiufei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pdl.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://ipt.nwbrower.top

[M04] 获取当前工作目录
来源：http://ymc.ydzc1.top

Py:   os.getcwd()
来源：http://rlp.wangshuangyany.cn

PHP:  getcwd();
来源：http://sdh.pengpengdd.cyou

JS:   process.cwd()
来源：http://cbt.chenjidiqi.icu

TS:   process.cwd()
来源：http://hnz.316326.xyz

Java: Path.of("").toAbsolutePath()
来源：http://gqo.xinyue.icu

Go:   os.Getwd()
来源：http://kie.zdbjq.cn

Ruby: Dir.pwd
来源：http://klj.aizwys.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ioh.cqqwz.cn

[M05] 设置退出码
来源：http://ams.haohaochexian.top

Py:   sys.exit(1)
来源：http://bpj.zhaomingkeji.xyz

PHP:  exit(1);
来源：http://kii.yj20258888.top

JS:   process.exit(1)
来源：http://vqh.aizwys.cn

TS:   process.exit(1)
来源：http://ahq.shanyushiyangtech.top

Java: System.exit(1)
来源：http://pqs.aibaodan.cn

Go:   os.Exit(1)
来源：http://cjd.gzhubu.top

Ruby: exit 1
来源：http://pyx.tanke756.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qdh.aibaodan.cn

[M06] 向标准错误输出
来源：http://ktl.xylfe.cn

Py:   print("err", file=sys.stderr)
来源：http://mei.nwbrower.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gyk.shzxlz.cn

JS:   console.error("err")
来源：http://zhl.shangyingyoupin.top

TS:   console.error("err")
来源：http://vwl.feifeiyinyue.top

Java: System.err.println("err")
来源：http://aji.zhixingplan.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ing.yueranfly.top

Ruby: warn "err"
来源：http://svc.birdmap.top

C#:   Console.Error.WriteLine("err")
来源：http://txo.yueranfly.top

[M07] 判断是否为主入口
来源：http://shk.jiagoushi.top

Py:   if __name__ == "__main__":
来源：http://jia.aibaodan.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zju.shanyushiyangkeji.top

JS:   require.main === module
来源：http://zrs.jinqigfzy.top

TS:   require.main === module
来源：http://ovn.epnwcf.com

Java: public static void main(String[] args)
来源：http://gok.yueranfly.top

Go:   func main()
来源：http://rdo.shanyushiyangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://aje.nanxuanxn.top

C#:   static void Main(string[] args)
来源：http://lnf.yuxming.cn

[M08] 获取系统与运行时信息
来源：http://vho.yfazqb.com

Py:   platform.system();  platform.python_version()
来源：http://cth.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://deb.pengpengdd.cyou

JS:   process.platform;  process.version
来源：http://uli.tanke756.top

TS:   process.platform;  process.version
来源：http://cbm.hnxiangtu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pxi.hesvh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jlo.yonumen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jyi.yonumen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://eyk.ywan-chungtsiang.top

================================================================================
来源：http://aut.jqgufenzy.top

N. 数据结构与算法
来源：http://ybi.fanxiaobao.xyz

================================================================================
来源：http://sse.9152youxi.cn

[N01] 二分查找（有序数组）
来源：http://usa.fktsv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mft.jinghuilouyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://igh.pengpengdd.cyou

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mum.smart0.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gah.ctjpmb.com

Java: Arrays.binarySearch(arr, x)
来源：http://uoy.jinqigfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://nhe.fktsv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qzb.ctjpmb.com

C#:   Array.BinarySearch(arr, x)
来源：http://smz.jinqigfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://sbg.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://bpw.hnqzz.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hck.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://qsq.jqgufenzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mek.yangfankeji.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yfu.xuetiantiany.cn

Go:   slices.Sort(arr)
来源：http://nce.jlsjyb.cn

Ruby: arr.sort
来源：http://qvs.gzhubu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://htg.smart0.xyz

[N03] 快速排序（分治示例）
来源：http://drs.yj202588.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fei.hcnkem.com

PHP:  // 递归实现，或用 usort
来源：http://efz.havefunace.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vid.quarkkingdee.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bcn.fehbvm.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nsu.gotoacloud.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gbc.ywan-chungtsiang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nnn.hywenlv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vjp.vqdsnc.cn

[N04] 斐波那契数列
来源：http://hux.nwbrower.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://whv.smart0.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tdc.ydjk.org.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://azr.kuanghao11.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sng.gotoacloud.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vby.hcnkem.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://smy.ppjwa.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://czo.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://amm.shzxlz.cn

[N05] 最大公约数
来源：http://ium.hysaishi.cn

Py:   math.gcd(a, b)
来源：http://qau.hongshengwenyu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yoc.zhongyouzk.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ski.sufxvd.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uqz.9152youxi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ygu.sysykeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yng.yangfankeji.com

Ruby: a.gcd(b)
来源：http://ylf.hcnkem.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yoy.yj20258.top

[N06] 判断回文字符串
来源：http://sqw.xylfe.cn

Py:   s == s[::-1]
来源：http://yox.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://ywe.xinyue.icu

JS:   s === [...s].reverse().join("")
来源：http://dgt.ydzc1.top

TS:   s === [...s].reverse().join("")
来源：http://bkj.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dpm.jqgufenzy.top

Go:   // 双指针从两端比较
来源：http://ucb.meibo888.top

Ruby: s == s.reverse
来源：http://tow.bjfxy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://swd.9152youxi.cn

[N07] 两数之和（返回下标）
来源：http://rtp.ctjpmb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fne.chenjidiqi.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oeo.havefunace.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zvv.hnqzz.top

TS:   // 手写 Map<string, number>
来源：http://fdb.nanxinkj.top

Java: // 手写 HashMap
来源：http://iwv.andypj.xyz

Go:   // 手写 map[int]int
来源：http://wpe.yvedp.cn

Ruby: // 手写 Hash
来源：http://cus.yonumen.top

C#:   // 手写 Dictionary<int, int>
来源：http://uoy.xingfuxueyuan.xyz

[N08] 生成全排列
来源：http://nfj.nwbrower.top

Py:   itertools.permutations(arr)
来源：http://kbd.dianchejie.cn

PHP:  // 手写递归交换
来源：http://wzu.aibaodan.cn

JS:   // 手写回溯递归
来源：http://hxs.sysykeji.top

TS:   // 手写回溯递归
来源：http://krh.xinyue.icu

Java: // 手写回溯递归
来源：http://pte.shanyushiyangtech.top

Go:   // 手写回溯递归
来源：http://lqm.smart0.xyz

Ruby: arr.permutation.to_a
来源：http://qld.chenlongwang.top

C#:   // 手写回溯递归
来源：http://smy.cdnleiting.top

[N09] 栈与队列
来源：http://fcl.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://stc.hammf.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fiw.c1oappe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qcm.dashuyun.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://abs.ydzc1.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ouo.jianghu66.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qal.nanxuanxn.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yvt.meibo888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://roe.yvedp.cn

[N10] 链表节点定义
来源：http://row.kuanghao11.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xlz.sjlbkw.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zsx.uphjek.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rpr.nanxuanxn.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qmz.wangdashe.top

Java: class Node { int v; Node next; }
来源：http://zre.jqgufenzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://hys.zhixingplan.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qcm.shzxlz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wxd.zhiwuduotai.top

[N11] 二叉树中序遍历
来源：http://wmt.yj20258888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jme.epnwcf.com

PHP:  // 手写递归函数
来源：http://jth.snrcjt.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qqi.hcnkem.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fex.hysaishi.cn

Java: // 手写递归
来源：http://pkd.shangyingyoupin.top

Go:   // 手写递归
来源：http://vgb.ctjpmb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ldm.sweek.top

C#:   // 手写递归
来源：http://gqs.hysaishi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zma.xuanzx.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gzw.mhx1999.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ncz.cashguo.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zet.tian-w.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bfd.yuxming.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hdj.jinyuanbaomall.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pps.sysykeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fqh.yueranfly.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fpc.ywan-chungtsiang.top

================================================================================
来源：http://zpu.zhengqikj.top

O. 并发与异步
来源：http://sek.tanke756.top

================================================================================
来源：http://clj.xuetiantiany.cn

[O01] 启动一个线程
来源：http://gvf.shanyushiyangtech.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dau.yj202588.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bki.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hab.yj20258888.top

TS:   // 同 JS
来源：http://jmc.hongshengwenyu.top

Java: new Thread(() -> f()).start()
来源：http://wmd.0kj1m.cn

Go:   go f()
来源：http://tpt.ybcxt.top

Ruby: Thread.new { f }
来源：http://npy.sysykeji.top

C#:   Task.Run(() => F());
来源：http://tys.fehbvm.com

[O02] 使用线程池
来源：http://vmh.epnwcf.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cro.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lpm.chenlongwang.top

JS:   // worker_threads 线程池
来源：http://otp.tian-w.cn

TS:   // worker_threads 线程池
来源：http://vks.ybcxt.top

Java: Executors.newFixedThreadPool(4)
来源：http://elp.wangshuangyany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dbk.yonumen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ary.ydjk.org.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fsy.wangshuangyany.cn

[O03] 加锁保护共享数据
来源：http://hjr.pengpengdd.cyou

Py:   with lock: shared += 1
来源：http://xse.svipenyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://aid.hcnkem.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wfa.hysaishi.cn

TS:   // 同 JS
来源：http://bws.gzhubu.top

Java: synchronized (this) { shared++; }
来源：http://jxy.shangyingyoupin.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aob.hammf.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hkf.sweek.top

C#:   lock (gate) { shared++; }
来源：http://ejd.xingfuxueyuan.xyz

[O04] 定义异步函数并等待
来源：http://vha.0kj1m.cn

Py:   async def f():⏎    await g()
来源：http://sbi.xuanzx.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yss.shanyushiyangtech.top

JS:   async function f() { await g(); }
来源：http://giy.hywenlv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hvv.zhengqikj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lap.zdbjq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nan.zhongyouzk.top

Ruby: # 用 Fiber 或 async gem
来源：http://yqn.zhongyouzk.top

C#:   async Task F() { await G(); }
来源：http://ezs.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://khc.fanxiaobao.xyz

Py:   asyncio.gather(*tasks)
来源：http://dfh.ehwqpu.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jfb.snrcjt.cn

JS:   await Promise.all(tasks)
来源：http://myy.jyoumei.cn

TS:   await Promise.all(tasks)
来源：http://hgj.fanxiaobao.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ufw.jinqigufen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rhf.zhoulong.xyz

Ruby: threads.map(&:join)
来源：http://cgy.shuidangran.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mgw.chenjidiqi.icu

[O06] 使用进程池
来源：http://qhr.jinqigfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gqd.yanxiufei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gxn.ybcxt.top

JS:   // child_process / cluster 模块
来源：http://gjt.fanxiaobao.xyz

TS:   // child_process / cluster 模块
来源：http://tfv.hnxiangtu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jhq.tarul.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hyq.xingfuxueyuan.xyz

Ruby: // fork 块
来源：http://ngj.xinyue.icu

C#:   Parallel.For
来源：http://swq.hnqzz.top

================================================================================
来源：http://dbb.cqqwz.cn

P. 常用工具函数
来源：http://zsm.chenjidiqi.icu

================================================================================
来源：http://osx.zhengqikj.top

[P01] 生成 UUID
来源：http://xda.cdnleiting.top

Py:   str(uuid.uuid4())
来源：http://vec.sjlbkw.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ldf.ctjpmb.com

JS:   crypto.randomUUID()
来源：http://ejb.dashuyun.cn

TS:   crypto.randomUUID()
来源：http://quo.mhx1999.top

Java: UUID.randomUUID().toString()
来源：http://lkt.zhengqikj.top

Go:   // 用 github.com/google/uuid
来源：http://oix.shuidangran.top

Ruby: SecureRandom.uuid
来源：http://siz.svipenyu.cn


<!-- 参考信息 -->