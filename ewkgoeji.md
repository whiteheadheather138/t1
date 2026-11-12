代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zdx.yvedp.cn

JS:   await fetch(url)
来源：http://kiy.haohaochexian.top

TS:   await fetch(url)
来源：http://meg.guowangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fir.xingfuxueyuan.xyz

Go:   resp, err := http.Get(url)
来源：http://leh.hcnkem.com

Ruby: Net::HTTP.get(URI(url))
来源：http://odj.cheryme.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xra.hesvh.cn

[L02] 发送 POST JSON
来源：http://tlc.zhaomingkeji.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://fnp.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://czk.zdqjudy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://exl.ppjwa.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ots.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xee.xuetiantiany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://psg.guowangkeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tfv.sufxvd.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vrs.nanxinkj.top

[L03] 设置自定义请求头
来源：http://gjq.fktsv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ous.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://klh.sysykeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://afy.ctjpmb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hnp.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zqk.bbcook.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bwi.iojbl.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fjb.yfazqb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bjq.tian-w.cn

[L04] 设置超时
来源：http://clg.cheryme.top

Py:   requests.get(url, timeout=5)
来源：http://utz.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rga.svipenyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qwv.xylfe.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mwu.tianlin.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wtj.52xcode.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xyy.wangshuangyany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aji.jinyuanbaomall.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wtf.ppjwa.cn

[L05] 上传文件（multipart）
来源：http://hgj.tarul.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://epz.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ogo.zdqjudy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mcw.dashuyun.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nrk.jqgufenzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://snv.redwolf501.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://paj.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hon.nanxinkj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jjo.ppjwa.cn

[L06] 解析响应为 JSON
来源：http://yek.zhongyouzk.top

Py:   resp.json()
来源：http://bzv.vehdjk.com

PHP:  json_decode($body, true);
来源：http://tfc.cdnleiting.top

JS:   await resp.json()
来源：http://hpl.ivvv.top

TS:   await resp.json()
来源：http://rpy.feifeiyinyue.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lkh.zhiwuduotai.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qyp.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://rqt.yuanzhike.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wui.chenjidiqi.icu

[L07] 处理 HTTP 状态码
来源：http://hhd.chenzaomai.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xie.zdbjq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fjy.fengsongda.top

JS:   resp.ok;  resp.status
来源：http://vhk.sxryk.cn

TS:   resp.ok;  resp.status
来源：http://uaq.snrcjt.cn

Java: resp.statusCode()
来源：http://ekq.sxryk.cn

Go:   resp.StatusCode
来源：http://ddk.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://yny.jqgufenzy.top

C#:   (int)resp.StatusCode
来源：http://lzl.yvedp.cn

[L08] 并发请求多个地址
来源：http://tfg.zhijiandao.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yly.epnwcf.com

PHP:  curl_multi_init() 系列
来源：http://fpo.cashguo.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xrw.meibo888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xvv.hongshengwenyu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sda.jyoumei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nue.hcnkem.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ybz.vehdjk.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nwf.ctjpmb.com

================================================================================
来源：http://hep.ywan-chungtsiang.top

M. 命令行 / 进程 / 环境
来源：http://bsx.havefunace.top

================================================================================
来源：http://ftr.chenzaomai.com

[M01] 读取命令行参数
来源：http://wtn.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://ljf.nanxinkj.top

PHP:  $argv;  $argc;
来源：http://xln.nanxuanxn.top

JS:   process.argv.slice(2)
来源：http://pre.gotoacloud.top

TS:   process.argv.slice(2)
来源：http://coi.sufxvd.cn

Java: args 数组（main 方法参数）
来源：http://uux.fehbvm.com

Go:   os.Args[1:]
来源：http://znw.yueranfly.top

Ruby: ARGV
来源：http://kjq.hcnkem.com

C#:   args 数组（Main 方法参数）
来源：http://rwq.fehbvm.com

[M02] 读取环境变量
来源：http://cyq.cashguo.top

Py:   os.environ.get("HOME")
来源：http://kdr.fengsongda.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bcx.chenlongwang.top

JS:   process.env.HOME
来源：http://xju.tian-w.cn

TS:   process.env.HOME
来源：http://wbu.jlsjyb.cn

Java: System.getenv("HOME")
来源：http://oxg.havefunace.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qjm.epnwcf.com

Ruby: ENV["HOME"]
来源：http://bta.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jyl.dashuyun.cn

[M03] 执行外部命令
来源：http://yhv.chenjidiqi.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://onj.birdmap.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://per.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://lts.fanxiaobao.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://iww.zhengqikj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yxs.shzxlz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://iaf.sjlbkw.cn

Ruby: system("ls -l");  `ls -l`
来源：http://twy.sweek.top

C#:   Process.Start("ls", "-l");
来源：http://ley.tanke756.top

[M04] 获取当前工作目录
来源：http://fbx.daxiang520.top

Py:   os.getcwd()
来源：http://gst.fengsongda.top

PHP:  getcwd();
来源：http://xcj.ehwqpu.com

JS:   process.cwd()
来源：http://yqe.iojbl.cn

TS:   process.cwd()
来源：http://rke.mhx1999.top

Java: Path.of("").toAbsolutePath()
来源：http://nec.cqqwz.cn

Go:   os.Getwd()
来源：http://xpk.jlsjyb.cn

Ruby: Dir.pwd
来源：http://ybs.c1oappe.top

C#:   Directory.GetCurrentDirectory()
来源：http://yux.shanyushiyangkeji.top

[M05] 设置退出码
来源：http://nob.ehwqpu.com

Py:   sys.exit(1)
来源：http://xbl.zhiwuduotai.top

PHP:  exit(1);
来源：http://bax.shanyushiyangkeji.top

JS:   process.exit(1)
来源：http://kdr.nwbrower.top

TS:   process.exit(1)
来源：http://nov.haohaochexian.top

Java: System.exit(1)
来源：http://upi.tarul.cn

Go:   os.Exit(1)
来源：http://ubz.daxiang520.top

Ruby: exit 1
来源：http://fqe.pengpengdd.cyou

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nji.hnqzz.top

[M06] 向标准错误输出
来源：http://lex.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://dkc.sweek.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vxl.zhiwuduotai.top

JS:   console.error("err")
来源：http://nao.yuxming.cn

TS:   console.error("err")
来源：http://rzr.xuetiantiany.cn

Java: System.err.println("err")
来源：http://evp.nanxuanxn.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wot.tarul.cn

Ruby: warn "err"
来源：http://cjf.kuanghao11.cn

C#:   Console.Error.WriteLine("err")
来源：http://sap.ppjwa.cn

[M07] 判断是否为主入口
来源：http://yob.daria6918.cn

Py:   if __name__ == "__main__":
来源：http://vxm.zhengqikj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nyz.jinqigufen.top

JS:   require.main === module
来源：http://nyb.c1oappe.top

TS:   require.main === module
来源：http://oxv.haohaochexian.top

Java: public static void main(String[] args)
来源：http://arx.yanxiufei.cn

Go:   func main()
来源：http://abn.fehbvm.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://usk.wangshuangyany.cn

C#:   static void Main(string[] args)
来源：http://wys.kuanghao11.cn

[M08] 获取系统与运行时信息
来源：http://man.quarkkingdee.top

Py:   platform.system();  platform.python_version()
来源：http://yjr.yanxiufei.cn

PHP:  PHP_OS;  phpversion();
来源：http://xhg.svipenyu.cn

JS:   process.platform;  process.version
来源：http://cwl.wangshuangyany.cn

TS:   process.platform;  process.version
来源：http://hcx.jinqigfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xms.wangshuangyany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://drl.kuanghao11.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eax.yanxiufei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://blo.fanxiaobao.xyz

================================================================================
来源：http://ghs.zycfv.cn

N. 数据结构与算法
来源：http://lnl.dianchejie.cn

================================================================================
来源：http://pmo.aizwys.cn

[N01] 二分查找（有序数组）
来源：http://dgh.haohaochexian.top

Py:   bisect.bisect_left(arr, x)
来源：http://vmh.yfazqb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bxt.shangyingyoupin.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uav.feifeiyinyue.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wfa.zycfv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://eph.sxryk.cn

Go:   sort.SearchInts(arr, x)
来源：http://jwm.yangfankeji.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://ent.0kj1m.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zlg.xziqi.cn

[N02] 排序（工程实践用内置实现）
来源：http://liv.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://nfk.tian-w.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kbp.xuanzx.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://kvk.snrcjt.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yyo.ctjpmb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wum.9152youxi.cn

Go:   slices.Sort(arr)
来源：http://tjq.sysykeji.top

Ruby: arr.sort
来源：http://bvs.ivvv.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nkj.chenlongwang.top

[N03] 快速排序（分治示例）
来源：http://tgp.jqgfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wcs.nanxinkj.top

PHP:  // 递归实现，或用 usort
来源：http://lbi.yj20258.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gvu.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vqn.zhiwuduotai.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://svy.bjfxy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://naf.aibaodan.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vkb.yj20258.top

C#:   // 手写递归，或 Array.Sort
来源：http://swd.shanyushiyangtech.top

[N04] 斐波那契数列
来源：http://ywd.yangfankeji.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://svy.hysaishi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yvc.chenzaomai.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pst.nanxinkj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fjv.shangyingyoupin.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://suq.0kj1m.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dfc.yj20258888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nyk.epnwcf.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vpw.yj20258.top

[N05] 最大公约数
来源：http://qxk.wangshuangyany.cn

Py:   math.gcd(a, b)
来源：http://oum.smart0.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dlb.ivvv.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kjb.yueranfly.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hek.cheryme.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://diq.yj20258888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xjo.yangfankeji.com

Ruby: a.gcd(b)
来源：http://xmt.yuxming.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cua.uphjek.com

[N06] 判断回文字符串
来源：http://ank.vqdsnc.cn

Py:   s == s[::-1]
来源：http://kuf.yongpay.top

PHP:  $s === strrev($s);
来源：http://syj.zhijiandao.cn

JS:   s === [...s].reverse().join("")
来源：http://abd.andypj.xyz

TS:   s === [...s].reverse().join("")
来源：http://dco.chenjidiqi.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fbc.c1oappe.top

Go:   // 双指针从两端比较
来源：http://nre.jinghuilouyu.cn

Ruby: s == s.reverse
来源：http://omu.ctjpmb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://cal.nanxinkj.top

[N07] 两数之和（返回下标）
来源：http://yvf.snrcjt.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rhu.ydjk.org.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qtu.fengsongda.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rkd.nwbrower.top

TS:   // 手写 Map<string, number>
来源：http://ihr.fktsv.cn

Java: // 手写 HashMap
来源：http://ssx.zdbjq.cn

Go:   // 手写 map[int]int
来源：http://htv.epnwcf.com

Ruby: // 手写 Hash
来源：http://qph.yvedp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zio.zhengqikj.top

[N08] 生成全排列
来源：http://svc.sufxvd.cn

Py:   itertools.permutations(arr)
来源：http://xmm.yj20258888.top

PHP:  // 手写递归交换
来源：http://swd.cashguo.top

JS:   // 手写回溯递归
来源：http://zzm.wangdashe.top

TS:   // 手写回溯递归
来源：http://bjv.zhongyouzk.top

Java: // 手写回溯递归
来源：http://qpd.guowangkeji.top

Go:   // 手写回溯递归
来源：http://wji.xuetiantiany.cn

Ruby: arr.permutation.to_a
来源：http://wmm.smart0.xyz

C#:   // 手写回溯递归
来源：http://pxh.ctjpmb.com

[N09] 栈与队列
来源：http://trl.zhixingplan.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bbi.zdqjudy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gcs.gogol.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://crr.ctjpmb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ytc.fengsongda.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lka.jinghuilouyu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mtc.andypj.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vog.jinqigfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wxa.xinyue.icu

[N10] 链表节点定义
来源：http://fic.birdmap.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://irw.zdbjq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gqj.pengpengdd.cyou

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://btr.yuxming.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kdh.dianchejie.cn

Java: class Node { int v; Node next; }
来源：http://uni.xuetiantiany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gyr.zhiwuduotai.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zgp.guowangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://yir.fzhhl.top

[N11] 二叉树中序遍历
来源：http://kgf.zhoulong.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vmt.iojbl.cn

PHP:  // 手写递归函数
来源：http://tdg.ivvv.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lgp.cqqwz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://plc.nwbrower.top

Java: // 手写递归
来源：http://hrb.sweek.top

Go:   // 手写递归
来源：http://aaq.bbcook.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eqx.quarkkingdee.top

C#:   // 手写递归
来源：http://tqo.ehwqpu.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vyb.jinghuilouyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blf.cdnleiting.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fox.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iuu.jlsjyb.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lac.jiagoushi.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vqv.haohaochexian.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tjo.tanke756.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yeb.chenjidiqi.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nmy.xuanzx.com

================================================================================
来源：http://nng.shanyushiyangtech.top

O. 并发与异步
来源：http://ghw.52xcode.cn

================================================================================
来源：http://pnk.yfazqb.com

[O01] 启动一个线程
来源：http://gtc.bbcook.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vjo.shanyushiyangtech.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xat.sysykeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://maf.snrcjt.cn

TS:   // 同 JS
来源：http://oon.dianchejie.cn

Java: new Thread(() -> f()).start()
来源：http://owj.havefunace.top

Go:   go f()
来源：http://ily.vqdsnc.cn

Ruby: Thread.new { f }
来源：http://nwi.gzhubu.top

C#:   Task.Run(() => F());
来源：http://ldr.hammf.cn

[O02] 使用线程池
来源：http://lrl.hammf.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yum.sjlbkw.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ikp.xuetiantiany.cn

JS:   // worker_threads 线程池
来源：http://tko.wangshuangyany.cn

TS:   // worker_threads 线程池
来源：http://pxj.nwbrower.top

Java: Executors.newFixedThreadPool(4)
来源：http://sxi.vqdsnc.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pwr.xziqi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tsq.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iii.gogol.net.cn

[O03] 加锁保护共享数据
来源：http://cbx.fehbvm.com

Py:   with lock: shared += 1
来源：http://gcy.chenjidiqi.icu

PHP:  // 用 flock() 做文件锁
来源：http://bqz.shanyushiyangtech.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jus.ybcxt.top

TS:   // 同 JS
来源：http://wpw.hnxiangtu.top

Java: synchronized (this) { shared++; }
来源：http://gdp.shzxlz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://igr.kuanghao11.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zpl.yj20258888.top

C#:   lock (gate) { shared++; }
来源：http://lkk.chenzaomai.com

[O04] 定义异步函数并等待
来源：http://xgi.52xcode.cn

Py:   async def f():⏎    await g()
来源：http://cax.bbcook.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yeh.hysaishi.cn

JS:   async function f() { await g(); }
来源：http://sgw.fengsongda.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rmh.ydzc1.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ktf.bbcook.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qju.vehdjk.com

Ruby: # 用 Fiber 或 async gem
来源：http://zmr.hnqzz.top

C#:   async Task F() { await G(); }
来源：http://gdj.jqgfzy.top

[O05] 并发执行并等待全部完成
来源：http://fvy.zhixingplan.top

Py:   asyncio.gather(*tasks)
来源：http://kdd.sysykeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pxl.sufxvd.cn

JS:   await Promise.all(tasks)
来源：http://ank.zdbjq.cn

TS:   await Promise.all(tasks)
来源：http://dal.kuanghao11.cn


<!-- 参考信息 -->