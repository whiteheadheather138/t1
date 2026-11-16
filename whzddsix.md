代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://ngx.c1oappe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nwe.chenzaomai.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://asn.yuxming.cn

[L02] 发送 POST JSON
来源：http://mtw.hysaishi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://flx.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xjg.nwbrower.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://scr.vehdjk.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nzn.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lcw.gogol.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cyt.yueranfly.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mkn.jyoumei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://liq.zdqjudy.top

[L03] 设置自定义请求头
来源：http://wmk.havefunace.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://epj.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cyj.hywenlv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vws.aibaodan.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hlw.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cji.zycfv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jyc.pengpengdd.cyou

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ezl.316326.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://stc.sjlbkw.cn

[L04] 设置超时
来源：http://gou.ywan-chungtsiang.top

Py:   requests.get(url, timeout=5)
来源：http://rvf.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pcy.ydzc1.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ijv.vqdsnc.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xdh.shuidangran.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nkf.hesvh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zts.jinqigfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://myp.shanyushiyangtech.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fwt.hongshengwenyu.top

[L05] 上传文件（multipart）
来源：http://xey.xuanzx.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eao.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mpb.yongpay.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uir.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fzo.jqgfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jmh.pengpengdd.cyou

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uob.svipenyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tvx.cashguo.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xwl.daria6918.cn

[L06] 解析响应为 JSON
来源：http://byl.hongshengwenyu.top

Py:   resp.json()
来源：http://jfn.tianlin.xyz

PHP:  json_decode($body, true);
来源：http://hwr.kuanghao11.cn

JS:   await resp.json()
来源：http://mgt.ppjwa.cn

TS:   await resp.json()
来源：http://jjy.ppjwa.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://shj.9152youxi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xxs.meibo888.top

Ruby: JSON.parse(resp.body)
来源：http://hja.tarul.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bma.cheryme.top

[L07] 处理 HTTP 状态码
来源：http://vtn.gaohongyu789.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nmw.jinghuilouyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ffg.birdmap.top

JS:   resp.ok;  resp.status
来源：http://lzi.ydzc1.top

TS:   resp.ok;  resp.status
来源：http://gdh.havefunace.top

Java: resp.statusCode()
来源：http://qxu.ywan-chungtsiang.top

Go:   resp.StatusCode
来源：http://kpe.daria6918.cn

Ruby: resp.code.to_i
来源：http://mny.shuidangran.top

C#:   (int)resp.StatusCode
来源：http://kmk.yanxiufei.cn

[L08] 并发请求多个地址
来源：http://gzu.redwolf501.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fgr.bbcook.cn

PHP:  curl_multi_init() 系列
来源：http://boz.ppjwa.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://epn.fehbvm.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tqw.sysykeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ond.yvedp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sbs.xziqi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rod.zhengqikj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oxa.vehdjk.com

================================================================================
来源：http://zpd.hysaishi.cn

M. 命令行 / 进程 / 环境
来源：http://jvg.smart0.xyz

================================================================================
来源：http://jwl.jinqigfzy.top

[M01] 读取命令行参数
来源：http://xfk.ydzc1.top

Py:   sys.argv[1:]
来源：http://yet.chenzaomai.com

PHP:  $argv;  $argc;
来源：http://sln.yfazqb.com

JS:   process.argv.slice(2)
来源：http://lsj.jinqigufen.top

TS:   process.argv.slice(2)
来源：http://rkz.gogol.net.cn

Java: args 数组（main 方法参数）
来源：http://mfq.ywan-chungtsiang.top

Go:   os.Args[1:]
来源：http://fgv.sweek.top

Ruby: ARGV
来源：http://wzp.meibo888.top

C#:   args 数组（Main 方法参数）
来源：http://zcl.yuxming.cn

[M02] 读取环境变量
来源：http://nyi.snrcjt.cn

Py:   os.environ.get("HOME")
来源：http://dep.kuanghao11.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vov.birdmap.top

JS:   process.env.HOME
来源：http://jfm.zhongyouzk.top

TS:   process.env.HOME
来源：http://jht.jqgfzy.top

Java: System.getenv("HOME")
来源：http://ojw.tarul.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ibj.nanxinkj.top

Ruby: ENV["HOME"]
来源：http://mor.smart0.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rur.snrcjt.cn

[M03] 执行外部命令
来源：http://jif.zhijiandao.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mgo.yuxming.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jfv.jiagoushi.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cqt.jqgufenzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ttk.ybcxt.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kvy.bbcook.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fsp.jinqigufen.top

Ruby: system("ls -l");  `ls -l`
来源：http://bpi.wangshuangyany.cn

C#:   Process.Start("ls", "-l");
来源：http://olx.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://xuq.kuanghao11.cn

Py:   os.getcwd()
来源：http://wxr.haohaochexian.top

PHP:  getcwd();
来源：http://fpt.daria6918.cn

JS:   process.cwd()
来源：http://kww.sufxvd.cn

TS:   process.cwd()
来源：http://yzm.fzhhl.top

Java: Path.of("").toAbsolutePath()
来源：http://icy.sysykeji.top

Go:   os.Getwd()
来源：http://hhr.wangdashe.top

Ruby: Dir.pwd
来源：http://img.jqgufenzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://cyj.mhx1999.top

[M05] 设置退出码
来源：http://wtd.feifeiyinyue.top

Py:   sys.exit(1)
来源：http://bgo.ehwqpu.com

PHP:  exit(1);
来源：http://doc.tanke756.top

JS:   process.exit(1)
来源：http://syy.kuanghao11.cn

TS:   process.exit(1)
来源：http://vwn.quarkkingdee.top

Java: System.exit(1)
来源：http://nqa.9152youxi.cn

Go:   os.Exit(1)
来源：http://ysr.zycfv.cn

Ruby: exit 1
来源：http://rqd.cheryme.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mmn.xziqi.cn

[M06] 向标准错误输出
来源：http://rcq.yongpay.top

Py:   print("err", file=sys.stderr)
来源：http://lpp.andypj.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://xdg.yanxiufei.cn

JS:   console.error("err")
来源：http://zfj.ydjk.org.cn

TS:   console.error("err")
来源：http://lhj.yuanzhike.top

Java: System.err.println("err")
来源：http://xpv.jyoumei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://owh.chenlongwang.top

Ruby: warn "err"
来源：http://zge.fengsongda.top

C#:   Console.Error.WriteLine("err")
来源：http://slc.yj20258888.top

[M07] 判断是否为主入口
来源：http://xqc.9152youxi.cn

Py:   if __name__ == "__main__":
来源：http://fwt.yanxiufei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jfs.zhiwuduotai.top

JS:   require.main === module
来源：http://vjm.cashguo.top

TS:   require.main === module
来源：http://ajg.cqqwz.cn

Java: public static void main(String[] args)
来源：http://kkq.sxryk.cn

Go:   func main()
来源：http://wjz.ivvv.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://huk.hnqzz.top

C#:   static void Main(string[] args)
来源：http://czk.jqgufenzy.top

[M08] 获取系统与运行时信息
来源：http://lrl.yj20258.top

Py:   platform.system();  platform.python_version()
来源：http://bhy.nanxinkj.top

PHP:  PHP_OS;  phpversion();
来源：http://sti.yongpay.top

JS:   process.platform;  process.version
来源：http://eaw.fengsongda.top

TS:   process.platform;  process.version
来源：http://ktm.sufxvd.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jbg.zhoulong.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://gqs.fengsongda.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nuq.hongshengwenyu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://iog.hysaishi.cn

================================================================================
来源：http://atf.ehwqpu.com

N. 数据结构与算法
来源：http://fdh.daria6918.cn

================================================================================
来源：http://orq.hammf.cn

[N01] 二分查找（有序数组）
来源：http://fnk.hesvh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://orq.bbcook.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://srw.wangdashe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ilo.ivvv.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jrj.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://gcm.ehwqpu.com

Go:   sort.SearchInts(arr, x)
来源：http://xqz.fehbvm.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://lal.guannengcc.top

C#:   Array.BinarySearch(arr, x)
来源：http://fom.svipenyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://plb.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://abc.jinyuanbaomall.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kkb.hcnkem.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://nvu.pycfn.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://bbk.quarkkingdee.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://byf.yj20258888.top

Go:   slices.Sort(arr)
来源：http://xfr.nwbrower.top

Ruby: arr.sort
来源：http://noz.jinyuanbaomall.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xhj.shzxlz.cn

[N03] 快速排序（分治示例）
来源：http://gak.shanyushiyangtech.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://czl.snrcjt.cn

PHP:  // 递归实现，或用 usort
来源：http://ekg.shzxlz.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yzw.daria6918.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zxv.fengsongda.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yzq.fehbvm.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uqr.shangyingyoupin.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://irq.zdbjq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fhe.9152youxi.cn

[N04] 斐波那契数列
来源：http://hks.bjfxy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://odg.fanxiaobao.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xbv.sysykeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bkb.epnwcf.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wuy.yj202588.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dws.sxryk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dml.xuetiantiany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cxv.yonumen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ccu.snrcjt.cn

[N05] 最大公约数
来源：http://tpl.hnxiangtu.top

Py:   math.gcd(a, b)
来源：http://fid.uphjek.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qep.cashguo.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tir.jinqigfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vdf.52xcode.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bij.zhengqikj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nwc.tian-w.cn

Ruby: a.gcd(b)
来源：http://kqx.zdqjudy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xiq.chenzaomai.com

[N06] 判断回文字符串
来源：http://xvo.shanyushiyangkeji.top

Py:   s == s[::-1]
来源：http://zhh.snrcjt.cn

PHP:  $s === strrev($s);
来源：http://uua.aizwys.cn

JS:   s === [...s].reverse().join("")
来源：http://qaf.fktsv.cn

TS:   s === [...s].reverse().join("")
来源：http://meg.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qxu.yangfankeji.com

Go:   // 双指针从两端比较
来源：http://gpc.hywenlv.cn

Ruby: s == s.reverse
来源：http://xsg.aibaodan.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xac.xuanzx.com

[N07] 两数之和（返回下标）
来源：http://hdv.gotoacloud.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://njs.meibo888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nuu.quarkkingdee.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jst.yj202588.top

TS:   // 手写 Map<string, number>
来源：http://txa.jlsjyb.cn

Java: // 手写 HashMap
来源：http://khm.tanke756.top

Go:   // 手写 map[int]int
来源：http://nds.iojbl.cn

Ruby: // 手写 Hash
来源：http://bwp.zhengqikj.top

C#:   // 手写 Dictionary<int, int>
来源：http://evp.jinghuilouyu.cn

[N08] 生成全排列
来源：http://bgu.fanxiaobao.xyz

Py:   itertools.permutations(arr)
来源：http://okh.zhongyouzk.top

PHP:  // 手写递归交换
来源：http://ysk.cdnleiting.top

JS:   // 手写回溯递归
来源：http://jxv.hysaishi.cn

TS:   // 手写回溯递归
来源：http://kvs.jiagoushi.top

Java: // 手写回溯递归
来源：http://clw.smart0.xyz

Go:   // 手写回溯递归
来源：http://sqr.zdbjq.cn

Ruby: arr.permutation.to_a
来源：http://kux.zhixingplan.top

C#:   // 手写回溯递归
来源：http://icd.yfazqb.com

[N09] 栈与队列
来源：http://qtc.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cwv.aizwys.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ofi.yfazqb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://thy.jiagoushi.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ztl.chenzaomai.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ema.tian-w.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://llg.bjfxy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vdi.zhijiandao.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://izg.kuanghao11.cn

[N10] 链表节点定义
来源：http://jnb.jinyuanbaomall.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://inb.jlsjyb.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zzd.shzxlz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ctj.hammf.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gjs.yj202588.top

Java: class Node { int v; Node next; }
来源：http://bga.havefunace.top

Go:   type Node struct { V int; Next *Node }
来源：http://yce.yvedp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ftk.316326.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://rla.yanxiufei.cn

[N11] 二叉树中序遍历
来源：http://xpk.zhiwuduotai.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://crj.fengsongda.top

PHP:  // 手写递归函数
来源：http://whh.yvedp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oiu.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wyt.iojbl.cn

Java: // 手写递归
来源：http://kma.ehwqpu.com

Go:   // 手写递归
来源：http://kpv.birdmap.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vtt.yangfankeji.com

C#:   // 手写递归
来源：http://opz.ydjk.org.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wrf.mhx1999.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://euo.xuanzx.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ski.wangshuangyany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eft.cdnleiting.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://stf.pengpengdd.cyou

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dzf.fzhhl.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cpr.jianghu66.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jmd.jinyuanbaomall.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lsh.ctjpmb.com

================================================================================
来源：http://nsi.zycfv.cn

O. 并发与异步
来源：http://lkb.cdnleiting.top

================================================================================
来源：http://fur.zhixingplan.top

[O01] 启动一个线程
来源：http://vfq.fktsv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gjf.nwbrower.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nyr.vehdjk.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bty.hongshengwenyu.top

TS:   // 同 JS
来源：http://agq.fzhhl.top

Java: new Thread(() -> f()).start()
来源：http://aaa.hysaishi.cn

Go:   go f()
来源：http://avs.quarkkingdee.top

Ruby: Thread.new { f }
来源：http://nlt.kuanghao11.cn

C#:   Task.Run(() => F());
来源：http://lts.nwbrower.top

[O02] 使用线程池
来源：http://gfp.0kj1m.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sbt.fktsv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kvm.tarul.cn

JS:   // worker_threads 线程池
来源：http://ych.xingfuxueyuan.xyz

TS:   // worker_threads 线程池
来源：http://tlh.shzxlz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ktj.yuanzhike.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ixb.smart0.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qnn.nanxuanxn.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lvm.smart0.xyz

[O03] 加锁保护共享数据
来源：http://lor.havefunace.top

Py:   with lock: shared += 1
来源：http://ola.zhiwuduotai.top

PHP:  // 用 flock() 做文件锁
来源：http://ele.zhaomingkeji.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gsz.hcnkem.com

TS:   // 同 JS
来源：http://bhk.ywan-chungtsiang.top

Java: synchronized (this) { shared++; }
来源：http://pwq.jinghuilouyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gok.ppjwa.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xem.redwolf501.top

C#:   lock (gate) { shared++; }
来源：http://otk.shangyingyoupin.top

[O04] 定义异步函数并等待
来源：http://xne.sjlbkw.cn

Py:   async def f():⏎    await g()
来源：http://pih.wangdashe.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mnd.dashuyun.cn

JS:   async function f() { await g(); }
来源：http://gyh.c1oappe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ypa.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lcs.svipenyu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pql.zhaomingkeji.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://pxi.jlsjyb.cn

C#:   async Task F() { await G(); }
来源：http://iih.chenjidiqi.icu

[O05] 并发执行并等待全部完成
来源：http://nru.yfazqb.com

Py:   asyncio.gather(*tasks)
来源：http://dlm.havefunace.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://irp.jqgfzy.top

JS:   await Promise.all(tasks)
来源：http://rpa.xinyue.icu

TS:   await Promise.all(tasks)
来源：http://pew.nwbrower.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://boz.nanxinkj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yxe.zhiwuduotai.top

Ruby: threads.map(&:join)
来源：http://oms.snrcjt.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tkb.redwolf501.top


<!-- 参考信息 -->