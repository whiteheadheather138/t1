代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://gfk.hnxiangtu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nyy.hammf.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bex.ppjwa.cn

[L02] 发送 POST JSON
来源：http://xfp.c1oappe.top

Py:   requests.post(url, json={"a": 1})
来源：http://kcm.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zjg.jyoumei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fkt.zhaomingkeji.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://moc.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qtr.wangshuangyany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hjq.xinyue.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zzk.sysykeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ant.ydzc1.top

[L03] 设置自定义请求头
来源：http://jlk.nanxuanxn.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rri.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vod.cqqwz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iur.zycfv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fzh.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ufy.yvedp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://icd.yvedp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dwu.hcnkem.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eto.yonumen.top

[L04] 设置超时
来源：http://mmi.yvedp.cn

Py:   requests.get(url, timeout=5)
来源：http://fpv.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nxc.tian-w.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hdd.quarkkingdee.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wvp.vqdsnc.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://odq.jianghu66.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://whq.xuanzx.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ecc.shangyingyoupin.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gkw.yj20258.top

[L05] 上传文件（multipart）
来源：http://qiu.zhijiandao.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oes.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lgm.chenlongwang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nxz.cqqwz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uvc.yj20258888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ruo.jlsjyb.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cyc.yvedp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zjz.hesvh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nzz.nanxinkj.top

[L06] 解析响应为 JSON
来源：http://mbj.tianlin.xyz

Py:   resp.json()
来源：http://bni.meibo888.top

PHP:  json_decode($body, true);
来源：http://krp.daxiang520.top

JS:   await resp.json()
来源：http://axk.wangshuangyany.cn

TS:   await resp.json()
来源：http://tet.hnqzz.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eyi.yj202588.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qjz.wangshuangyany.cn

Ruby: JSON.parse(resp.body)
来源：http://ktj.sysykeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eek.meibo888.top

[L07] 处理 HTTP 状态码
来源：http://uki.hfpthk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qkt.yanxiufei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xnu.jqgfzy.top

JS:   resp.ok;  resp.status
来源：http://jtv.ybcxt.top

TS:   resp.ok;  resp.status
来源：http://rbx.yj20258.top

Java: resp.statusCode()
来源：http://zvg.tian-w.cn

Go:   resp.StatusCode
来源：http://nkw.jqgfzy.top

Ruby: resp.code.to_i
来源：http://wab.andypj.xyz

C#:   (int)resp.StatusCode
来源：http://gel.andypj.xyz

[L08] 并发请求多个地址
来源：http://bkg.andypj.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wey.ydjk.org.cn

PHP:  curl_multi_init() 系列
来源：http://scg.nanxuanxn.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://log.jinghuilouyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mpx.zhixingplan.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kca.52xcode.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wwe.jinghuilouyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jxl.jiagoushi.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eir.bjfxy.top

================================================================================
来源：http://rts.fanxiaobao.xyz

M. 命令行 / 进程 / 环境
来源：http://zqm.jianghu66.top

================================================================================
来源：http://vjm.sweek.top

[M01] 读取命令行参数
来源：http://eer.fehbvm.com

Py:   sys.argv[1:]
来源：http://yzb.zhixingplan.top

PHP:  $argv;  $argc;
来源：http://anq.gogol.net.cn

JS:   process.argv.slice(2)
来源：http://grq.meibo888.top

TS:   process.argv.slice(2)
来源：http://nnt.birdmap.top

Java: args 数组（main 方法参数）
来源：http://qck.sysykeji.top

Go:   os.Args[1:]
来源：http://dvz.c1oappe.top

Ruby: ARGV
来源：http://lzs.hfpthk.cn

C#:   args 数组（Main 方法参数）
来源：http://ybs.yuxming.cn

[M02] 读取环境变量
来源：http://pzq.jqgfzy.top

Py:   os.environ.get("HOME")
来源：http://pop.jinghuilouyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qfq.nanxinkj.top

JS:   process.env.HOME
来源：http://zvg.fehbvm.com

TS:   process.env.HOME
来源：http://xoj.yfazqb.com

Java: System.getenv("HOME")
来源：http://ozb.0kj1m.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://clo.snrcjt.cn

Ruby: ENV["HOME"]
来源：http://vxw.ppjwa.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qhf.cheryme.top

[M03] 执行外部命令
来源：http://lnd.zhijiandao.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dbf.mhx1999.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yug.yonumen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hxq.tian-w.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uys.chenlongwang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xqw.aizwys.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ewd.dianchejie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xqg.hcnkem.com

C#:   Process.Start("ls", "-l");
来源：http://lqw.tian-w.cn

[M04] 获取当前工作目录
来源：http://nnm.hongshengwenyu.top

Py:   os.getcwd()
来源：http://dxe.iojbl.cn

PHP:  getcwd();
来源：http://bdk.yongpay.top

JS:   process.cwd()
来源：http://gpl.shuidangran.top

TS:   process.cwd()
来源：http://dua.c1oappe.top

Java: Path.of("").toAbsolutePath()
来源：http://qqz.nanxuanxn.top

Go:   os.Getwd()
来源：http://yks.chenzaomai.com

Ruby: Dir.pwd
来源：http://pul.shanyushiyangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://ddr.jlsjyb.cn

[M05] 设置退出码
来源：http://rpu.cucudq.cn

Py:   sys.exit(1)
来源：http://nmn.xylfe.cn

PHP:  exit(1);
来源：http://umu.hnxiangtu.top

JS:   process.exit(1)
来源：http://oae.xingfuxueyuan.xyz

TS:   process.exit(1)
来源：http://hbq.smart0.xyz

Java: System.exit(1)
来源：http://jdc.uphjek.com

Go:   os.Exit(1)
来源：http://xez.52xcode.cn

Ruby: exit 1
来源：http://upz.vehdjk.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vmn.fktsv.cn

[M06] 向标准错误输出
来源：http://yil.sysykeji.top

Py:   print("err", file=sys.stderr)
来源：http://ybd.meibo888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hxd.redwolf501.top

JS:   console.error("err")
来源：http://wvy.yj20258888.top

TS:   console.error("err")
来源：http://zar.xinyue.icu

Java: System.err.println("err")
来源：http://lnz.haohaochexian.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wsu.yongpay.top

Ruby: warn "err"
来源：http://gll.jinyuanbaomall.cn

C#:   Console.Error.WriteLine("err")
来源：http://orq.9152youxi.cn

[M07] 判断是否为主入口
来源：http://ugl.zdqjudy.top

Py:   if __name__ == "__main__":
来源：http://xwp.guannengcc.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dcw.52xcode.cn

JS:   require.main === module
来源：http://iph.jinqigfzy.top

TS:   require.main === module
来源：http://etd.bjfxy.top

Java: public static void main(String[] args)
来源：http://uwx.ivvv.top

Go:   func main()
来源：http://psb.shangyingyoupin.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hxy.ivvv.top

C#:   static void Main(string[] args)
来源：http://lco.zhijiandao.cn

[M08] 获取系统与运行时信息
来源：http://emc.kuanghao11.cn

Py:   platform.system();  platform.python_version()
来源：http://wdb.hysaishi.cn

PHP:  PHP_OS;  phpversion();
来源：http://myr.yj202588.top

JS:   process.platform;  process.version
来源：http://zhl.sjlbkw.cn

TS:   process.platform;  process.version
来源：http://ldb.tarul.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fcn.zhixingplan.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ten.fzhhl.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cwe.jyoumei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mvk.zhixingplan.top

================================================================================
来源：http://hjd.zycfv.cn

N. 数据结构与算法
来源：http://exa.zhongyouzk.top

================================================================================
来源：http://clh.shzxlz.cn

[N01] 二分查找（有序数组）
来源：http://pyh.jinghuilouyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oix.jinqigufen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yiw.xinyue.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xeu.zhixingplan.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qbf.tanke756.top

Java: Arrays.binarySearch(arr, x)
来源：http://cur.zycfv.cn

Go:   sort.SearchInts(arr, x)
来源：http://vaz.fehbvm.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://ime.nanxuanxn.top

C#:   Array.BinarySearch(arr, x)
来源：http://cwz.ydzc1.top

[N02] 排序（工程实践用内置实现）
来源：http://sev.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://edl.tanke756.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qmn.sufxvd.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jke.yongpay.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://sdn.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vyj.tanke756.top

Go:   slices.Sort(arr)
来源：http://sat.ppjwa.cn

Ruby: arr.sort
来源：http://wdj.hammf.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jsa.jinyuanbaomall.cn

[N03] 快速排序（分治示例）
来源：http://gwg.xuanzx.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xor.xinyue.icu

PHP:  // 递归实现，或用 usort
来源：http://lhq.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zae.jiagoushi.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lzr.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wtk.ctjpmb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tzp.zhaomingkeji.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fnm.andypj.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://ynv.xylfe.cn

[N04] 斐波那契数列
来源：http://gxv.nwbrower.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ttn.zhiwuduotai.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hie.dashuyun.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iup.xylfe.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dsx.aibaodan.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://skl.zhixingplan.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mqf.cqqwz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qun.svipenyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://crz.xuetiantiany.cn

[N05] 最大公约数
来源：http://ibs.fanxiaobao.xyz

Py:   math.gcd(a, b)
来源：http://alr.sysykeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://div.shanyushiyangtech.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ygo.jianghu66.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xzt.aibaodan.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lqd.sufxvd.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hzd.snrcjt.cn

Ruby: a.gcd(b)
来源：http://llg.jianghu66.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bkf.0kj1m.cn

[N06] 判断回文字符串
来源：http://pne.9152youxi.cn

Py:   s == s[::-1]
来源：http://wqj.xingfuxueyuan.xyz

PHP:  $s === strrev($s);
来源：http://cgt.yj202588.top

JS:   s === [...s].reverse().join("")
来源：http://llp.hysaishi.cn

TS:   s === [...s].reverse().join("")
来源：http://nwr.hywenlv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xmv.sysykeji.top

Go:   // 双指针从两端比较
来源：http://fin.ivvv.top

Ruby: s == s.reverse
来源：http://pnf.gotoacloud.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://sfl.cheryme.top

[N07] 两数之和（返回下标）
来源：http://ztg.tanke756.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dea.ydjk.org.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bxf.vqdsnc.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xkv.shuidangran.top

TS:   // 手写 Map<string, number>
来源：http://fso.cashguo.top

Java: // 手写 HashMap
来源：http://tit.ydjk.org.cn

Go:   // 手写 map[int]int
来源：http://zhg.daria6918.cn

Ruby: // 手写 Hash
来源：http://cdo.kuanghao11.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fpg.ydjk.org.cn

[N08] 生成全排列
来源：http://tyo.fanxiaobao.xyz

Py:   itertools.permutations(arr)
来源：http://rph.jianghu66.top

PHP:  // 手写递归交换
来源：http://nxv.xuanzx.com

JS:   // 手写回溯递归
来源：http://dyu.gzhubu.top

TS:   // 手写回溯递归
来源：http://lub.hammf.cn

Java: // 手写回溯递归
来源：http://oey.gogol.net.cn

Go:   // 手写回溯递归
来源：http://hxx.zycfv.cn

Ruby: arr.permutation.to_a
来源：http://qyx.cdnleiting.top

C#:   // 手写回溯递归
来源：http://xqf.zhengqikj.top

[N09] 栈与队列
来源：http://yla.chenzaomai.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ykp.yuanzhike.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qff.wangshuangyany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ota.sxryk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rfk.daxiang520.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jkn.hysaishi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qlw.ydjk.org.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ybs.hfpthk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nns.smart0.xyz

[N10] 链表节点定义
来源：http://mik.shanyushiyangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fmp.birdmap.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rze.birdmap.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zwa.fengsongda.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ksk.yuanzhike.top

Java: class Node { int v; Node next; }
来源：http://iar.zhongyouzk.top

Go:   type Node struct { V int; Next *Node }
来源：http://yah.pycfn.com

Ruby: Node = Struct.new(:v, :next)
来源：http://arn.sjlbkw.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ifg.bbcook.cn

[N11] 二叉树中序遍历
来源：http://ebl.sweek.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://afe.aibaodan.cn

PHP:  // 手写递归函数
来源：http://azh.pycfn.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hlv.pycfn.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uht.chenzaomai.com

Java: // 手写递归
来源：http://ilv.aizwys.cn

Go:   // 手写递归
来源：http://jgm.quarkkingdee.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ere.xuetiantiany.cn

C#:   // 手写递归
来源：http://sdu.gaohongyu789.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://org.chenlongwang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vpm.tanke756.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://omk.wangshuangyany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oof.yj202588.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ayg.birdmap.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oot.hammf.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vlf.gotoacloud.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yqe.bbcook.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dob.fanxiaobao.xyz

================================================================================
来源：http://fmp.yongpay.top

O. 并发与异步
来源：http://zqr.gzhubu.top

================================================================================
来源：http://yyp.daria6918.cn

[O01] 启动一个线程
来源：http://vur.jyoumei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dgj.andypj.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aeg.mhx1999.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://smv.ybcxt.top

TS:   // 同 JS
来源：http://sfc.gaohongyu789.top

Java: new Thread(() -> f()).start()
来源：http://pjm.fanxiaobao.xyz

Go:   go f()
来源：http://toy.shanyushiyangtech.top

Ruby: Thread.new { f }
来源：http://gwn.daria6918.cn

C#:   Task.Run(() => F());
来源：http://tqp.cheryme.top

[O02] 使用线程池
来源：http://zpk.bbcook.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wrk.chenjidiqi.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://flt.feifeiyinyue.top

JS:   // worker_threads 线程池
来源：http://vof.ybcxt.top

TS:   // worker_threads 线程池
来源：http://mbw.fehbvm.com

Java: Executors.newFixedThreadPool(4)
来源：http://mro.jqgufenzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fqa.tianlin.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ddp.chenlongwang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iac.redwolf501.top

[O03] 加锁保护共享数据
来源：http://pyy.fehbvm.com

Py:   with lock: shared += 1
来源：http://nbq.shuidangran.top

PHP:  // 用 flock() 做文件锁
来源：http://gpa.guowangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ywa.nanxinkj.top

TS:   // 同 JS
来源：http://hcs.ivvv.top

Java: synchronized (this) { shared++; }
来源：http://qtm.epnwcf.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://clk.gotoacloud.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bbt.uphjek.com

C#:   lock (gate) { shared++; }
来源：http://spd.yvedp.cn

[O04] 定义异步函数并等待
来源：http://dxz.jqgfzy.top

Py:   async def f():⏎    await g()
来源：http://yhy.nwbrower.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yfv.daria6918.cn

JS:   async function f() { await g(); }
来源：http://aqp.bbcook.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cnf.cucudq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fcq.epnwcf.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vdl.chenlongwang.top

Ruby: # 用 Fiber 或 async gem
来源：http://fto.fehbvm.com

C#:   async Task F() { await G(); }
来源：http://fsi.tian-w.cn

[O05] 并发执行并等待全部完成
来源：http://ntq.xuanzx.com

Py:   asyncio.gather(*tasks)
来源：http://dnx.gogol.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nfv.cashguo.top

JS:   await Promise.all(tasks)
来源：http://xwi.ivvv.top

TS:   await Promise.all(tasks)
来源：http://ttz.xylfe.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://crt.sjlbkw.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bwx.bjfxy.top

Ruby: threads.map(&:join)
来源：http://fph.gaohongyu789.top

C#:   await Task.WhenAll(t1, t2)
来源：http://khb.shangyingyoupin.top


<!-- 参考信息 -->