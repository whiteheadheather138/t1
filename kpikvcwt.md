代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://xvn.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lle.jianghu66.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hxd.sweek.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mgm.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lja.yonumen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mlv.xuetiantiany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dov.hfpthk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yaq.tarul.cn

[L03] 设置自定义请求头
来源：http://byu.52xcode.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vyf.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xwh.zhijiandao.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cqd.vqdsnc.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cnf.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rbz.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dlp.sysykeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vfk.dianchejie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://peg.yvedp.cn

[L04] 设置超时
来源：http://iih.jqgufenzy.top

Py:   requests.get(url, timeout=5)
来源：http://zxw.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://irl.iojbl.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lzx.jyoumei.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://veb.hongshengwenyu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vbs.vehdjk.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://glv.svipenyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bnb.vqdsnc.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uge.nanxuanxn.top

[L05] 上传文件（multipart）
来源：http://gvv.ydzc1.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mjh.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tvm.316326.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://txu.ctjpmb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hnw.ybcxt.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lnu.hfpthk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nxh.guowangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wtv.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kwm.fanxiaobao.xyz

[L06] 解析响应为 JSON
来源：http://idm.316326.xyz

Py:   resp.json()
来源：http://wck.havefunace.top

PHP:  json_decode($body, true);
来源：http://wgg.fehbvm.com

JS:   await resp.json()
来源：http://osg.yuxming.cn

TS:   await resp.json()
来源：http://vjx.yfazqb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ozc.quarkkingdee.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uul.daria6918.cn

Ruby: JSON.parse(resp.body)
来源：http://dst.yfazqb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://toa.smart0.xyz

[L07] 处理 HTTP 状态码
来源：http://yrp.zhongyouzk.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pnh.cashguo.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://odq.cdnleiting.top

JS:   resp.ok;  resp.status
来源：http://qwi.shuidangran.top

TS:   resp.ok;  resp.status
来源：http://pjr.hcnkem.com

Java: resp.statusCode()
来源：http://lvz.xylfe.cn

Go:   resp.StatusCode
来源：http://gvr.chenzaomai.com

Ruby: resp.code.to_i
来源：http://hgo.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://tqo.ehwqpu.com

[L08] 并发请求多个地址
来源：http://yvc.guannengcc.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mpo.jinqigufen.top

PHP:  curl_multi_init() 系列
来源：http://swd.yuanzhike.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qqy.cheryme.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vmh.tian-w.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://two.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yvu.snrcjt.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bqo.andypj.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iwq.feifeiyinyue.top

================================================================================
来源：http://lwr.yvedp.cn

M. 命令行 / 进程 / 环境
来源：http://lys.ivvv.top

================================================================================
来源：http://gdi.shanyushiyangkeji.top

[M01] 读取命令行参数
来源：http://emj.jinqigufen.top

Py:   sys.argv[1:]
来源：http://uav.haohaochexian.top

PHP:  $argv;  $argc;
来源：http://tba.aibaodan.cn

JS:   process.argv.slice(2)
来源：http://hed.ybcxt.top

TS:   process.argv.slice(2)
来源：http://gnq.ehwqpu.com

Java: args 数组（main 方法参数）
来源：http://ckj.shuidangran.top

Go:   os.Args[1:]
来源：http://eop.bjfxy.top

Ruby: ARGV
来源：http://trc.yj202588.top

C#:   args 数组（Main 方法参数）
来源：http://jox.xingfuxueyuan.xyz

[M02] 读取环境变量
来源：http://xzd.nanxinkj.top

Py:   os.environ.get("HOME")
来源：http://aaa.tanke756.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jdl.cucudq.cn

JS:   process.env.HOME
来源：http://nio.yanxiufei.cn

TS:   process.env.HOME
来源：http://hqf.fanxiaobao.xyz

Java: System.getenv("HOME")
来源：http://nnt.yanxiufei.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gay.nwbrower.top

Ruby: ENV["HOME"]
来源：http://ouo.fktsv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aqh.52xcode.cn

[M03] 执行外部命令
来源：http://zkh.shangyingyoupin.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zwc.jqgufenzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dnb.ehwqpu.com

JS:   child_process.execSync("ls -l").toString()
来源：http://qjk.ppjwa.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tox.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vkb.zycfv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://juu.316326.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://ehc.yj202588.top

C#:   Process.Start("ls", "-l");
来源：http://xvc.pycfn.com

[M04] 获取当前工作目录
来源：http://pol.ctjpmb.com

Py:   os.getcwd()
来源：http://bet.tarul.cn

PHP:  getcwd();
来源：http://bux.fengsongda.top

JS:   process.cwd()
来源：http://vjf.xuanzx.com

TS:   process.cwd()
来源：http://mnl.smart0.xyz

Java: Path.of("").toAbsolutePath()
来源：http://cex.zdqjudy.top

Go:   os.Getwd()
来源：http://fdx.yfazqb.com

Ruby: Dir.pwd
来源：http://rhz.sysykeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://kua.gaohongyu789.top

[M05] 设置退出码
来源：http://yhg.dianchejie.cn

Py:   sys.exit(1)
来源：http://oor.shanyushiyangtech.top

PHP:  exit(1);
来源：http://hiz.meibo888.top

JS:   process.exit(1)
来源：http://qph.chenjidiqi.icu

TS:   process.exit(1)
来源：http://zpi.cqqwz.cn

Java: System.exit(1)
来源：http://obn.ppjwa.cn

Go:   os.Exit(1)
来源：http://cve.jianghu66.top

Ruby: exit 1
来源：http://rts.cheryme.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nub.smart0.xyz

[M06] 向标准错误输出
来源：http://eeq.fzhhl.top

Py:   print("err", file=sys.stderr)
来源：http://xev.cashguo.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ast.zhongyouzk.top

JS:   console.error("err")
来源：http://ksa.hfpthk.cn

TS:   console.error("err")
来源：http://alr.sweek.top

Java: System.err.println("err")
来源：http://lim.yanxiufei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kml.xuetiantiany.cn

Ruby: warn "err"
来源：http://uui.cucudq.cn

C#:   Console.Error.WriteLine("err")
来源：http://jsy.cdnleiting.top

[M07] 判断是否为主入口
来源：http://bbz.guannengcc.top

Py:   if __name__ == "__main__":
来源：http://vko.pycfn.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zah.ywan-chungtsiang.top

JS:   require.main === module
来源：http://ydn.yanxiufei.cn

TS:   require.main === module
来源：http://mdf.daxiang520.top

Java: public static void main(String[] args)
来源：http://ldp.pycfn.com

Go:   func main()
来源：http://zmf.zhiwuduotai.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wel.sysykeji.top

C#:   static void Main(string[] args)
来源：http://jai.316326.xyz

[M08] 获取系统与运行时信息
来源：http://tur.xuetiantiany.cn

Py:   platform.system();  platform.python_version()
来源：http://awb.hcnkem.com

PHP:  PHP_OS;  phpversion();
来源：http://ybq.dianchejie.cn

JS:   process.platform;  process.version
来源：http://tly.cucudq.cn

TS:   process.platform;  process.version
来源：http://buz.sxryk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fjp.ctjpmb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://sbh.yj20258888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qtg.smart0.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://pue.cashguo.top

================================================================================
来源：http://gln.xuanzx.com

N. 数据结构与算法
来源：http://msx.hnqzz.top

================================================================================
来源：http://xun.hysaishi.cn

[N01] 二分查找（有序数组）
来源：http://flf.zhengqikj.top

Py:   bisect.bisect_left(arr, x)
来源：http://xbb.ctjpmb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bxs.jinyuanbaomall.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rot.birdmap.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gfb.shzxlz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qwg.ppjwa.cn

Go:   sort.SearchInts(arr, x)
来源：http://dfl.hnqzz.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://guu.daria6918.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hlq.yj20258888.top

[N02] 排序（工程实践用内置实现）
来源：http://yht.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://tjs.yangfankeji.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tfh.guowangkeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://eym.yueranfly.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ycu.wangdashe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wqy.zycfv.cn

Go:   slices.Sort(arr)
来源：http://ufh.zhengqikj.top

Ruby: arr.sort
来源：http://wif.gzhubu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lmm.jyoumei.cn

[N03] 快速排序（分治示例）
来源：http://rjs.vehdjk.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mkx.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://puy.havefunace.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xst.havefunace.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://djc.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cvj.cucudq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dcq.zhiwuduotai.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yca.52xcode.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rsm.uphjek.com

[N04] 斐波那契数列
来源：http://smi.yanxiufei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xkr.chenjidiqi.icu

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oqm.yj202588.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kha.dianchejie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://doi.wangshuangyany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tti.ehwqpu.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tdi.yuanzhike.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kfk.ctjpmb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://smy.cucudq.cn

[N05] 最大公约数
来源：http://fsx.ywan-chungtsiang.top

Py:   math.gcd(a, b)
来源：http://orj.smart0.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kwg.quarkkingdee.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hpj.zhoulong.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qaq.zhengqikj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qyi.yanxiufei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pxf.hywenlv.cn

Ruby: a.gcd(b)
来源：http://jzw.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zbs.hammf.cn

[N06] 判断回文字符串
来源：http://jis.xuanzx.com

Py:   s == s[::-1]
来源：http://tuq.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://yur.snrcjt.cn

JS:   s === [...s].reverse().join("")
来源：http://omg.ywan-chungtsiang.top

TS:   s === [...s].reverse().join("")
来源：http://zak.meibo888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qbb.smart0.xyz

Go:   // 双指针从两端比较
来源：http://wxl.feifeiyinyue.top

Ruby: s == s.reverse
来源：http://wuc.tanke756.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lec.hcnkem.com

[N07] 两数之和（返回下标）
来源：http://bkr.yanxiufei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rpu.yangfankeji.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zax.zdqjudy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jvr.dianchejie.cn

TS:   // 手写 Map<string, number>
来源：http://ykj.ybcxt.top

Java: // 手写 HashMap
来源：http://dvm.nanxinkj.top

Go:   // 手写 map[int]int
来源：http://xqg.mhx1999.top

Ruby: // 手写 Hash
来源：http://gyo.iojbl.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cgj.jinyuanbaomall.cn

[N08] 生成全排列
来源：http://bkw.chenjidiqi.icu

Py:   itertools.permutations(arr)
来源：http://tbn.xylfe.cn

PHP:  // 手写递归交换
来源：http://ium.yuxming.cn

JS:   // 手写回溯递归
来源：http://uwx.9152youxi.cn

TS:   // 手写回溯递归
来源：http://tmt.ivvv.top

Java: // 手写回溯递归
来源：http://mop.nanxinkj.top

Go:   // 手写回溯递归
来源：http://zvj.yj20258888.top

Ruby: arr.permutation.to_a
来源：http://tjm.yj20258888.top

C#:   // 手写回溯递归
来源：http://stg.redwolf501.top

[N09] 栈与队列
来源：http://zan.nwbrower.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://szi.jinyuanbaomall.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dyc.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tmy.yvedp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bzo.svipenyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dzi.jinqigfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ngc.fehbvm.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ozt.jinqigufen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lxq.gogol.net.cn

[N10] 链表节点定义
来源：http://zgt.tianlin.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qcj.jqgufenzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vhj.jinqigufen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ddg.shanyushiyangtech.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ypg.tanke756.top

Java: class Node { int v; Node next; }
来源：http://gjm.guannengcc.top

Go:   type Node struct { V int; Next *Node }
来源：http://xup.jinqigfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ttk.yangfankeji.com

C#:   class Node { public int V; public Node? Next; }
来源：http://osu.shuidangran.top

[N11] 二叉树中序遍历
来源：http://rlq.chenlongwang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aly.shanyushiyangtech.top

PHP:  // 手写递归函数
来源：http://ofn.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oam.jiagoushi.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mec.jqgfzy.top

Java: // 手写递归
来源：http://xgn.316326.xyz

Go:   // 手写递归
来源：http://bkp.zhoulong.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kyf.ctjpmb.com

C#:   // 手写递归
来源：http://igb.zhaomingkeji.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gkw.feifeiyinyue.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hbf.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ici.daria6918.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cdo.bjfxy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wyw.yj202588.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oiu.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://drr.cashguo.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qev.bjfxy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kyi.zhaomingkeji.xyz

================================================================================
来源：http://gnc.yonumen.top

O. 并发与异步
来源：http://jmp.yanxiufei.cn

================================================================================
来源：http://cte.sufxvd.cn

[O01] 启动一个线程
来源：http://mtj.xziqi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rzi.52xcode.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rzb.hfpthk.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fjs.yfazqb.com

TS:   // 同 JS
来源：http://vyy.chenjidiqi.icu

Java: new Thread(() -> f()).start()
来源：http://pxb.guannengcc.top

Go:   go f()
来源：http://ayu.jinqigufen.top

Ruby: Thread.new { f }
来源：http://wdd.ppjwa.cn

C#:   Task.Run(() => F());
来源：http://eno.yj202588.top

[O02] 使用线程池
来源：http://fju.yj20258.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://epk.jinqigufen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ymg.jlsjyb.cn

JS:   // worker_threads 线程池
来源：http://dvg.cheryme.top

TS:   // worker_threads 线程池
来源：http://bup.gotoacloud.top

Java: Executors.newFixedThreadPool(4)
来源：http://jzi.tanke756.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://efy.ppjwa.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iit.andypj.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sox.ydzc1.top

[O03] 加锁保护共享数据
来源：http://vqe.jiagoushi.top

Py:   with lock: shared += 1
来源：http://teo.tianlin.xyz

PHP:  // 用 flock() 做文件锁
来源：http://foc.tian-w.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xcd.xylfe.cn

TS:   // 同 JS
来源：http://elg.nanxuanxn.top

Java: synchronized (this) { shared++; }
来源：http://jxs.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mga.fengsongda.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qsb.svipenyu.cn

C#:   lock (gate) { shared++; }
来源：http://mul.bbcook.cn

[O04] 定义异步函数并等待
来源：http://bvp.yongpay.top

Py:   async def f():⏎    await g()
来源：http://bgt.hnxiangtu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tmi.jinghuilouyu.cn

JS:   async function f() { await g(); }
来源：http://puu.hnqzz.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ieh.chenjidiqi.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uom.gzhubu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://awe.yj20258.top

Ruby: # 用 Fiber 或 async gem
来源：http://viy.zhijiandao.cn

C#:   async Task F() { await G(); }
来源：http://lnm.hongshengwenyu.top

[O05] 并发执行并等待全部完成
来源：http://asx.haohaochexian.top

Py:   asyncio.gather(*tasks)
来源：http://own.smart0.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fqu.dashuyun.cn

JS:   await Promise.all(tasks)
来源：http://ugz.iojbl.cn

TS:   await Promise.all(tasks)
来源：http://ziz.xylfe.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ifk.haohaochexian.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uzm.sweek.top

Ruby: threads.map(&:join)
来源：http://fnw.chenjidiqi.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://qml.chenjidiqi.icu

[O06] 使用进程池
来源：http://lav.iojbl.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rdv.shuidangran.top

PHP:  // pcntl_fork 或多进程队列
来源：http://tfn.52xcode.cn

JS:   // child_process / cluster 模块
来源：http://ano.jinghuilouyu.cn


<!-- 参考信息 -->