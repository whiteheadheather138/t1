代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://xbm.chenzaomai.com

Ruby: Net::HTTP.get(URI(url))
来源：http://bvd.yfazqb.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fsw.shzxlz.cn

[L02] 发送 POST JSON
来源：http://wtn.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://mjz.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gdz.yueranfly.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sxh.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gum.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jws.fktsv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yzy.jqgufenzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://upc.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ipm.gogol.net.cn

[L03] 设置自定义请求头
来源：http://jmq.tarul.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://stv.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zch.zhijiandao.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pcp.fanxiaobao.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nim.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xtt.sweek.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wem.tianlin.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lto.wangshuangyany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mxt.ehwqpu.com

[L04] 设置超时
来源：http://dib.jianghu66.top

Py:   requests.get(url, timeout=5)
来源：http://qmv.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yfd.zhiwuduotai.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://emm.hnxiangtu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://apt.mhx1999.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gbo.yj20258888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wbh.shanyushiyangtech.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oce.kuanghao11.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oos.xingfuxueyuan.xyz

[L05] 上传文件（multipart）
来源：http://gqc.feifeiyinyue.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tqi.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zoc.epnwcf.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ncn.epnwcf.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cuu.ydjk.org.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qvk.shzxlz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://owy.epnwcf.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zgc.zhijiandao.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nrx.9152youxi.cn

[L06] 解析响应为 JSON
来源：http://iik.nwbrower.top

Py:   resp.json()
来源：http://zgb.hcnkem.com

PHP:  json_decode($body, true);
来源：http://csx.tanke756.top

JS:   await resp.json()
来源：http://ifp.ydjk.org.cn

TS:   await resp.json()
来源：http://gox.hongshengwenyu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://okj.guowangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wvg.316326.xyz

Ruby: JSON.parse(resp.body)
来源：http://rjl.epnwcf.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ckc.dashuyun.cn

[L07] 处理 HTTP 状态码
来源：http://iaf.hongshengwenyu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://iyi.ydjk.org.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nss.hammf.cn

JS:   resp.ok;  resp.status
来源：http://gln.fktsv.cn

TS:   resp.ok;  resp.status
来源：http://hss.feifeiyinyue.top

Java: resp.statusCode()
来源：http://jjw.shanyushiyangtech.top

Go:   resp.StatusCode
来源：http://gzq.xinyue.icu

Ruby: resp.code.to_i
来源：http://jdb.jinqigfzy.top

C#:   (int)resp.StatusCode
来源：http://tjz.52xcode.cn

[L08] 并发请求多个地址
来源：http://uer.cashguo.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://azt.hysaishi.cn

PHP:  curl_multi_init() 系列
来源：http://bmh.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yaw.yangfankeji.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ehp.hnqzz.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://whg.yvedp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mkq.jyoumei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ljx.xuetiantiany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bpp.sjlbkw.cn

================================================================================
来源：http://kqk.dianchejie.cn

M. 命令行 / 进程 / 环境
来源：http://npz.shangyingyoupin.top

================================================================================
来源：http://ccc.ybcxt.top

[M01] 读取命令行参数
来源：http://inu.tarul.cn

Py:   sys.argv[1:]
来源：http://slc.tanke756.top

PHP:  $argv;  $argc;
来源：http://leo.hammf.cn

JS:   process.argv.slice(2)
来源：http://jui.aizwys.cn

TS:   process.argv.slice(2)
来源：http://qok.0kj1m.cn

Java: args 数组（main 方法参数）
来源：http://skh.gotoacloud.top

Go:   os.Args[1:]
来源：http://bad.tianlin.xyz

Ruby: ARGV
来源：http://dlu.zhijiandao.cn

C#:   args 数组（Main 方法参数）
来源：http://ezs.9152youxi.cn

[M02] 读取环境变量
来源：http://xpe.yanxiufei.cn

Py:   os.environ.get("HOME")
来源：http://fum.smart0.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lcw.jiagoushi.top

JS:   process.env.HOME
来源：http://opj.52xcode.cn

TS:   process.env.HOME
来源：http://dox.yj20258888.top

Java: System.getenv("HOME")
来源：http://rma.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zys.jianghu66.top

Ruby: ENV["HOME"]
来源：http://uqn.shangyingyoupin.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nhq.zdbjq.cn

[M03] 执行外部命令
来源：http://ihj.jqgufenzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mkp.zhixingplan.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zss.guowangkeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fnq.ehwqpu.com

TS:   child_process.execSync("ls -l").toString()
来源：http://spy.ivvv.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lkn.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kes.fengsongda.top

Ruby: system("ls -l");  `ls -l`
来源：http://hxe.chenjidiqi.icu

C#:   Process.Start("ls", "-l");
来源：http://xww.ppjwa.cn

[M04] 获取当前工作目录
来源：http://cys.c1oappe.top

Py:   os.getcwd()
来源：http://ptv.aibaodan.cn

PHP:  getcwd();
来源：http://bgn.shanyushiyangkeji.top

JS:   process.cwd()
来源：http://jnh.aibaodan.cn

TS:   process.cwd()
来源：http://cdz.feifeiyinyue.top

Java: Path.of("").toAbsolutePath()
来源：http://dyr.sxryk.cn

Go:   os.Getwd()
来源：http://miu.bjfxy.top

Ruby: Dir.pwd
来源：http://ntc.aibaodan.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lxw.andypj.xyz

[M05] 设置退出码
来源：http://wbl.zhengqikj.top

Py:   sys.exit(1)
来源：http://foi.shuidangran.top

PHP:  exit(1);
来源：http://cra.gotoacloud.top

JS:   process.exit(1)
来源：http://twj.xuanzx.com

TS:   process.exit(1)
来源：http://fds.chenjidiqi.icu

Java: System.exit(1)
来源：http://evk.tian-w.cn

Go:   os.Exit(1)
来源：http://kfa.yuanzhike.top

Ruby: exit 1
来源：http://rjh.havefunace.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://laz.ydjk.org.cn

[M06] 向标准错误输出
来源：http://fzi.ehwqpu.com

Py:   print("err", file=sys.stderr)
来源：http://qfc.zhengqikj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lsy.jyoumei.cn

JS:   console.error("err")
来源：http://qqb.dianchejie.cn

TS:   console.error("err")
来源：http://wqy.jyoumei.cn

Java: System.err.println("err")
来源：http://ywt.yuanzhike.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wpc.snrcjt.cn

Ruby: warn "err"
来源：http://ocf.fengsongda.top

C#:   Console.Error.WriteLine("err")
来源：http://wjq.shanyushiyangtech.top

[M07] 判断是否为主入口
来源：http://xeb.vqdsnc.cn

Py:   if __name__ == "__main__":
来源：http://nuf.birdmap.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nom.hysaishi.cn

JS:   require.main === module
来源：http://pev.ehwqpu.com

TS:   require.main === module
来源：http://ddd.jyoumei.cn

Java: public static void main(String[] args)
来源：http://cal.ywan-chungtsiang.top

Go:   func main()
来源：http://pnm.ydzc1.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jsb.hammf.cn

C#:   static void Main(string[] args)
来源：http://kes.yfazqb.com

[M08] 获取系统与运行时信息
来源：http://mei.0kj1m.cn

Py:   platform.system();  platform.python_version()
来源：http://kbc.bbcook.cn

PHP:  PHP_OS;  phpversion();
来源：http://cga.yonumen.top

JS:   process.platform;  process.version
来源：http://tlh.jqgufenzy.top

TS:   process.platform;  process.version
来源：http://prp.yangfankeji.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jwy.zhiwuduotai.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://usm.feifeiyinyue.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cjg.cqqwz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ywx.birdmap.top

================================================================================
来源：http://tua.vqdsnc.cn

N. 数据结构与算法
来源：http://kye.hywenlv.cn

================================================================================
来源：http://jap.daria6918.cn

[N01] 二分查找（有序数组）
来源：http://cda.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://vjn.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mbu.xingfuxueyuan.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qlq.dashuyun.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rjy.yfazqb.com

Java: Arrays.binarySearch(arr, x)
来源：http://shk.jinqigfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://ett.yj20258888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://adm.zhoulong.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://elp.yvedp.cn

[N02] 排序（工程实践用内置实现）
来源：http://lya.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://rym.0kj1m.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tvv.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://dwz.tian-w.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xme.cashguo.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://afl.dianchejie.cn

Go:   slices.Sort(arr)
来源：http://nso.zdbjq.cn

Ruby: arr.sort
来源：http://owx.dianchejie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wyr.andypj.xyz

[N03] 快速排序（分治示例）
来源：http://siu.yuxming.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ini.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://ntq.iojbl.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dqw.hywenlv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ejb.yongpay.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fiz.hongshengwenyu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rtj.havefunace.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bpq.uphjek.com

C#:   // 手写递归，或 Array.Sort
来源：http://tjd.birdmap.top

[N04] 斐波那契数列
来源：http://rly.yfazqb.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lfw.ctjpmb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dfo.xinyue.icu

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lsi.ywan-chungtsiang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://chp.aizwys.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cjx.yongpay.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dkn.fengsongda.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://trr.xingfuxueyuan.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oip.zhengqikj.top

[N05] 最大公约数
来源：http://bxk.sweek.top

Py:   math.gcd(a, b)
来源：http://zyg.ivvv.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bij.hnqzz.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xgz.ydjk.org.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vpx.andypj.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rqj.hywenlv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://smr.zdbjq.cn

Ruby: a.gcd(b)
来源：http://hhi.ywan-chungtsiang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ryp.316326.xyz

[N06] 判断回文字符串
来源：http://kde.vehdjk.com

Py:   s == s[::-1]
来源：http://xzv.fanxiaobao.xyz

PHP:  $s === strrev($s);
来源：http://maf.haohaochexian.top

JS:   s === [...s].reverse().join("")
来源：http://npf.hywenlv.cn

TS:   s === [...s].reverse().join("")
来源：http://zuu.jinghuilouyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vuh.smart0.xyz

Go:   // 双指针从两端比较
来源：http://vdr.snrcjt.cn

Ruby: s == s.reverse
来源：http://ezd.0kj1m.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gmt.yueranfly.top

[N07] 两数之和（返回下标）
来源：http://svs.nwbrower.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yxw.52xcode.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://goe.ivvv.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mlo.jinyuanbaomall.cn

TS:   // 手写 Map<string, number>
来源：http://zhv.epnwcf.com

Java: // 手写 HashMap
来源：http://hjw.redwolf501.top

Go:   // 手写 map[int]int
来源：http://vsd.shuidangran.top

Ruby: // 手写 Hash
来源：http://pbl.cucudq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xfx.hammf.cn

[N08] 生成全排列
来源：http://zms.ctjpmb.com

Py:   itertools.permutations(arr)
来源：http://emf.yueranfly.top

PHP:  // 手写递归交换
来源：http://nxl.yj20258.top

JS:   // 手写回溯递归
来源：http://ajg.ywan-chungtsiang.top

TS:   // 手写回溯递归
来源：http://hwc.zhaomingkeji.xyz

Java: // 手写回溯递归
来源：http://yvk.gzhubu.top

Go:   // 手写回溯递归
来源：http://lky.nanxuanxn.top

Ruby: arr.permutation.to_a
来源：http://cly.fengsongda.top

C#:   // 手写回溯递归
来源：http://rwi.zhijiandao.cn

[N09] 栈与队列
来源：http://lil.cucudq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mda.shzxlz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://buh.sufxvd.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mtk.zhijiandao.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rxy.vqdsnc.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dms.jinqigfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nze.hcnkem.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vlz.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://neo.sxryk.cn

[N10] 链表节点定义
来源：http://obr.hnqzz.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fpc.sxryk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yth.tian-w.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nos.uphjek.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xwg.nanxuanxn.top

Java: class Node { int v; Node next; }
来源：http://did.haohaochexian.top

Go:   type Node struct { V int; Next *Node }
来源：http://dcz.gzhubu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://glw.jinyuanbaomall.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mlx.wangdashe.top

[N11] 二叉树中序遍历
来源：http://pcy.vqdsnc.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dxx.pengpengdd.cyou

PHP:  // 手写递归函数
来源：http://ogg.jianghu66.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kzx.feifeiyinyue.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wxp.tanke756.top

Java: // 手写递归
来源：http://tog.tianlin.xyz

Go:   // 手写递归
来源：http://qly.zhoulong.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yto.pengpengdd.cyou

C#:   // 手写递归
来源：http://dsg.chenjidiqi.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qcc.xuanzx.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ckk.316326.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vix.fanxiaobao.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gaw.tianlin.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qkb.shanyushiyangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ttj.iojbl.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://byh.gaohongyu789.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ndf.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://trr.jinghuilouyu.cn

================================================================================
来源：http://qeq.9152youxi.cn

O. 并发与异步
来源：http://rsj.smart0.xyz

================================================================================
来源：http://jop.kuanghao11.cn

[O01] 启动一个线程
来源：http://rmb.yuanzhike.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tpf.jqgufenzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vbg.iojbl.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lfe.xziqi.cn

TS:   // 同 JS
来源：http://tav.hysaishi.cn

Java: new Thread(() -> f()).start()
来源：http://hla.hcnkem.com

Go:   go f()
来源：http://azc.xuanzx.com

Ruby: Thread.new { f }
来源：http://ocb.ppjwa.cn

C#:   Task.Run(() => F());
来源：http://qkf.c1oappe.top

[O02] 使用线程池
来源：http://cbe.sweek.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wez.xingfuxueyuan.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hgm.cqqwz.cn

JS:   // worker_threads 线程池
来源：http://lyc.hesvh.cn

TS:   // worker_threads 线程池
来源：http://xty.mhx1999.top

Java: Executors.newFixedThreadPool(4)
来源：http://uui.xziqi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zga.zhengqikj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pxn.zhengqikj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uwp.meibo888.top

[O03] 加锁保护共享数据
来源：http://vqr.redwolf501.top

Py:   with lock: shared += 1
来源：http://amp.cqqwz.cn

PHP:  // 用 flock() 做文件锁
来源：http://psu.daria6918.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mbe.cucudq.cn

TS:   // 同 JS
来源：http://xsu.316326.xyz

Java: synchronized (this) { shared++; }
来源：http://fjz.birdmap.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nwq.ppjwa.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rfv.ivvv.top

C#:   lock (gate) { shared++; }
来源：http://bwt.zdqjudy.top

[O04] 定义异步函数并等待
来源：http://kxp.vqdsnc.cn

Py:   async def f():⏎    await g()
来源：http://pjo.ctjpmb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://otv.svipenyu.cn

JS:   async function f() { await g(); }
来源：http://kiq.guannengcc.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dhj.shzxlz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yki.yueranfly.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vgs.yj20258.top

Ruby: # 用 Fiber 或 async gem
来源：http://wgk.sjlbkw.cn

C#:   async Task F() { await G(); }
来源：http://qdr.iojbl.cn

[O05] 并发执行并等待全部完成
来源：http://ohl.jqgfzy.top

Py:   asyncio.gather(*tasks)
来源：http://iox.sufxvd.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yqt.yuanzhike.top

JS:   await Promise.all(tasks)
来源：http://jqp.9152youxi.cn

TS:   await Promise.all(tasks)
来源：http://sfr.cashguo.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hzk.jyoumei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://avz.tianlin.xyz

Ruby: threads.map(&:join)
来源：http://cjv.cashguo.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zdh.gotoacloud.top


<!-- 参考信息 -->