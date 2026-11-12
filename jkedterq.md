代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://axu.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dyc.wangshuangyany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wda.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yce.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vaq.ydjk.org.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://byk.feifeiyinyue.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kpb.yueranfly.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zia.gotoacloud.top

[L03] 设置自定义请求头
来源：http://hjr.nanxinkj.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qxx.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mep.uphjek.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ved.cqqwz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eyq.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lbv.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://glt.yvedp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ihl.hongshengwenyu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://izq.cashguo.top

[L04] 设置超时
来源：http://czs.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://rjn.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://llh.daxiang520.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zmi.52xcode.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://udv.hesvh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ilo.aizwys.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nmb.vehdjk.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rty.sweek.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jaz.shzxlz.cn

[L05] 上传文件（multipart）
来源：http://xwu.daxiang520.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ppg.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jho.ywan-chungtsiang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cuj.tanke756.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qtv.mhx1999.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ekz.yvedp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gdf.0kj1m.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://epn.birdmap.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qkv.fanxiaobao.xyz

[L06] 解析响应为 JSON
来源：http://sav.dianchejie.cn

Py:   resp.json()
来源：http://dqs.kuanghao11.cn

PHP:  json_decode($body, true);
来源：http://udd.ehwqpu.com

JS:   await resp.json()
来源：http://ysi.ehwqpu.com

TS:   await resp.json()
来源：http://alc.yanxiufei.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dub.havefunace.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nuz.xingfuxueyuan.xyz

Ruby: JSON.parse(resp.body)
来源：http://ozm.snrcjt.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lou.gaohongyu789.top

[L07] 处理 HTTP 状态码
来源：http://yah.redwolf501.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uwi.zhijiandao.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zen.pengpengdd.cyou

JS:   resp.ok;  resp.status
来源：http://fgp.zdqjudy.top

TS:   resp.ok;  resp.status
来源：http://xch.yvedp.cn

Java: resp.statusCode()
来源：http://srl.hcnkem.com

Go:   resp.StatusCode
来源：http://uob.daria6918.cn

Ruby: resp.code.to_i
来源：http://ond.jinghuilouyu.cn

C#:   (int)resp.StatusCode
来源：http://ivi.dianchejie.cn

[L08] 并发请求多个地址
来源：http://jvv.yonumen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bsn.bbcook.cn

PHP:  curl_multi_init() 系列
来源：http://cke.gzhubu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ymd.hcnkem.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fnr.zhiwuduotai.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ftd.yj20258888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ndi.daxiang520.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jju.316326.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lch.epnwcf.com

================================================================================
来源：http://fsn.iojbl.cn

M. 命令行 / 进程 / 环境
来源：http://oty.hammf.cn

================================================================================
来源：http://gee.cucudq.cn

[M01] 读取命令行参数
来源：http://ydl.ywan-chungtsiang.top

Py:   sys.argv[1:]
来源：http://baf.316326.xyz

PHP:  $argv;  $argc;
来源：http://gfj.hysaishi.cn

JS:   process.argv.slice(2)
来源：http://zzz.zhixingplan.top

TS:   process.argv.slice(2)
来源：http://amy.xylfe.cn

Java: args 数组（main 方法参数）
来源：http://gzt.wangdashe.top

Go:   os.Args[1:]
来源：http://juk.hammf.cn

Ruby: ARGV
来源：http://tyt.hnqzz.top

C#:   args 数组（Main 方法参数）
来源：http://wge.gogol.net.cn

[M02] 读取环境变量
来源：http://vkb.cashguo.top

Py:   os.environ.get("HOME")
来源：http://tek.hfpthk.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bhu.jinyuanbaomall.cn

JS:   process.env.HOME
来源：http://kmb.yfazqb.com

TS:   process.env.HOME
来源：http://anq.9152youxi.cn

Java: System.getenv("HOME")
来源：http://nir.bjfxy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rdy.ehwqpu.com

Ruby: ENV["HOME"]
来源：http://jpq.uphjek.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dgc.chenjidiqi.icu

[M03] 执行外部命令
来源：http://zke.ybcxt.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xll.gotoacloud.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zor.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bdp.jyoumei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ndu.tanke756.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://smu.svipenyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jyc.yanxiufei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kxp.chenlongwang.top

C#:   Process.Start("ls", "-l");
来源：http://kfv.snrcjt.cn

[M04] 获取当前工作目录
来源：http://ykd.xingfuxueyuan.xyz

Py:   os.getcwd()
来源：http://ije.hnqzz.top

PHP:  getcwd();
来源：http://lse.dashuyun.cn

JS:   process.cwd()
来源：http://rjy.fzhhl.top

TS:   process.cwd()
来源：http://tzs.epnwcf.com

Java: Path.of("").toAbsolutePath()
来源：http://smk.hammf.cn

Go:   os.Getwd()
来源：http://oud.pengpengdd.cyou

Ruby: Dir.pwd
来源：http://klr.dashuyun.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lfn.ydjk.org.cn

[M05] 设置退出码
来源：http://rae.fktsv.cn

Py:   sys.exit(1)
来源：http://woo.guannengcc.top

PHP:  exit(1);
来源：http://fur.bjfxy.top

JS:   process.exit(1)
来源：http://fss.52xcode.cn

TS:   process.exit(1)
来源：http://vsc.cashguo.top

Java: System.exit(1)
来源：http://zsm.jianghu66.top

Go:   os.Exit(1)
来源：http://kuc.zdbjq.cn

Ruby: exit 1
来源：http://nyh.wangshuangyany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cpz.aibaodan.cn

[M06] 向标准错误输出
来源：http://mip.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://unv.gotoacloud.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tot.wangdashe.top

JS:   console.error("err")
来源：http://wbo.kuanghao11.cn

TS:   console.error("err")
来源：http://fcx.feifeiyinyue.top

Java: System.err.println("err")
来源：http://wdj.xuanzx.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fgm.shuidangran.top

Ruby: warn "err"
来源：http://gwo.guannengcc.top

C#:   Console.Error.WriteLine("err")
来源：http://sgt.hnqzz.top

[M07] 判断是否为主入口
来源：http://nkx.fktsv.cn

Py:   if __name__ == "__main__":
来源：http://pxo.hywenlv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hkf.fengsongda.top

JS:   require.main === module
来源：http://iqf.fanxiaobao.xyz

TS:   require.main === module
来源：http://can.zhoulong.xyz

Java: public static void main(String[] args)
来源：http://bio.zdbjq.cn

Go:   func main()
来源：http://whh.sjlbkw.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hri.ybcxt.top

C#:   static void Main(string[] args)
来源：http://whr.redwolf501.top

[M08] 获取系统与运行时信息
来源：http://yvg.nanxuanxn.top

Py:   platform.system();  platform.python_version()
来源：http://usn.zhoulong.xyz

PHP:  PHP_OS;  phpversion();
来源：http://ijc.9152youxi.cn

JS:   process.platform;  process.version
来源：http://nbe.yfazqb.com

TS:   process.platform;  process.version
来源：http://bqv.xinyue.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lpq.jqgufenzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tny.sysykeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://paa.zhaomingkeji.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://ikv.meibo888.top

================================================================================
来源：http://xxt.aizwys.cn

N. 数据结构与算法
来源：http://ggj.shanyushiyangkeji.top

================================================================================
来源：http://lte.meibo888.top

[N01] 二分查找（有序数组）
来源：http://pey.tanke756.top

Py:   bisect.bisect_left(arr, x)
来源：http://ybx.fengsongda.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gdk.xziqi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nbx.daxiang520.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xlv.cqqwz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jem.xziqi.cn

Go:   sort.SearchInts(arr, x)
来源：http://yxb.yuxming.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://beb.yuanzhike.top

C#:   Array.BinarySearch(arr, x)
来源：http://ptq.sxryk.cn

[N02] 排序（工程实践用内置实现）
来源：http://fes.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://oyl.yj202588.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bzw.gaohongyu789.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ggt.ywan-chungtsiang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xfl.jinyuanbaomall.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://clr.shzxlz.cn

Go:   slices.Sort(arr)
来源：http://ibo.zhijiandao.cn

Ruby: arr.sort
来源：http://vxl.cdnleiting.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://snr.ywan-chungtsiang.top

[N03] 快速排序（分治示例）
来源：http://tro.aibaodan.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sdj.redwolf501.top

PHP:  // 递归实现，或用 usort
来源：http://hhd.zhiwuduotai.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lyf.tarul.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mst.cdnleiting.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oss.xuetiantiany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ezs.chenjidiqi.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zfp.fengsongda.top

C#:   // 手写递归，或 Array.Sort
来源：http://hlf.cdnleiting.top

[N04] 斐波那契数列
来源：http://yzf.fanxiaobao.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zqd.kuanghao11.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vcr.tanke756.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zgr.yj202588.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nfx.jianghu66.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tnn.ydjk.org.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hym.sjlbkw.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yfk.c1oappe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://skp.hesvh.cn

[N05] 最大公约数
来源：http://lfq.ivvv.top

Py:   math.gcd(a, b)
来源：http://cde.ybcxt.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://umd.yj20258888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://afq.pycfn.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gtx.guowangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wzf.sweek.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rxb.zycfv.cn

Ruby: a.gcd(b)
来源：http://vzq.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gqt.chenlongwang.top

[N06] 判断回文字符串
来源：http://mzf.ctjpmb.com

Py:   s == s[::-1]
来源：http://qgv.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://hgb.yanxiufei.cn

JS:   s === [...s].reverse().join("")
来源：http://ccr.jinghuilouyu.cn

TS:   s === [...s].reverse().join("")
来源：http://fkm.jinyuanbaomall.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ojm.zhengqikj.top

Go:   // 双指针从两端比较
来源：http://xad.jinqigfzy.top

Ruby: s == s.reverse
来源：http://iyc.snrcjt.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sua.sxryk.cn

[N07] 两数之和（返回下标）
来源：http://cxe.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://roc.jqgufenzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://miu.yj20258.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vzt.zdbjq.cn

TS:   // 手写 Map<string, number>
来源：http://qbd.bjfxy.top

Java: // 手写 HashMap
来源：http://rbw.chenlongwang.top

Go:   // 手写 map[int]int
来源：http://zcn.tanke756.top

Ruby: // 手写 Hash
来源：http://fzq.yangfankeji.com

C#:   // 手写 Dictionary<int, int>
来源：http://rds.hcnkem.com

[N08] 生成全排列
来源：http://pdu.xziqi.cn

Py:   itertools.permutations(arr)
来源：http://dch.aizwys.cn

PHP:  // 手写递归交换
来源：http://dlh.nwbrower.top

JS:   // 手写回溯递归
来源：http://dsz.xinyue.icu

TS:   // 手写回溯递归
来源：http://lkq.yvedp.cn

Java: // 手写回溯递归
来源：http://nnl.uphjek.com

Go:   // 手写回溯递归
来源：http://zip.fehbvm.com

Ruby: arr.permutation.to_a
来源：http://yig.zhoulong.xyz

C#:   // 手写回溯递归
来源：http://oof.zdbjq.cn

[N09] 栈与队列
来源：http://god.shanyushiyangtech.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ivz.yonumen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qts.aibaodan.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lxp.svipenyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dzo.chenjidiqi.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://khs.yvedp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://czb.daria6918.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://toy.vqdsnc.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jnr.wangdashe.top

[N10] 链表节点定义
来源：http://vlv.jinghuilouyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ixi.zhijiandao.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://moo.wangdashe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wfh.cqqwz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qwc.dianchejie.cn

Java: class Node { int v; Node next; }
来源：http://ryx.zhijiandao.cn

Go:   type Node struct { V int; Next *Node }
来源：http://axo.ehwqpu.com

Ruby: Node = Struct.new(:v, :next)
来源：http://xib.cashguo.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lsp.fehbvm.com

[N11] 二叉树中序遍历
来源：http://opx.hongshengwenyu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zuf.sufxvd.cn

PHP:  // 手写递归函数
来源：http://col.redwolf501.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://opb.haohaochexian.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://odu.zhixingplan.top

Java: // 手写递归
来源：http://rmk.aizwys.cn

Go:   // 手写递归
来源：http://nzk.iojbl.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kef.aibaodan.cn

C#:   // 手写递归
来源：http://qgz.wangdashe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hbt.tarul.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vak.jianghu66.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://awi.fktsv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://auz.aizwys.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jto.tian-w.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ojt.hesvh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wwu.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hwp.c1oappe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eda.jinghuilouyu.cn

================================================================================
来源：http://uhg.hammf.cn

O. 并发与异步
来源：http://jfv.jiagoushi.top

================================================================================
来源：http://ppp.fktsv.cn

[O01] 启动一个线程
来源：http://qcz.shzxlz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://efk.yonumen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jwk.hfpthk.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nbz.yfazqb.com

TS:   // 同 JS
来源：http://huz.fehbvm.com

Java: new Thread(() -> f()).start()
来源：http://fip.hesvh.cn

Go:   go f()
来源：http://dzd.fengsongda.top

Ruby: Thread.new { f }
来源：http://job.haohaochexian.top

C#:   Task.Run(() => F());
来源：http://vrf.zycfv.cn

[O02] 使用线程池
来源：http://lhv.dianchejie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bjg.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rah.bbcook.cn

JS:   // worker_threads 线程池
来源：http://ppi.haohaochexian.top

TS:   // worker_threads 线程池
来源：http://rtt.birdmap.top

Java: Executors.newFixedThreadPool(4)
来源：http://pzv.iojbl.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mgg.gzhubu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://spy.sjlbkw.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://joe.epnwcf.com

[O03] 加锁保护共享数据
来源：http://boq.bbcook.cn

Py:   with lock: shared += 1
来源：http://zjh.hnqzz.top

PHP:  // 用 flock() 做文件锁
来源：http://pbu.meibo888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://svo.jlsjyb.cn

TS:   // 同 JS
来源：http://ing.aibaodan.cn

Java: synchronized (this) { shared++; }
来源：http://zeu.jianghu66.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://otp.jinyuanbaomall.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cjh.haohaochexian.top

C#:   lock (gate) { shared++; }
来源：http://plh.iojbl.cn

[O04] 定义异步函数并等待
来源：http://exu.wangdashe.top

Py:   async def f():⏎    await g()
来源：http://udm.fzhhl.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fgu.zhengqikj.top

JS:   async function f() { await g(); }
来源：http://sjq.cqqwz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gng.zdqjudy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://apy.smart0.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://llk.cashguo.top

Ruby: # 用 Fiber 或 async gem
来源：http://bsw.hesvh.cn

C#:   async Task F() { await G(); }
来源：http://nvw.ydjk.org.cn

[O05] 并发执行并等待全部完成
来源：http://mms.zhengqikj.top

Py:   asyncio.gather(*tasks)
来源：http://lxg.jqgfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dmu.chenzaomai.com

JS:   await Promise.all(tasks)
来源：http://phi.ehwqpu.com

TS:   await Promise.all(tasks)
来源：http://npr.zhongyouzk.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wdn.xuanzx.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://spt.gogol.net.cn

Ruby: threads.map(&:join)
来源：http://jyx.yj20258.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pzc.hnxiangtu.top

[O06] 使用进程池
来源：http://pvt.uphjek.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qgp.yuxming.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wrn.xinyue.icu

JS:   // child_process / cluster 模块
来源：http://fka.uphjek.com


<!-- 参考信息 -->