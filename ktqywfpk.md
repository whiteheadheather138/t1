代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pqn.quarkkingdee.top

JS:   await fetch(url)
来源：http://ymi.dianchejie.cn

TS:   await fetch(url)
来源：http://ezv.ydzc1.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uss.dashuyun.cn

Go:   resp, err := http.Get(url)
来源：http://iea.chenzaomai.com

Ruby: Net::HTTP.get(URI(url))
来源：http://huv.mhx1999.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uth.zhongyouzk.top

[L02] 发送 POST JSON
来源：http://nkx.gotoacloud.top

Py:   requests.post(url, json={"a": 1})
来源：http://mkg.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://meh.yfazqb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eyw.ehwqpu.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://few.316326.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nbo.cucudq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://piq.chenlongwang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qvl.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://prw.daria6918.cn

[L03] 设置自定义请求头
来源：http://dnf.hysaishi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jru.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xfi.hongshengwenyu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dmi.tarul.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dbi.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zkj.shangyingyoupin.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mxm.yj20258.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pfw.meibo888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gnm.tarul.cn

[L04] 设置超时
来源：http://ttx.cdnleiting.top

Py:   requests.get(url, timeout=5)
来源：http://dkd.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://syb.cheryme.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jvc.shanyushiyangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://orp.shanyushiyangtech.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://krt.sxryk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kmo.vehdjk.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ogx.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zur.mhx1999.top

[L05] 上传文件（multipart）
来源：http://jlf.xinyue.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://czi.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://phv.hesvh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gbr.yongpay.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://djw.quarkkingdee.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://amw.fengsongda.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kqg.svipenyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tdm.jinghuilouyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://upf.fengsongda.top

[L06] 解析响应为 JSON
来源：http://cmt.hnqzz.top

Py:   resp.json()
来源：http://tem.sjlbkw.cn

PHP:  json_decode($body, true);
来源：http://gbt.nwbrower.top

JS:   await resp.json()
来源：http://eog.hywenlv.cn

TS:   await resp.json()
来源：http://oll.zdqjudy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lvk.ydjk.org.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kvd.chenlongwang.top

Ruby: JSON.parse(resp.body)
来源：http://nwx.zhixingplan.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dyc.dashuyun.cn

[L07] 处理 HTTP 状态码
来源：http://vxz.nanxinkj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zvh.ppjwa.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://spe.jqgufenzy.top

JS:   resp.ok;  resp.status
来源：http://mjh.guannengcc.top

TS:   resp.ok;  resp.status
来源：http://scp.c1oappe.top

Java: resp.statusCode()
来源：http://ryv.hysaishi.cn

Go:   resp.StatusCode
来源：http://brz.yonumen.top

Ruby: resp.code.to_i
来源：http://yrl.hesvh.cn

C#:   (int)resp.StatusCode
来源：http://vid.ydzc1.top

[L08] 并发请求多个地址
来源：http://saw.vqdsnc.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ine.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://ltf.dashuyun.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://you.epnwcf.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jop.tarul.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mwh.jyoumei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://byy.c1oappe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ils.daxiang520.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iqg.shangyingyoupin.top

================================================================================
来源：http://bih.ehwqpu.com

M. 命令行 / 进程 / 环境
来源：http://yub.zhixingplan.top

================================================================================
来源：http://khq.cucudq.cn

[M01] 读取命令行参数
来源：http://igs.jiagoushi.top

Py:   sys.argv[1:]
来源：http://tjq.ctjpmb.com

PHP:  $argv;  $argc;
来源：http://kcv.quarkkingdee.top

JS:   process.argv.slice(2)
来源：http://fwc.shuidangran.top

TS:   process.argv.slice(2)
来源：http://lrz.xuetiantiany.cn

Java: args 数组（main 方法参数）
来源：http://jgp.feifeiyinyue.top

Go:   os.Args[1:]
来源：http://zva.gzhubu.top

Ruby: ARGV
来源：http://okt.9152youxi.cn

C#:   args 数组（Main 方法参数）
来源：http://sag.yj20258888.top

[M02] 读取环境变量
来源：http://fwb.hfpthk.cn

Py:   os.environ.get("HOME")
来源：http://ljc.sufxvd.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pba.shanyushiyangkeji.top

JS:   process.env.HOME
来源：http://jbi.tanke756.top

TS:   process.env.HOME
来源：http://iay.jqgufenzy.top

Java: System.getenv("HOME")
来源：http://udn.wangdashe.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bfu.cucudq.cn

Ruby: ENV["HOME"]
来源：http://wzt.hnqzz.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://opp.hcnkem.com

[M03] 执行外部命令
来源：http://ebt.yuanzhike.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xjp.xinyue.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kth.hcnkem.com

JS:   child_process.execSync("ls -l").toString()
来源：http://wht.cdnleiting.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lnf.gzhubu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uxk.zhixingplan.top

Go:   exec.Command("ls", "-l").Output()
来源：http://isx.smart0.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://bam.shangyingyoupin.top

C#:   Process.Start("ls", "-l");
来源：http://gwo.yanxiufei.cn

[M04] 获取当前工作目录
来源：http://nzc.nanxinkj.top

Py:   os.getcwd()
来源：http://mrp.zdqjudy.top

PHP:  getcwd();
来源：http://pym.epnwcf.com

JS:   process.cwd()
来源：http://lja.xinyue.icu

TS:   process.cwd()
来源：http://tut.yongpay.top

Java: Path.of("").toAbsolutePath()
来源：http://nrr.quarkkingdee.top

Go:   os.Getwd()
来源：http://euz.yvedp.cn

Ruby: Dir.pwd
来源：http://xht.aizwys.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xvy.ppjwa.cn

[M05] 设置退出码
来源：http://nrt.yanxiufei.cn

Py:   sys.exit(1)
来源：http://zdf.shanyushiyangkeji.top

PHP:  exit(1);
来源：http://jvx.yonumen.top

JS:   process.exit(1)
来源：http://nez.haohaochexian.top

TS:   process.exit(1)
来源：http://kff.sweek.top

Java: System.exit(1)
来源：http://nre.jiagoushi.top

Go:   os.Exit(1)
来源：http://ifd.yj202588.top

Ruby: exit 1
来源：http://cwt.jinqigufen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zev.mhx1999.top

[M06] 向标准错误输出
来源：http://ksx.meibo888.top

Py:   print("err", file=sys.stderr)
来源：http://pwe.snrcjt.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://eup.sysykeji.top

JS:   console.error("err")
来源：http://okw.shzxlz.cn

TS:   console.error("err")
来源：http://uxe.ehwqpu.com

Java: System.err.println("err")
来源：http://ysz.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jee.xinyue.icu

Ruby: warn "err"
来源：http://eov.tianlin.xyz

C#:   Console.Error.WriteLine("err")
来源：http://dhr.yj20258888.top

[M07] 判断是否为主入口
来源：http://grl.jiagoushi.top

Py:   if __name__ == "__main__":
来源：http://ztv.tarul.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yre.epnwcf.com

JS:   require.main === module
来源：http://ipo.guowangkeji.top

TS:   require.main === module
来源：http://enb.daria6918.cn

Java: public static void main(String[] args)
来源：http://puf.sysykeji.top

Go:   func main()
来源：http://pir.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bkp.jinqigfzy.top

C#:   static void Main(string[] args)
来源：http://emh.mhx1999.top

[M08] 获取系统与运行时信息
来源：http://sop.zdbjq.cn

Py:   platform.system();  platform.python_version()
来源：http://otc.tianlin.xyz

PHP:  PHP_OS;  phpversion();
来源：http://ohx.jinghuilouyu.cn

JS:   process.platform;  process.version
来源：http://jko.vqdsnc.cn

TS:   process.platform;  process.version
来源：http://xnh.jinghuilouyu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xuw.jinqigufen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xyz.tarul.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uzq.jyoumei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nbr.cashguo.top

================================================================================
来源：http://bxb.hongshengwenyu.top

N. 数据结构与算法
来源：http://qtp.bbcook.cn

================================================================================
来源：http://dqr.yj202588.top

[N01] 二分查找（有序数组）
来源：http://spl.shangyingyoupin.top

Py:   bisect.bisect_left(arr, x)
来源：http://cvl.gzhubu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rav.zdqjudy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hde.ybcxt.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zne.yfazqb.com

Java: Arrays.binarySearch(arr, x)
来源：http://pii.xziqi.cn

Go:   sort.SearchInts(arr, x)
来源：http://wii.xinyue.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://ziw.zhaomingkeji.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://pcm.9152youxi.cn

[N02] 排序（工程实践用内置实现）
来源：http://vda.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://wqp.xziqi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zif.yueranfly.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://atx.316326.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://bkj.xingfuxueyuan.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sha.hywenlv.cn

Go:   slices.Sort(arr)
来源：http://grl.zhongyouzk.top

Ruby: arr.sort
来源：http://yuf.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://bij.yfazqb.com

[N03] 快速排序（分治示例）
来源：http://fmb.shuidangran.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gok.gogol.net.cn

PHP:  // 递归实现，或用 usort
来源：http://olz.haohaochexian.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tuf.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rat.epnwcf.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zlm.chenzaomai.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zrt.cucudq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sfz.havefunace.top

C#:   // 手写递归，或 Array.Sort
来源：http://tkr.ydjk.org.cn

[N04] 斐波那契数列
来源：http://khx.vehdjk.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kfi.xuetiantiany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xpi.jlsjyb.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ibe.hywenlv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zig.daria6918.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vul.ehwqpu.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fdl.mhx1999.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lus.52xcode.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://euw.yvedp.cn

[N05] 最大公约数
来源：http://idv.xuanzx.com

Py:   math.gcd(a, b)
来源：http://trb.shanyushiyangtech.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://edx.yongpay.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gdl.jiagoushi.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qle.feifeiyinyue.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hga.sxryk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://esz.hywenlv.cn

Ruby: a.gcd(b)
来源：http://msl.chenzaomai.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://arw.wangshuangyany.cn

[N06] 判断回文字符串
来源：http://dgz.bjfxy.top

Py:   s == s[::-1]
来源：http://hxj.meibo888.top

PHP:  $s === strrev($s);
来源：http://zba.jinqigfzy.top

JS:   s === [...s].reverse().join("")
来源：http://nrv.svipenyu.cn

TS:   s === [...s].reverse().join("")
来源：http://sao.fengsongda.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aek.kuanghao11.cn

Go:   // 双指针从两端比较
来源：http://isn.vqdsnc.cn

Ruby: s == s.reverse
来源：http://bed.guannengcc.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hye.pycfn.com

[N07] 两数之和（返回下标）
来源：http://ljk.cdnleiting.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dhi.zhijiandao.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rdh.cucudq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pkk.zhoulong.xyz

TS:   // 手写 Map<string, number>
来源：http://yxf.hongshengwenyu.top

Java: // 手写 HashMap
来源：http://tbx.jiagoushi.top

Go:   // 手写 map[int]int
来源：http://irj.andypj.xyz

Ruby: // 手写 Hash
来源：http://uee.zdqjudy.top

C#:   // 手写 Dictionary<int, int>
来源：http://wmh.316326.xyz

[N08] 生成全排列
来源：http://ckj.yj20258888.top

Py:   itertools.permutations(arr)
来源：http://xsx.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://mwf.nanxinkj.top

JS:   // 手写回溯递归
来源：http://peu.yj20258888.top

TS:   // 手写回溯递归
来源：http://zwk.xinyue.icu

Java: // 手写回溯递归
来源：http://viu.yj202588.top

Go:   // 手写回溯递归
来源：http://aei.ydzc1.top

Ruby: arr.permutation.to_a
来源：http://hbr.gaohongyu789.top

C#:   // 手写回溯递归
来源：http://yvm.jinghuilouyu.cn

[N09] 栈与队列
来源：http://fym.ydzc1.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zgj.xinyue.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://shl.wangshuangyany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://skw.hammf.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oql.hnqzz.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ijj.zhengqikj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://knz.daria6918.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rty.jianghu66.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xot.smart0.xyz

[N10] 链表节点定义
来源：http://pio.zhiwuduotai.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://khs.jlsjyb.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uki.havefunace.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ovj.iojbl.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eif.snrcjt.cn

Java: class Node { int v; Node next; }
来源：http://ozk.xingfuxueyuan.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://gck.iojbl.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dnz.316326.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://rfa.ehwqpu.com

[N11] 二叉树中序遍历
来源：http://cwt.kuanghao11.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ukn.ehwqpu.com

PHP:  // 手写递归函数
来源：http://nir.hnxiangtu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://osd.hongshengwenyu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://izs.yj202588.top

Java: // 手写递归
来源：http://mqt.ivvv.top

Go:   // 手写递归
来源：http://adc.andypj.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cnh.xziqi.cn

C#:   // 手写递归
来源：http://png.havefunace.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hih.zdqjudy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://htj.aibaodan.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zji.yanxiufei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cok.yj20258888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zjf.cashguo.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wmn.iojbl.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ohw.vehdjk.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nxb.yonumen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zgf.shzxlz.cn

================================================================================
来源：http://eca.yangfankeji.com

O. 并发与异步
来源：http://xwk.cdnleiting.top

================================================================================
来源：http://gcj.zhixingplan.top

[O01] 启动一个线程
来源：http://kas.hnxiangtu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://asc.hnqzz.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://beq.yj20258.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tze.yj20258.top

TS:   // 同 JS
来源：http://isj.xuetiantiany.cn

Java: new Thread(() -> f()).start()
来源：http://gnu.fzhhl.top

Go:   go f()
来源：http://sec.jinyuanbaomall.cn

Ruby: Thread.new { f }
来源：http://uci.yj20258888.top

C#:   Task.Run(() => F());
来源：http://yax.jinqigufen.top

[O02] 使用线程池
来源：http://kfh.birdmap.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://apo.nwbrower.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bdt.jianghu66.top

JS:   // worker_threads 线程池
来源：http://uar.havefunace.top

TS:   // worker_threads 线程池
来源：http://aju.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://ekg.birdmap.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rug.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aof.52xcode.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nle.yanxiufei.cn

[O03] 加锁保护共享数据
来源：http://wpv.haohaochexian.top

Py:   with lock: shared += 1
来源：http://uxh.ppjwa.cn

PHP:  // 用 flock() 做文件锁
来源：http://ssi.tianlin.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dup.zdbjq.cn

TS:   // 同 JS
来源：http://yuo.ehwqpu.com

Java: synchronized (this) { shared++; }
来源：http://lil.hnxiangtu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://inr.zdbjq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://odf.52xcode.cn

C#:   lock (gate) { shared++; }
来源：http://por.aibaodan.cn

[O04] 定义异步函数并等待
来源：http://qev.chenjidiqi.icu

Py:   async def f():⏎    await g()
来源：http://dbe.zycfv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://evp.feifeiyinyue.top

JS:   async function f() { await g(); }
来源：http://gnb.0kj1m.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hbg.zhongyouzk.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nsp.daxiang520.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mxl.xuanzx.com

Ruby: # 用 Fiber 或 async gem
来源：http://vyf.aibaodan.cn

C#:   async Task F() { await G(); }
来源：http://zdm.yueranfly.top

[O05] 并发执行并等待全部完成
来源：http://aqu.hesvh.cn

Py:   asyncio.gather(*tasks)
来源：http://enq.epnwcf.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iwm.vqdsnc.cn

JS:   await Promise.all(tasks)
来源：http://owz.yueranfly.top

TS:   await Promise.all(tasks)
来源：http://uch.tianlin.xyz


<!-- 参考信息 -->