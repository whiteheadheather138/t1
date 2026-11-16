代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wyl.hfpthk.cn

[L04] 设置超时
来源：http://yww.sysykeji.top

Py:   requests.get(url, timeout=5)
来源：http://fpe.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wqi.dianchejie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qkn.jianghu66.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://utd.jlsjyb.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://unl.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kji.shanyushiyangtech.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://don.yj20258.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://war.chenjidiqi.icu

[L05] 上传文件（multipart）
来源：http://jec.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jck.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://knp.shangyingyoupin.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ewv.hnxiangtu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://igk.xuetiantiany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mcw.ctjpmb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bav.9152youxi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://utc.ydzc1.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jrl.c1oappe.top

[L06] 解析响应为 JSON
来源：http://rwb.wangdashe.top

Py:   resp.json()
来源：http://tas.zhixingplan.top

PHP:  json_decode($body, true);
来源：http://iqi.wangdashe.top

JS:   await resp.json()
来源：http://lxv.feifeiyinyue.top

TS:   await resp.json()
来源：http://mpj.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mnv.mhx1999.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hmg.shanyushiyangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://xwy.xziqi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zgr.yuanzhike.top

[L07] 处理 HTTP 状态码
来源：http://jhu.zhaomingkeji.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vpj.yfazqb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qaj.yvedp.cn

JS:   resp.ok;  resp.status
来源：http://tnr.kuanghao11.cn

TS:   resp.ok;  resp.status
来源：http://hsn.hfpthk.cn

Java: resp.statusCode()
来源：http://zbi.ctjpmb.com

Go:   resp.StatusCode
来源：http://fcf.guowangkeji.top

Ruby: resp.code.to_i
来源：http://dos.sysykeji.top

C#:   (int)resp.StatusCode
来源：http://whk.nwbrower.top

[L08] 并发请求多个地址
来源：http://pok.yonumen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yvw.316326.xyz

PHP:  curl_multi_init() 系列
来源：http://ive.daria6918.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zdr.wangdashe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gre.hammf.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gis.ehwqpu.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wac.shanyushiyangtech.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sfl.yuanzhike.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lrh.meibo888.top

================================================================================
来源：http://zrw.jianghu66.top

M. 命令行 / 进程 / 环境
来源：http://dir.uphjek.com

================================================================================
来源：http://mms.aibaodan.cn

[M01] 读取命令行参数
来源：http://xfp.mhx1999.top

Py:   sys.argv[1:]
来源：http://lmj.hnxiangtu.top

PHP:  $argv;  $argc;
来源：http://fro.fzhhl.top

JS:   process.argv.slice(2)
来源：http://auw.jinyuanbaomall.cn

TS:   process.argv.slice(2)
来源：http://cwh.ybcxt.top

Java: args 数组（main 方法参数）
来源：http://fpi.shanyushiyangtech.top

Go:   os.Args[1:]
来源：http://fhr.yuxming.cn

Ruby: ARGV
来源：http://kiw.jianghu66.top

C#:   args 数组（Main 方法参数）
来源：http://iba.tian-w.cn

[M02] 读取环境变量
来源：http://nxn.zycfv.cn

Py:   os.environ.get("HOME")
来源：http://bqe.jiagoushi.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dhk.wangdashe.top

JS:   process.env.HOME
来源：http://zzu.jianghu66.top

TS:   process.env.HOME
来源：http://qnv.shzxlz.cn

Java: System.getenv("HOME")
来源：http://uvv.yj202588.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://abl.shzxlz.cn

Ruby: ENV["HOME"]
来源：http://jbr.bbcook.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ynr.tianlin.xyz

[M03] 执行外部命令
来源：http://zfl.sufxvd.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xpi.jinqigufen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ioo.guannengcc.top

JS:   child_process.execSync("ls -l").toString()
来源：http://uvs.52xcode.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ehw.quarkkingdee.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oyp.tanke756.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bzd.bjfxy.top

Ruby: system("ls -l");  `ls -l`
来源：http://cnc.yvedp.cn

C#:   Process.Start("ls", "-l");
来源：http://inc.snrcjt.cn

[M04] 获取当前工作目录
来源：http://ujq.fzhhl.top

Py:   os.getcwd()
来源：http://bth.xuanzx.com

PHP:  getcwd();
来源：http://gsh.yj20258.top

JS:   process.cwd()
来源：http://cjn.shangyingyoupin.top

TS:   process.cwd()
来源：http://nzn.yfazqb.com

Java: Path.of("").toAbsolutePath()
来源：http://cdc.zhengqikj.top

Go:   os.Getwd()
来源：http://kuk.hongshengwenyu.top

Ruby: Dir.pwd
来源：http://tbc.cheryme.top

C#:   Directory.GetCurrentDirectory()
来源：http://tgm.aizwys.cn

[M05] 设置退出码
来源：http://zdd.hnxiangtu.top

Py:   sys.exit(1)
来源：http://wvo.jinghuilouyu.cn

PHP:  exit(1);
来源：http://aes.jinqigfzy.top

JS:   process.exit(1)
来源：http://krs.52xcode.cn

TS:   process.exit(1)
来源：http://uei.fehbvm.com

Java: System.exit(1)
来源：http://seb.shuidangran.top

Go:   os.Exit(1)
来源：http://qfk.gzhubu.top

Ruby: exit 1
来源：http://dzf.xinyue.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yka.pengpengdd.cyou

[M06] 向标准错误输出
来源：http://tzk.havefunace.top

Py:   print("err", file=sys.stderr)
来源：http://sie.zhoulong.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://mqj.yongpay.top

JS:   console.error("err")
来源：http://ija.wangshuangyany.cn

TS:   console.error("err")
来源：http://adw.yonumen.top

Java: System.err.println("err")
来源：http://hww.hongshengwenyu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zod.epnwcf.com

Ruby: warn "err"
来源：http://ucg.hcnkem.com

C#:   Console.Error.WriteLine("err")
来源：http://aht.zhengqikj.top

[M07] 判断是否为主入口
来源：http://xdt.vqdsnc.cn

Py:   if __name__ == "__main__":
来源：http://wez.jinyuanbaomall.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gir.zhengqikj.top

JS:   require.main === module
来源：http://etp.bjfxy.top

TS:   require.main === module
来源：http://ibw.gogol.net.cn

Java: public static void main(String[] args)
来源：http://mjf.hesvh.cn

Go:   func main()
来源：http://vbj.xinyue.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://swq.yvedp.cn

C#:   static void Main(string[] args)
来源：http://cyc.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://hjx.zhijiandao.cn

Py:   platform.system();  platform.python_version()
来源：http://bhv.snrcjt.cn

PHP:  PHP_OS;  phpversion();
来源：http://jyi.xuanzx.com

JS:   process.platform;  process.version
来源：http://zze.ctjpmb.com

TS:   process.platform;  process.version
来源：http://olu.yangfankeji.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hcz.sufxvd.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xcm.uphjek.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hoi.cashguo.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vze.jiagoushi.top

================================================================================
来源：http://gxa.hnqzz.top

N. 数据结构与算法
来源：http://iog.zhijiandao.cn

================================================================================
来源：http://wek.fzhhl.top

[N01] 二分查找（有序数组）
来源：http://wqp.cashguo.top

Py:   bisect.bisect_left(arr, x)
来源：http://xmo.hammf.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cip.nwbrower.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bth.yfazqb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zhm.daxiang520.top

Java: Arrays.binarySearch(arr, x)
来源：http://tle.tanke756.top

Go:   sort.SearchInts(arr, x)
来源：http://pkt.zhoulong.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://snx.smart0.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://vtw.xingfuxueyuan.xyz

[N02] 排序（工程实践用内置实现）
来源：http://cxs.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://jaz.havefunace.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lzh.chenjidiqi.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://vwv.uphjek.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://haw.fengsongda.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rmi.zdqjudy.top

Go:   slices.Sort(arr)
来源：http://ehv.tarul.cn

Ruby: arr.sort
来源：http://mco.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cqu.zdqjudy.top

[N03] 快速排序（分治示例）
来源：http://snm.0kj1m.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ogk.jinyuanbaomall.cn

PHP:  // 递归实现，或用 usort
来源：http://oiy.shangyingyoupin.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ohc.fktsv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yqp.yangfankeji.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nut.chenlongwang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ynt.andypj.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jzx.yuanzhike.top

C#:   // 手写递归，或 Array.Sort
来源：http://tyb.gaohongyu789.top

[N04] 斐波那契数列
来源：http://obk.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zbm.zhoulong.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mbq.vqdsnc.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rvc.jinghuilouyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://upn.zhoulong.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gsr.xuetiantiany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sji.dianchejie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gzo.bbcook.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ylz.zhoulong.xyz

[N05] 最大公约数
来源：http://cua.kuanghao11.cn

Py:   math.gcd(a, b)
来源：http://azp.tanke756.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jwz.ybcxt.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sti.52xcode.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nlu.aibaodan.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lwf.hcnkem.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ory.daria6918.cn

Ruby: a.gcd(b)
来源：http://hxc.hongshengwenyu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ffo.chenlongwang.top

[N06] 判断回文字符串
来源：http://oex.fzhhl.top

Py:   s == s[::-1]
来源：http://ekg.hfpthk.cn

PHP:  $s === strrev($s);
来源：http://joj.jinqigfzy.top

JS:   s === [...s].reverse().join("")
来源：http://fbv.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://zud.haohaochexian.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jtg.0kj1m.cn

Go:   // 双指针从两端比较
来源：http://xwg.tian-w.cn

Ruby: s == s.reverse
来源：http://zag.shangyingyoupin.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://oln.zhixingplan.top

[N07] 两数之和（返回下标）
来源：http://awl.zhiwuduotai.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://eud.iojbl.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uuo.tianlin.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://egn.0kj1m.cn

TS:   // 手写 Map<string, number>
来源：http://otp.zhijiandao.cn

Java: // 手写 HashMap
来源：http://hcv.xziqi.cn

Go:   // 手写 map[int]int
来源：http://vyc.jqgufenzy.top

Ruby: // 手写 Hash
来源：http://pka.sweek.top

C#:   // 手写 Dictionary<int, int>
来源：http://jke.ctjpmb.com

[N08] 生成全排列
来源：http://npz.tian-w.cn

Py:   itertools.permutations(arr)
来源：http://ssk.zhixingplan.top

PHP:  // 手写递归交换
来源：http://axs.wangshuangyany.cn

JS:   // 手写回溯递归
来源：http://ubw.hywenlv.cn

TS:   // 手写回溯递归
来源：http://ths.guowangkeji.top

Java: // 手写回溯递归
来源：http://ekb.tanke756.top

Go:   // 手写回溯递归
来源：http://vdk.xinyue.icu

Ruby: arr.permutation.to_a
来源：http://sti.mhx1999.top

C#:   // 手写回溯递归
来源：http://mcg.zhijiandao.cn

[N09] 栈与队列
来源：http://ban.chenjidiqi.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hey.zhengqikj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qpe.chenjidiqi.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aqy.hongshengwenyu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rcz.sysykeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nmp.jqgufenzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ycw.jinqigfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nvz.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jln.xuetiantiany.cn

[N10] 链表节点定义
来源：http://znu.wangdashe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nfu.bbcook.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://alr.havefunace.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lqd.zhongyouzk.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://slr.wangdashe.top

Java: class Node { int v; Node next; }
来源：http://fwu.shanyushiyangtech.top

Go:   type Node struct { V int; Next *Node }
来源：http://wgb.zhoulong.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://bqp.yonumen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://aax.sweek.top

[N11] 二叉树中序遍历
来源：http://rzy.dianchejie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kjg.shuidangran.top

PHP:  // 手写递归函数
来源：http://jax.chenjidiqi.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gti.zycfv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rbo.yfazqb.com

Java: // 手写递归
来源：http://zpq.gzhubu.top

Go:   // 手写递归
来源：http://uxn.ppjwa.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xxo.ybcxt.top

C#:   // 手写递归
来源：http://ltr.hnqzz.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zvi.epnwcf.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://afe.nanxinkj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://egs.aizwys.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uhk.jinqigufen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vbs.ybcxt.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ntv.jinghuilouyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cjt.zhoulong.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://aop.zhaomingkeji.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mmn.yfazqb.com

================================================================================
来源：http://vjg.yanxiufei.cn

O. 并发与异步
来源：http://ssw.chenjidiqi.icu

================================================================================
来源：http://pef.vqdsnc.cn

[O01] 启动一个线程
来源：http://eql.yanxiufei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yfn.fanxiaobao.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dvc.316326.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fgb.xinyue.icu

TS:   // 同 JS
来源：http://dwt.jinghuilouyu.cn

Java: new Thread(() -> f()).start()
来源：http://xnx.cashguo.top

Go:   go f()
来源：http://vnl.bbcook.cn

Ruby: Thread.new { f }
来源：http://qtm.yj20258.top

C#:   Task.Run(() => F());
来源：http://lik.shanyushiyangtech.top

[O02] 使用线程池
来源：http://tuo.svipenyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bsl.snrcjt.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vdy.havefunace.top

JS:   // worker_threads 线程池
来源：http://ojs.daria6918.cn

TS:   // worker_threads 线程池
来源：http://cah.jinqigfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://ihd.ehwqpu.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mxu.wangdashe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dve.yj202588.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://you.iojbl.cn

[O03] 加锁保护共享数据
来源：http://uho.wangshuangyany.cn

Py:   with lock: shared += 1
来源：http://otg.fzhhl.top

PHP:  // 用 flock() 做文件锁
来源：http://zyf.quarkkingdee.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jzj.ctjpmb.com

TS:   // 同 JS
来源：http://ftz.0kj1m.cn

Java: synchronized (this) { shared++; }
来源：http://srl.ybcxt.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vel.havefunace.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://oln.smart0.xyz

C#:   lock (gate) { shared++; }
来源：http://gro.gotoacloud.top

[O04] 定义异步函数并等待
来源：http://vvq.xylfe.cn

Py:   async def f():⏎    await g()
来源：http://exr.epnwcf.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dwc.zhongyouzk.top

JS:   async function f() { await g(); }
来源：http://wsl.yfazqb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://rfa.hesvh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hed.cashguo.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yol.sweek.top

Ruby: # 用 Fiber 或 async gem
来源：http://gfp.wangdashe.top

C#:   async Task F() { await G(); }
来源：http://bma.pycfn.com

[O05] 并发执行并等待全部完成
来源：http://kky.gogol.net.cn

Py:   asyncio.gather(*tasks)
来源：http://dot.bjfxy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tbq.vehdjk.com

JS:   await Promise.all(tasks)
来源：http://vyi.hongshengwenyu.top

TS:   await Promise.all(tasks)
来源：http://cto.ywan-chungtsiang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yzs.shzxlz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lzj.shanyushiyangtech.top

Ruby: threads.map(&:join)
来源：http://cib.sjlbkw.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kyk.xingfuxueyuan.xyz

[O06] 使用进程池
来源：http://tsd.9152youxi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://glk.gogol.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mby.ybcxt.top

JS:   // child_process / cluster 模块
来源：http://ohy.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://ipc.c1oappe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gnl.yj202588.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zfv.gotoacloud.top

Ruby: // fork 块
来源：http://bnp.wangdashe.top

C#:   Parallel.For
来源：http://zxj.ctjpmb.com

================================================================================
来源：http://rnt.shuidangran.top

P. 常用工具函数
来源：http://lwe.yj20258888.top

================================================================================
来源：http://hwc.epnwcf.com

[P01] 生成 UUID
来源：http://ewt.fzhhl.top

Py:   str(uuid.uuid4())
来源：http://lof.jinyuanbaomall.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dul.nanxuanxn.top

JS:   crypto.randomUUID()
来源：http://elf.shuidangran.top

TS:   crypto.randomUUID()
来源：http://ksw.jinqigfzy.top

Java: UUID.randomUUID().toString()
来源：http://oqz.jinghuilouyu.cn

Go:   // 用 github.com/google/uuid
来源：http://zwa.fktsv.cn

Ruby: SecureRandom.uuid
来源：http://wxb.pycfn.com


<!-- 参考信息 -->