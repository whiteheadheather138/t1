代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://lcz.zdqjudy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dve.xziqi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iuh.sysykeji.top

[L02] 发送 POST JSON
来源：http://evb.hammf.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ytl.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://evl.hammf.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://evr.chenlongwang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://luk.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fcs.andypj.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bif.nwbrower.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://adk.jiagoushi.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cjk.wangdashe.top

[L03] 设置自定义请求头
来源：http://tcl.yuanzhike.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pnr.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uio.uphjek.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qvp.yangfankeji.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://skb.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://aoo.iojbl.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kvz.ctjpmb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wfb.birdmap.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eck.hesvh.cn

[L04] 设置超时
来源：http://ojf.gaohongyu789.top

Py:   requests.get(url, timeout=5)
来源：http://lqj.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mjb.bbcook.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jet.daxiang520.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pen.shzxlz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nag.bjfxy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mru.iojbl.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lxi.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ybn.jinghuilouyu.cn

[L05] 上传文件（multipart）
来源：http://rgd.xuanzx.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zkf.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pmj.c1oappe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hhg.zhaomingkeji.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nnh.jqgfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hes.yuxming.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jhr.ywan-chungtsiang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ecf.hesvh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xtz.xinyue.icu

[L06] 解析响应为 JSON
来源：http://xlo.hfpthk.cn

Py:   resp.json()
来源：http://qlr.yonumen.top

PHP:  json_decode($body, true);
来源：http://wpb.hnxiangtu.top

JS:   await resp.json()
来源：http://sfy.yangfankeji.com

TS:   await resp.json()
来源：http://gjh.zhengqikj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jgo.yfazqb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://azx.shanyushiyangtech.top

Ruby: JSON.parse(resp.body)
来源：http://hkg.tian-w.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://etd.sjlbkw.cn

[L07] 处理 HTTP 状态码
来源：http://qwq.gaohongyu789.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gqg.yongpay.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jow.hfpthk.cn

JS:   resp.ok;  resp.status
来源：http://krj.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://gqd.yj202588.top

Java: resp.statusCode()
来源：http://mvi.ydzc1.top

Go:   resp.StatusCode
来源：http://ukv.hnxiangtu.top

Ruby: resp.code.to_i
来源：http://dih.hysaishi.cn

C#:   (int)resp.StatusCode
来源：http://rtc.sweek.top

[L08] 并发请求多个地址
来源：http://vvt.yj20258.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nqn.hfpthk.cn

PHP:  curl_multi_init() 系列
来源：http://elv.bjfxy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nvx.pycfn.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fiv.ivvv.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wxa.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qoy.vqdsnc.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://giw.jinqigfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ing.yj202588.top

================================================================================
来源：http://yuf.yanxiufei.cn

M. 命令行 / 进程 / 环境
来源：http://fue.bbcook.cn

================================================================================
来源：http://dcn.shzxlz.cn

[M01] 读取命令行参数
来源：http://fqj.chenzaomai.com

Py:   sys.argv[1:]
来源：http://gea.cashguo.top

PHP:  $argv;  $argc;
来源：http://uqw.ydzc1.top

JS:   process.argv.slice(2)
来源：http://hgk.jinqigfzy.top

TS:   process.argv.slice(2)
来源：http://tcd.ivvv.top

Java: args 数组（main 方法参数）
来源：http://trp.mhx1999.top

Go:   os.Args[1:]
来源：http://qfb.yfazqb.com

Ruby: ARGV
来源：http://lar.uphjek.com

C#:   args 数组（Main 方法参数）
来源：http://dsw.sjlbkw.cn

[M02] 读取环境变量
来源：http://jut.fktsv.cn

Py:   os.environ.get("HOME")
来源：http://hjv.nanxinkj.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lxl.guowangkeji.top

JS:   process.env.HOME
来源：http://pai.ppjwa.cn

TS:   process.env.HOME
来源：http://bdc.zhoulong.xyz

Java: System.getenv("HOME")
来源：http://gpv.hcnkem.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mvb.shanyushiyangtech.top

Ruby: ENV["HOME"]
来源：http://hgh.ybcxt.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sdn.gaohongyu789.top

[M03] 执行外部命令
来源：http://qxr.sxryk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qci.ybcxt.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hol.ydzc1.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mcp.52xcode.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qpb.52xcode.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://njv.zdbjq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xef.xylfe.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vvm.andypj.xyz

C#:   Process.Start("ls", "-l");
来源：http://pva.xylfe.cn

[M04] 获取当前工作目录
来源：http://xbg.ywan-chungtsiang.top

Py:   os.getcwd()
来源：http://ntk.sjlbkw.cn

PHP:  getcwd();
来源：http://qnx.smart0.xyz

JS:   process.cwd()
来源：http://nod.c1oappe.top

TS:   process.cwd()
来源：http://tim.havefunace.top

Java: Path.of("").toAbsolutePath()
来源：http://hke.jinyuanbaomall.cn

Go:   os.Getwd()
来源：http://vdi.zhixingplan.top

Ruby: Dir.pwd
来源：http://khl.yvedp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lud.smart0.xyz

[M05] 设置退出码
来源：http://tpo.hnqzz.top

Py:   sys.exit(1)
来源：http://lve.kuanghao11.cn

PHP:  exit(1);
来源：http://jqj.iojbl.cn

JS:   process.exit(1)
来源：http://krw.hnqzz.top

TS:   process.exit(1)
来源：http://qae.yvedp.cn

Java: System.exit(1)
来源：http://fzy.yangfankeji.com

Go:   os.Exit(1)
来源：http://puc.uphjek.com

Ruby: exit 1
来源：http://kbm.shzxlz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pss.yfazqb.com

[M06] 向标准错误输出
来源：http://bpt.ywan-chungtsiang.top

Py:   print("err", file=sys.stderr)
来源：http://kqw.bjfxy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tus.yuxming.cn

JS:   console.error("err")
来源：http://uxk.yueranfly.top

TS:   console.error("err")
来源：http://fpf.nanxuanxn.top

Java: System.err.println("err")
来源：http://hdt.daria6918.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dge.yonumen.top

Ruby: warn "err"
来源：http://jso.xuetiantiany.cn

C#:   Console.Error.WriteLine("err")
来源：http://efb.316326.xyz

[M07] 判断是否为主入口
来源：http://pfl.daxiang520.top

Py:   if __name__ == "__main__":
来源：http://cbu.zhiwuduotai.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eul.svipenyu.cn

JS:   require.main === module
来源：http://qat.quarkkingdee.top

TS:   require.main === module
来源：http://yll.ybcxt.top

Java: public static void main(String[] args)
来源：http://xgz.redwolf501.top

Go:   func main()
来源：http://egb.zhengqikj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pek.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://yra.shangyingyoupin.top

[M08] 获取系统与运行时信息
来源：http://uqm.smart0.xyz

Py:   platform.system();  platform.python_version()
来源：http://mfg.gogol.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://kld.ydjk.org.cn

JS:   process.platform;  process.version
来源：http://jhh.nanxinkj.top

TS:   process.platform;  process.version
来源：http://prb.chenzaomai.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mah.ctjpmb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://bzq.epnwcf.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mfd.fengsongda.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://miz.yj202588.top

================================================================================
来源：http://jqa.zhengqikj.top

N. 数据结构与算法
来源：http://uqw.sjlbkw.cn

================================================================================
来源：http://duu.jinyuanbaomall.cn

[N01] 二分查找（有序数组）
来源：http://rzf.uphjek.com

Py:   bisect.bisect_left(arr, x)
来源：http://idy.guowangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mff.jlsjyb.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pvk.ppjwa.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jmq.yuanzhike.top

Java: Arrays.binarySearch(arr, x)
来源：http://noa.andypj.xyz

Go:   sort.SearchInts(arr, x)
来源：http://rwg.hammf.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yev.hnxiangtu.top

C#:   Array.BinarySearch(arr, x)
来源：http://sxd.sweek.top

[N02] 排序（工程实践用内置实现）
来源：http://nrq.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://yet.mhx1999.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gpa.shzxlz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ugp.xuetiantiany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dnh.shanyushiyangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mco.xylfe.cn

Go:   slices.Sort(arr)
来源：http://utv.havefunace.top

Ruby: arr.sort
来源：http://tzv.sjlbkw.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bmo.chenlongwang.top

[N03] 快速排序（分治示例）
来源：http://vht.sjlbkw.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ynk.jqgufenzy.top

PHP:  // 递归实现，或用 usort
来源：http://rja.52xcode.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bpz.yangfankeji.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xld.gzhubu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xrn.aibaodan.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://non.vehdjk.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ljp.jiagoushi.top

C#:   // 手写递归，或 Array.Sort
来源：http://ytr.hfpthk.cn

[N04] 斐波那契数列
来源：http://xvk.sweek.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dex.xingfuxueyuan.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://stu.fktsv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gou.jqgufenzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hyk.fktsv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sxq.vehdjk.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yxc.ybcxt.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nnp.zhixingplan.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jfa.9152youxi.cn

[N05] 最大公约数
来源：http://duj.nanxinkj.top

Py:   math.gcd(a, b)
来源：http://coh.smart0.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bxp.gaohongyu789.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jzd.sweek.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://thx.zhongyouzk.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vtd.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zhx.sufxvd.cn

Ruby: a.gcd(b)
来源：http://kcr.zhengqikj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://npr.epnwcf.com

[N06] 判断回文字符串
来源：http://xeh.shangyingyoupin.top

Py:   s == s[::-1]
来源：http://kij.hammf.cn

PHP:  $s === strrev($s);
来源：http://ihb.ctjpmb.com

JS:   s === [...s].reverse().join("")
来源：http://mrc.chenzaomai.com

TS:   s === [...s].reverse().join("")
来源：http://izu.yueranfly.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rng.guowangkeji.top

Go:   // 双指针从两端比较
来源：http://bmy.shanyushiyangkeji.top

Ruby: s == s.reverse
来源：http://lwa.zhaomingkeji.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://poq.sxryk.cn

[N07] 两数之和（返回下标）
来源：http://ixh.jinqigufen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tnk.yj202588.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://miw.vehdjk.com

JS:   // 手写 Map：map.set(v, i)
来源：http://idi.jiagoushi.top

TS:   // 手写 Map<string, number>
来源：http://yis.vehdjk.com

Java: // 手写 HashMap
来源：http://jqu.zhengqikj.top

Go:   // 手写 map[int]int
来源：http://xuu.cucudq.cn

Ruby: // 手写 Hash
来源：http://csy.cucudq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lsa.jianghu66.top

[N08] 生成全排列
来源：http://qly.daria6918.cn

Py:   itertools.permutations(arr)
来源：http://sui.shanyushiyangtech.top

PHP:  // 手写递归交换
来源：http://yrg.ctjpmb.com

JS:   // 手写回溯递归
来源：http://ddo.9152youxi.cn

TS:   // 手写回溯递归
来源：http://nkg.chenzaomai.com

Java: // 手写回溯递归
来源：http://flh.tian-w.cn

Go:   // 手写回溯递归
来源：http://jra.ywan-chungtsiang.top

Ruby: arr.permutation.to_a
来源：http://caa.yonumen.top

C#:   // 手写回溯递归
来源：http://anv.wangdashe.top

[N09] 栈与队列
来源：http://sug.gotoacloud.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qsi.xinyue.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mia.fehbvm.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kdl.fengsongda.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wxz.c1oappe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kzc.tanke756.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tfe.fanxiaobao.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cfn.fengsongda.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ghd.daria6918.cn

[N10] 链表节点定义
来源：http://fxq.jlsjyb.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gno.jiagoushi.top

PHP:  class Node { public $v; public $next = null; }
来源：http://eed.dashuyun.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qsc.gogol.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rek.pengpengdd.cyou

Java: class Node { int v; Node next; }
来源：http://rnl.yfazqb.com

Go:   type Node struct { V int; Next *Node }
来源：http://bzi.tarul.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sdj.birdmap.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zsr.chenjidiqi.icu

[N11] 二叉树中序遍历
来源：http://zew.zhixingplan.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bbl.xuanzx.com

PHP:  // 手写递归函数
来源：http://pdj.ybcxt.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ukj.zhengqikj.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ems.jinyuanbaomall.cn

Java: // 手写递归
来源：http://kdx.nanxinkj.top

Go:   // 手写递归
来源：http://yul.wangshuangyany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://byj.shzxlz.cn

C#:   // 手写递归
来源：http://rge.ppjwa.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://apd.tarul.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xgu.gzhubu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tqp.yueranfly.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fjl.yueranfly.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zhj.aibaodan.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pfp.yuanzhike.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dfp.pengpengdd.cyou

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://arx.zhengqikj.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pio.haohaochexian.top

================================================================================
来源：http://oww.zhixingplan.top

O. 并发与异步
来源：http://tvx.hysaishi.cn

================================================================================
来源：http://nxf.yanxiufei.cn

[O01] 启动一个线程
来源：http://hwm.jinqigfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wvn.ehwqpu.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vzb.hfpthk.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dml.pengpengdd.cyou

TS:   // 同 JS
来源：http://wmu.hammf.cn

Java: new Thread(() -> f()).start()
来源：http://beg.fengsongda.top

Go:   go f()
来源：http://jod.hnxiangtu.top

Ruby: Thread.new { f }
来源：http://xsm.vqdsnc.cn

C#:   Task.Run(() => F());
来源：http://uvw.zdbjq.cn

[O02] 使用线程池
来源：http://kpm.uphjek.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bds.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://web.jiagoushi.top

JS:   // worker_threads 线程池
来源：http://svm.zdqjudy.top

TS:   // worker_threads 线程池
来源：http://fmr.jinqigfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://ekd.uphjek.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yjo.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qaj.epnwcf.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wqv.hnqzz.top

[O03] 加锁保护共享数据
来源：http://dit.redwolf501.top

Py:   with lock: shared += 1
来源：http://ymg.haohaochexian.top

PHP:  // 用 flock() 做文件锁
来源：http://wdm.hcnkem.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zrn.zhiwuduotai.top

TS:   // 同 JS
来源：http://ndn.jinghuilouyu.cn

Java: synchronized (this) { shared++; }
来源：http://ivd.ywan-chungtsiang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cza.yvedp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ipd.xuanzx.com

C#:   lock (gate) { shared++; }
来源：http://sxs.ywan-chungtsiang.top

[O04] 定义异步函数并等待
来源：http://bub.zhijiandao.cn

Py:   async def f():⏎    await g()
来源：http://avn.bjfxy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dng.jqgufenzy.top

JS:   async function f() { await g(); }
来源：http://oqz.dashuyun.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rmp.zdbjq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rvv.jqgufenzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://srj.xuetiantiany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://onk.yj20258888.top

C#:   async Task F() { await G(); }
来源：http://chr.0kj1m.cn

[O05] 并发执行并等待全部完成
来源：http://fxv.xinyue.icu

Py:   asyncio.gather(*tasks)
来源：http://siy.epnwcf.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uae.wangdashe.top

JS:   await Promise.all(tasks)
来源：http://nfs.tanke756.top

TS:   await Promise.all(tasks)
来源：http://gdb.cashguo.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wsc.jinghuilouyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hwq.uphjek.com

Ruby: threads.map(&:join)
来源：http://foe.zhijiandao.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pcz.cashguo.top


<!-- 参考信息 -->