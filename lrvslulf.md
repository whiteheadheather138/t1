代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://lxx.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://try.ctjpmb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gvw.kuanghao11.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wlv.dashuyun.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qfn.chenjidiqi.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://axv.ydjk.org.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vim.hnqzz.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eqg.zhaomingkeji.xyz

[L03] 设置自定义请求头
来源：http://fuv.yfazqb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jig.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sws.chenzaomai.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bze.pycfn.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://epe.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wpg.iojbl.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wya.c1oappe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yua.fktsv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bqr.jlsjyb.cn

[L04] 设置超时
来源：http://qbw.shuidangran.top

Py:   requests.get(url, timeout=5)
来源：http://sfh.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ttr.shzxlz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xwf.hammf.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bon.sxryk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yrg.zhoulong.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nwg.pycfn.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aqm.9152youxi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yha.zdqjudy.top

[L05] 上传文件（multipart）
来源：http://lub.ppjwa.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ewc.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://duf.hywenlv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iyn.birdmap.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://run.pengpengdd.cyou

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://drw.zhijiandao.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xtp.shuidangran.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tyo.hywenlv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mwy.birdmap.top

[L06] 解析响应为 JSON
来源：http://rjq.tian-w.cn

Py:   resp.json()
来源：http://cmm.sysykeji.top

PHP:  json_decode($body, true);
来源：http://sry.meibo888.top

JS:   await resp.json()
来源：http://bsd.andypj.xyz

TS:   await resp.json()
来源：http://gip.jinqigfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ctb.hnxiangtu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fgy.shangyingyoupin.top

Ruby: JSON.parse(resp.body)
来源：http://dfg.chenzaomai.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cev.sufxvd.cn

[L07] 处理 HTTP 状态码
来源：http://yzc.yanxiufei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cxp.fanxiaobao.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pwg.tarul.cn

JS:   resp.ok;  resp.status
来源：http://cvp.jinqigfzy.top

TS:   resp.ok;  resp.status
来源：http://kpp.guowangkeji.top

Java: resp.statusCode()
来源：http://tll.hammf.cn

Go:   resp.StatusCode
来源：http://plh.yj202588.top

Ruby: resp.code.to_i
来源：http://scb.9152youxi.cn

C#:   (int)resp.StatusCode
来源：http://ztw.yanxiufei.cn

[L08] 并发请求多个地址
来源：http://okx.meibo888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hdl.sjlbkw.cn

PHP:  curl_multi_init() 系列
来源：http://yvs.hongshengwenyu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://imo.yanxiufei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bce.nanxinkj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ykp.guowangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pan.fktsv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vok.hywenlv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ccq.mhx1999.top

================================================================================
来源：http://zvr.dianchejie.cn

M. 命令行 / 进程 / 环境
来源：http://zda.ctjpmb.com

================================================================================
来源：http://tyi.chenlongwang.top

[M01] 读取命令行参数
来源：http://kjf.zhixingplan.top

Py:   sys.argv[1:]
来源：http://apx.ctjpmb.com

PHP:  $argv;  $argc;
来源：http://lpy.xuanzx.com

JS:   process.argv.slice(2)
来源：http://kdz.zhixingplan.top

TS:   process.argv.slice(2)
来源：http://ast.daria6918.cn

Java: args 数组（main 方法参数）
来源：http://ekf.yuanzhike.top

Go:   os.Args[1:]
来源：http://bgm.sxryk.cn

Ruby: ARGV
来源：http://pvs.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://bie.xuetiantiany.cn

[M02] 读取环境变量
来源：http://ivo.zhengqikj.top

Py:   os.environ.get("HOME")
来源：http://jqb.haohaochexian.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wxu.vqdsnc.cn

JS:   process.env.HOME
来源：http://ulj.chenlongwang.top

TS:   process.env.HOME
来源：http://rra.sweek.top

Java: System.getenv("HOME")
来源：http://ekd.chenzaomai.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rrr.yangfankeji.com

Ruby: ENV["HOME"]
来源：http://qfi.cheryme.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dlt.svipenyu.cn

[M03] 执行外部命令
来源：http://rgg.redwolf501.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fyo.jinqigfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tan.hfpthk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ylr.redwolf501.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qqn.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vyn.chenzaomai.com

Go:   exec.Command("ls", "-l").Output()
来源：http://fgc.52xcode.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zec.xuetiantiany.cn

C#:   Process.Start("ls", "-l");
来源：http://hve.hcnkem.com

[M04] 获取当前工作目录
来源：http://bcc.uphjek.com

Py:   os.getcwd()
来源：http://otp.zhiwuduotai.top

PHP:  getcwd();
来源：http://bsu.yonumen.top

JS:   process.cwd()
来源：http://amw.yfazqb.com

TS:   process.cwd()
来源：http://zrs.wangdashe.top

Java: Path.of("").toAbsolutePath()
来源：http://gsu.zhiwuduotai.top

Go:   os.Getwd()
来源：http://hvy.dashuyun.cn

Ruby: Dir.pwd
来源：http://sck.wangshuangyany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ljg.jinqigfzy.top

[M05] 设置退出码
来源：http://qkf.ctjpmb.com

Py:   sys.exit(1)
来源：http://lkg.redwolf501.top

PHP:  exit(1);
来源：http://bsd.zhiwuduotai.top

JS:   process.exit(1)
来源：http://lrj.xinyue.icu

TS:   process.exit(1)
来源：http://wdt.yfazqb.com

Java: System.exit(1)
来源：http://znt.yangfankeji.com

Go:   os.Exit(1)
来源：http://alx.cqqwz.cn

Ruby: exit 1
来源：http://yyg.fzhhl.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hfw.nanxuanxn.top

[M06] 向标准错误输出
来源：http://ghl.chenjidiqi.icu

Py:   print("err", file=sys.stderr)
来源：http://too.cdnleiting.top

PHP:  fwrite(STDERR, "err\n");
来源：http://acp.hammf.cn

JS:   console.error("err")
来源：http://kkl.andypj.xyz

TS:   console.error("err")
来源：http://nww.nanxinkj.top

Java: System.err.println("err")
来源：http://vuq.cqqwz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ubq.cdnleiting.top

Ruby: warn "err"
来源：http://dvv.yvedp.cn

C#:   Console.Error.WriteLine("err")
来源：http://chn.0kj1m.cn

[M07] 判断是否为主入口
来源：http://xlq.pengpengdd.cyou

Py:   if __name__ == "__main__":
来源：http://xrt.zhaomingkeji.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://niq.52xcode.cn

JS:   require.main === module
来源：http://qrh.guowangkeji.top

TS:   require.main === module
来源：http://xrp.jqgfzy.top

Java: public static void main(String[] args)
来源：http://oev.jianghu66.top

Go:   func main()
来源：http://yyc.xziqi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nye.zdbjq.cn

C#:   static void Main(string[] args)
来源：http://jup.iojbl.cn

[M08] 获取系统与运行时信息
来源：http://sig.sxryk.cn

Py:   platform.system();  platform.python_version()
来源：http://hsm.sxryk.cn

PHP:  PHP_OS;  phpversion();
来源：http://ogo.nwbrower.top

JS:   process.platform;  process.version
来源：http://kda.hongshengwenyu.top

TS:   process.platform;  process.version
来源：http://plc.ppjwa.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gre.tian-w.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wcq.cashguo.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nkb.tian-w.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://klk.daria6918.cn

================================================================================
来源：http://fuh.zdqjudy.top

N. 数据结构与算法
来源：http://rwp.birdmap.top

================================================================================
来源：http://udo.jlsjyb.cn

[N01] 二分查找（有序数组）
来源：http://lii.cashguo.top

Py:   bisect.bisect_left(arr, x)
来源：http://sxz.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bku.jqgufenzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vwv.ydzc1.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zfb.cdnleiting.top

Java: Arrays.binarySearch(arr, x)
来源：http://rvf.hywenlv.cn

Go:   sort.SearchInts(arr, x)
来源：http://eua.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://woc.nanxinkj.top

C#:   Array.BinarySearch(arr, x)
来源：http://qgj.316326.xyz

[N02] 排序（工程实践用内置实现）
来源：http://cln.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://dac.hnqzz.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cyk.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://jej.feifeiyinyue.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mnl.jiagoushi.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pln.ydzc1.top

Go:   slices.Sort(arr)
来源：http://rah.aibaodan.cn

Ruby: arr.sort
来源：http://nys.zhongyouzk.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yzg.fanxiaobao.xyz

[N03] 快速排序（分治示例）
来源：http://cpy.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://phl.bbcook.cn

PHP:  // 递归实现，或用 usort
来源：http://why.chenjidiqi.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://otl.daxiang520.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wgf.quarkkingdee.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nug.jyoumei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zkd.bbcook.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uog.nanxuanxn.top

C#:   // 手写递归，或 Array.Sort
来源：http://dej.xingfuxueyuan.xyz

[N04] 斐波那契数列
来源：http://fuv.nanxinkj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vkk.yj20258888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gbj.yongpay.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xrx.ivvv.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nqu.fktsv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jdq.fanxiaobao.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://okg.aizwys.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wqr.feifeiyinyue.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gvt.ppjwa.cn

[N05] 最大公约数
来源：http://dxx.dashuyun.cn

Py:   math.gcd(a, b)
来源：http://jce.nwbrower.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yop.tarul.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kdp.nanxuanxn.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://knc.yuanzhike.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zru.zdqjudy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pyi.0kj1m.cn

Ruby: a.gcd(b)
来源：http://cbg.shangyingyoupin.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bla.jiagoushi.top

[N06] 判断回文字符串
来源：http://quz.zhaomingkeji.xyz

Py:   s == s[::-1]
来源：http://hru.hnqzz.top

PHP:  $s === strrev($s);
来源：http://zob.shanyushiyangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://lsp.sweek.top

TS:   s === [...s].reverse().join("")
来源：http://mas.nwbrower.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://non.fktsv.cn

Go:   // 双指针从两端比较
来源：http://wnk.jlsjyb.cn

Ruby: s == s.reverse
来源：http://zcn.zhixingplan.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pxv.yongpay.top

[N07] 两数之和（返回下标）
来源：http://mms.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hzb.zhijiandao.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kdc.guowangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ihg.haohaochexian.top

TS:   // 手写 Map<string, number>
来源：http://gbz.meibo888.top

Java: // 手写 HashMap
来源：http://vta.shuidangran.top

Go:   // 手写 map[int]int
来源：http://qvj.aizwys.cn

Ruby: // 手写 Hash
来源：http://maf.cashguo.top

C#:   // 手写 Dictionary<int, int>
来源：http://mkf.jiagoushi.top

[N08] 生成全排列
来源：http://kpb.nanxuanxn.top

Py:   itertools.permutations(arr)
来源：http://jkl.cdnleiting.top

PHP:  // 手写递归交换
来源：http://mem.hnqzz.top

JS:   // 手写回溯递归
来源：http://chd.jiagoushi.top

TS:   // 手写回溯递归
来源：http://akf.zhengqikj.top

Java: // 手写回溯递归
来源：http://utw.sjlbkw.cn

Go:   // 手写回溯递归
来源：http://ycv.hfpthk.cn

Ruby: arr.permutation.to_a
来源：http://dkp.dianchejie.cn

C#:   // 手写回溯递归
来源：http://yoq.yvedp.cn

[N09] 栈与队列
来源：http://pts.yj202588.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pia.quarkkingdee.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://umk.cucudq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cod.xziqi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vkx.316326.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://grt.vehdjk.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kcz.316326.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qae.ehwqpu.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ole.gaohongyu789.top

[N10] 链表节点定义
来源：http://kpo.jianghu66.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tba.zdbjq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qyb.meibo888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xlm.jlsjyb.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ymo.dashuyun.cn

Java: class Node { int v; Node next; }
来源：http://ntu.cashguo.top

Go:   type Node struct { V int; Next *Node }
来源：http://iaz.pycfn.com

Ruby: Node = Struct.new(:v, :next)
来源：http://xew.hnxiangtu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zwk.gotoacloud.top

[N11] 二叉树中序遍历
来源：http://mxn.shanyushiyangtech.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vgx.gotoacloud.top

PHP:  // 手写递归函数
来源：http://eco.yongpay.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wwh.nanxinkj.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cnh.daria6918.cn

Java: // 手写递归
来源：http://ugp.havefunace.top

Go:   // 手写递归
来源：http://lvz.jianghu66.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ajb.hnxiangtu.top

C#:   // 手写递归
来源：http://ogx.vehdjk.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lpk.epnwcf.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bnn.zdqjudy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zhp.yj202588.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wxp.sxryk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yph.yonumen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jkn.zhixingplan.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blj.feifeiyinyue.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xxa.yj20258888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qsl.yj202588.top

================================================================================
来源：http://hgq.jinyuanbaomall.cn

O. 并发与异步
来源：http://nfm.gaohongyu789.top

================================================================================
来源：http://oqq.sjlbkw.cn

[O01] 启动一个线程
来源：http://xwt.jyoumei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fuk.zhiwuduotai.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mjx.shanyushiyangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xrb.kuanghao11.cn

TS:   // 同 JS
来源：http://hga.sufxvd.cn

Java: new Thread(() -> f()).start()
来源：http://flr.jyoumei.cn

Go:   go f()
来源：http://ahp.pengpengdd.cyou

Ruby: Thread.new { f }
来源：http://wfs.hnqzz.top

C#:   Task.Run(() => F());
来源：http://ico.jqgufenzy.top

[O02] 使用线程池
来源：http://jxt.wangshuangyany.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mzt.shangyingyoupin.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sam.hcnkem.com

JS:   // worker_threads 线程池
来源：http://qrm.ctjpmb.com

TS:   // worker_threads 线程池
来源：http://cjj.zycfv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sgr.jianghu66.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qwr.havefunace.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nzc.ehwqpu.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rdq.tanke756.top

[O03] 加锁保护共享数据
来源：http://tib.chenzaomai.com

Py:   with lock: shared += 1
来源：http://inv.ivvv.top

PHP:  // 用 flock() 做文件锁
来源：http://qfx.shangyingyoupin.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nro.gzhubu.top

TS:   // 同 JS
来源：http://tmp.fktsv.cn

Java: synchronized (this) { shared++; }
来源：http://api.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gar.cheryme.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://euc.cheryme.top

C#:   lock (gate) { shared++; }
来源：http://syr.nanxinkj.top

[O04] 定义异步函数并等待
来源：http://asa.cashguo.top

Py:   async def f():⏎    await g()
来源：http://wol.zhengqikj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://syl.xuetiantiany.cn

JS:   async function f() { await g(); }
来源：http://dzk.gogol.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qit.epnwcf.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jhu.cdnleiting.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rlf.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ljs.chenjidiqi.icu

C#:   async Task F() { await G(); }
来源：http://uyi.shangyingyoupin.top

[O05] 并发执行并等待全部完成
来源：http://nad.vqdsnc.cn

Py:   asyncio.gather(*tasks)
来源：http://xly.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jky.nanxinkj.top

JS:   await Promise.all(tasks)
来源：http://ums.hywenlv.cn

TS:   await Promise.all(tasks)
来源：http://drt.yangfankeji.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://shz.xinyue.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ogk.fanxiaobao.xyz

Ruby: threads.map(&:join)
来源：http://pxw.tianlin.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://qwu.feifeiyinyue.top

[O06] 使用进程池
来源：http://mfc.gotoacloud.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qwk.havefunace.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nbm.0kj1m.cn

JS:   // child_process / cluster 模块
来源：http://cam.fengsongda.top


<!-- 参考信息 -->