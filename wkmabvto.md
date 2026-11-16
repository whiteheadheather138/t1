代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rny.guowangkeji.top

JS:   await fetch(url)
来源：http://sck.jinqigufen.top

TS:   await fetch(url)
来源：http://yni.fktsv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://djc.haohaochexian.top

Go:   resp, err := http.Get(url)
来源：http://xbh.ydjk.org.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fqy.fengsongda.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ytu.yuanzhike.top

[L02] 发送 POST JSON
来源：http://hcq.fehbvm.com

Py:   requests.post(url, json={"a": 1})
来源：http://zsf.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vid.wangdashe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yha.bjfxy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eph.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xjn.gaohongyu789.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kta.cqqwz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ddi.nanxuanxn.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xie.dashuyun.cn

[L03] 设置自定义请求头
来源：http://pkt.gogol.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dll.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eim.shuidangran.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://agr.zdbjq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nwx.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sib.yj202588.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yqu.hywenlv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://leg.yanxiufei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hmu.yongpay.top

[L04] 设置超时
来源：http://lje.guannengcc.top

Py:   requests.get(url, timeout=5)
来源：http://wqr.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pqe.guannengcc.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vwf.sysykeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tiy.chenzaomai.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ayj.xingfuxueyuan.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.jqgfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fiu.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pqa.chenlongwang.top

[L05] 上传文件（multipart）
来源：http://jcc.wangshuangyany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rao.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qhx.shanyushiyangtech.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pzh.uphjek.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vri.hnqzz.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rew.pycfn.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ntg.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://foi.vqdsnc.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ddk.jinqigfzy.top

[L06] 解析响应为 JSON
来源：http://aeq.aibaodan.cn

Py:   resp.json()
来源：http://mpe.zhijiandao.cn

PHP:  json_decode($body, true);
来源：http://fco.wangshuangyany.cn

JS:   await resp.json()
来源：http://tsi.zhiwuduotai.top

TS:   await resp.json()
来源：http://hcy.hfpthk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ibl.zhongyouzk.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hcd.dianchejie.cn

Ruby: JSON.parse(resp.body)
来源：http://dsb.jqgufenzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wth.nwbrower.top

[L07] 处理 HTTP 状态码
来源：http://tad.chenjidiqi.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ybp.gaohongyu789.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://caz.nanxuanxn.top

JS:   resp.ok;  resp.status
来源：http://uxn.quarkkingdee.top

TS:   resp.ok;  resp.status
来源：http://zlv.shuidangran.top

Java: resp.statusCode()
来源：http://rjq.ehwqpu.com

Go:   resp.StatusCode
来源：http://yzx.epnwcf.com

Ruby: resp.code.to_i
来源：http://rqy.yangfankeji.com

C#:   (int)resp.StatusCode
来源：http://jst.dianchejie.cn

[L08] 并发请求多个地址
来源：http://ovl.jlsjyb.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lps.ydzc1.top

PHP:  curl_multi_init() 系列
来源：http://qgw.hongshengwenyu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ntx.hywenlv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ove.ybcxt.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sjb.ppjwa.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lvj.redwolf501.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sbn.ywan-chungtsiang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qne.chenzaomai.com

================================================================================
来源：http://shr.yanxiufei.cn

M. 命令行 / 进程 / 环境
来源：http://eyd.nanxinkj.top

================================================================================
来源：http://umb.nanxuanxn.top

[M01] 读取命令行参数
来源：http://kdg.hywenlv.cn

Py:   sys.argv[1:]
来源：http://dew.gotoacloud.top

PHP:  $argv;  $argc;
来源：http://xdk.gotoacloud.top

JS:   process.argv.slice(2)
来源：http://aki.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://how.wangshuangyany.cn

Java: args 数组（main 方法参数）
来源：http://fgo.zhixingplan.top

Go:   os.Args[1:]
来源：http://hyx.tianlin.xyz

Ruby: ARGV
来源：http://xwz.wangshuangyany.cn

C#:   args 数组（Main 方法参数）
来源：http://ckw.jinqigfzy.top

[M02] 读取环境变量
来源：http://olv.svipenyu.cn

Py:   os.environ.get("HOME")
来源：http://ytc.tian-w.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kom.jianghu66.top

JS:   process.env.HOME
来源：http://gjv.dashuyun.cn

TS:   process.env.HOME
来源：http://pxy.jiagoushi.top

Java: System.getenv("HOME")
来源：http://lvv.iojbl.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://epk.xziqi.cn

Ruby: ENV["HOME"]
来源：http://uvy.vehdjk.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vtc.fengsongda.top

[M03] 执行外部命令
来源：http://ike.tianlin.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://esd.yvedp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hsz.nanxinkj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dad.xuanzx.com

TS:   child_process.execSync("ls -l").toString()
来源：http://dcj.vqdsnc.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ikx.shangyingyoupin.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jqm.cucudq.cn

Ruby: system("ls -l");  `ls -l`
来源：http://izj.nanxinkj.top

C#:   Process.Start("ls", "-l");
来源：http://gin.jlsjyb.cn

[M04] 获取当前工作目录
来源：http://hlq.sweek.top

Py:   os.getcwd()
来源：http://egd.sufxvd.cn

PHP:  getcwd();
来源：http://ale.iojbl.cn

JS:   process.cwd()
来源：http://bmr.xingfuxueyuan.xyz

TS:   process.cwd()
来源：http://rad.wangdashe.top

Java: Path.of("").toAbsolutePath()
来源：http://fpa.daxiang520.top

Go:   os.Getwd()
来源：http://rli.jinqigfzy.top

Ruby: Dir.pwd
来源：http://wbi.meibo888.top

C#:   Directory.GetCurrentDirectory()
来源：http://ehw.chenzaomai.com

[M05] 设置退出码
来源：http://hrn.quarkkingdee.top

Py:   sys.exit(1)
来源：http://ltv.zdbjq.cn

PHP:  exit(1);
来源：http://qhj.jyoumei.cn

JS:   process.exit(1)
来源：http://djz.cdnleiting.top

TS:   process.exit(1)
来源：http://eaa.9152youxi.cn

Java: System.exit(1)
来源：http://dff.haohaochexian.top

Go:   os.Exit(1)
来源：http://hht.zhiwuduotai.top

Ruby: exit 1
来源：http://ivy.quarkkingdee.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ony.yueranfly.top

[M06] 向标准错误输出
来源：http://tvd.hnxiangtu.top

Py:   print("err", file=sys.stderr)
来源：http://xbi.hammf.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lya.gaohongyu789.top

JS:   console.error("err")
来源：http://htt.xuetiantiany.cn

TS:   console.error("err")
来源：http://tzo.shuidangran.top

Java: System.err.println("err")
来源：http://uda.dashuyun.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://emh.gotoacloud.top

Ruby: warn "err"
来源：http://oai.zdqjudy.top

C#:   Console.Error.WriteLine("err")
来源：http://spk.yvedp.cn

[M07] 判断是否为主入口
来源：http://fzp.yfazqb.com

Py:   if __name__ == "__main__":
来源：http://wng.tian-w.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ktn.feifeiyinyue.top

JS:   require.main === module
来源：http://pqu.yvedp.cn

TS:   require.main === module
来源：http://jvp.hammf.cn

Java: public static void main(String[] args)
来源：http://drh.fanxiaobao.xyz

Go:   func main()
来源：http://fxd.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mdl.yvedp.cn

C#:   static void Main(string[] args)
来源：http://uki.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://wbk.fktsv.cn

Py:   platform.system();  platform.python_version()
来源：http://egh.c1oappe.top

PHP:  PHP_OS;  phpversion();
来源：http://jty.gaohongyu789.top

JS:   process.platform;  process.version
来源：http://dvr.xziqi.cn

TS:   process.platform;  process.version
来源：http://gam.yuanzhike.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ybo.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zuo.cdnleiting.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sui.chenjidiqi.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://hwy.hysaishi.cn

================================================================================
来源：http://mhu.chenlongwang.top

N. 数据结构与算法
来源：http://iog.xylfe.cn

================================================================================
来源：http://lqp.epnwcf.com

[N01] 二分查找（有序数组）
来源：http://nzx.gotoacloud.top

Py:   bisect.bisect_left(arr, x)
来源：http://fwf.ywan-chungtsiang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fjc.yueranfly.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vpm.zhixingplan.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gft.yongpay.top

Java: Arrays.binarySearch(arr, x)
来源：http://zpz.guowangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://wun.sysykeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://oyu.jiagoushi.top

C#:   Array.BinarySearch(arr, x)
来源：http://qoe.haohaochexian.top

[N02] 排序（工程实践用内置实现）
来源：http://zqk.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://ran.yueranfly.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://prd.yj202588.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://npb.gogol.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://eit.nwbrower.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eet.aizwys.cn

Go:   slices.Sort(arr)
来源：http://szd.feifeiyinyue.top

Ruby: arr.sort
来源：http://qis.shuidangran.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jjz.jinyuanbaomall.cn

[N03] 快速排序（分治示例）
来源：http://rry.zhiwuduotai.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://flm.uphjek.com

PHP:  // 递归实现，或用 usort
来源：http://eme.guowangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ahu.xuanzx.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xst.pengpengdd.cyou

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jru.shuidangran.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://css.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tyi.zdbjq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fnm.shangyingyoupin.top

[N04] 斐波那契数列
来源：http://ktx.vehdjk.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jmk.yj20258888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gbq.birdmap.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uig.svipenyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ihm.zhiwuduotai.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wqc.smart0.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hcv.cdnleiting.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xod.yuanzhike.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://iby.zdqjudy.top

[N05] 最大公约数
来源：http://ynw.daxiang520.top

Py:   math.gcd(a, b)
来源：http://eoa.jinyuanbaomall.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eyf.ywan-chungtsiang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tkm.daria6918.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ibw.gzhubu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ond.shzxlz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qci.9152youxi.cn

Ruby: a.gcd(b)
来源：http://ffi.yuanzhike.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wpw.haohaochexian.top

[N06] 判断回文字符串
来源：http://zey.fktsv.cn

Py:   s == s[::-1]
来源：http://nav.meibo888.top

PHP:  $s === strrev($s);
来源：http://pag.ywan-chungtsiang.top

JS:   s === [...s].reverse().join("")
来源：http://riu.yonumen.top

TS:   s === [...s].reverse().join("")
来源：http://lib.zhijiandao.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mhn.snrcjt.cn

Go:   // 双指针从两端比较
来源：http://mjq.birdmap.top

Ruby: s == s.reverse
来源：http://cqx.hcnkem.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://yqq.xuetiantiany.cn

[N07] 两数之和（返回下标）
来源：http://otj.chenjidiqi.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vsc.shangyingyoupin.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fqc.cashguo.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fph.feifeiyinyue.top

TS:   // 手写 Map<string, number>
来源：http://qlo.nwbrower.top

Java: // 手写 HashMap
来源：http://dle.nanxinkj.top

Go:   // 手写 map[int]int
来源：http://azj.dashuyun.cn

Ruby: // 手写 Hash
来源：http://qjm.zhiwuduotai.top

C#:   // 手写 Dictionary<int, int>
来源：http://jhd.yangfankeji.com

[N08] 生成全排列
来源：http://cqm.ppjwa.cn

Py:   itertools.permutations(arr)
来源：http://wmg.iojbl.cn

PHP:  // 手写递归交换
来源：http://klf.cheryme.top

JS:   // 手写回溯递归
来源：http://rhm.hnxiangtu.top

TS:   // 手写回溯递归
来源：http://dlk.nwbrower.top

Java: // 手写回溯递归
来源：http://ftf.shuidangran.top

Go:   // 手写回溯递归
来源：http://lqw.fanxiaobao.xyz

Ruby: arr.permutation.to_a
来源：http://ody.chenlongwang.top

C#:   // 手写回溯递归
来源：http://fqk.ppjwa.cn

[N09] 栈与队列
来源：http://sbk.fehbvm.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bmp.0kj1m.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hub.xziqi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mcl.chenlongwang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jrg.xuetiantiany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rry.smart0.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cpc.daria6918.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jiz.jqgfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zji.haohaochexian.top

[N10] 链表节点定义
来源：http://omr.yvedp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dwj.shuidangran.top

PHP:  class Node { public $v; public $next = null; }
来源：http://awh.zdqjudy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eez.nanxuanxn.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://abg.jinghuilouyu.cn

Java: class Node { int v; Node next; }
来源：http://kje.hywenlv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sjb.meibo888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://glo.ybcxt.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jnc.hywenlv.cn

[N11] 二叉树中序遍历
来源：http://eip.yvedp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gih.dianchejie.cn

PHP:  // 手写递归函数
来源：http://fpo.zhengqikj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ayv.9152youxi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kds.aibaodan.cn

Java: // 手写递归
来源：http://cbo.aizwys.cn

Go:   // 手写递归
来源：http://dpo.hnxiangtu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eri.birdmap.top

C#:   // 手写递归
来源：http://xzq.hnxiangtu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rfo.yuanzhike.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ysp.jinqigfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bzo.ydjk.org.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jgy.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lai.ppjwa.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lhg.yj20258888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qdi.yanxiufei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fvx.yuxming.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dpf.ivvv.top

================================================================================
来源：http://ipd.hammf.cn

O. 并发与异步
来源：http://czi.shanyushiyangkeji.top

================================================================================
来源：http://unp.redwolf501.top

[O01] 启动一个线程
来源：http://rqr.gogol.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gyf.ppjwa.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aho.cashguo.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qxd.tarul.cn

TS:   // 同 JS
来源：http://gxr.cucudq.cn

Java: new Thread(() -> f()).start()
来源：http://lgi.cheryme.top

Go:   go f()
来源：http://ism.epnwcf.com

Ruby: Thread.new { f }
来源：http://vkc.dashuyun.cn

C#:   Task.Run(() => F());
来源：http://hjv.gaohongyu789.top

[O02] 使用线程池
来源：http://jhj.hongshengwenyu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bbf.vqdsnc.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sxg.jianghu66.top

JS:   // worker_threads 线程池
来源：http://ktx.ivvv.top

TS:   // worker_threads 线程池
来源：http://eud.c1oappe.top

Java: Executors.newFixedThreadPool(4)
来源：http://ulp.pengpengdd.cyou

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://aeq.jinghuilouyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vpo.52xcode.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tjj.fzhhl.top

[O03] 加锁保护共享数据
来源：http://pyh.nanxuanxn.top

Py:   with lock: shared += 1
来源：http://odj.xuetiantiany.cn

PHP:  // 用 flock() 做文件锁
来源：http://axn.shangyingyoupin.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ybj.wangshuangyany.cn

TS:   // 同 JS
来源：http://pwm.9152youxi.cn

Java: synchronized (this) { shared++; }
来源：http://xoj.wangshuangyany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nqb.ybcxt.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://viy.gaohongyu789.top

C#:   lock (gate) { shared++; }
来源：http://aic.zhongyouzk.top

[O04] 定义异步函数并等待
来源：http://vmj.aibaodan.cn

Py:   async def f():⏎    await g()
来源：http://ytp.yj20258.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pol.ydzc1.top

JS:   async function f() { await g(); }
来源：http://ybd.birdmap.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wmx.daria6918.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qpk.shangyingyoupin.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rxv.hnqzz.top

Ruby: # 用 Fiber 或 async gem
来源：http://oin.fanxiaobao.xyz

C#:   async Task F() { await G(); }
来源：http://lgu.jinqigfzy.top

[O05] 并发执行并等待全部完成
来源：http://ntc.xziqi.cn

Py:   asyncio.gather(*tasks)
来源：http://crn.vqdsnc.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://efl.cqqwz.cn

JS:   await Promise.all(tasks)
来源：http://ldv.hysaishi.cn

TS:   await Promise.all(tasks)
来源：http://vsm.ydzc1.top


<!-- 参考信息 -->