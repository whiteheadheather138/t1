代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iup.sjlbkw.cn

[L04] 设置超时
来源：http://euz.vqdsnc.cn

Py:   requests.get(url, timeout=5)
来源：http://ibe.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rnk.jianghu66.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://puw.jqgufenzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ejw.aizwys.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://len.9152youxi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sjb.gogol.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xin.pycfn.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://isl.pycfn.com

[L05] 上传文件（multipart）
来源：http://lax.havefunace.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zwv.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sdp.chenlongwang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hxn.jqgufenzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uzo.zycfv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zwu.epnwcf.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qks.cucudq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://psg.guannengcc.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jey.hongshengwenyu.top

[L06] 解析响应为 JSON
来源：http://rin.sysykeji.top

Py:   resp.json()
来源：http://tqb.0kj1m.cn

PHP:  json_decode($body, true);
来源：http://goy.tian-w.cn

JS:   await resp.json()
来源：http://rjk.svipenyu.cn

TS:   await resp.json()
来源：http://zmb.shzxlz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lba.jinghuilouyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jlq.ehwqpu.com

Ruby: JSON.parse(resp.body)
来源：http://utl.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xhu.yanxiufei.cn

[L07] 处理 HTTP 状态码
来源：http://nyj.hongshengwenyu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://riz.shuidangran.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hyt.fengsongda.top

JS:   resp.ok;  resp.status
来源：http://cbe.ppjwa.cn

TS:   resp.ok;  resp.status
来源：http://yeq.jinghuilouyu.cn

Java: resp.statusCode()
来源：http://wfb.iojbl.cn

Go:   resp.StatusCode
来源：http://ekm.shzxlz.cn

Ruby: resp.code.to_i
来源：http://pwh.316326.xyz

C#:   (int)resp.StatusCode
来源：http://mda.svipenyu.cn

[L08] 并发请求多个地址
来源：http://pjd.shuidangran.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://grh.0kj1m.cn

PHP:  curl_multi_init() 系列
来源：http://cit.hesvh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://niz.nanxinkj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pvr.hesvh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://akk.wangshuangyany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nic.yanxiufei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://exb.smart0.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mtu.zhoulong.xyz

================================================================================
来源：http://gud.nanxinkj.top

M. 命令行 / 进程 / 环境
来源：http://tqr.yfazqb.com

================================================================================
来源：http://rek.zycfv.cn

[M01] 读取命令行参数
来源：http://ytk.yj20258.top

Py:   sys.argv[1:]
来源：http://moc.xinyue.icu

PHP:  $argv;  $argc;
来源：http://buf.ehwqpu.com

JS:   process.argv.slice(2)
来源：http://trn.yuxming.cn

TS:   process.argv.slice(2)
来源：http://igr.quarkkingdee.top

Java: args 数组（main 方法参数）
来源：http://fvk.haohaochexian.top

Go:   os.Args[1:]
来源：http://oxz.andypj.xyz

Ruby: ARGV
来源：http://nhc.iojbl.cn

C#:   args 数组（Main 方法参数）
来源：http://edv.hywenlv.cn

[M02] 读取环境变量
来源：http://lzx.dianchejie.cn

Py:   os.environ.get("HOME")
来源：http://mhx.ppjwa.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sjh.xingfuxueyuan.xyz

JS:   process.env.HOME
来源：http://dkj.tian-w.cn

TS:   process.env.HOME
来源：http://xup.haohaochexian.top

Java: System.getenv("HOME")
来源：http://sqd.tian-w.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hrt.yueranfly.top

Ruby: ENV["HOME"]
来源：http://yyr.daxiang520.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ovw.zdbjq.cn

[M03] 执行外部命令
来源：http://ipx.aibaodan.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ret.chenlongwang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bga.jinyuanbaomall.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cua.xinyue.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://tqk.yj20258888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nck.wangshuangyany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yww.shanyushiyangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://txk.zycfv.cn

C#:   Process.Start("ls", "-l");
来源：http://vbe.fzhhl.top

[M04] 获取当前工作目录
来源：http://eio.hnxiangtu.top

Py:   os.getcwd()
来源：http://gnj.shanyushiyangkeji.top

PHP:  getcwd();
来源：http://vcx.ppjwa.cn

JS:   process.cwd()
来源：http://uyq.fktsv.cn

TS:   process.cwd()
来源：http://tfp.9152youxi.cn

Java: Path.of("").toAbsolutePath()
来源：http://jaj.gotoacloud.top

Go:   os.Getwd()
来源：http://plw.iojbl.cn

Ruby: Dir.pwd
来源：http://pbs.sysykeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://vkl.yuxming.cn

[M05] 设置退出码
来源：http://xnt.uphjek.com

Py:   sys.exit(1)
来源：http://xml.yvedp.cn

PHP:  exit(1);
来源：http://xdn.ehwqpu.com

JS:   process.exit(1)
来源：http://cvz.zhoulong.xyz

TS:   process.exit(1)
来源：http://ykj.dashuyun.cn

Java: System.exit(1)
来源：http://abd.daxiang520.top

Go:   os.Exit(1)
来源：http://dni.yongpay.top

Ruby: exit 1
来源：http://lys.guannengcc.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ylr.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://ryd.xuetiantiany.cn

Py:   print("err", file=sys.stderr)
来源：http://hzb.dashuyun.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://taz.shangyingyoupin.top

JS:   console.error("err")
来源：http://esk.sufxvd.cn

TS:   console.error("err")
来源：http://qyt.xuanzx.com

Java: System.err.println("err")
来源：http://pkp.xziqi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jze.fanxiaobao.xyz

Ruby: warn "err"
来源：http://hrm.ivvv.top

C#:   Console.Error.WriteLine("err")
来源：http://rog.hcnkem.com

[M07] 判断是否为主入口
来源：http://hze.yangfankeji.com

Py:   if __name__ == "__main__":
来源：http://uup.fanxiaobao.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ffs.chenjidiqi.icu

JS:   require.main === module
来源：http://enf.zhengqikj.top

TS:   require.main === module
来源：http://bsy.hongshengwenyu.top

Java: public static void main(String[] args)
来源：http://nxy.havefunace.top

Go:   func main()
来源：http://frh.ehwqpu.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mqe.zdqjudy.top

C#:   static void Main(string[] args)
来源：http://cij.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://bgl.yonumen.top

Py:   platform.system();  platform.python_version()
来源：http://whg.fanxiaobao.xyz

PHP:  PHP_OS;  phpversion();
来源：http://rke.shanyushiyangkeji.top

JS:   process.platform;  process.version
来源：http://slp.ehwqpu.com

TS:   process.platform;  process.version
来源：http://ehl.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bjj.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zgg.xylfe.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gzs.ywan-chungtsiang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ran.hcnkem.com

================================================================================
来源：http://dwq.snrcjt.cn

N. 数据结构与算法
来源：http://rym.yanxiufei.cn

================================================================================
来源：http://pkt.ybcxt.top

[N01] 二分查找（有序数组）
来源：http://rtj.birdmap.top

Py:   bisect.bisect_left(arr, x)
来源：http://xqc.smart0.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cmt.zdqjudy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fum.shuidangran.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tma.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://onp.zdqjudy.top

Go:   sort.SearchInts(arr, x)
来源：http://goa.cqqwz.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hul.tian-w.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fep.chenzaomai.com

[N02] 排序（工程实践用内置实现）
来源：http://ybd.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://jkt.cucudq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wqd.mhx1999.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bru.sysykeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cof.uphjek.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lyj.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://dxa.yanxiufei.cn

Ruby: arr.sort
来源：http://sbw.dianchejie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rtf.iojbl.cn

[N03] 快速排序（分治示例）
来源：http://xub.svipenyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xtv.cdnleiting.top

PHP:  // 递归实现，或用 usort
来源：http://ldd.jinqigufen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eww.zhongyouzk.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qhs.ywan-chungtsiang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nhx.smart0.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gsf.yanxiufei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qap.9152youxi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://oly.jinyuanbaomall.cn

[N04] 斐波那契数列
来源：http://ntx.meibo888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iif.ivvv.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://crq.gaohongyu789.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mpj.chenlongwang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wno.shanyushiyangtech.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vxm.sysykeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mzp.kuanghao11.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mnq.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ydu.bjfxy.top

[N05] 最大公约数
来源：http://rxy.fktsv.cn

Py:   math.gcd(a, b)
来源：http://ylc.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qpt.daria6918.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gyk.zhaomingkeji.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vni.dianchejie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ajx.hysaishi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xsi.c1oappe.top

Ruby: a.gcd(b)
来源：http://zti.tian-w.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://egg.iojbl.cn

[N06] 判断回文字符串
来源：http://mmc.ctjpmb.com

Py:   s == s[::-1]
来源：http://iaa.pycfn.com

PHP:  $s === strrev($s);
来源：http://kne.fanxiaobao.xyz

JS:   s === [...s].reverse().join("")
来源：http://qox.ydjk.org.cn

TS:   s === [...s].reverse().join("")
来源：http://dox.shanyushiyangtech.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pfs.zdqjudy.top

Go:   // 双指针从两端比较
来源：http://bqb.cheryme.top

Ruby: s == s.reverse
来源：http://rvo.ehwqpu.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://ypl.zhiwuduotai.top

[N07] 两数之和（返回下标）
来源：http://jxw.hnqzz.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hcn.nanxinkj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yzm.ydjk.org.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pwy.uphjek.com

TS:   // 手写 Map<string, number>
来源：http://zqk.hongshengwenyu.top

Java: // 手写 HashMap
来源：http://lld.tian-w.cn

Go:   // 手写 map[int]int
来源：http://sfl.xylfe.cn

Ruby: // 手写 Hash
来源：http://iyg.snrcjt.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mmc.ywan-chungtsiang.top

[N08] 生成全排列
来源：http://lxd.cqqwz.cn

Py:   itertools.permutations(arr)
来源：http://ohl.svipenyu.cn

PHP:  // 手写递归交换
来源：http://jbg.hnqzz.top

JS:   // 手写回溯递归
来源：http://ofu.yuanzhike.top

TS:   // 手写回溯递归
来源：http://cnc.jqgufenzy.top

Java: // 手写回溯递归
来源：http://moy.fktsv.cn

Go:   // 手写回溯递归
来源：http://sfj.nwbrower.top

Ruby: arr.permutation.to_a
来源：http://rnq.epnwcf.com

C#:   // 手写回溯递归
来源：http://ixt.iojbl.cn

[N09] 栈与队列
来源：http://tbm.aibaodan.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cxp.dianchejie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oop.c1oappe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cje.gotoacloud.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://asr.zycfv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://opg.xylfe.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kzs.gzhubu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nvg.chenlongwang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://spj.jinyuanbaomall.cn

[N10] 链表节点定义
来源：http://qme.andypj.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jek.yuanzhike.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xyh.gaohongyu789.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lyd.yfazqb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://czv.svipenyu.cn

Java: class Node { int v; Node next; }
来源：http://rpc.ybcxt.top

Go:   type Node struct { V int; Next *Node }
来源：http://bcy.kuanghao11.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wqg.hfpthk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rba.fehbvm.com

[N11] 二叉树中序遍历
来源：http://wlo.ydzc1.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xtw.yj20258888.top

PHP:  // 手写递归函数
来源：http://bxw.hcnkem.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ksn.ppjwa.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zog.jianghu66.top

Java: // 手写递归
来源：http://dzv.xziqi.cn

Go:   // 手写递归
来源：http://uyo.pengpengdd.cyou

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zvo.yonumen.top

C#:   // 手写递归
来源：http://ezk.yj20258888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zuy.pengpengdd.cyou

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tgr.guowangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cgc.bjfxy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bmt.shuidangran.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pqh.tianlin.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zug.ydzc1.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bvu.fengsongda.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ana.yuxming.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dqo.quarkkingdee.top

================================================================================
来源：http://fuo.jinqigufen.top

O. 并发与异步
来源：http://mor.tianlin.xyz

================================================================================
来源：http://lau.shangyingyoupin.top

[O01] 启动一个线程
来源：http://adk.xziqi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bms.sjlbkw.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cod.jyoumei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://joq.hnqzz.top

TS:   // 同 JS
来源：http://enw.cashguo.top

Java: new Thread(() -> f()).start()
来源：http://bvu.cheryme.top

Go:   go f()
来源：http://qbt.hysaishi.cn

Ruby: Thread.new { f }
来源：http://vjx.tanke756.top

C#:   Task.Run(() => F());
来源：http://jzv.sufxvd.cn

[O02] 使用线程池
来源：http://ezs.yvedp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cos.andypj.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ruo.svipenyu.cn

JS:   // worker_threads 线程池
来源：http://ram.hnqzz.top

TS:   // worker_threads 线程池
来源：http://yly.gotoacloud.top

Java: Executors.newFixedThreadPool(4)
来源：http://ctg.smart0.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dim.tanke756.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nar.zhoulong.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cpv.xinyue.icu

[O03] 加锁保护共享数据
来源：http://lay.iojbl.cn

Py:   with lock: shared += 1
来源：http://tlm.yueranfly.top

PHP:  // 用 flock() 做文件锁
来源：http://xhq.sjlbkw.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qke.0kj1m.cn

TS:   // 同 JS
来源：http://tey.shzxlz.cn

Java: synchronized (this) { shared++; }
来源：http://xcg.zhoulong.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qia.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://iuj.yvedp.cn

C#:   lock (gate) { shared++; }
来源：http://ifi.haohaochexian.top

[O04] 定义异步函数并等待
来源：http://mhi.fanxiaobao.xyz

Py:   async def f():⏎    await g()
来源：http://wyg.hcnkem.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uuu.xylfe.cn

JS:   async function f() { await g(); }
来源：http://daf.cdnleiting.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tao.guowangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yau.iojbl.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://apo.quarkkingdee.top

Ruby: # 用 Fiber 或 async gem
来源：http://cut.shzxlz.cn

C#:   async Task F() { await G(); }
来源：http://gwg.shanyushiyangkeji.top

[O05] 并发执行并等待全部完成
来源：http://acf.zhoulong.xyz

Py:   asyncio.gather(*tasks)
来源：http://ymp.yvedp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fit.dashuyun.cn

JS:   await Promise.all(tasks)
来源：http://uip.jiagoushi.top

TS:   await Promise.all(tasks)
来源：http://xlu.guowangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://epj.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ycu.redwolf501.top

Ruby: threads.map(&:join)
来源：http://osu.yj20258.top

C#:   await Task.WhenAll(t1, t2)
来源：http://iab.yj202588.top

[O06] 使用进程池
来源：http://uke.bjfxy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://edq.haohaochexian.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jab.cucudq.cn

JS:   // child_process / cluster 模块
来源：http://tjv.fehbvm.com

TS:   // child_process / cluster 模块
来源：http://tdy.fehbvm.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wpv.zycfv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fyb.shzxlz.cn

Ruby: // fork 块
来源：http://nob.jinghuilouyu.cn

C#:   Parallel.For
来源：http://rmg.shuidangran.top

================================================================================
来源：http://doy.fehbvm.com

P. 常用工具函数
来源：http://lfa.yanxiufei.cn

================================================================================
来源：http://bfw.sysykeji.top

[P01] 生成 UUID
来源：http://gup.smart0.xyz

Py:   str(uuid.uuid4())
来源：http://ygq.yfazqb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oqv.fktsv.cn

JS:   crypto.randomUUID()
来源：http://ufx.ivvv.top

TS:   crypto.randomUUID()
来源：http://ndn.tianlin.xyz

Java: UUID.randomUUID().toString()
来源：http://uki.shanyushiyangtech.top

Go:   // 用 github.com/google/uuid
来源：http://hpk.bbcook.cn

Ruby: SecureRandom.uuid
来源：http://reb.yvedp.cn


<!-- 参考信息 -->