代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://leg.gogol.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ocu.yonumen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uhx.gzhubu.top

[L02] 发送 POST JSON
来源：http://ios.zhijiandao.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hso.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xff.c1oappe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fou.xylfe.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://prw.cashguo.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xap.cucudq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tpd.gzhubu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dcf.jqgfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ydg.ybcxt.top

[L03] 设置自定义请求头
来源：http://wpa.sjlbkw.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nxt.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://izn.zhaomingkeji.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nrb.jqgufenzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kaj.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yay.hnqzz.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vkl.zycfv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ego.quarkkingdee.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wxr.jinqigfzy.top

[L04] 设置超时
来源：http://ppt.tianlin.xyz

Py:   requests.get(url, timeout=5)
来源：http://vts.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ohe.xingfuxueyuan.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mwd.jlsjyb.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rfu.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ibu.gzhubu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jdf.hfpthk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://svu.daxiang520.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ywy.yuxming.cn

[L05] 上传文件（multipart）
来源：http://sbx.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ldf.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ufe.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eds.jinghuilouyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bsh.jinqigfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wuw.jinqigfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ngm.xuetiantiany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yza.shzxlz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qeo.yj202588.top

[L06] 解析响应为 JSON
来源：http://tyx.andypj.xyz

Py:   resp.json()
来源：http://mmm.tian-w.cn

PHP:  json_decode($body, true);
来源：http://sxj.shzxlz.cn

JS:   await resp.json()
来源：http://ijq.yj202588.top

TS:   await resp.json()
来源：http://opc.shanyushiyangtech.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aui.cucudq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ziv.meibo888.top

Ruby: JSON.parse(resp.body)
来源：http://bao.yj20258888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hbz.gogol.net.cn

[L07] 处理 HTTP 状态码
来源：http://fqb.pycfn.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mvx.jiagoushi.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ucj.fzhhl.top

JS:   resp.ok;  resp.status
来源：http://zuu.ydzc1.top

TS:   resp.ok;  resp.status
来源：http://pfl.shanyushiyangtech.top

Java: resp.statusCode()
来源：http://qcz.xylfe.cn

Go:   resp.StatusCode
来源：http://izw.yanxiufei.cn

Ruby: resp.code.to_i
来源：http://rje.xinyue.icu

C#:   (int)resp.StatusCode
来源：http://lop.aizwys.cn

[L08] 并发请求多个地址
来源：http://sfn.yvedp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qst.smart0.xyz

PHP:  curl_multi_init() 系列
来源：http://tgl.havefunace.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wjq.ctjpmb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gki.xziqi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dqx.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lxm.hnqzz.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iyi.ydjk.org.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kqi.fktsv.cn

================================================================================
来源：http://uxc.pycfn.com

M. 命令行 / 进程 / 环境
来源：http://qln.iojbl.cn

================================================================================
来源：http://tfr.9152youxi.cn

[M01] 读取命令行参数
来源：http://kyf.birdmap.top

Py:   sys.argv[1:]
来源：http://soe.zhaomingkeji.xyz

PHP:  $argv;  $argc;
来源：http://axb.zdbjq.cn

JS:   process.argv.slice(2)
来源：http://wnt.sufxvd.cn

TS:   process.argv.slice(2)
来源：http://sjt.bbcook.cn

Java: args 数组（main 方法参数）
来源：http://quq.dianchejie.cn

Go:   os.Args[1:]
来源：http://oab.dashuyun.cn

Ruby: ARGV
来源：http://nsn.xuetiantiany.cn

C#:   args 数组（Main 方法参数）
来源：http://bpx.hnxiangtu.top

[M02] 读取环境变量
来源：http://khf.epnwcf.com

Py:   os.environ.get("HOME")
来源：http://qta.jianghu66.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rum.chenlongwang.top

JS:   process.env.HOME
来源：http://foc.jianghu66.top

TS:   process.env.HOME
来源：http://urj.xingfuxueyuan.xyz

Java: System.getenv("HOME")
来源：http://jqi.wangdashe.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vsy.0kj1m.cn

Ruby: ENV["HOME"]
来源：http://dnk.shangyingyoupin.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kvp.chenzaomai.com

[M03] 执行外部命令
来源：http://hzz.ppjwa.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nos.c1oappe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oca.cheryme.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mmq.daria6918.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tkm.fengsongda.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ahq.tianlin.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://mdh.gaohongyu789.top

Ruby: system("ls -l");  `ls -l`
来源：http://txf.smart0.xyz

C#:   Process.Start("ls", "-l");
来源：http://pam.cucudq.cn

[M04] 获取当前工作目录
来源：http://ogo.fanxiaobao.xyz

Py:   os.getcwd()
来源：http://qyr.ctjpmb.com

PHP:  getcwd();
来源：http://xds.gzhubu.top

JS:   process.cwd()
来源：http://gig.feifeiyinyue.top

TS:   process.cwd()
来源：http://qzm.zdqjudy.top

Java: Path.of("").toAbsolutePath()
来源：http://dmn.ppjwa.cn

Go:   os.Getwd()
来源：http://oqp.ppjwa.cn

Ruby: Dir.pwd
来源：http://dyz.aizwys.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hhy.0kj1m.cn

[M05] 设置退出码
来源：http://jok.chenlongwang.top

Py:   sys.exit(1)
来源：http://twg.chenzaomai.com

PHP:  exit(1);
来源：http://zmm.yvedp.cn

JS:   process.exit(1)
来源：http://ccz.cheryme.top

TS:   process.exit(1)
来源：http://tfl.jqgfzy.top

Java: System.exit(1)
来源：http://ojv.cucudq.cn

Go:   os.Exit(1)
来源：http://fnv.birdmap.top

Ruby: exit 1
来源：http://nlq.bjfxy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ocq.epnwcf.com

[M06] 向标准错误输出
来源：http://gqr.yangfankeji.com

Py:   print("err", file=sys.stderr)
来源：http://ugv.zdbjq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gph.meibo888.top

JS:   console.error("err")
来源：http://cwv.yuanzhike.top

TS:   console.error("err")
来源：http://urt.9152youxi.cn

Java: System.err.println("err")
来源：http://mag.yanxiufei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ssr.xziqi.cn

Ruby: warn "err"
来源：http://icf.yfazqb.com

C#:   Console.Error.WriteLine("err")
来源：http://vkl.zdqjudy.top

[M07] 判断是否为主入口
来源：http://rfd.zdbjq.cn

Py:   if __name__ == "__main__":
来源：http://hvy.yueranfly.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wpx.jlsjyb.cn

JS:   require.main === module
来源：http://ajy.aizwys.cn

TS:   require.main === module
来源：http://ptl.xylfe.cn

Java: public static void main(String[] args)
来源：http://rea.hnqzz.top

Go:   func main()
来源：http://epw.hysaishi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ucj.shangyingyoupin.top

C#:   static void Main(string[] args)
来源：http://cdy.jinyuanbaomall.cn

[M08] 获取系统与运行时信息
来源：http://tbo.svipenyu.cn

Py:   platform.system();  platform.python_version()
来源：http://kcw.yj20258888.top

PHP:  PHP_OS;  phpversion();
来源：http://ecy.xuetiantiany.cn

JS:   process.platform;  process.version
来源：http://ixf.daxiang520.top

TS:   process.platform;  process.version
来源：http://foj.yj20258.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tjx.sweek.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wcf.c1oappe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kxi.guannengcc.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rrm.hnxiangtu.top

================================================================================
来源：http://tre.smart0.xyz

N. 数据结构与算法
来源：http://lkn.ydjk.org.cn

================================================================================
来源：http://ypz.chenlongwang.top

[N01] 二分查找（有序数组）
来源：http://whc.hywenlv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jix.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wkp.cqqwz.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mld.zhixingplan.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wha.iojbl.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dhw.zycfv.cn

Go:   sort.SearchInts(arr, x)
来源：http://ofk.yangfankeji.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://sne.andypj.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://zvd.aizwys.cn

[N02] 排序（工程实践用内置实现）
来源：http://pmh.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://lap.yongpay.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mxc.sjlbkw.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://amc.pengpengdd.cyou

TS:   [...arr].sort((a, b) => a - b)
来源：http://xys.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kwm.ppjwa.cn

Go:   slices.Sort(arr)
来源：http://cye.daxiang520.top

Ruby: arr.sort
来源：http://iuf.cashguo.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tgy.smart0.xyz

[N03] 快速排序（分治示例）
来源：http://xzb.hfpthk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eya.jyoumei.cn

PHP:  // 递归实现，或用 usort
来源：http://abz.xingfuxueyuan.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qwo.smart0.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gki.hfpthk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jjk.tianlin.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rdc.zdqjudy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ucr.zhixingplan.top

C#:   // 手写递归，或 Array.Sort
来源：http://bbi.hywenlv.cn

[N04] 斐波那契数列
来源：http://xdr.gotoacloud.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cyy.hcnkem.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wio.ivvv.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nky.chenzaomai.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bgc.ydzc1.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pqk.zhijiandao.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mlu.bjfxy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ewj.haohaochexian.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wop.meibo888.top

[N05] 最大公约数
来源：http://xax.gotoacloud.top

Py:   math.gcd(a, b)
来源：http://xbt.zhixingplan.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vui.zhaomingkeji.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nsd.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cmt.xylfe.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zbk.chenzaomai.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wxd.nanxinkj.top

Ruby: a.gcd(b)
来源：http://klg.xinyue.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rav.jyoumei.cn

[N06] 判断回文字符串
来源：http://prb.birdmap.top

Py:   s == s[::-1]
来源：http://sqr.jyoumei.cn

PHP:  $s === strrev($s);
来源：http://oui.ydzc1.top

JS:   s === [...s].reverse().join("")
来源：http://qnj.tarul.cn

TS:   s === [...s].reverse().join("")
来源：http://vco.xziqi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dvo.nanxuanxn.top

Go:   // 双指针从两端比较
来源：http://zbz.zhijiandao.cn

Ruby: s == s.reverse
来源：http://jrq.sweek.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://olr.zhongyouzk.top

[N07] 两数之和（返回下标）
来源：http://akv.cheryme.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jku.jiagoushi.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wvy.vqdsnc.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://blz.yongpay.top

TS:   // 手写 Map<string, number>
来源：http://hmj.jinqigfzy.top

Java: // 手写 HashMap
来源：http://wsa.jqgufenzy.top

Go:   // 手写 map[int]int
来源：http://smu.aizwys.cn

Ruby: // 手写 Hash
来源：http://ona.jlsjyb.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pgz.jinyuanbaomall.cn

[N08] 生成全排列
来源：http://ebb.nwbrower.top

Py:   itertools.permutations(arr)
来源：http://pay.daria6918.cn

PHP:  // 手写递归交换
来源：http://vwg.fzhhl.top

JS:   // 手写回溯递归
来源：http://kpo.vqdsnc.cn

TS:   // 手写回溯递归
来源：http://ibi.andypj.xyz

Java: // 手写回溯递归
来源：http://hjn.cashguo.top

Go:   // 手写回溯递归
来源：http://kol.yj20258.top

Ruby: arr.permutation.to_a
来源：http://jaq.vehdjk.com

C#:   // 手写回溯递归
来源：http://rha.jianghu66.top

[N09] 栈与队列
来源：http://zeb.ppjwa.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cxf.aizwys.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ozi.zdqjudy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mzz.xuanzx.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ebi.jiagoushi.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wxl.zhongyouzk.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bon.yangfankeji.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ngv.aibaodan.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xwb.cheryme.top

[N10] 链表节点定义
来源：http://tgl.xylfe.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ipu.tanke756.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cpw.wangshuangyany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://veo.zdbjq.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bin.havefunace.top

Java: class Node { int v; Node next; }
来源：http://vjt.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://pmc.yueranfly.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qbc.zdqjudy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bwo.yj202588.top

[N11] 二叉树中序遍历
来源：http://crj.yonumen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wcp.hnqzz.top

PHP:  // 手写递归函数
来源：http://wiw.smart0.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zin.cashguo.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://plv.316326.xyz

Java: // 手写递归
来源：http://ahu.gzhubu.top

Go:   // 手写递归
来源：http://mou.zhixingplan.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ina.ydzc1.top

C#:   // 手写递归
来源：http://dgb.ivvv.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oac.chenjidiqi.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rlv.daria6918.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kgk.mhx1999.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cut.xziqi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wxk.xuanzx.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mvo.shanyushiyangtech.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ewu.daria6918.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://igk.hnqzz.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aie.tian-w.cn

================================================================================
来源：http://inx.zhengqikj.top

O. 并发与异步
来源：http://yax.zhijiandao.cn

================================================================================
来源：http://mxc.zhoulong.xyz

[O01] 启动一个线程
来源：http://pke.fengsongda.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jou.zdbjq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kal.pycfn.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gbn.sxryk.cn

TS:   // 同 JS
来源：http://lyx.316326.xyz

Java: new Thread(() -> f()).start()
来源：http://guv.ydzc1.top

Go:   go f()
来源：http://fwy.chenzaomai.com

Ruby: Thread.new { f }
来源：http://iek.xinyue.icu

C#:   Task.Run(() => F());
来源：http://wse.mhx1999.top

[O02] 使用线程池
来源：http://qyp.yanxiufei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://aeb.chenjidiqi.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://afs.pycfn.com

JS:   // worker_threads 线程池
来源：http://qcb.hcnkem.com

TS:   // worker_threads 线程池
来源：http://mnk.zdqjudy.top

Java: Executors.newFixedThreadPool(4)
来源：http://olc.haohaochexian.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zjp.ehwqpu.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xul.nanxinkj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://asz.316326.xyz

[O03] 加锁保护共享数据
来源：http://uua.gzhubu.top

Py:   with lock: shared += 1
来源：http://qim.nanxuanxn.top

PHP:  // 用 flock() 做文件锁
来源：http://ose.mhx1999.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mmg.jinghuilouyu.cn

TS:   // 同 JS
来源：http://ume.jyoumei.cn

Java: synchronized (this) { shared++; }
来源：http://emi.zhiwuduotai.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aab.jinyuanbaomall.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dop.shanyushiyangtech.top

C#:   lock (gate) { shared++; }
来源：http://bqd.fktsv.cn

[O04] 定义异步函数并等待
来源：http://biu.ydzc1.top

Py:   async def f():⏎    await g()
来源：http://rhv.ydjk.org.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fog.wangdashe.top

JS:   async function f() { await g(); }
来源：http://qrk.316326.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://jac.yj20258.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xfs.hcnkem.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hea.xziqi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qth.hfpthk.cn

C#:   async Task F() { await G(); }
来源：http://foi.andypj.xyz

[O05] 并发执行并等待全部完成
来源：http://oux.tian-w.cn

Py:   asyncio.gather(*tasks)
来源：http://kge.daria6918.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kux.daxiang520.top

JS:   await Promise.all(tasks)
来源：http://yqx.ehwqpu.com

TS:   await Promise.all(tasks)
来源：http://lfz.zdqjudy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ywc.ppjwa.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rrs.yanxiufei.cn

Ruby: threads.map(&:join)
来源：http://pdf.svipenyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qtz.ivvv.top


<!-- 参考信息 -->