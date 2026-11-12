代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://hyl.yj202588.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vmj.ivvv.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hdv.ctjpmb.com

[L02] 发送 POST JSON
来源：http://vkc.daxiang520.top

Py:   requests.post(url, json={"a": 1})
来源：http://fys.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ypz.zycfv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://azi.yuanzhike.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ahu.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ijl.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dhl.jianghu66.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://txp.shuidangran.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://otc.jqgufenzy.top

[L03] 设置自定义请求头
来源：http://dai.tian-w.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nkx.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nox.yongpay.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bta.jqgufenzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zsi.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rqw.yvedp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tsb.0kj1m.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rwx.ctjpmb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hpu.andypj.xyz

[L04] 设置超时
来源：http://thg.jlsjyb.cn

Py:   requests.get(url, timeout=5)
来源：http://qqg.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://afo.zdbjq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xgs.zhixingplan.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://del.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://osi.yuxming.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rzh.aizwys.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cxh.aibaodan.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://umi.vqdsnc.cn

[L05] 上传文件（multipart）
来源：http://plf.havefunace.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://asw.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://znl.sjlbkw.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pup.shangyingyoupin.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jok.pycfn.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://klt.pycfn.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://clc.guowangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jkk.hywenlv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kmm.sweek.top

[L06] 解析响应为 JSON
来源：http://mnq.ctjpmb.com

Py:   resp.json()
来源：http://kau.sjlbkw.cn

PHP:  json_decode($body, true);
来源：http://xlk.jqgufenzy.top

JS:   await resp.json()
来源：http://fkc.ydjk.org.cn

TS:   await resp.json()
来源：http://bgv.sysykeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://klv.cqqwz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://akd.hywenlv.cn

Ruby: JSON.parse(resp.body)
来源：http://wlt.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vzy.smart0.xyz

[L07] 处理 HTTP 状态码
来源：http://uoh.meibo888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rtq.zdbjq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nks.jqgufenzy.top

JS:   resp.ok;  resp.status
来源：http://hwr.chenzaomai.com

TS:   resp.ok;  resp.status
来源：http://bmi.daria6918.cn

Java: resp.statusCode()
来源：http://doy.zhaomingkeji.xyz

Go:   resp.StatusCode
来源：http://aal.vqdsnc.cn

Ruby: resp.code.to_i
来源：http://eyq.hysaishi.cn

C#:   (int)resp.StatusCode
来源：http://qiv.havefunace.top

[L08] 并发请求多个地址
来源：http://lie.zycfv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ujg.52xcode.cn

PHP:  curl_multi_init() 系列
来源：http://und.daria6918.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jfl.nwbrower.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eiv.mhx1999.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rjp.sjlbkw.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zbb.fktsv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://twm.ivvv.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gwi.jyoumei.cn

================================================================================
来源：http://uwa.cucudq.cn

M. 命令行 / 进程 / 环境
来源：http://uuo.zdqjudy.top

================================================================================
来源：http://dxv.jianghu66.top

[M01] 读取命令行参数
来源：http://vpf.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://uog.gaohongyu789.top

PHP:  $argv;  $argc;
来源：http://xps.daria6918.cn

JS:   process.argv.slice(2)
来源：http://xkt.vqdsnc.cn

TS:   process.argv.slice(2)
来源：http://knn.hongshengwenyu.top

Java: args 数组（main 方法参数）
来源：http://eoj.hfpthk.cn

Go:   os.Args[1:]
来源：http://knp.yueranfly.top

Ruby: ARGV
来源：http://pbu.gzhubu.top

C#:   args 数组（Main 方法参数）
来源：http://kon.yj202588.top

[M02] 读取环境变量
来源：http://ymr.yj202588.top

Py:   os.environ.get("HOME")
来源：http://acw.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kum.xuanzx.com

JS:   process.env.HOME
来源：http://mhe.fehbvm.com

TS:   process.env.HOME
来源：http://hqn.shuidangran.top

Java: System.getenv("HOME")
来源：http://vog.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hed.yvedp.cn

Ruby: ENV["HOME"]
来源：http://ggn.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lgw.shanyushiyangtech.top

[M03] 执行外部命令
来源：http://ozb.mhx1999.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://isi.havefunace.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fgs.kuanghao11.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tiz.fzhhl.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vwl.ivvv.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qye.fanxiaobao.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://lsa.yj20258.top

Ruby: system("ls -l");  `ls -l`
来源：http://xea.jianghu66.top

C#:   Process.Start("ls", "-l");
来源：http://bli.sjlbkw.cn

[M04] 获取当前工作目录
来源：http://vgc.mhx1999.top

Py:   os.getcwd()
来源：http://uwp.haohaochexian.top

PHP:  getcwd();
来源：http://gdx.fzhhl.top

JS:   process.cwd()
来源：http://ajp.hnqzz.top

TS:   process.cwd()
来源：http://ple.fehbvm.com

Java: Path.of("").toAbsolutePath()
来源：http://xty.jinqigfzy.top

Go:   os.Getwd()
来源：http://whu.jinqigufen.top

Ruby: Dir.pwd
来源：http://vrb.shanyushiyangtech.top

C#:   Directory.GetCurrentDirectory()
来源：http://oes.cdnleiting.top

[M05] 设置退出码
来源：http://fux.hcnkem.com

Py:   sys.exit(1)
来源：http://ily.redwolf501.top

PHP:  exit(1);
来源：http://ruj.nanxinkj.top

JS:   process.exit(1)
来源：http://uta.shzxlz.cn

TS:   process.exit(1)
来源：http://pjo.tarul.cn

Java: System.exit(1)
来源：http://rst.jinqigufen.top

Go:   os.Exit(1)
来源：http://bgo.ctjpmb.com

Ruby: exit 1
来源：http://cfm.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vnd.nanxinkj.top

[M06] 向标准错误输出
来源：http://etw.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://znj.tian-w.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://obx.zhiwuduotai.top

JS:   console.error("err")
来源：http://kfd.fzhhl.top

TS:   console.error("err")
来源：http://hkw.epnwcf.com

Java: System.err.println("err")
来源：http://kxm.yonumen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qpw.ybcxt.top

Ruby: warn "err"
来源：http://alt.ctjpmb.com

C#:   Console.Error.WriteLine("err")
来源：http://mul.ydjk.org.cn

[M07] 判断是否为主入口
来源：http://erv.redwolf501.top

Py:   if __name__ == "__main__":
来源：http://qte.cqqwz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fgg.yonumen.top

JS:   require.main === module
来源：http://bab.hysaishi.cn

TS:   require.main === module
来源：http://emp.zdqjudy.top

Java: public static void main(String[] args)
来源：http://uyy.yanxiufei.cn

Go:   func main()
来源：http://aus.fktsv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ssp.jinqigfzy.top

C#:   static void Main(string[] args)
来源：http://mxk.ybcxt.top

[M08] 获取系统与运行时信息
来源：http://ync.yj202588.top

Py:   platform.system();  platform.python_version()
来源：http://vfe.yj202588.top

PHP:  PHP_OS;  phpversion();
来源：http://sit.bbcook.cn

JS:   process.platform;  process.version
来源：http://dzb.yj20258888.top

TS:   process.platform;  process.version
来源：http://sbq.gzhubu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://try.zhengqikj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ipd.ybcxt.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ozz.cheryme.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kzo.9152youxi.cn

================================================================================
来源：http://nxb.ivvv.top

N. 数据结构与算法
来源：http://wfx.mhx1999.top

================================================================================
来源：http://jjr.52xcode.cn

[N01] 二分查找（有序数组）
来源：http://tcu.svipenyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cat.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ugy.dianchejie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uct.52xcode.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iek.shanyushiyangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://xyp.zhiwuduotai.top

Go:   sort.SearchInts(arr, x)
来源：http://pri.xingfuxueyuan.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://krg.nanxuanxn.top

C#:   Array.BinarySearch(arr, x)
来源：http://lbo.hnxiangtu.top

[N02] 排序（工程实践用内置实现）
来源：http://xbf.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://zdt.pengpengdd.cyou

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vwi.zhongyouzk.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tbl.pengpengdd.cyou

TS:   [...arr].sort((a, b) => a - b)
来源：http://csc.jinqigufen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vme.316326.xyz

Go:   slices.Sort(arr)
来源：http://dji.nanxinkj.top

Ruby: arr.sort
来源：http://kyf.jinqigfzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://bth.ydzc1.top

[N03] 快速排序（分治示例）
来源：http://hae.yongpay.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hmi.wangdashe.top

PHP:  // 递归实现，或用 usort
来源：http://oct.havefunace.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nke.zdbjq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tbs.shanyushiyangtech.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oya.ivvv.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fek.cdnleiting.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oae.jqgufenzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://gmt.yuanzhike.top

[N04] 斐波那契数列
来源：http://rbp.hongshengwenyu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zjp.aizwys.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://llx.guowangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iry.hcnkem.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://djd.jianghu66.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oxc.snrcjt.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cll.hywenlv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gwk.sweek.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vtt.yangfankeji.com

[N05] 最大公约数
来源：http://jyq.zhijiandao.cn

Py:   math.gcd(a, b)
来源：http://lpu.tianlin.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ftk.zhoulong.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nzx.316326.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qwq.ydzc1.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xwb.zhoulong.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://egn.redwolf501.top

Ruby: a.gcd(b)
来源：http://ucb.fktsv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mwt.xylfe.cn

[N06] 判断回文字符串
来源：http://ixw.gotoacloud.top

Py:   s == s[::-1]
来源：http://erh.guannengcc.top

PHP:  $s === strrev($s);
来源：http://fsj.mhx1999.top

JS:   s === [...s].reverse().join("")
来源：http://xwj.andypj.xyz

TS:   s === [...s].reverse().join("")
来源：http://smc.jqgufenzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aqj.tarul.cn

Go:   // 双指针从两端比较
来源：http://xet.cheryme.top

Ruby: s == s.reverse
来源：http://fyi.bjfxy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://tuz.nanxinkj.top

[N07] 两数之和（返回下标）
来源：http://aby.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bqp.wangshuangyany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ptm.fzhhl.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dhi.fehbvm.com

TS:   // 手写 Map<string, number>
来源：http://ubn.yueranfly.top

Java: // 手写 HashMap
来源：http://mcs.xuetiantiany.cn

Go:   // 手写 map[int]int
来源：http://wsa.shangyingyoupin.top

Ruby: // 手写 Hash
来源：http://wrc.yj20258888.top

C#:   // 手写 Dictionary<int, int>
来源：http://acs.shangyingyoupin.top

[N08] 生成全排列
来源：http://tld.quarkkingdee.top

Py:   itertools.permutations(arr)
来源：http://mjq.jinqigufen.top

PHP:  // 手写递归交换
来源：http://shm.nwbrower.top

JS:   // 手写回溯递归
来源：http://qia.ivvv.top

TS:   // 手写回溯递归
来源：http://vyr.0kj1m.cn

Java: // 手写回溯递归
来源：http://ths.hfpthk.cn

Go:   // 手写回溯递归
来源：http://lkb.cheryme.top

Ruby: arr.permutation.to_a
来源：http://vum.cdnleiting.top

C#:   // 手写回溯递归
来源：http://rpi.quarkkingdee.top

[N09] 栈与队列
来源：http://ixu.hywenlv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aso.ydzc1.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pay.fehbvm.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fjv.hesvh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://abw.tanke756.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cde.hnqzz.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ipl.cucudq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vun.ppjwa.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mdh.mhx1999.top

[N10] 链表节点定义
来源：http://xqt.xuetiantiany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sws.tanke756.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ziy.jqgfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wwu.yongpay.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://adi.zhijiandao.cn

Java: class Node { int v; Node next; }
来源：http://ecb.epnwcf.com

Go:   type Node struct { V int; Next *Node }
来源：http://xab.meibo888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://pwm.shangyingyoupin.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lwd.hnxiangtu.top

[N11] 二叉树中序遍历
来源：http://zmi.xziqi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zor.jyoumei.cn

PHP:  // 手写递归函数
来源：http://sfo.yj20258888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://alm.hcnkem.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ujo.tanke756.top

Java: // 手写递归
来源：http://nbr.jiagoushi.top

Go:   // 手写递归
来源：http://adi.0kj1m.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://utr.hfpthk.cn

C#:   // 手写递归
来源：http://jsk.ywan-chungtsiang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wig.hysaishi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wpw.ehwqpu.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kxv.meibo888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jmn.hnqzz.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pna.ehwqpu.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://par.tian-w.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ntk.ywan-chungtsiang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hvy.cdnleiting.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xvj.c1oappe.top

================================================================================
来源：http://smv.yvedp.cn

O. 并发与异步
来源：http://faw.cashguo.top

================================================================================
来源：http://awg.yuxming.cn

[O01] 启动一个线程
来源：http://rae.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qkw.ydjk.org.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rbt.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xhk.vqdsnc.cn

TS:   // 同 JS
来源：http://zbe.haohaochexian.top

Java: new Thread(() -> f()).start()
来源：http://bxa.ppjwa.cn

Go:   go f()
来源：http://jpq.zhoulong.xyz

Ruby: Thread.new { f }
来源：http://ilq.shuidangran.top

C#:   Task.Run(() => F());
来源：http://pvx.316326.xyz

[O02] 使用线程池
来源：http://ojq.zhiwuduotai.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nvx.ybcxt.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ssv.xingfuxueyuan.xyz

JS:   // worker_threads 线程池
来源：http://blx.yj20258888.top

TS:   // worker_threads 线程池
来源：http://psj.hywenlv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mfv.vehdjk.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ics.nanxuanxn.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oxk.ehwqpu.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eai.yfazqb.com

[O03] 加锁保护共享数据
来源：http://xtm.ppjwa.cn

Py:   with lock: shared += 1
来源：http://yra.xylfe.cn

PHP:  // 用 flock() 做文件锁
来源：http://yla.gzhubu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qpk.tanke756.top

TS:   // 同 JS
来源：http://avr.jqgfzy.top

Java: synchronized (this) { shared++; }
来源：http://qad.hnqzz.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://riu.yueranfly.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xrh.cashguo.top

C#:   lock (gate) { shared++; }
来源：http://pkv.sjlbkw.cn

[O04] 定义异步函数并等待
来源：http://kme.c1oappe.top

Py:   async def f():⏎    await g()
来源：http://dws.chenjidiqi.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://trr.daria6918.cn

JS:   async function f() { await g(); }
来源：http://uvh.9152youxi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qtb.sxryk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qer.chenjidiqi.icu

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ukp.0kj1m.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ipm.zhixingplan.top

C#:   async Task F() { await G(); }
来源：http://bff.xziqi.cn

[O05] 并发执行并等待全部完成
来源：http://bpx.fktsv.cn

Py:   asyncio.gather(*tasks)
来源：http://cmt.yuanzhike.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ffo.meibo888.top

JS:   await Promise.all(tasks)
来源：http://hck.chenzaomai.com

TS:   await Promise.all(tasks)
来源：http://ota.fengsongda.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fma.shuidangran.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qas.hnxiangtu.top

Ruby: threads.map(&:join)
来源：http://dyr.c1oappe.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hmh.bbcook.cn


<!-- 参考信息 -->