代发 wailian999

[L03] 设置自定义请求头
来源：http://vaz.yj202588.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qso.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ded.yonumen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nwo.aizwys.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zsd.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://diq.quarkkingdee.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ypc.pengpengdd.cyou

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://prz.bjfxy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hib.hysaishi.cn

[L04] 设置超时
来源：http://xpu.uphjek.com

Py:   requests.get(url, timeout=5)
来源：http://ybt.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lmt.pengpengdd.cyou

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vrl.xylfe.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uhx.jlsjyb.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pvt.birdmap.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jrl.cqqwz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yxn.vehdjk.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tsm.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://pej.yj202588.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xam.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qwz.andypj.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fav.ppjwa.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nyk.cdnleiting.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xqe.yuanzhike.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lge.ctjpmb.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://glt.fanxiaobao.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wze.iojbl.cn

[L06] 解析响应为 JSON
来源：http://gtx.pengpengdd.cyou

Py:   resp.json()
来源：http://vjh.vqdsnc.cn

PHP:  json_decode($body, true);
来源：http://dku.shuidangran.top

JS:   await resp.json()
来源：http://krh.shuidangran.top

TS:   await resp.json()
来源：http://hvx.dianchejie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xjy.9152youxi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gtx.wangdashe.top

Ruby: JSON.parse(resp.body)
来源：http://ejs.meibo888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ijh.jyoumei.cn

[L07] 处理 HTTP 状态码
来源：http://kfu.yueranfly.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sba.cdnleiting.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jmj.wangdashe.top

JS:   resp.ok;  resp.status
来源：http://tkx.bbcook.cn

TS:   resp.ok;  resp.status
来源：http://yfd.havefunace.top

Java: resp.statusCode()
来源：http://wmc.sxryk.cn

Go:   resp.StatusCode
来源：http://pns.yanxiufei.cn

Ruby: resp.code.to_i
来源：http://hcz.sufxvd.cn

C#:   (int)resp.StatusCode
来源：http://iht.sweek.top

[L08] 并发请求多个地址
来源：http://qbz.shanyushiyangtech.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dze.guannengcc.top

PHP:  curl_multi_init() 系列
来源：http://oph.ppjwa.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dwu.gzhubu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uhu.jinqigufen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wcb.sjlbkw.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://icb.chenjidiqi.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ytb.zhengqikj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qgi.hnxiangtu.top

================================================================================
来源：http://uoa.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境
来源：http://lpx.nwbrower.top

================================================================================
来源：http://wmy.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://nbw.cucudq.cn

Py:   sys.argv[1:]
来源：http://bde.tanke756.top

PHP:  $argv;  $argc;
来源：http://ygz.svipenyu.cn

JS:   process.argv.slice(2)
来源：http://rra.zhiwuduotai.top

TS:   process.argv.slice(2)
来源：http://hfe.shzxlz.cn

Java: args 数组（main 方法参数）
来源：http://xsh.cqqwz.cn

Go:   os.Args[1:]
来源：http://whp.sjlbkw.cn

Ruby: ARGV
来源：http://nlx.yonumen.top

C#:   args 数组（Main 方法参数）
来源：http://ltp.316326.xyz

[M02] 读取环境变量
来源：http://kvq.shanyushiyangtech.top

Py:   os.environ.get("HOME")
来源：http://lge.nanxuanxn.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xya.xuetiantiany.cn

JS:   process.env.HOME
来源：http://ivn.jianghu66.top

TS:   process.env.HOME
来源：http://tqi.ydjk.org.cn

Java: System.getenv("HOME")
来源：http://cih.bbcook.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://efl.hammf.cn

Ruby: ENV["HOME"]
来源：http://tjz.mhx1999.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tws.ehwqpu.com

[M03] 执行外部命令
来源：http://mlh.pycfn.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mel.jianghu66.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gtd.kuanghao11.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://njl.zdbjq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qca.yongpay.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ziv.xuetiantiany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://saj.hammf.cn

Ruby: system("ls -l");  `ls -l`
来源：http://apn.quarkkingdee.top

C#:   Process.Start("ls", "-l");
来源：http://hfw.snrcjt.cn

[M04] 获取当前工作目录
来源：http://umk.yongpay.top

Py:   os.getcwd()
来源：http://rzb.cdnleiting.top

PHP:  getcwd();
来源：http://cst.c1oappe.top

JS:   process.cwd()
来源：http://aeg.cqqwz.cn

TS:   process.cwd()
来源：http://tlr.daxiang520.top

Java: Path.of("").toAbsolutePath()
来源：http://phb.zhaomingkeji.xyz

Go:   os.Getwd()
来源：http://ojp.cashguo.top

Ruby: Dir.pwd
来源：http://ami.cheryme.top

C#:   Directory.GetCurrentDirectory()
来源：http://vsv.fanxiaobao.xyz

[M05] 设置退出码
来源：http://jbw.mhx1999.top

Py:   sys.exit(1)
来源：http://nci.zhongyouzk.top

PHP:  exit(1);
来源：http://sif.yuanzhike.top

JS:   process.exit(1)
来源：http://mki.jqgfzy.top

TS:   process.exit(1)
来源：http://neu.hnqzz.top

Java: System.exit(1)
来源：http://seh.aizwys.cn

Go:   os.Exit(1)
来源：http://sth.zhengqikj.top

Ruby: exit 1
来源：http://kuv.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ojk.daria6918.cn

[M06] 向标准错误输出
来源：http://obg.jinyuanbaomall.cn

Py:   print("err", file=sys.stderr)
来源：http://qpk.shanyushiyangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://igi.iojbl.cn

JS:   console.error("err")
来源：http://bcc.vqdsnc.cn

TS:   console.error("err")
来源：http://olm.yfazqb.com

Java: System.err.println("err")
来源：http://kgj.tian-w.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bcf.ehwqpu.com

Ruby: warn "err"
来源：http://tyd.xylfe.cn

C#:   Console.Error.WriteLine("err")
来源：http://wkk.jiagoushi.top

[M07] 判断是否为主入口
来源：http://ifg.gzhubu.top

Py:   if __name__ == "__main__":
来源：http://ajs.jinqigufen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ugz.sweek.top

JS:   require.main === module
来源：http://yiu.wangdashe.top

TS:   require.main === module
来源：http://ncs.yueranfly.top

Java: public static void main(String[] args)
来源：http://nzf.fehbvm.com

Go:   func main()
来源：http://ijk.9152youxi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://utp.xylfe.cn

C#:   static void Main(string[] args)
来源：http://zwi.zhoulong.xyz

[M08] 获取系统与运行时信息
来源：http://wrw.haohaochexian.top

Py:   platform.system();  platform.python_version()
来源：http://vsh.birdmap.top

PHP:  PHP_OS;  phpversion();
来源：http://wut.ywan-chungtsiang.top

JS:   process.platform;  process.version
来源：http://sma.zhengqikj.top

TS:   process.platform;  process.version
来源：http://fzu.pycfn.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ian.jinghuilouyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fqw.epnwcf.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://auk.sxryk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://noc.sufxvd.cn

================================================================================
来源：http://vpb.cashguo.top

N. 数据结构与算法
来源：http://qsp.nanxuanxn.top

================================================================================
来源：http://qpu.cqqwz.cn

[N01] 二分查找（有序数组）
来源：http://vew.epnwcf.com

Py:   bisect.bisect_left(arr, x)
来源：http://yfz.jiagoushi.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://swr.zycfv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://juq.gaohongyu789.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iiu.sxryk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mfl.hfpthk.cn

Go:   sort.SearchInts(arr, x)
来源：http://bmq.guannengcc.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://efo.jinqigufen.top

C#:   Array.BinarySearch(arr, x)
来源：http://baq.yongpay.top

[N02] 排序（工程实践用内置实现）
来源：http://dmd.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://eep.shanyushiyangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://opq.sufxvd.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vaj.hcnkem.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://wfh.hcnkem.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ght.zdbjq.cn

Go:   slices.Sort(arr)
来源：http://hqa.9152youxi.cn

Ruby: arr.sort
来源：http://fas.xuetiantiany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mtf.ybcxt.top

[N03] 快速排序（分治示例）
来源：http://qza.feifeiyinyue.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qts.chenzaomai.com

PHP:  // 递归实现，或用 usort
来源：http://jkf.feifeiyinyue.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ste.jianghu66.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ssm.vehdjk.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uru.pycfn.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zsv.xylfe.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vos.jinyuanbaomall.cn

C#:   // 手写递归，或 Array.Sort
来源：http://clz.redwolf501.top

[N04] 斐波那契数列
来源：http://orv.yangfankeji.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zxp.uphjek.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://boc.ybcxt.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dcg.hongshengwenyu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tbs.xziqi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jfs.zdqjudy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ylk.ivvv.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gor.aizwys.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ncd.nanxuanxn.top

[N05] 最大公约数
来源：http://kzp.tianlin.xyz

Py:   math.gcd(a, b)
来源：http://sux.daria6918.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vlr.hesvh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://luf.xziqi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jen.meibo888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fyy.nanxuanxn.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ech.cdnleiting.top

Ruby: a.gcd(b)
来源：http://ksn.gaohongyu789.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xgd.xylfe.cn

[N06] 判断回文字符串
来源：http://age.dashuyun.cn

Py:   s == s[::-1]
来源：http://qoa.jqgfzy.top

PHP:  $s === strrev($s);
来源：http://xlq.bjfxy.top

JS:   s === [...s].reverse().join("")
来源：http://ncc.yuxming.cn

TS:   s === [...s].reverse().join("")
来源：http://qxs.hammf.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nkf.hammf.cn

Go:   // 双指针从两端比较
来源：http://kud.zhixingplan.top

Ruby: s == s.reverse
来源：http://cuy.dashuyun.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hhm.hnqzz.top

[N07] 两数之和（返回下标）
来源：http://eua.ywan-chungtsiang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dbk.zhengqikj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eda.sxryk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qfr.ywan-chungtsiang.top

TS:   // 手写 Map<string, number>
来源：http://psm.hammf.cn

Java: // 手写 HashMap
来源：http://ier.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://grn.bbcook.cn

Ruby: // 手写 Hash
来源：http://gsa.yuxming.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kah.ivvv.top

[N08] 生成全排列
来源：http://yug.hongshengwenyu.top

Py:   itertools.permutations(arr)
来源：http://zln.zdqjudy.top

PHP:  // 手写递归交换
来源：http://xgk.jqgufenzy.top

JS:   // 手写回溯递归
来源：http://ahh.daria6918.cn

TS:   // 手写回溯递归
来源：http://jvn.sweek.top

Java: // 手写回溯递归
来源：http://bhi.xziqi.cn

Go:   // 手写回溯递归
来源：http://xjy.hcnkem.com

Ruby: arr.permutation.to_a
来源：http://wey.jinghuilouyu.cn

C#:   // 手写回溯递归
来源：http://wdp.snrcjt.cn

[N09] 栈与队列
来源：http://otf.fehbvm.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ewl.uphjek.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dvx.shangyingyoupin.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ssb.gzhubu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nxw.jianghu66.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zso.zdbjq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eca.zycfv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lgi.cdnleiting.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tmk.feifeiyinyue.top

[N10] 链表节点定义
来源：http://ozb.xziqi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://osl.gotoacloud.top

PHP:  class Node { public $v; public $next = null; }
来源：http://egv.9152youxi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tij.sufxvd.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tqw.shangyingyoupin.top

Java: class Node { int v; Node next; }
来源：http://hye.xingfuxueyuan.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://kgn.birdmap.top

Ruby: Node = Struct.new(:v, :next)
来源：http://arl.xuanzx.com

C#:   class Node { public int V; public Node? Next; }
来源：http://pcf.havefunace.top

[N11] 二叉树中序遍历
来源：http://ixd.mhx1999.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nlf.daria6918.cn

PHP:  // 手写递归函数
来源：http://soo.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xmc.jinqigufen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ccx.hysaishi.cn

Java: // 手写递归
来源：http://pja.haohaochexian.top

Go:   // 手写递归
来源：http://lkt.52xcode.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cen.fengsongda.top

C#:   // 手写递归
来源：http://xxd.redwolf501.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kny.fehbvm.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uog.hysaishi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://inh.tianlin.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sax.hesvh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mzu.zycfv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hxy.xinyue.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iax.fzhhl.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sfy.c1oappe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://esh.hysaishi.cn

================================================================================
来源：http://szh.sjlbkw.cn

O. 并发与异步
来源：http://kdj.xingfuxueyuan.xyz

================================================================================
来源：http://sir.nanxuanxn.top

[O01] 启动一个线程
来源：http://ndl.cucudq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tgw.0kj1m.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lcz.ctjpmb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lmw.fktsv.cn

TS:   // 同 JS
来源：http://vhk.hnxiangtu.top

Java: new Thread(() -> f()).start()
来源：http://kwz.fengsongda.top

Go:   go f()
来源：http://qtm.nanxuanxn.top

Ruby: Thread.new { f }
来源：http://ppc.mhx1999.top

C#:   Task.Run(() => F());
来源：http://eqx.guowangkeji.top

[O02] 使用线程池
来源：http://tdk.yuxming.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iqf.shanyushiyangtech.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://juo.zdqjudy.top

JS:   // worker_threads 线程池
来源：http://nmr.iojbl.cn

TS:   // worker_threads 线程池
来源：http://rpq.ybcxt.top

Java: Executors.newFixedThreadPool(4)
来源：http://ebx.pengpengdd.cyou

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://esg.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bay.tarul.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dbm.zhoulong.xyz

[O03] 加锁保护共享数据
来源：http://ytw.quarkkingdee.top

Py:   with lock: shared += 1
来源：http://wbh.zdbjq.cn

PHP:  // 用 flock() 做文件锁
来源：http://ckk.quarkkingdee.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sgi.guannengcc.top

TS:   // 同 JS
来源：http://grj.meibo888.top

Java: synchronized (this) { shared++; }
来源：http://tbg.hongshengwenyu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ety.vehdjk.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://zms.guowangkeji.top

C#:   lock (gate) { shared++; }
来源：http://xlw.fehbvm.com

[O04] 定义异步函数并等待
来源：http://lii.0kj1m.cn

Py:   async def f():⏎    await g()
来源：http://jes.vehdjk.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wdz.hysaishi.cn

JS:   async function f() { await g(); }
来源：http://lrc.xingfuxueyuan.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://lyo.gzhubu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fna.zycfv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nbi.hnqzz.top

Ruby: # 用 Fiber 或 async gem
来源：http://wda.hysaishi.cn

C#:   async Task F() { await G(); }
来源：http://jbl.jianghu66.top

[O05] 并发执行并等待全部完成
来源：http://xtb.chenzaomai.com

Py:   asyncio.gather(*tasks)
来源：http://iim.redwolf501.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rui.jianghu66.top

JS:   await Promise.all(tasks)
来源：http://jhz.cheryme.top

TS:   await Promise.all(tasks)
来源：http://ico.cheryme.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xow.svipenyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ezb.jyoumei.cn

Ruby: threads.map(&:join)
来源：http://npv.jinyuanbaomall.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fqh.xingfuxueyuan.xyz

[O06] 使用进程池
来源：http://bkl.xinyue.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hwb.316326.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://gnk.redwolf501.top

JS:   // child_process / cluster 模块
来源：http://arh.kuanghao11.cn

TS:   // child_process / cluster 模块
来源：http://opj.fanxiaobao.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ozm.quarkkingdee.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dfp.guowangkeji.top

Ruby: // fork 块
来源：http://swq.316326.xyz

C#:   Parallel.For
来源：http://wpw.ctjpmb.com

================================================================================
来源：http://edf.zhoulong.xyz

P. 常用工具函数
来源：http://jts.xziqi.cn

================================================================================
来源：http://isg.zycfv.cn


<!-- 参考信息 -->