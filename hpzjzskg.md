代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://iho.yuanzhike.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dtt.9152youxi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ekl.sweek.top

[L02] 发送 POST JSON
来源：http://kit.shangyingyoupin.top

Py:   requests.post(url, json={"a": 1})
来源：http://nfs.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jiv.daria6918.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kqu.hesvh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jkp.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vbb.zhoulong.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xms.zhoulong.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://owa.jyoumei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xij.xinyue.icu

[L03] 设置自定义请求头
来源：http://ijy.tarul.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ytw.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ryp.xingfuxueyuan.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nsz.xingfuxueyuan.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hsb.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wrz.jqgufenzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rwr.jqgfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vfx.jqgufenzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iff.yangfankeji.com

[L04] 设置超时
来源：http://wrz.havefunace.top

Py:   requests.get(url, timeout=5)
来源：http://nln.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vsf.ydzc1.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gyu.yanxiufei.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jxj.guowangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xma.gotoacloud.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tgw.feifeiyinyue.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zkv.fehbvm.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://juy.cucudq.cn

[L05] 上传文件（multipart）
来源：http://szk.smart0.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ier.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gzp.hnxiangtu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zgt.tianlin.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rvi.zhaomingkeji.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xng.cucudq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xog.gzhubu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://chz.fehbvm.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xbk.bbcook.cn

[L06] 解析响应为 JSON
来源：http://kck.316326.xyz

Py:   resp.json()
来源：http://qtg.zdbjq.cn

PHP:  json_decode($body, true);
来源：http://yoy.0kj1m.cn

JS:   await resp.json()
来源：http://qhr.ydjk.org.cn

TS:   await resp.json()
来源：http://vni.nwbrower.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rlc.fehbvm.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dpj.yj20258888.top

Ruby: JSON.parse(resp.body)
来源：http://kcz.zhixingplan.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tcz.pycfn.com

[L07] 处理 HTTP 状态码
来源：http://xoh.chenzaomai.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fqk.ppjwa.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pbs.sysykeji.top

JS:   resp.ok;  resp.status
来源：http://jce.jyoumei.cn

TS:   resp.ok;  resp.status
来源：http://ufo.fzhhl.top

Java: resp.statusCode()
来源：http://zdc.hammf.cn

Go:   resp.StatusCode
来源：http://vsk.vqdsnc.cn

Ruby: resp.code.to_i
来源：http://foq.iojbl.cn

C#:   (int)resp.StatusCode
来源：http://aqs.hesvh.cn

[L08] 并发请求多个地址
来源：http://xep.cdnleiting.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://glr.cheryme.top

PHP:  curl_multi_init() 系列
来源：http://kyj.chenlongwang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wwj.hnqzz.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bzg.yanxiufei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wsu.0kj1m.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://clu.smart0.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://saa.chenlongwang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gom.ywan-chungtsiang.top

================================================================================
来源：http://emb.yonumen.top

M. 命令行 / 进程 / 环境
来源：http://krq.guowangkeji.top

================================================================================
来源：http://ctu.zhoulong.xyz

[M01] 读取命令行参数
来源：http://fap.bbcook.cn

Py:   sys.argv[1:]
来源：http://aae.ppjwa.cn

PHP:  $argv;  $argc;
来源：http://tts.9152youxi.cn

JS:   process.argv.slice(2)
来源：http://ppw.kuanghao11.cn

TS:   process.argv.slice(2)
来源：http://aam.ydjk.org.cn

Java: args 数组（main 方法参数）
来源：http://hfn.birdmap.top

Go:   os.Args[1:]
来源：http://ijm.fzhhl.top

Ruby: ARGV
来源：http://idx.jiagoushi.top

C#:   args 数组（Main 方法参数）
来源：http://zep.haohaochexian.top

[M02] 读取环境变量
来源：http://pqn.nwbrower.top

Py:   os.environ.get("HOME")
来源：http://hah.chenzaomai.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rqt.cheryme.top

JS:   process.env.HOME
来源：http://dqn.hesvh.cn

TS:   process.env.HOME
来源：http://tyc.snrcjt.cn

Java: System.getenv("HOME")
来源：http://jlh.hcnkem.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://myp.vqdsnc.cn

Ruby: ENV["HOME"]
来源：http://ipu.kuanghao11.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://haq.feifeiyinyue.top

[M03] 执行外部命令
来源：http://rmd.yuanzhike.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ngq.xziqi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kbs.hcnkem.com

JS:   child_process.execSync("ls -l").toString()
来源：http://ucy.sxryk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://eai.sweek.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oao.epnwcf.com

Go:   exec.Command("ls", "-l").Output()
来源：http://cwn.sysykeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://lzg.yuxming.cn

C#:   Process.Start("ls", "-l");
来源：http://htp.wangshuangyany.cn

[M04] 获取当前工作目录
来源：http://qod.svipenyu.cn

Py:   os.getcwd()
来源：http://tvz.dashuyun.cn

PHP:  getcwd();
来源：http://xxx.zdqjudy.top

JS:   process.cwd()
来源：http://bmy.shuidangran.top

TS:   process.cwd()
来源：http://dld.yongpay.top

Java: Path.of("").toAbsolutePath()
来源：http://vib.dianchejie.cn

Go:   os.Getwd()
来源：http://cql.tian-w.cn

Ruby: Dir.pwd
来源：http://ikw.pycfn.com

C#:   Directory.GetCurrentDirectory()
来源：http://zkv.sufxvd.cn

[M05] 设置退出码
来源：http://zlq.hysaishi.cn

Py:   sys.exit(1)
来源：http://joi.hesvh.cn

PHP:  exit(1);
来源：http://zkm.sjlbkw.cn

JS:   process.exit(1)
来源：http://jlg.jyoumei.cn

TS:   process.exit(1)
来源：http://shk.bjfxy.top

Java: System.exit(1)
来源：http://epx.ppjwa.cn

Go:   os.Exit(1)
来源：http://pro.ehwqpu.com

Ruby: exit 1
来源：http://lmf.zhijiandao.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://htp.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://smf.0kj1m.cn

Py:   print("err", file=sys.stderr)
来源：http://bce.0kj1m.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://grm.yanxiufei.cn

JS:   console.error("err")
来源：http://bca.guowangkeji.top

TS:   console.error("err")
来源：http://vst.xziqi.cn

Java: System.err.println("err")
来源：http://ewp.jqgfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vfu.haohaochexian.top

Ruby: warn "err"
来源：http://rha.sxryk.cn

C#:   Console.Error.WriteLine("err")
来源：http://fgj.jiagoushi.top

[M07] 判断是否为主入口
来源：http://rnr.hfpthk.cn

Py:   if __name__ == "__main__":
来源：http://czl.fengsongda.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sko.guowangkeji.top

JS:   require.main === module
来源：http://zqb.0kj1m.cn

TS:   require.main === module
来源：http://btm.zdbjq.cn

Java: public static void main(String[] args)
来源：http://pnh.jqgufenzy.top

Go:   func main()
来源：http://ygb.havefunace.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lte.tarul.cn

C#:   static void Main(string[] args)
来源：http://lyt.xziqi.cn

[M08] 获取系统与运行时信息
来源：http://tex.redwolf501.top

Py:   platform.system();  platform.python_version()
来源：http://pim.birdmap.top

PHP:  PHP_OS;  phpversion();
来源：http://rfl.shangyingyoupin.top

JS:   process.platform;  process.version
来源：http://pfd.cdnleiting.top

TS:   process.platform;  process.version
来源：http://uew.ctjpmb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lqm.zhengqikj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://yko.sufxvd.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hey.daxiang520.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xdm.ydjk.org.cn

================================================================================
来源：http://khc.fanxiaobao.xyz

N. 数据结构与算法
来源：http://jlt.sxryk.cn

================================================================================
来源：http://nrh.gzhubu.top

[N01] 二分查找（有序数组）
来源：http://nzv.yanxiufei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zij.yongpay.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://olg.xinyue.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iix.zhixingplan.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vet.hongshengwenyu.top

Java: Arrays.binarySearch(arr, x)
来源：http://zmr.jinyuanbaomall.cn

Go:   sort.SearchInts(arr, x)
来源：http://fqu.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://eow.wangdashe.top

C#:   Array.BinarySearch(arr, x)
来源：http://stv.zycfv.cn

[N02] 排序（工程实践用内置实现）
来源：http://wwa.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://vdb.daxiang520.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qcs.shzxlz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mbj.yvedp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ozp.316326.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tts.havefunace.top

Go:   slices.Sort(arr)
来源：http://pzd.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://zop.ehwqpu.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://ier.uphjek.com

[N03] 快速排序（分治示例）
来源：http://aud.yvedp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rme.shangyingyoupin.top

PHP:  // 递归实现，或用 usort
来源：http://uiv.yonumen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hlr.hammf.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bpn.yj20258888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kvo.fehbvm.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rtk.xuanzx.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bfc.bjfxy.top

C#:   // 手写递归，或 Array.Sort
来源：http://gmz.quarkkingdee.top

[N04] 斐波那契数列
来源：http://slu.hfpthk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kzi.daxiang520.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hab.quarkkingdee.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dgc.wangdashe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dxp.yuxming.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hev.jinyuanbaomall.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tip.jlsjyb.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tol.yuxming.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fue.hnxiangtu.top

[N05] 最大公约数
来源：http://rqy.sweek.top

Py:   math.gcd(a, b)
来源：http://cuw.xingfuxueyuan.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nyu.chenjidiqi.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iwx.sysykeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://piw.meibo888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lij.zhaomingkeji.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xgc.xziqi.cn

Ruby: a.gcd(b)
来源：http://opl.vehdjk.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dxz.kuanghao11.cn

[N06] 判断回文字符串
来源：http://gbj.daria6918.cn

Py:   s == s[::-1]
来源：http://dmc.c1oappe.top

PHP:  $s === strrev($s);
来源：http://tyf.jlsjyb.cn

JS:   s === [...s].reverse().join("")
来源：http://lak.fktsv.cn

TS:   s === [...s].reverse().join("")
来源：http://eot.zycfv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://neh.jinqigufen.top

Go:   // 双指针从两端比较
来源：http://awb.yangfankeji.com

Ruby: s == s.reverse
来源：http://twy.tian-w.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mxz.redwolf501.top

[N07] 两数之和（返回下标）
来源：http://smn.aizwys.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hvh.zhiwuduotai.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://msi.zhijiandao.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pac.hfpthk.cn

TS:   // 手写 Map<string, number>
来源：http://rbx.hesvh.cn

Java: // 手写 HashMap
来源：http://cin.tianlin.xyz

Go:   // 手写 map[int]int
来源：http://llv.daxiang520.top

Ruby: // 手写 Hash
来源：http://trw.zhengqikj.top

C#:   // 手写 Dictionary<int, int>
来源：http://vzk.shanyushiyangtech.top

[N08] 生成全排列
来源：http://tnf.52xcode.cn

Py:   itertools.permutations(arr)
来源：http://pko.hesvh.cn

PHP:  // 手写递归交换
来源：http://ihe.jyoumei.cn

JS:   // 手写回溯递归
来源：http://agw.tanke756.top

TS:   // 手写回溯递归
来源：http://ted.xuetiantiany.cn

Java: // 手写回溯递归
来源：http://cud.zdqjudy.top

Go:   // 手写回溯递归
来源：http://prb.shangyingyoupin.top

Ruby: arr.permutation.to_a
来源：http://mox.cashguo.top

C#:   // 手写回溯递归
来源：http://vyg.gaohongyu789.top

[N09] 栈与队列
来源：http://flb.0kj1m.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ghh.cucudq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iwx.kuanghao11.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mxv.meibo888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vah.shanyushiyangtech.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://irc.zhixingplan.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mwy.hammf.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ill.andypj.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fdz.ivvv.top

[N10] 链表节点定义
来源：http://uvm.havefunace.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mna.yangfankeji.com

PHP:  class Node { public $v; public $next = null; }
来源：http://oob.shuidangran.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xak.jinqigufen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mjz.hfpthk.cn

Java: class Node { int v; Node next; }
来源：http://qsx.cdnleiting.top

Go:   type Node struct { V int; Next *Node }
来源：http://vpg.aizwys.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pix.jinghuilouyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yux.pycfn.com

[N11] 二叉树中序遍历
来源：http://srf.wangdashe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vbf.hesvh.cn

PHP:  // 手写递归函数
来源：http://eof.smart0.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fps.zycfv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://enp.zdqjudy.top

Java: // 手写递归
来源：http://lux.mhx1999.top

Go:   // 手写递归
来源：http://smj.xylfe.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://adw.sufxvd.cn

C#:   // 手写递归
来源：http://bgw.ydzc1.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ugo.jinghuilouyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vyq.hesvh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oih.aibaodan.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vix.cashguo.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kby.ybcxt.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ymj.dianchejie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hhh.pycfn.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zrh.vqdsnc.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gdd.yongpay.top

================================================================================
来源：http://xma.hnxiangtu.top

O. 并发与异步
来源：http://yjr.shzxlz.cn

================================================================================
来源：http://niv.cheryme.top

[O01] 启动一个线程
来源：http://muh.hfpthk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kzc.fengsongda.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eoq.ybcxt.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://szq.jqgufenzy.top

TS:   // 同 JS
来源：http://fwn.cucudq.cn

Java: new Thread(() -> f()).start()
来源：http://adk.feifeiyinyue.top

Go:   go f()
来源：http://mjs.feifeiyinyue.top

Ruby: Thread.new { f }
来源：http://mdj.nwbrower.top

C#:   Task.Run(() => F());
来源：http://fgd.fanxiaobao.xyz

[O02] 使用线程池
来源：http://lhy.9152youxi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://epk.shanyushiyangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rth.xuetiantiany.cn

JS:   // worker_threads 线程池
来源：http://eah.pengpengdd.cyou

TS:   // worker_threads 线程池
来源：http://tta.sxryk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xly.yj20258.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qgx.svipenyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cxq.sweek.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nqw.ybcxt.top

[O03] 加锁保护共享数据
来源：http://aub.chenjidiqi.icu

Py:   with lock: shared += 1
来源：http://zsa.xinyue.icu

PHP:  // 用 flock() 做文件锁
来源：http://rhz.fktsv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kcv.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://wev.gogol.net.cn

Java: synchronized (this) { shared++; }
来源：http://mhf.xuetiantiany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rqg.ydzc1.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jlm.yongpay.top

C#:   lock (gate) { shared++; }
来源：http://ynw.andypj.xyz

[O04] 定义异步函数并等待
来源：http://acb.cheryme.top

Py:   async def f():⏎    await g()
来源：http://bay.hysaishi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://emz.snrcjt.cn

JS:   async function f() { await g(); }
来源：http://lsj.nwbrower.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pbw.jqgufenzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yse.tanke756.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ocl.chenlongwang.top

Ruby: # 用 Fiber 或 async gem
来源：http://hzc.zhongyouzk.top

C#:   async Task F() { await G(); }
来源：http://aja.sysykeji.top

[O05] 并发执行并等待全部完成
来源：http://meg.birdmap.top

Py:   asyncio.gather(*tasks)
来源：http://urz.smart0.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rgj.gaohongyu789.top

JS:   await Promise.all(tasks)
来源：http://xeo.tanke756.top

TS:   await Promise.all(tasks)
来源：http://xrj.andypj.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kwe.wangshuangyany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ebf.uphjek.com

Ruby: threads.map(&:join)
来源：http://ell.tarul.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://prj.sufxvd.cn


<!-- 参考信息 -->