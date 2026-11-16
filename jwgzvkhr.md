代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://zzl.feifeiyinyue.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lgo.tianlin.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uya.ctjpmb.com

[L02] 发送 POST JSON
来源：http://qzc.aizwys.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dod.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cpi.cdnleiting.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gkl.jiagoushi.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bfx.hammf.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jhp.jqgfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://umv.nanxuanxn.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ygz.jinghuilouyu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ict.hongshengwenyu.top

[L03] 设置自定义请求头
来源：http://ymy.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ovk.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hvm.zycfv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ydw.sjlbkw.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iqf.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qhn.ydjk.org.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vbi.sysykeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wij.hysaishi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dan.ydzc1.top

[L04] 设置超时
来源：http://bsp.zhengqikj.top

Py:   requests.get(url, timeout=5)
来源：http://pbx.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yuk.gaohongyu789.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tvv.zhengqikj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ddc.zhaomingkeji.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uwq.jinghuilouyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://flu.hysaishi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vvz.gzhubu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bkq.xinyue.icu

[L05] 上传文件（multipart）
来源：http://vfl.xziqi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nsk.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nuk.hfpthk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ysu.shangyingyoupin.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nds.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kvh.hammf.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xdx.yanxiufei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ebw.yongpay.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uel.yvedp.cn

[L06] 解析响应为 JSON
来源：http://xhq.bbcook.cn

Py:   resp.json()
来源：http://wke.andypj.xyz

PHP:  json_decode($body, true);
来源：http://aqd.sufxvd.cn

JS:   await resp.json()
来源：http://uoq.jqgufenzy.top

TS:   await resp.json()
来源：http://lhx.jyoumei.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://njt.birdmap.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vib.jyoumei.cn

Ruby: JSON.parse(resp.body)
来源：http://nxv.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://naa.zdqjudy.top

[L07] 处理 HTTP 状态码
来源：http://umu.fzhhl.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://heo.zhijiandao.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hcv.jinqigufen.top

JS:   resp.ok;  resp.status
来源：http://vlq.feifeiyinyue.top

TS:   resp.ok;  resp.status
来源：http://xhv.sysykeji.top

Java: resp.statusCode()
来源：http://yby.ivvv.top

Go:   resp.StatusCode
来源：http://vsp.sxryk.cn

Ruby: resp.code.to_i
来源：http://hcx.wangdashe.top

C#:   (int)resp.StatusCode
来源：http://ccg.hysaishi.cn

[L08] 并发请求多个地址
来源：http://isc.chenzaomai.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eei.zdqjudy.top

PHP:  curl_multi_init() 系列
来源：http://csk.nwbrower.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qzi.zhixingplan.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ptt.zhaomingkeji.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jat.guowangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pkd.xinyue.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ihj.daxiang520.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://odj.sweek.top

================================================================================
来源：http://scd.ppjwa.cn

M. 命令行 / 进程 / 环境
来源：http://hya.hywenlv.cn

================================================================================
来源：http://vfm.bbcook.cn

[M01] 读取命令行参数
来源：http://cbb.xinyue.icu

Py:   sys.argv[1:]
来源：http://ayx.chenlongwang.top

PHP:  $argv;  $argc;
来源：http://nnm.dashuyun.cn

JS:   process.argv.slice(2)
来源：http://dat.daxiang520.top

TS:   process.argv.slice(2)
来源：http://qfe.fanxiaobao.xyz

Java: args 数组（main 方法参数）
来源：http://dao.ywan-chungtsiang.top

Go:   os.Args[1:]
来源：http://zkw.ydjk.org.cn

Ruby: ARGV
来源：http://zwd.yj20258.top

C#:   args 数组（Main 方法参数）
来源：http://upb.cashguo.top

[M02] 读取环境变量
来源：http://ujj.52xcode.cn

Py:   os.environ.get("HOME")
来源：http://krc.ehwqpu.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jfs.dashuyun.cn

JS:   process.env.HOME
来源：http://vvm.jinqigufen.top

TS:   process.env.HOME
来源：http://wjd.jinqigfzy.top

Java: System.getenv("HOME")
来源：http://frh.birdmap.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eho.9152youxi.cn

Ruby: ENV["HOME"]
来源：http://fwj.jianghu66.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gcd.wangshuangyany.cn

[M03] 执行外部命令
来源：http://orn.redwolf501.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://trt.redwolf501.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tfb.jyoumei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qgc.uphjek.com

TS:   child_process.execSync("ls -l").toString()
来源：http://sep.fanxiaobao.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hac.zycfv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yit.chenzaomai.com

Ruby: system("ls -l");  `ls -l`
来源：http://ivx.aizwys.cn

C#:   Process.Start("ls", "-l");
来源：http://stl.gzhubu.top

[M04] 获取当前工作目录
来源：http://qrh.hongshengwenyu.top

Py:   os.getcwd()
来源：http://wuq.hesvh.cn

PHP:  getcwd();
来源：http://tic.tian-w.cn

JS:   process.cwd()
来源：http://zde.shanyushiyangkeji.top

TS:   process.cwd()
来源：http://suw.zhiwuduotai.top

Java: Path.of("").toAbsolutePath()
来源：http://smd.316326.xyz

Go:   os.Getwd()
来源：http://naq.hnqzz.top

Ruby: Dir.pwd
来源：http://gop.shanyushiyangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://dsx.cdnleiting.top

[M05] 设置退出码
来源：http://amf.zdbjq.cn

Py:   sys.exit(1)
来源：http://qiq.yj202588.top

PHP:  exit(1);
来源：http://mlk.birdmap.top

JS:   process.exit(1)
来源：http://ynf.vehdjk.com

TS:   process.exit(1)
来源：http://gcx.cucudq.cn

Java: System.exit(1)
来源：http://jhf.xinyue.icu

Go:   os.Exit(1)
来源：http://tcl.9152youxi.cn

Ruby: exit 1
来源：http://rab.yuanzhike.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xlp.havefunace.top

[M06] 向标准错误输出
来源：http://nim.xingfuxueyuan.xyz

Py:   print("err", file=sys.stderr)
来源：http://pzk.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://fhy.zhixingplan.top

JS:   console.error("err")
来源：http://ciq.yj202588.top

TS:   console.error("err")
来源：http://gyv.yvedp.cn

Java: System.err.println("err")
来源：http://dtb.ywan-chungtsiang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wnv.sweek.top

Ruby: warn "err"
来源：http://ryl.uphjek.com

C#:   Console.Error.WriteLine("err")
来源：http://eic.andypj.xyz

[M07] 判断是否为主入口
来源：http://yoi.vqdsnc.cn

Py:   if __name__ == "__main__":
来源：http://vfq.xingfuxueyuan.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ypc.jyoumei.cn

JS:   require.main === module
来源：http://wzf.jinghuilouyu.cn

TS:   require.main === module
来源：http://igk.nwbrower.top

Java: public static void main(String[] args)
来源：http://gly.hcnkem.com

Go:   func main()
来源：http://pof.xziqi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://imu.aizwys.cn

C#:   static void Main(string[] args)
来源：http://mrq.sysykeji.top

[M08] 获取系统与运行时信息
来源：http://gvg.jqgfzy.top

Py:   platform.system();  platform.python_version()
来源：http://fcj.sxryk.cn

PHP:  PHP_OS;  phpversion();
来源：http://hda.ehwqpu.com

JS:   process.platform;  process.version
来源：http://wnq.bjfxy.top

TS:   process.platform;  process.version
来源：http://mhz.bbcook.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nea.feifeiyinyue.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mkn.jinghuilouyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wga.shanyushiyangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jfr.cqqwz.cn

================================================================================
来源：http://ron.cucudq.cn

N. 数据结构与算法
来源：http://hjz.zhijiandao.cn

================================================================================
来源：http://fxh.jqgfzy.top

[N01] 二分查找（有序数组）
来源：http://utp.sufxvd.cn

Py:   bisect.bisect_left(arr, x)
来源：http://thh.sufxvd.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jwe.kuanghao11.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gkx.daxiang520.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nxu.hysaishi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dgn.fzhhl.top

Go:   sort.SearchInts(arr, x)
来源：http://gug.iojbl.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kmi.zhiwuduotai.top

C#:   Array.BinarySearch(arr, x)
来源：http://fln.xuanzx.com

[N02] 排序（工程实践用内置实现）
来源：http://wxi.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://bay.smart0.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tmt.hesvh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://whs.pycfn.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://vqc.yueranfly.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kqt.shanyushiyangtech.top

Go:   slices.Sort(arr)
来源：http://lcf.zdbjq.cn

Ruby: arr.sort
来源：http://ouo.uphjek.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://bwm.chenjidiqi.icu

[N03] 快速排序（分治示例）
来源：http://ayu.pycfn.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vdg.bjfxy.top

PHP:  // 递归实现，或用 usort
来源：http://row.zycfv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eep.meibo888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://alt.zycfv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jju.tarul.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cjk.xylfe.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://typ.ybcxt.top

C#:   // 手写递归，或 Array.Sort
来源：http://msg.c1oappe.top

[N04] 斐波那契数列
来源：http://rxd.hfpthk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gbx.yj202588.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qjt.gaohongyu789.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://grh.tarul.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sdj.sysykeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qjn.xuanzx.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pur.chenzaomai.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qzy.feifeiyinyue.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dgm.xuetiantiany.cn

[N05] 最大公约数
来源：http://kwr.ydzc1.top

Py:   math.gcd(a, b)
来源：http://laa.hnxiangtu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jqx.jinqigufen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://itm.xuanzx.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dmj.tanke756.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yna.tarul.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hpg.sweek.top

Ruby: a.gcd(b)
来源：http://poh.yvedp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dxa.shuidangran.top

[N06] 判断回文字符串
来源：http://gpc.gogol.net.cn

Py:   s == s[::-1]
来源：http://lve.tianlin.xyz

PHP:  $s === strrev($s);
来源：http://daq.xylfe.cn

JS:   s === [...s].reverse().join("")
来源：http://met.meibo888.top

TS:   s === [...s].reverse().join("")
来源：http://fsu.yongpay.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qes.zhijiandao.cn

Go:   // 双指针从两端比较
来源：http://wri.hnqzz.top

Ruby: s == s.reverse
来源：http://bui.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://arz.yongpay.top

[N07] 两数之和（返回下标）
来源：http://oqe.jlsjyb.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://crs.gogol.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hgh.zdbjq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gut.zdbjq.cn

TS:   // 手写 Map<string, number>
来源：http://bkb.cheryme.top

Java: // 手写 HashMap
来源：http://zvs.jqgfzy.top

Go:   // 手写 map[int]int
来源：http://dnw.havefunace.top

Ruby: // 手写 Hash
来源：http://kxz.yj20258888.top

C#:   // 手写 Dictionary<int, int>
来源：http://vhj.hongshengwenyu.top

[N08] 生成全排列
来源：http://htb.fengsongda.top

Py:   itertools.permutations(arr)
来源：http://lno.cqqwz.cn

PHP:  // 手写递归交换
来源：http://xhb.hnqzz.top

JS:   // 手写回溯递归
来源：http://byc.tanke756.top

TS:   // 手写回溯递归
来源：http://iye.guowangkeji.top

Java: // 手写回溯递归
来源：http://awv.epnwcf.com

Go:   // 手写回溯递归
来源：http://cru.vqdsnc.cn

Ruby: arr.permutation.to_a
来源：http://kaf.feifeiyinyue.top

C#:   // 手写回溯递归
来源：http://eec.jqgfzy.top

[N09] 栈与队列
来源：http://ghd.zhoulong.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jgv.dianchejie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ouw.jinghuilouyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kcy.jiagoushi.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://azv.316326.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uql.nwbrower.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hnw.hywenlv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ckb.hywenlv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bvo.wangshuangyany.cn

[N10] 链表节点定义
来源：http://zuq.birdmap.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qjp.kuanghao11.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bqd.sjlbkw.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pdd.bbcook.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dqu.cqqwz.cn

Java: class Node { int v; Node next; }
来源：http://bwg.cdnleiting.top

Go:   type Node struct { V int; Next *Node }
来源：http://tiz.xuanzx.com

Ruby: Node = Struct.new(:v, :next)
来源：http://pdu.yueranfly.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ckf.hfpthk.cn

[N11] 二叉树中序遍历
来源：http://lrk.yuanzhike.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oxj.zhiwuduotai.top

PHP:  // 手写递归函数
来源：http://vpl.zhoulong.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://seh.sysykeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aja.wangdashe.top

Java: // 手写递归
来源：http://ftz.0kj1m.cn

Go:   // 手写递归
来源：http://tnx.feifeiyinyue.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lpn.zhongyouzk.top

C#:   // 手写递归
来源：http://ary.chenjidiqi.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vff.vqdsnc.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bsd.jyoumei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ggb.feifeiyinyue.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ktj.chenjidiqi.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zfp.guannengcc.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bxs.tianlin.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vyh.vehdjk.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ebq.cheryme.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baf.hfpthk.cn

================================================================================
来源：http://swj.yj202588.top

O. 并发与异步
来源：http://kcv.bbcook.cn

================================================================================
来源：http://fej.gotoacloud.top

[O01] 启动一个线程
来源：http://cdo.c1oappe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ixn.jianghu66.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dkw.yfazqb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ttm.zdqjudy.top

TS:   // 同 JS
来源：http://egd.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://slg.yfazqb.com

Go:   go f()
来源：http://gpc.yj20258.top

Ruby: Thread.new { f }
来源：http://fyu.haohaochexian.top

C#:   Task.Run(() => F());
来源：http://eng.zhongyouzk.top

[O02] 使用线程池
来源：http://tqy.shanyushiyangtech.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://msu.fehbvm.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ryb.meibo888.top

JS:   // worker_threads 线程池
来源：http://eso.kuanghao11.cn

TS:   // worker_threads 线程池
来源：http://mzp.c1oappe.top

Java: Executors.newFixedThreadPool(4)
来源：http://tqx.shanyushiyangtech.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bsz.zhijiandao.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ini.hongshengwenyu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rcp.zhengqikj.top

[O03] 加锁保护共享数据
来源：http://mfy.fzhhl.top

Py:   with lock: shared += 1
来源：http://buo.ywan-chungtsiang.top

PHP:  // 用 flock() 做文件锁
来源：http://dka.yangfankeji.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://trk.nanxuanxn.top

TS:   // 同 JS
来源：http://eqe.pengpengdd.cyou

Java: synchronized (this) { shared++; }
来源：http://rvm.hesvh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dgg.zhongyouzk.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://grs.nanxuanxn.top

C#:   lock (gate) { shared++; }
来源：http://dua.meibo888.top

[O04] 定义异步函数并等待
来源：http://dba.jinghuilouyu.cn

Py:   async def f():⏎    await g()
来源：http://ksk.9152youxi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vqo.guannengcc.top

JS:   async function f() { await g(); }
来源：http://byt.shuidangran.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wuk.nanxuanxn.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kga.ydjk.org.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tph.zhijiandao.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hrp.shanyushiyangtech.top

C#:   async Task F() { await G(); }
来源：http://nrn.hcnkem.com

[O05] 并发执行并等待全部完成
来源：http://ynd.uphjek.com

Py:   asyncio.gather(*tasks)
来源：http://kmr.yanxiufei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fdw.hammf.cn

JS:   await Promise.all(tasks)
来源：http://zyk.vqdsnc.cn

TS:   await Promise.all(tasks)
来源：http://gxm.zhaomingkeji.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ajg.ydjk.org.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qeo.jlsjyb.cn

Ruby: threads.map(&:join)
来源：http://lhb.ivvv.top

C#:   await Task.WhenAll(t1, t2)
来源：http://egi.ybcxt.top


<!-- 参考信息 -->