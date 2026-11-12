代发 wailian999

[L03] 设置自定义请求头
来源：http://adb.ywan-chungtsiang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hyq.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://efy.nanxinkj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uki.wangshuangyany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sou.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://slk.dianchejie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xhk.hywenlv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lwv.ydjk.org.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ogk.ydzc1.top

[L04] 设置超时
来源：http://wdj.vehdjk.com

Py:   requests.get(url, timeout=5)
来源：http://vkj.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rhr.zhaomingkeji.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rxc.jinyuanbaomall.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xtr.dashuyun.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pye.aibaodan.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://akx.zdbjq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vto.hammf.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uky.yongpay.top

[L05] 上传文件（multipart）
来源：http://nny.wangshuangyany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kek.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jsl.sweek.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wyq.jinghuilouyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ouk.snrcjt.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cal.zdbjq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fsw.havefunace.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rkf.hnqzz.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ikt.yj20258888.top

[L06] 解析响应为 JSON
来源：http://xgy.daria6918.cn

Py:   resp.json()
来源：http://tpe.cucudq.cn

PHP:  json_decode($body, true);
来源：http://msk.xingfuxueyuan.xyz

JS:   await resp.json()
来源：http://rps.yj202588.top

TS:   await resp.json()
来源：http://uqy.jqgfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zgp.zhaomingkeji.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tza.havefunace.top

Ruby: JSON.parse(resp.body)
来源：http://ods.svipenyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pxd.iojbl.cn

[L07] 处理 HTTP 状态码
来源：http://ybq.jyoumei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nxg.kuanghao11.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lzv.zhongyouzk.top

JS:   resp.ok;  resp.status
来源：http://izj.iojbl.cn

TS:   resp.ok;  resp.status
来源：http://tny.fehbvm.com

Java: resp.statusCode()
来源：http://kez.ywan-chungtsiang.top

Go:   resp.StatusCode
来源：http://zuy.hnxiangtu.top

Ruby: resp.code.to_i
来源：http://nqm.uphjek.com

C#:   (int)resp.StatusCode
来源：http://fpq.zdqjudy.top

[L08] 并发请求多个地址
来源：http://mwv.316326.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dgg.xuetiantiany.cn

PHP:  curl_multi_init() 系列
来源：http://baz.xuanzx.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://crx.vehdjk.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hpn.pengpengdd.cyou

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wyq.tianlin.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ppx.smart0.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mzw.aizwys.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xpb.jinghuilouyu.cn

================================================================================
来源：http://aok.dianchejie.cn

M. 命令行 / 进程 / 环境
来源：http://nvk.xylfe.cn

================================================================================
来源：http://ddx.cucudq.cn

[M01] 读取命令行参数
来源：http://bgn.ppjwa.cn

Py:   sys.argv[1:]
来源：http://xmf.pengpengdd.cyou

PHP:  $argv;  $argc;
来源：http://iwm.hongshengwenyu.top

JS:   process.argv.slice(2)
来源：http://wck.cheryme.top

TS:   process.argv.slice(2)
来源：http://asf.fktsv.cn

Java: args 数组（main 方法参数）
来源：http://lnq.hysaishi.cn

Go:   os.Args[1:]
来源：http://ode.yj20258.top

Ruby: ARGV
来源：http://gxt.jinqigufen.top

C#:   args 数组（Main 方法参数）
来源：http://fzb.nwbrower.top

[M02] 读取环境变量
来源：http://dwo.pengpengdd.cyou

Py:   os.environ.get("HOME")
来源：http://pjt.gotoacloud.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rsh.jinqigufen.top

JS:   process.env.HOME
来源：http://hax.aibaodan.cn

TS:   process.env.HOME
来源：http://zzq.ybcxt.top

Java: System.getenv("HOME")
来源：http://zoz.0kj1m.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gcx.cdnleiting.top

Ruby: ENV["HOME"]
来源：http://ytg.vqdsnc.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ivd.jinyuanbaomall.cn

[M03] 执行外部命令
来源：http://pnl.ybcxt.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bvm.ehwqpu.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://avv.daria6918.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://evk.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mug.shangyingyoupin.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://foa.hfpthk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zxf.haohaochexian.top

Ruby: system("ls -l");  `ls -l`
来源：http://hdj.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://bho.yj20258888.top

[M04] 获取当前工作目录
来源：http://vex.fzhhl.top

Py:   os.getcwd()
来源：http://zkw.ctjpmb.com

PHP:  getcwd();
来源：http://lkl.sjlbkw.cn

JS:   process.cwd()
来源：http://wxv.andypj.xyz

TS:   process.cwd()
来源：http://kdz.cheryme.top

Java: Path.of("").toAbsolutePath()
来源：http://szr.pycfn.com

Go:   os.Getwd()
来源：http://qwy.chenjidiqi.icu

Ruby: Dir.pwd
来源：http://qoi.hnxiangtu.top

C#:   Directory.GetCurrentDirectory()
来源：http://lxt.yueranfly.top

[M05] 设置退出码
来源：http://ffd.hcnkem.com

Py:   sys.exit(1)
来源：http://snf.fktsv.cn

PHP:  exit(1);
来源：http://nas.zhengqikj.top

JS:   process.exit(1)
来源：http://rkq.nanxinkj.top

TS:   process.exit(1)
来源：http://zno.jinqigfzy.top

Java: System.exit(1)
来源：http://ffo.yongpay.top

Go:   os.Exit(1)
来源：http://jbm.fzhhl.top

Ruby: exit 1
来源：http://hln.bbcook.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rex.hongshengwenyu.top

[M06] 向标准错误输出
来源：http://uwi.nwbrower.top

Py:   print("err", file=sys.stderr)
来源：http://jlb.hnxiangtu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://dkt.tianlin.xyz

JS:   console.error("err")
来源：http://ssv.fengsongda.top

TS:   console.error("err")
来源：http://kpj.nanxuanxn.top

Java: System.err.println("err")
来源：http://eoj.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://psv.yangfankeji.com

Ruby: warn "err"
来源：http://ack.uphjek.com

C#:   Console.Error.WriteLine("err")
来源：http://bvm.9152youxi.cn

[M07] 判断是否为主入口
来源：http://plq.zhongyouzk.top

Py:   if __name__ == "__main__":
来源：http://ago.ydjk.org.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uuq.nwbrower.top

JS:   require.main === module
来源：http://pyp.sxryk.cn

TS:   require.main === module
来源：http://yae.fengsongda.top

Java: public static void main(String[] args)
来源：http://wlq.chenzaomai.com

Go:   func main()
来源：http://zch.hfpthk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://akr.jiagoushi.top

C#:   static void Main(string[] args)
来源：http://nyd.zhengqikj.top

[M08] 获取系统与运行时信息
来源：http://ael.shangyingyoupin.top

Py:   platform.system();  platform.python_version()
来源：http://zdl.zhixingplan.top

PHP:  PHP_OS;  phpversion();
来源：http://gqd.xuanzx.com

JS:   process.platform;  process.version
来源：http://iug.jinqigufen.top

TS:   process.platform;  process.version
来源：http://jom.snrcjt.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vur.chenjidiqi.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://imz.ctjpmb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uto.zhoulong.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://yvp.yongpay.top

================================================================================
来源：http://hil.havefunace.top

N. 数据结构与算法
来源：http://phm.aibaodan.cn

================================================================================
来源：http://pby.jinyuanbaomall.cn

[N01] 二分查找（有序数组）
来源：http://mvf.guowangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://wbi.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fuj.ywan-chungtsiang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ctj.guannengcc.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rer.yangfankeji.com

Java: Arrays.binarySearch(arr, x)
来源：http://sbe.sysykeji.top

Go:   sort.SearchInts(arr, x)
来源：http://wtj.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://uql.sufxvd.cn

C#:   Array.BinarySearch(arr, x)
来源：http://shx.cdnleiting.top

[N02] 排序（工程实践用内置实现）
来源：http://hpd.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://pfk.hysaishi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ljj.shzxlz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qrb.andypj.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://ihz.iojbl.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hci.hysaishi.cn

Go:   slices.Sort(arr)
来源：http://tog.yueranfly.top

Ruby: arr.sort
来源：http://fij.ivvv.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gxd.jyoumei.cn

[N03] 快速排序（分治示例）
来源：http://syi.ppjwa.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xlg.zhaomingkeji.xyz

PHP:  // 递归实现，或用 usort
来源：http://oop.jyoumei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mzb.zdqjudy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wnt.wangdashe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fnz.wangshuangyany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ltv.zhiwuduotai.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jlh.jianghu66.top

C#:   // 手写递归，或 Array.Sort
来源：http://pgf.sysykeji.top

[N04] 斐波那契数列
来源：http://dbh.dianchejie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://liw.bbcook.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://afn.jyoumei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uhw.daria6918.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://use.tarul.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gjt.feifeiyinyue.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rbp.ppjwa.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kbx.bbcook.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mjl.hnqzz.top

[N05] 最大公约数
来源：http://wpw.fanxiaobao.xyz

Py:   math.gcd(a, b)
来源：http://dkm.xziqi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bar.vqdsnc.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yqx.aizwys.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dls.sysykeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bse.uphjek.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zpl.shanyushiyangtech.top

Ruby: a.gcd(b)
来源：http://fwi.yj202588.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rhn.daxiang520.top

[N06] 判断回文字符串
来源：http://xel.cqqwz.cn

Py:   s == s[::-1]
来源：http://osf.chenzaomai.com

PHP:  $s === strrev($s);
来源：http://awv.chenjidiqi.icu

JS:   s === [...s].reverse().join("")
来源：http://lqv.jiagoushi.top

TS:   s === [...s].reverse().join("")
来源：http://rtg.yueranfly.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gyj.xinyue.icu

Go:   // 双指针从两端比较
来源：http://hms.c1oappe.top

Ruby: s == s.reverse
来源：http://wuh.ywan-chungtsiang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://sdi.aibaodan.cn

[N07] 两数之和（返回下标）
来源：http://cml.jiagoushi.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tzo.xuanzx.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xci.52xcode.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://iae.epnwcf.com

TS:   // 手写 Map<string, number>
来源：http://dlu.cashguo.top

Java: // 手写 HashMap
来源：http://udh.guannengcc.top

Go:   // 手写 map[int]int
来源：http://jib.redwolf501.top

Ruby: // 手写 Hash
来源：http://wdz.hnqzz.top

C#:   // 手写 Dictionary<int, int>
来源：http://bsl.aibaodan.cn

[N08] 生成全排列
来源：http://rud.xziqi.cn

Py:   itertools.permutations(arr)
来源：http://wmd.wangdashe.top

PHP:  // 手写递归交换
来源：http://iib.cashguo.top

JS:   // 手写回溯递归
来源：http://vql.hammf.cn

TS:   // 手写回溯递归
来源：http://bnc.fktsv.cn

Java: // 手写回溯递归
来源：http://zye.xuanzx.com

Go:   // 手写回溯递归
来源：http://ppl.jlsjyb.cn

Ruby: arr.permutation.to_a
来源：http://glp.tarul.cn

C#:   // 手写回溯递归
来源：http://ryp.tian-w.cn

[N09] 栈与队列
来源：http://esv.xuetiantiany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://icq.iojbl.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lxr.sufxvd.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wmd.nanxinkj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tqb.bbcook.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lea.hfpthk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zvh.zycfv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uam.kuanghao11.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ivo.yfazqb.com

[N10] 链表节点定义
来源：http://wgq.ivvv.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sio.hywenlv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nqr.yfazqb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xos.aibaodan.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tfk.gotoacloud.top

Java: class Node { int v; Node next; }
来源：http://hti.snrcjt.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hkn.wangshuangyany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://evy.ybcxt.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ndg.c1oappe.top

[N11] 二叉树中序遍历
来源：http://lmm.shuidangran.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rch.daria6918.cn

PHP:  // 手写递归函数
来源：http://phl.xziqi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gpa.nwbrower.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fid.yj202588.top

Java: // 手写递归
来源：http://lvr.iojbl.cn

Go:   // 手写递归
来源：http://wfm.xingfuxueyuan.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dqt.ybcxt.top

C#:   // 手写递归
来源：http://rbx.yj20258.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pfu.hnqzz.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xyn.dashuyun.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dxo.uphjek.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://taf.yvedp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oev.yj20258888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zig.yanxiufei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://otl.jianghu66.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jlo.yfazqb.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uli.hammf.cn

================================================================================
来源：http://sti.hongshengwenyu.top

O. 并发与异步
来源：http://vha.fzhhl.top

================================================================================
来源：http://ppz.quarkkingdee.top

[O01] 启动一个线程
来源：http://zdc.zhaomingkeji.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bmx.c1oappe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jee.havefunace.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wsp.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://fyh.ctjpmb.com

Java: new Thread(() -> f()).start()
来源：http://yny.pengpengdd.cyou

Go:   go f()
来源：http://jcg.zhaomingkeji.xyz

Ruby: Thread.new { f }
来源：http://sor.birdmap.top

C#:   Task.Run(() => F());
来源：http://zwz.xziqi.cn

[O02] 使用线程池
来源：http://rjz.hnxiangtu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zgf.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xrp.jlsjyb.cn

JS:   // worker_threads 线程池
来源：http://xcv.epnwcf.com

TS:   // worker_threads 线程池
来源：http://hvu.cashguo.top

Java: Executors.newFixedThreadPool(4)
来源：http://kly.havefunace.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lhq.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hdk.gzhubu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mxe.gzhubu.top

[O03] 加锁保护共享数据
来源：http://zfx.zycfv.cn

Py:   with lock: shared += 1
来源：http://eyt.52xcode.cn

PHP:  // 用 flock() 做文件锁
来源：http://fno.redwolf501.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vwq.sweek.top

TS:   // 同 JS
来源：http://bfh.nwbrower.top

Java: synchronized (this) { shared++; }
来源：http://dkd.yuanzhike.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kzj.hfpthk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nqq.ctjpmb.com

C#:   lock (gate) { shared++; }
来源：http://thg.aizwys.cn

[O04] 定义异步函数并等待
来源：http://hen.zhaomingkeji.xyz

Py:   async def f():⏎    await g()
来源：http://jad.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sji.316326.xyz

JS:   async function f() { await g(); }
来源：http://hsl.meibo888.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lgw.uphjek.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xxc.316326.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sfv.fengsongda.top

Ruby: # 用 Fiber 或 async gem
来源：http://cun.yuxming.cn

C#:   async Task F() { await G(); }
来源：http://rdi.fanxiaobao.xyz

[O05] 并发执行并等待全部完成
来源：http://url.yueranfly.top

Py:   asyncio.gather(*tasks)
来源：http://uma.gaohongyu789.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rbc.jinghuilouyu.cn

JS:   await Promise.all(tasks)
来源：http://bno.ydzc1.top

TS:   await Promise.all(tasks)
来源：http://map.gaohongyu789.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iwg.iojbl.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kgi.xylfe.cn

Ruby: threads.map(&:join)
来源：http://awb.jinyuanbaomall.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jvo.dashuyun.cn

[O06] 使用进程池
来源：http://gfu.hywenlv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mqc.fanxiaobao.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://gfu.havefunace.top

JS:   // child_process / cluster 模块
来源：http://zki.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://vws.cucudq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gid.ydzc1.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wuf.bbcook.cn

Ruby: // fork 块
来源：http://tak.zhaomingkeji.xyz

C#:   Parallel.For
来源：http://vex.yangfankeji.com

================================================================================
来源：http://xba.snrcjt.cn

P. 常用工具函数
来源：http://amq.fktsv.cn

================================================================================
来源：http://sfd.sweek.top


<!-- 参考信息 -->