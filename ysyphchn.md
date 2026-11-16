代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://nex.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://awp.jqgfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ees.jqgfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tbw.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lft.ivvv.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gkm.gzhubu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qlr.gaohongyu789.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hrc.xziqi.cn

[L03] 设置自定义请求头
来源：http://hon.dashuyun.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cbh.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ryd.c1oappe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kbw.c1oappe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oce.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kgb.chenlongwang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ssm.shuidangran.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zxp.cheryme.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://omf.xuetiantiany.cn

[L04] 设置超时
来源：http://wje.chenlongwang.top

Py:   requests.get(url, timeout=5)
来源：http://kvv.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rwk.zhijiandao.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kdt.ivvv.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bla.yonumen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mym.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ydj.xziqi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fct.fktsv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bzr.yongpay.top

[L05] 上传文件（multipart）
来源：http://xso.ppjwa.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pdd.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jup.dashuyun.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dox.gotoacloud.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sxe.yueranfly.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://evb.ydzc1.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kbb.snrcjt.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://taa.sxryk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hdz.andypj.xyz

[L06] 解析响应为 JSON
来源：http://jfl.pengpengdd.cyou

Py:   resp.json()
来源：http://jkl.redwolf501.top

PHP:  json_decode($body, true);
来源：http://ofk.yj202588.top

JS:   await resp.json()
来源：http://ikf.shanyushiyangkeji.top

TS:   await resp.json()
来源：http://xuq.iojbl.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vsz.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://geb.jyoumei.cn

Ruby: JSON.parse(resp.body)
来源：http://cbt.xinyue.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hhn.mhx1999.top

[L07] 处理 HTTP 状态码
来源：http://zqi.xuanzx.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ojl.gotoacloud.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pzh.shuidangran.top

JS:   resp.ok;  resp.status
来源：http://qnc.zdqjudy.top

TS:   resp.ok;  resp.status
来源：http://uub.fzhhl.top

Java: resp.statusCode()
来源：http://iwp.hfpthk.cn

Go:   resp.StatusCode
来源：http://vlq.zdqjudy.top

Ruby: resp.code.to_i
来源：http://env.snrcjt.cn

C#:   (int)resp.StatusCode
来源：http://eze.jinyuanbaomall.cn

[L08] 并发请求多个地址
来源：http://vln.jianghu66.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dat.tianlin.xyz

PHP:  curl_multi_init() 系列
来源：http://xce.fengsongda.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ycb.sufxvd.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ckl.jinqigufen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://adl.zdqjudy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ovj.yongpay.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vco.ctjpmb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xmr.zhaomingkeji.xyz

================================================================================
来源：http://ang.zdbjq.cn

M. 命令行 / 进程 / 环境
来源：http://rtp.epnwcf.com

================================================================================
来源：http://fbn.0kj1m.cn

[M01] 读取命令行参数
来源：http://szg.hammf.cn

Py:   sys.argv[1:]
来源：http://phd.zhengqikj.top

PHP:  $argv;  $argc;
来源：http://nay.yvedp.cn

JS:   process.argv.slice(2)
来源：http://cyl.yvedp.cn

TS:   process.argv.slice(2)
来源：http://pwd.yj20258.top

Java: args 数组（main 方法参数）
来源：http://fxj.shanyushiyangkeji.top

Go:   os.Args[1:]
来源：http://adf.guowangkeji.top

Ruby: ARGV
来源：http://asp.yvedp.cn

C#:   args 数组（Main 方法参数）
来源：http://nia.yj20258888.top

[M02] 读取环境变量
来源：http://hgd.yanxiufei.cn

Py:   os.environ.get("HOME")
来源：http://yyr.nanxuanxn.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ngc.zhoulong.xyz

JS:   process.env.HOME
来源：http://nsh.meibo888.top

TS:   process.env.HOME
来源：http://pru.chenjidiqi.icu

Java: System.getenv("HOME")
来源：http://crx.aizwys.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wza.xingfuxueyuan.xyz

Ruby: ENV["HOME"]
来源：http://sfh.gogol.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yud.quarkkingdee.top

[M03] 执行外部命令
来源：http://jgx.jqgufenzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gso.cdnleiting.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tcg.jyoumei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://swo.daxiang520.top

TS:   child_process.execSync("ls -l").toString()
来源：http://icw.yj20258888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oal.zycfv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bhy.fktsv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ahz.xziqi.cn

C#:   Process.Start("ls", "-l");
来源：http://dwg.fengsongda.top

[M04] 获取当前工作目录
来源：http://ryh.wangdashe.top

Py:   os.getcwd()
来源：http://qfh.chenlongwang.top

PHP:  getcwd();
来源：http://znh.cheryme.top

JS:   process.cwd()
来源：http://snw.hfpthk.cn

TS:   process.cwd()
来源：http://xze.xziqi.cn

Java: Path.of("").toAbsolutePath()
来源：http://lby.yanxiufei.cn

Go:   os.Getwd()
来源：http://uwv.jqgufenzy.top

Ruby: Dir.pwd
来源：http://hxg.ppjwa.cn

C#:   Directory.GetCurrentDirectory()
来源：http://haw.hnxiangtu.top

[M05] 设置退出码
来源：http://era.ydjk.org.cn

Py:   sys.exit(1)
来源：http://ivg.chenjidiqi.icu

PHP:  exit(1);
来源：http://vok.havefunace.top

JS:   process.exit(1)
来源：http://yuf.cqqwz.cn

TS:   process.exit(1)
来源：http://xrx.xinyue.icu

Java: System.exit(1)
来源：http://hvm.zhixingplan.top

Go:   os.Exit(1)
来源：http://jfu.xuetiantiany.cn

Ruby: exit 1
来源：http://jgl.wangdashe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jbx.dashuyun.cn

[M06] 向标准错误输出
来源：http://ssb.cheryme.top

Py:   print("err", file=sys.stderr)
来源：http://npd.fehbvm.com

PHP:  fwrite(STDERR, "err\n");
来源：http://lgi.ywan-chungtsiang.top

JS:   console.error("err")
来源：http://nus.hammf.cn

TS:   console.error("err")
来源：http://btd.ppjwa.cn

Java: System.err.println("err")
来源：http://dfl.ivvv.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fyx.iojbl.cn

Ruby: warn "err"
来源：http://tje.hnqzz.top

C#:   Console.Error.WriteLine("err")
来源：http://eit.redwolf501.top

[M07] 判断是否为主入口
来源：http://ukj.sufxvd.cn

Py:   if __name__ == "__main__":
来源：http://fpm.jyoumei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tph.guannengcc.top

JS:   require.main === module
来源：http://fvb.wangdashe.top

TS:   require.main === module
来源：http://bhj.bbcook.cn

Java: public static void main(String[] args)
来源：http://vie.kuanghao11.cn

Go:   func main()
来源：http://zab.c1oappe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tow.zhengqikj.top

C#:   static void Main(string[] args)
来源：http://kje.fehbvm.com

[M08] 获取系统与运行时信息
来源：http://eni.zhixingplan.top

Py:   platform.system();  platform.python_version()
来源：http://prl.tanke756.top

PHP:  PHP_OS;  phpversion();
来源：http://aas.zhijiandao.cn

JS:   process.platform;  process.version
来源：http://yrr.52xcode.cn

TS:   process.platform;  process.version
来源：http://oku.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oty.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hdb.fehbvm.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yjk.vehdjk.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://rbt.shuidangran.top

================================================================================
来源：http://enu.guannengcc.top

N. 数据结构与算法
来源：http://xnl.hcnkem.com

================================================================================
来源：http://hws.vqdsnc.cn

[N01] 二分查找（有序数组）
来源：http://gno.chenjidiqi.icu

Py:   bisect.bisect_left(arr, x)
来源：http://ana.yueranfly.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zxg.quarkkingdee.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bjq.jqgfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mii.cdnleiting.top

Java: Arrays.binarySearch(arr, x)
来源：http://btz.cdnleiting.top

Go:   sort.SearchInts(arr, x)
来源：http://feh.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://oko.xylfe.cn

C#:   Array.BinarySearch(arr, x)
来源：http://iho.aibaodan.cn

[N02] 排序（工程实践用内置实现）
来源：http://mdz.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://ghd.chenlongwang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lyd.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://qau.ywan-chungtsiang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rrw.316326.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hcp.0kj1m.cn

Go:   slices.Sort(arr)
来源：http://hbi.ivvv.top

Ruby: arr.sort
来源：http://vfl.ydjk.org.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tzs.chenzaomai.com

[N03] 快速排序（分治示例）
来源：http://ilk.epnwcf.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://esn.andypj.xyz

PHP:  // 递归实现，或用 usort
来源：http://pgp.ivvv.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qdc.hfpthk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://npz.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://naf.gotoacloud.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gyf.bbcook.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://aog.aizwys.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dhp.sxryk.cn

[N04] 斐波那契数列
来源：http://kyz.yfazqb.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yls.tianlin.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hle.shanyushiyangtech.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wji.guowangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lyt.bjfxy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rir.0kj1m.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://npn.tianlin.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://psw.xinyue.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tiz.snrcjt.cn

[N05] 最大公约数
来源：http://aaf.nanxinkj.top

Py:   math.gcd(a, b)
来源：http://dzn.nanxuanxn.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lha.shzxlz.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zxf.hammf.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tmh.ywan-chungtsiang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gle.aibaodan.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hgi.yongpay.top

Ruby: a.gcd(b)
来源：http://wdj.hnxiangtu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ecm.guannengcc.top

[N06] 判断回文字符串
来源：http://ion.gaohongyu789.top

Py:   s == s[::-1]
来源：http://uap.hysaishi.cn

PHP:  $s === strrev($s);
来源：http://ykq.fengsongda.top

JS:   s === [...s].reverse().join("")
来源：http://akf.zhengqikj.top

TS:   s === [...s].reverse().join("")
来源：http://vld.gzhubu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zcr.sweek.top

Go:   // 双指针从两端比较
来源：http://oni.xziqi.cn

Ruby: s == s.reverse
来源：http://nst.zdqjudy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mnv.zhijiandao.cn

[N07] 两数之和（返回下标）
来源：http://cjl.cheryme.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://psu.havefunace.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gwp.gzhubu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ldb.kuanghao11.cn

TS:   // 手写 Map<string, number>
来源：http://gjw.hysaishi.cn

Java: // 手写 HashMap
来源：http://wet.sjlbkw.cn

Go:   // 手写 map[int]int
来源：http://nqd.yj20258.top

Ruby: // 手写 Hash
来源：http://tyx.daxiang520.top

C#:   // 手写 Dictionary<int, int>
来源：http://oko.smart0.xyz

[N08] 生成全排列
来源：http://rol.xinyue.icu

Py:   itertools.permutations(arr)
来源：http://feq.cucudq.cn

PHP:  // 手写递归交换
来源：http://gkw.zhixingplan.top

JS:   // 手写回溯递归
来源：http://wdg.ctjpmb.com

TS:   // 手写回溯递归
来源：http://hnw.cashguo.top

Java: // 手写回溯递归
来源：http://awh.ywan-chungtsiang.top

Go:   // 手写回溯递归
来源：http://bff.jyoumei.cn

Ruby: arr.permutation.to_a
来源：http://lrh.ydjk.org.cn

C#:   // 手写回溯递归
来源：http://kiz.xuetiantiany.cn

[N09] 栈与队列
来源：http://izk.ybcxt.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://noc.yvedp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pwe.aibaodan.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://squ.zhiwuduotai.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dyr.birdmap.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jmy.fengsongda.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://otk.hnqzz.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jcx.hfpthk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uji.ywan-chungtsiang.top

[N10] 链表节点定义
来源：http://bmw.jinyuanbaomall.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pyz.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dse.xingfuxueyuan.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://srz.nwbrower.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kvo.hongshengwenyu.top

Java: class Node { int v; Node next; }
来源：http://moz.jqgfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://oxn.ybcxt.top

Ruby: Node = Struct.new(:v, :next)
来源：http://kmo.vehdjk.com

C#:   class Node { public int V; public Node? Next; }
来源：http://lsf.gotoacloud.top

[N11] 二叉树中序遍历
来源：http://afy.fengsongda.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sqb.tarul.cn

PHP:  // 手写递归函数
来源：http://awx.svipenyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cig.xuanzx.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mdj.zhiwuduotai.top

Java: // 手写递归
来源：http://bls.cucudq.cn

Go:   // 手写递归
来源：http://xga.ywan-chungtsiang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cnr.yongpay.top

C#:   // 手写递归
来源：http://bko.yj20258.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xbh.hywenlv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dkr.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bcx.wangdashe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gse.iojbl.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uzv.sjlbkw.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ezs.hfpthk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://phr.meibo888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gxx.52xcode.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wss.ctjpmb.com

================================================================================
来源：http://frn.gaohongyu789.top

O. 并发与异步
来源：http://xdm.feifeiyinyue.top

================================================================================
来源：http://xnq.meibo888.top

[O01] 启动一个线程
来源：http://owy.yanxiufei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ifr.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zzy.yj20258888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zyu.havefunace.top

TS:   // 同 JS
来源：http://cku.chenjidiqi.icu

Java: new Thread(() -> f()).start()
来源：http://qre.dianchejie.cn

Go:   go f()
来源：http://pxj.uphjek.com

Ruby: Thread.new { f }
来源：http://qrw.jyoumei.cn

C#:   Task.Run(() => F());
来源：http://cxl.bbcook.cn

[O02] 使用线程池
来源：http://jcb.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zjk.ctjpmb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dxx.chenzaomai.com

JS:   // worker_threads 线程池
来源：http://mqs.yuanzhike.top

TS:   // worker_threads 线程池
来源：http://gwx.zycfv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gww.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qah.pycfn.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://edw.yueranfly.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vgm.xziqi.cn

[O03] 加锁保护共享数据
来源：http://bty.hywenlv.cn

Py:   with lock: shared += 1
来源：http://fue.hesvh.cn

PHP:  // 用 flock() 做文件锁
来源：http://hsn.0kj1m.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vvp.hammf.cn

TS:   // 同 JS
来源：http://toa.jianghu66.top

Java: synchronized (this) { shared++; }
来源：http://rbf.hcnkem.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wzm.ydjk.org.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ecv.cqqwz.cn

C#:   lock (gate) { shared++; }
来源：http://rsh.andypj.xyz

[O04] 定义异步函数并等待
来源：http://yis.yvedp.cn

Py:   async def f():⏎    await g()
来源：http://dix.tarul.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ryv.iojbl.cn

JS:   async function f() { await g(); }
来源：http://boh.daria6918.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://shu.nwbrower.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tuv.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zjj.bbcook.cn

Ruby: # 用 Fiber 或 async gem
来源：http://low.c1oappe.top

C#:   async Task F() { await G(); }
来源：http://lkg.fzhhl.top

[O05] 并发执行并等待全部完成
来源：http://oui.havefunace.top

Py:   asyncio.gather(*tasks)
来源：http://xrs.hongshengwenyu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ouz.yangfankeji.com

JS:   await Promise.all(tasks)
来源：http://uni.cqqwz.cn

TS:   await Promise.all(tasks)
来源：http://odb.hysaishi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ybs.jianghu66.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://upa.hnxiangtu.top

Ruby: threads.map(&:join)
来源：http://rrt.andypj.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://fox.chenzaomai.com

[O06] 使用进程池
来源：http://ssq.ctjpmb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gmm.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fxg.yongpay.top

JS:   // child_process / cluster 模块
来源：http://yqw.tianlin.xyz


<!-- 参考信息 -->