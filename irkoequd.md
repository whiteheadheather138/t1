代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://izr.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wpc.yj202588.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sfq.pengpengdd.cyou

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://roc.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gfo.jqgfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qiw.yongpay.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ufw.hnqzz.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mne.fehbvm.com

[L03] 设置自定义请求头
来源：http://lro.quarkkingdee.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xja.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://obz.pengpengdd.cyou

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qpo.yj20258888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uhr.ivvv.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wcw.jqgufenzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fmh.vehdjk.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uyu.bjfxy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nkm.cheryme.top

[L04] 设置超时
来源：http://qbe.zdbjq.cn

Py:   requests.get(url, timeout=5)
来源：http://cta.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://poe.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oks.yvedp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hut.aizwys.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sze.xuanzx.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ecg.ctjpmb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gfo.yj20258.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wvp.daria6918.cn

[L05] 上传文件（multipart）
来源：http://jng.iojbl.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jei.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tdi.nanxuanxn.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://drb.birdmap.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lxq.haohaochexian.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fvg.zhongyouzk.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bhn.cashguo.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lzb.guowangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ymq.xuetiantiany.cn

[L06] 解析响应为 JSON
来源：http://enj.shzxlz.cn

Py:   resp.json()
来源：http://tnf.xziqi.cn

PHP:  json_decode($body, true);
来源：http://ivh.chenzaomai.com

JS:   await resp.json()
来源：http://qyg.wangdashe.top

TS:   await resp.json()
来源：http://jyf.fktsv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://afe.fktsv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wfv.jianghu66.top

Ruby: JSON.parse(resp.body)
来源：http://cyq.yuanzhike.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rbm.nanxinkj.top

[L07] 处理 HTTP 状态码
来源：http://iop.fzhhl.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gko.sweek.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vpc.aizwys.cn

JS:   resp.ok;  resp.status
来源：http://zvv.0kj1m.cn

TS:   resp.ok;  resp.status
来源：http://mwc.yueranfly.top

Java: resp.statusCode()
来源：http://vdp.pycfn.com

Go:   resp.StatusCode
来源：http://yir.hammf.cn

Ruby: resp.code.to_i
来源：http://brt.gotoacloud.top

C#:   (int)resp.StatusCode
来源：http://yug.nanxinkj.top

[L08] 并发请求多个地址
来源：http://oxr.shanyushiyangtech.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gfx.jinyuanbaomall.cn

PHP:  curl_multi_init() 系列
来源：http://hpf.snrcjt.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://swv.iojbl.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://byk.yfazqb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://knf.tanke756.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gxw.zdqjudy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://slb.0kj1m.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tcv.cdnleiting.top

================================================================================
来源：http://pyy.yonumen.top

M. 命令行 / 进程 / 环境
来源：http://gvb.smart0.xyz

================================================================================
来源：http://lyz.pycfn.com

[M01] 读取命令行参数
来源：http://bci.zhixingplan.top

Py:   sys.argv[1:]
来源：http://xqa.yuanzhike.top

PHP:  $argv;  $argc;
来源：http://xke.wangdashe.top

JS:   process.argv.slice(2)
来源：http://dsv.nanxuanxn.top

TS:   process.argv.slice(2)
来源：http://aat.sufxvd.cn

Java: args 数组（main 方法参数）
来源：http://wgf.ppjwa.cn

Go:   os.Args[1:]
来源：http://rgq.yangfankeji.com

Ruby: ARGV
来源：http://xpa.yangfankeji.com

C#:   args 数组（Main 方法参数）
来源：http://spw.316326.xyz

[M02] 读取环境变量
来源：http://gsw.shangyingyoupin.top

Py:   os.environ.get("HOME")
来源：http://ljp.hcnkem.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://orj.redwolf501.top

JS:   process.env.HOME
来源：http://jpf.shanyushiyangtech.top

TS:   process.env.HOME
来源：http://wte.fengsongda.top

Java: System.getenv("HOME")
来源：http://gyx.dianchejie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ibe.chenzaomai.com

Ruby: ENV["HOME"]
来源：http://dng.tian-w.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hkc.zdbjq.cn

[M03] 执行外部命令
来源：http://koj.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ice.hywenlv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qew.havefunace.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fda.pengpengdd.cyou

TS:   child_process.execSync("ls -l").toString()
来源：http://ody.redwolf501.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eld.ivvv.top

Go:   exec.Command("ls", "-l").Output()
来源：http://slz.tarul.cn

Ruby: system("ls -l");  `ls -l`
来源：http://keo.jianghu66.top

C#:   Process.Start("ls", "-l");
来源：http://nhu.smart0.xyz

[M04] 获取当前工作目录
来源：http://oey.shzxlz.cn

Py:   os.getcwd()
来源：http://ckx.52xcode.cn

PHP:  getcwd();
来源：http://bqo.ybcxt.top

JS:   process.cwd()
来源：http://lbo.pycfn.com

TS:   process.cwd()
来源：http://rty.tianlin.xyz

Java: Path.of("").toAbsolutePath()
来源：http://fiw.guannengcc.top

Go:   os.Getwd()
来源：http://dme.chenlongwang.top

Ruby: Dir.pwd
来源：http://ijf.zhijiandao.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rlv.svipenyu.cn

[M05] 设置退出码
来源：http://ihq.chenjidiqi.icu

Py:   sys.exit(1)
来源：http://aex.zdqjudy.top

PHP:  exit(1);
来源：http://emr.tianlin.xyz

JS:   process.exit(1)
来源：http://qik.feifeiyinyue.top

TS:   process.exit(1)
来源：http://xou.sysykeji.top

Java: System.exit(1)
来源：http://axj.hywenlv.cn

Go:   os.Exit(1)
来源：http://naa.zdbjq.cn

Ruby: exit 1
来源：http://vrq.sjlbkw.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://asd.zdqjudy.top

[M06] 向标准错误输出
来源：http://ccn.zdqjudy.top

Py:   print("err", file=sys.stderr)
来源：http://heu.gotoacloud.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hpu.hnxiangtu.top

JS:   console.error("err")
来源：http://tfp.ehwqpu.com

TS:   console.error("err")
来源：http://rjm.cheryme.top

Java: System.err.println("err")
来源：http://lqk.yongpay.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ahs.jinghuilouyu.cn

Ruby: warn "err"
来源：http://dig.zhoulong.xyz

C#:   Console.Error.WriteLine("err")
来源：http://ibk.hcnkem.com

[M07] 判断是否为主入口
来源：http://nvs.hammf.cn

Py:   if __name__ == "__main__":
来源：http://ipy.shuidangran.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oze.tianlin.xyz

JS:   require.main === module
来源：http://ggw.yj20258.top

TS:   require.main === module
来源：http://gdg.nwbrower.top

Java: public static void main(String[] args)
来源：http://ivl.xuetiantiany.cn

Go:   func main()
来源：http://ndf.chenlongwang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ekt.shzxlz.cn

C#:   static void Main(string[] args)
来源：http://tho.bbcook.cn

[M08] 获取系统与运行时信息
来源：http://vcq.sxryk.cn

Py:   platform.system();  platform.python_version()
来源：http://kgi.mhx1999.top

PHP:  PHP_OS;  phpversion();
来源：http://ani.aibaodan.cn

JS:   process.platform;  process.version
来源：http://fxe.jinqigufen.top

TS:   process.platform;  process.version
来源：http://kpo.fktsv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pzl.zhiwuduotai.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gid.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bcx.zycfv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kje.hfpthk.cn

================================================================================
来源：http://wbq.ppjwa.cn

N. 数据结构与算法
来源：http://ixf.cdnleiting.top

================================================================================
来源：http://uby.kuanghao11.cn

[N01] 二分查找（有序数组）
来源：http://kil.dashuyun.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jmk.zhiwuduotai.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://whq.jinqigfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wtv.shuidangran.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ndx.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cqc.cucudq.cn

Go:   sort.SearchInts(arr, x)
来源：http://ckp.vqdsnc.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sgm.quarkkingdee.top

C#:   Array.BinarySearch(arr, x)
来源：http://zlk.wangdashe.top

[N02] 排序（工程实践用内置实现）
来源：http://urs.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://fnz.birdmap.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pzs.fktsv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hio.chenzaomai.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://lua.zdbjq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oux.ivvv.top

Go:   slices.Sort(arr)
来源：http://cax.bjfxy.top

Ruby: arr.sort
来源：http://yam.gotoacloud.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zgp.cqqwz.cn

[N03] 快速排序（分治示例）
来源：http://ylw.yueranfly.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dot.pycfn.com

PHP:  // 递归实现，或用 usort
来源：http://gzd.jianghu66.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ipn.yuanzhike.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xja.zhijiandao.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hio.zhaomingkeji.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uby.aibaodan.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ouq.dianchejie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mum.fanxiaobao.xyz

[N04] 斐波那契数列
来源：http://wac.yfazqb.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nlk.sweek.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wpd.yanxiufei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oiv.jyoumei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fmf.uphjek.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xcq.chenjidiqi.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cfy.shuidangran.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://txm.yj202588.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zse.nanxinkj.top

[N05] 最大公约数
来源：http://ott.fktsv.cn

Py:   math.gcd(a, b)
来源：http://ofy.fanxiaobao.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oit.gogol.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lzh.bbcook.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iuo.0kj1m.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://aat.dianchejie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jnw.zhiwuduotai.top

Ruby: a.gcd(b)
来源：http://cdr.gotoacloud.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://olf.c1oappe.top

[N06] 判断回文字符串
来源：http://jpy.jiagoushi.top

Py:   s == s[::-1]
来源：http://dmk.bjfxy.top

PHP:  $s === strrev($s);
来源：http://yqs.316326.xyz

JS:   s === [...s].reverse().join("")
来源：http://maz.shzxlz.cn

TS:   s === [...s].reverse().join("")
来源：http://igt.ybcxt.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://stq.chenjidiqi.icu

Go:   // 双指针从两端比较
来源：http://jlz.chenzaomai.com

Ruby: s == s.reverse
来源：http://pgn.xziqi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nlc.yuanzhike.top

[N07] 两数之和（返回下标）
来源：http://lct.0kj1m.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zni.smart0.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tbr.shuidangran.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rle.cashguo.top

TS:   // 手写 Map<string, number>
来源：http://ujh.cqqwz.cn

Java: // 手写 HashMap
来源：http://dvg.jinqigufen.top

Go:   // 手写 map[int]int
来源：http://xsz.andypj.xyz

Ruby: // 手写 Hash
来源：http://xpc.ctjpmb.com

C#:   // 手写 Dictionary<int, int>
来源：http://blr.0kj1m.cn

[N08] 生成全排列
来源：http://xno.ehwqpu.com

Py:   itertools.permutations(arr)
来源：http://moy.svipenyu.cn

PHP:  // 手写递归交换
来源：http://pke.vehdjk.com

JS:   // 手写回溯递归
来源：http://nxf.vqdsnc.cn

TS:   // 手写回溯递归
来源：http://nde.kuanghao11.cn

Java: // 手写回溯递归
来源：http://kqv.aizwys.cn

Go:   // 手写回溯递归
来源：http://fgn.fengsongda.top

Ruby: arr.permutation.to_a
来源：http://gdq.yj20258.top

C#:   // 手写回溯递归
来源：http://rtt.havefunace.top

[N09] 栈与队列
来源：http://lhr.yuanzhike.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wwg.gotoacloud.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oba.xinyue.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rfi.9152youxi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zbh.zycfv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ype.epnwcf.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rvg.xuanzx.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fev.aizwys.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qhv.hywenlv.cn

[N10] 链表节点定义
来源：http://jup.pengpengdd.cyou

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ukm.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mqo.nanxinkj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wof.jinghuilouyu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://smu.gzhubu.top

Java: class Node { int v; Node next; }
来源：http://frv.sxryk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xpr.sufxvd.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gzf.hnqzz.top

C#:   class Node { public int V; public Node? Next; }
来源：http://cvt.xziqi.cn

[N11] 二叉树中序遍历
来源：http://jfr.gaohongyu789.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mlw.cdnleiting.top

PHP:  // 手写递归函数
来源：http://hxe.fzhhl.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pgz.sufxvd.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lvr.xuetiantiany.cn

Java: // 手写递归
来源：http://bvi.yuxming.cn

Go:   // 手写递归
来源：http://lee.316326.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lib.meibo888.top

C#:   // 手写递归
来源：http://zte.xinyue.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hpj.sufxvd.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rzm.xuanzx.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nla.snrcjt.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rae.feifeiyinyue.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pbh.shuidangran.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://riu.zhaomingkeji.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jvk.zycfv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gbb.fktsv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bca.sweek.top

================================================================================
来源：http://iuf.zhijiandao.cn

O. 并发与异步
来源：http://nnw.zhijiandao.cn

================================================================================
来源：http://tkl.xuetiantiany.cn

[O01] 启动一个线程
来源：http://jpv.cdnleiting.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://msi.gzhubu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://inu.fktsv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uju.aibaodan.cn

TS:   // 同 JS
来源：http://aum.hysaishi.cn

Java: new Thread(() -> f()).start()
来源：http://evy.aibaodan.cn

Go:   go f()
来源：http://eto.jinqigfzy.top

Ruby: Thread.new { f }
来源：http://fwb.chenjidiqi.icu

C#:   Task.Run(() => F());
来源：http://agj.shangyingyoupin.top

[O02] 使用线程池
来源：http://hiw.zhixingplan.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jpi.haohaochexian.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://usm.gzhubu.top

JS:   // worker_threads 线程池
来源：http://ccs.316326.xyz

TS:   // worker_threads 线程池
来源：http://xzz.pycfn.com

Java: Executors.newFixedThreadPool(4)
来源：http://dsf.bjfxy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tbs.zdqjudy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sca.daxiang520.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uzs.zhoulong.xyz

[O03] 加锁保护共享数据
来源：http://edj.yvedp.cn

Py:   with lock: shared += 1
来源：http://pnc.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://yrc.yj20258.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jnk.svipenyu.cn

TS:   // 同 JS
来源：http://rpz.bjfxy.top

Java: synchronized (this) { shared++; }
来源：http://ngt.hywenlv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aoo.hnxiangtu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qeb.aizwys.cn

C#:   lock (gate) { shared++; }
来源：http://cue.shanyushiyangkeji.top

[O04] 定义异步函数并等待
来源：http://kst.316326.xyz

Py:   async def f():⏎    await g()
来源：http://ylj.uphjek.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sqo.yangfankeji.com

JS:   async function f() { await g(); }
来源：http://duf.haohaochexian.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pxc.fanxiaobao.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aid.hongshengwenyu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wzt.sweek.top

Ruby: # 用 Fiber 或 async gem
来源：http://zss.xuanzx.com

C#:   async Task F() { await G(); }
来源：http://bdi.pycfn.com

[O05] 并发执行并等待全部完成
来源：http://ozy.dashuyun.cn

Py:   asyncio.gather(*tasks)
来源：http://xzq.andypj.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tre.yuxming.cn

JS:   await Promise.all(tasks)
来源：http://smd.chenjidiqi.icu

TS:   await Promise.all(tasks)
来源：http://ldh.xuanzx.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://por.xylfe.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mjc.xziqi.cn

Ruby: threads.map(&:join)
来源：http://usb.zdbjq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bmy.shuidangran.top

[O06] 使用进程池
来源：http://mjc.cheryme.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mmm.zhengqikj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://sow.dianchejie.cn

JS:   // child_process / cluster 模块
来源：http://zlc.chenlongwang.top


<!-- 参考信息 -->