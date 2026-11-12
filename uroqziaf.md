代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://nlt.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zog.jianghu66.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://azc.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vky.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://glk.guannengcc.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bvn.yangfankeji.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cxi.epnwcf.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mme.9152youxi.cn

[L03] 设置自定义请求头
来源：http://acj.zhiwuduotai.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jrx.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xqv.yfazqb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hcj.shzxlz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oso.hysaishi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gqh.yanxiufei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://phy.hammf.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hhe.cdnleiting.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pxm.jqgfzy.top

[L04] 设置超时
来源：http://rmi.ydjk.org.cn

Py:   requests.get(url, timeout=5)
来源：http://ibr.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pbd.hcnkem.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ptd.zhoulong.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xcl.shangyingyoupin.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://abp.shanyushiyangtech.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kiy.hongshengwenyu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pir.jlsjyb.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lyd.xylfe.cn

[L05] 上传文件（multipart）
来源：http://hul.snrcjt.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://llc.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hzo.hysaishi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xlo.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ibu.ehwqpu.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eol.cashguo.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ccw.haohaochexian.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fya.tian-w.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uiv.wangshuangyany.cn

[L06] 解析响应为 JSON
来源：http://eee.tarul.cn

Py:   resp.json()
来源：http://pws.cdnleiting.top

PHP:  json_decode($body, true);
来源：http://fhy.ivvv.top

JS:   await resp.json()
来源：http://pfg.gaohongyu789.top

TS:   await resp.json()
来源：http://zcb.cdnleiting.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kri.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ilf.zhaomingkeji.xyz

Ruby: JSON.parse(resp.body)
来源：http://aim.52xcode.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ypf.fengsongda.top

[L07] 处理 HTTP 状态码
来源：http://vzu.fanxiaobao.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fot.daxiang520.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yye.yj20258888.top

JS:   resp.ok;  resp.status
来源：http://soc.cdnleiting.top

TS:   resp.ok;  resp.status
来源：http://pgn.hysaishi.cn

Java: resp.statusCode()
来源：http://roy.zhixingplan.top

Go:   resp.StatusCode
来源：http://qke.fzhhl.top

Ruby: resp.code.to_i
来源：http://kwu.pengpengdd.cyou

C#:   (int)resp.StatusCode
来源：http://xnc.yj20258.top

[L08] 并发请求多个地址
来源：http://hsd.yongpay.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wop.xziqi.cn

PHP:  curl_multi_init() 系列
来源：http://lnc.kuanghao11.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xto.9152youxi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://asx.xylfe.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xvc.gogol.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ybr.0kj1m.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mbp.ppjwa.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hpj.haohaochexian.top

================================================================================
来源：http://chz.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://gmr.cucudq.cn

================================================================================
来源：http://est.yfazqb.com

[M01] 读取命令行参数
来源：http://rsn.xylfe.cn

Py:   sys.argv[1:]
来源：http://trp.shanyushiyangtech.top

PHP:  $argv;  $argc;
来源：http://pgh.gaohongyu789.top

JS:   process.argv.slice(2)
来源：http://hzl.aizwys.cn

TS:   process.argv.slice(2)
来源：http://qxb.haohaochexian.top

Java: args 数组（main 方法参数）
来源：http://zry.zdbjq.cn

Go:   os.Args[1:]
来源：http://tha.zhoulong.xyz

Ruby: ARGV
来源：http://oav.dianchejie.cn

C#:   args 数组（Main 方法参数）
来源：http://csu.pengpengdd.cyou

[M02] 读取环境变量
来源：http://ycs.fengsongda.top

Py:   os.environ.get("HOME")
来源：http://kuh.svipenyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gup.shangyingyoupin.top

JS:   process.env.HOME
来源：http://all.ivvv.top

TS:   process.env.HOME
来源：http://dwv.xuetiantiany.cn

Java: System.getenv("HOME")
来源：http://tlj.zycfv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qze.iojbl.cn

Ruby: ENV["HOME"]
来源：http://zmw.jinyuanbaomall.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ojj.daxiang520.top

[M03] 执行外部命令
来源：http://gyd.aibaodan.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ydx.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mau.quarkkingdee.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kln.316326.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://ved.shanyushiyangtech.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eyu.aizwys.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vok.fanxiaobao.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://gsx.shzxlz.cn

C#:   Process.Start("ls", "-l");
来源：http://fkx.hywenlv.cn

[M04] 获取当前工作目录
来源：http://fyo.xingfuxueyuan.xyz

Py:   os.getcwd()
来源：http://efm.redwolf501.top

PHP:  getcwd();
来源：http://tpq.fanxiaobao.xyz

JS:   process.cwd()
来源：http://nui.yuanzhike.top

TS:   process.cwd()
来源：http://srk.ehwqpu.com

Java: Path.of("").toAbsolutePath()
来源：http://hsl.fktsv.cn

Go:   os.Getwd()
来源：http://ksf.hammf.cn

Ruby: Dir.pwd
来源：http://gql.yongpay.top

C#:   Directory.GetCurrentDirectory()
来源：http://zka.epnwcf.com

[M05] 设置退出码
来源：http://dbx.zdbjq.cn

Py:   sys.exit(1)
来源：http://miu.zhijiandao.cn

PHP:  exit(1);
来源：http://xpa.ctjpmb.com

JS:   process.exit(1)
来源：http://rwj.zhijiandao.cn

TS:   process.exit(1)
来源：http://bqi.zdqjudy.top

Java: System.exit(1)
来源：http://wgm.sufxvd.cn

Go:   os.Exit(1)
来源：http://vwp.sysykeji.top

Ruby: exit 1
来源：http://wcw.gogol.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://laj.zhongyouzk.top

[M06] 向标准错误输出
来源：http://nkb.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://qsr.gaohongyu789.top

PHP:  fwrite(STDERR, "err\n");
来源：http://apo.jianghu66.top

JS:   console.error("err")
来源：http://gim.guowangkeji.top

TS:   console.error("err")
来源：http://wej.guowangkeji.top

Java: System.err.println("err")
来源：http://mmg.fzhhl.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://aip.kuanghao11.cn

Ruby: warn "err"
来源：http://djb.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://rtq.fzhhl.top

[M07] 判断是否为主入口
来源：http://ufb.yj20258888.top

Py:   if __name__ == "__main__":
来源：http://dny.svipenyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://alh.hywenlv.cn

JS:   require.main === module
来源：http://ihc.zycfv.cn

TS:   require.main === module
来源：http://qzt.jiagoushi.top

Java: public static void main(String[] args)
来源：http://thz.aizwys.cn

Go:   func main()
来源：http://apt.svipenyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://brh.sjlbkw.cn

C#:   static void Main(string[] args)
来源：http://cys.wangshuangyany.cn

[M08] 获取系统与运行时信息
来源：http://lns.dianchejie.cn

Py:   platform.system();  platform.python_version()
来源：http://dqn.sufxvd.cn

PHP:  PHP_OS;  phpversion();
来源：http://esq.birdmap.top

JS:   process.platform;  process.version
来源：http://tzh.epnwcf.com

TS:   process.platform;  process.version
来源：http://uth.hnqzz.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ciu.cheryme.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xfn.shanyushiyangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bir.xuanzx.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://niv.gaohongyu789.top

================================================================================
来源：http://rvb.yuxming.cn

N. 数据结构与算法
来源：http://lwm.yvedp.cn

================================================================================
来源：http://edu.sysykeji.top

[N01] 二分查找（有序数组）
来源：http://bhd.gogol.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bxj.fktsv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ikv.hcnkem.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ldu.yangfankeji.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pil.jqgfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://zzw.tian-w.cn

Go:   sort.SearchInts(arr, x)
来源：http://dho.xinyue.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://vul.hnqzz.top

C#:   Array.BinarySearch(arr, x)
来源：http://ykt.zdqjudy.top

[N02] 排序（工程实践用内置实现）
来源：http://pkt.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://das.meibo888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ekb.ywan-chungtsiang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bzp.fanxiaobao.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://ori.gogol.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mjz.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://dyg.ivvv.top

Ruby: arr.sort
来源：http://xbq.yj20258.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dgl.bbcook.cn

[N03] 快速排序（分治示例）
来源：http://rse.fktsv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rox.yanxiufei.cn

PHP:  // 递归实现，或用 usort
来源：http://kja.tanke756.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ccc.zhixingplan.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jnn.meibo888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gka.sjlbkw.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uth.sxryk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://knk.jiagoushi.top

C#:   // 手写递归，或 Array.Sort
来源：http://cpl.hcnkem.com

[N04] 斐波那契数列
来源：http://hys.hnxiangtu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hyo.gotoacloud.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lrn.hesvh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xjj.cucudq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ebx.zhaomingkeji.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kyt.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fjf.jyoumei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vku.hfpthk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://esi.pengpengdd.cyou

[N05] 最大公约数
来源：http://dqu.sysykeji.top

Py:   math.gcd(a, b)
来源：http://lrx.fehbvm.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hlg.zycfv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bxb.tanke756.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lep.ehwqpu.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hul.yangfankeji.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lch.ppjwa.cn

Ruby: a.gcd(b)
来源：http://qes.ehwqpu.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qos.dianchejie.cn

[N06] 判断回文字符串
来源：http://qnc.hammf.cn

Py:   s == s[::-1]
来源：http://bia.ctjpmb.com

PHP:  $s === strrev($s);
来源：http://mxz.gotoacloud.top

JS:   s === [...s].reverse().join("")
来源：http://rky.birdmap.top

TS:   s === [...s].reverse().join("")
来源：http://unh.gzhubu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://epe.jqgfzy.top

Go:   // 双指针从两端比较
来源：http://etk.haohaochexian.top

Ruby: s == s.reverse
来源：http://num.hongshengwenyu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vuc.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://kcv.cqqwz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://joa.shzxlz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mcq.jlsjyb.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gep.zhoulong.xyz

TS:   // 手写 Map<string, number>
来源：http://hbr.cdnleiting.top

Java: // 手写 HashMap
来源：http://exg.fanxiaobao.xyz

Go:   // 手写 map[int]int
来源：http://spi.sxryk.cn

Ruby: // 手写 Hash
来源：http://mvr.redwolf501.top

C#:   // 手写 Dictionary<int, int>
来源：http://cia.haohaochexian.top

[N08] 生成全排列
来源：http://ywm.dashuyun.cn

Py:   itertools.permutations(arr)
来源：http://yeu.xziqi.cn

PHP:  // 手写递归交换
来源：http://umh.smart0.xyz

JS:   // 手写回溯递归
来源：http://llb.zhixingplan.top

TS:   // 手写回溯递归
来源：http://mjm.dashuyun.cn

Java: // 手写回溯递归
来源：http://uga.tianlin.xyz

Go:   // 手写回溯递归
来源：http://ula.tarul.cn

Ruby: arr.permutation.to_a
来源：http://crd.zhiwuduotai.top

C#:   // 手写回溯递归
来源：http://qva.mhx1999.top

[N09] 栈与队列
来源：http://jin.shangyingyoupin.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bjr.nwbrower.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nqx.zhongyouzk.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dfa.haohaochexian.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zpe.yueranfly.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nil.jyoumei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zza.cqqwz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xke.quarkkingdee.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dmm.cashguo.top

[N10] 链表节点定义
来源：http://wss.jianghu66.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mgs.ydzc1.top

PHP:  class Node { public $v; public $next = null; }
来源：http://eqi.sysykeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lsz.shanyushiyangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wff.tarul.cn

Java: class Node { int v; Node next; }
来源：http://xrg.fehbvm.com

Go:   type Node struct { V int; Next *Node }
来源：http://nbm.birdmap.top

Ruby: Node = Struct.new(:v, :next)
来源：http://blr.shangyingyoupin.top

C#:   class Node { public int V; public Node? Next; }
来源：http://aeb.fehbvm.com

[N11] 二叉树中序遍历
来源：http://nzu.dashuyun.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://taw.gogol.net.cn

PHP:  // 手写递归函数
来源：http://rpx.chenlongwang.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uiu.gotoacloud.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mbi.yueranfly.top

Java: // 手写递归
来源：http://efx.zhijiandao.cn

Go:   // 手写递归
来源：http://qkv.ctjpmb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ojl.9152youxi.cn

C#:   // 手写递归
来源：http://ean.316326.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vpf.dashuyun.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fyk.aizwys.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nto.yueranfly.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wph.fktsv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gqu.316326.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tyn.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://naj.c1oappe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pnx.havefunace.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hrl.sweek.top

================================================================================
来源：http://afx.bjfxy.top

O. 并发与异步
来源：http://laz.fzhhl.top

================================================================================
来源：http://jmv.jiagoushi.top

[O01] 启动一个线程
来源：http://kqv.fengsongda.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ttj.mhx1999.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kjc.smart0.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pun.havefunace.top

TS:   // 同 JS
来源：http://qif.jinyuanbaomall.cn

Java: new Thread(() -> f()).start()
来源：http://thi.tarul.cn

Go:   go f()
来源：http://wqd.zhoulong.xyz

Ruby: Thread.new { f }
来源：http://cjr.iojbl.cn

C#:   Task.Run(() => F());
来源：http://gxn.xinyue.icu

[O02] 使用线程池
来源：http://fsz.chenlongwang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://skd.fanxiaobao.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bjv.zhengqikj.top

JS:   // worker_threads 线程池
来源：http://bsf.c1oappe.top

TS:   // worker_threads 线程池
来源：http://lqg.zhengqikj.top

Java: Executors.newFixedThreadPool(4)
来源：http://luj.svipenyu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iay.vqdsnc.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xmw.pycfn.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pbl.vehdjk.com

[O03] 加锁保护共享数据
来源：http://bye.fanxiaobao.xyz

Py:   with lock: shared += 1
来源：http://jqo.hnxiangtu.top

PHP:  // 用 flock() 做文件锁
来源：http://arc.aizwys.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rau.ybcxt.top

TS:   // 同 JS
来源：http://wfl.0kj1m.cn

Java: synchronized (this) { shared++; }
来源：http://cuq.ybcxt.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jdu.gaohongyu789.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jks.nwbrower.top

C#:   lock (gate) { shared++; }
来源：http://ffk.jiagoushi.top

[O04] 定义异步函数并等待
来源：http://kkx.jinqigufen.top

Py:   async def f():⏎    await g()
来源：http://tvp.hywenlv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ndb.daria6918.cn

JS:   async function f() { await g(); }
来源：http://rjy.ydzc1.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qyn.chenjidiqi.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jnm.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tsq.daxiang520.top

Ruby: # 用 Fiber 或 async gem
来源：http://eos.wangshuangyany.cn

C#:   async Task F() { await G(); }
来源：http://dhh.tarul.cn

[O05] 并发执行并等待全部完成
来源：http://mhs.sweek.top

Py:   asyncio.gather(*tasks)
来源：http://iom.redwolf501.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jzk.guannengcc.top

JS:   await Promise.all(tasks)
来源：http://uin.daria6918.cn

TS:   await Promise.all(tasks)
来源：http://abc.yuanzhike.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mue.tianlin.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qyu.shzxlz.cn

Ruby: threads.map(&:join)
来源：http://mdg.0kj1m.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://odl.dashuyun.cn

[O06] 使用进程池
来源：http://yvj.meibo888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://akg.redwolf501.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fmc.yueranfly.top

JS:   // child_process / cluster 模块
来源：http://tiq.jinqigufen.top


<!-- 参考信息 -->