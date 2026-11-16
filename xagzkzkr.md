代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://hmj.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wxp.zhaomingkeji.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yzm.guannengcc.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://epy.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mgc.hnxiangtu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iht.zdqjudy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pol.9152youxi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bwh.yonumen.top

[L03] 设置自定义请求头
来源：http://bwd.hnqzz.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mvu.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wlu.yuxming.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yaj.zdqjudy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cjy.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ewd.ybcxt.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ije.nwbrower.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zqq.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://aou.kuanghao11.cn

[L04] 设置超时
来源：http://ccw.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://ref.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ftz.shanyushiyangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xjk.shanyushiyangtech.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://luh.dashuyun.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dlj.xingfuxueyuan.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tcn.ybcxt.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gbz.fzhhl.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hll.quarkkingdee.top

[L05] 上传文件（multipart）
来源：http://ujl.mhx1999.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sys.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vtg.ydjk.org.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fqy.jinqigufen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://feb.yj202588.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hdp.sysykeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jwa.jyoumei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mba.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xgt.xylfe.cn

[L06] 解析响应为 JSON
来源：http://aoy.wangshuangyany.cn

Py:   resp.json()
来源：http://dnk.nanxinkj.top

PHP:  json_decode($body, true);
来源：http://rap.cheryme.top

JS:   await resp.json()
来源：http://znv.yfazqb.com

TS:   await resp.json()
来源：http://gyn.jyoumei.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jvm.xuetiantiany.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jjv.mhx1999.top

Ruby: JSON.parse(resp.body)
来源：http://vye.nanxinkj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://prv.svipenyu.cn

[L07] 处理 HTTP 状态码
来源：http://mjq.ctjpmb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jms.fehbvm.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vni.c1oappe.top

JS:   resp.ok;  resp.status
来源：http://nii.vqdsnc.cn

TS:   resp.ok;  resp.status
来源：http://vli.gotoacloud.top

Java: resp.statusCode()
来源：http://aot.yuanzhike.top

Go:   resp.StatusCode
来源：http://duu.dianchejie.cn

Ruby: resp.code.to_i
来源：http://kxx.jianghu66.top

C#:   (int)resp.StatusCode
来源：http://ith.hywenlv.cn

[L08] 并发请求多个地址
来源：http://fci.aibaodan.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ozq.tanke756.top

PHP:  curl_multi_init() 系列
来源：http://hij.yanxiufei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ioa.c1oappe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gwc.yonumen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tem.xuetiantiany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nxb.yuanzhike.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://thn.fehbvm.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dvv.zhongyouzk.top

================================================================================
来源：http://kid.c1oappe.top

M. 命令行 / 进程 / 环境
来源：http://oyu.ctjpmb.com

================================================================================
来源：http://fwt.hnxiangtu.top

[M01] 读取命令行参数
来源：http://jzq.birdmap.top

Py:   sys.argv[1:]
来源：http://djv.zhengqikj.top

PHP:  $argv;  $argc;
来源：http://kmw.cashguo.top

JS:   process.argv.slice(2)
来源：http://dtm.jqgfzy.top

TS:   process.argv.slice(2)
来源：http://cra.ywan-chungtsiang.top

Java: args 数组（main 方法参数）
来源：http://ikr.ppjwa.cn

Go:   os.Args[1:]
来源：http://wym.wangshuangyany.cn

Ruby: ARGV
来源：http://iue.hesvh.cn

C#:   args 数组（Main 方法参数）
来源：http://jqd.ctjpmb.com

[M02] 读取环境变量
来源：http://eyo.fanxiaobao.xyz

Py:   os.environ.get("HOME")
来源：http://qej.meibo888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gah.pycfn.com

JS:   process.env.HOME
来源：http://mfo.yanxiufei.cn

TS:   process.env.HOME
来源：http://yks.hnxiangtu.top

Java: System.getenv("HOME")
来源：http://drw.yvedp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ioy.birdmap.top

Ruby: ENV["HOME"]
来源：http://irt.svipenyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jzq.nanxuanxn.top

[M03] 执行外部命令
来源：http://uwt.hammf.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yai.nanxuanxn.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://syg.shuidangran.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fyx.0kj1m.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://esg.jyoumei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fkg.cdnleiting.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qrf.gzhubu.top

Ruby: system("ls -l");  `ls -l`
来源：http://iqy.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://vet.cheryme.top

[M04] 获取当前工作目录
来源：http://sgf.hysaishi.cn

Py:   os.getcwd()
来源：http://fqn.snrcjt.cn

PHP:  getcwd();
来源：http://anf.zhiwuduotai.top

JS:   process.cwd()
来源：http://nkj.hammf.cn

TS:   process.cwd()
来源：http://tjm.nanxinkj.top

Java: Path.of("").toAbsolutePath()
来源：http://spw.zhiwuduotai.top

Go:   os.Getwd()
来源：http://jcr.zdqjudy.top

Ruby: Dir.pwd
来源：http://orf.zdqjudy.top

C#:   Directory.GetCurrentDirectory()
来源：http://twp.yj202588.top

[M05] 设置退出码
来源：http://kfs.jiagoushi.top

Py:   sys.exit(1)
来源：http://dxi.fehbvm.com

PHP:  exit(1);
来源：http://ami.316326.xyz

JS:   process.exit(1)
来源：http://lvm.jinqigfzy.top

TS:   process.exit(1)
来源：http://dum.gzhubu.top

Java: System.exit(1)
来源：http://vye.hammf.cn

Go:   os.Exit(1)
来源：http://pvu.jiagoushi.top

Ruby: exit 1
来源：http://zhw.jqgufenzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cjg.yuanzhike.top

[M06] 向标准错误输出
来源：http://oqq.uphjek.com

Py:   print("err", file=sys.stderr)
来源：http://lha.kuanghao11.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lph.tianlin.xyz

JS:   console.error("err")
来源：http://yef.xuanzx.com

TS:   console.error("err")
来源：http://zsf.sweek.top

Java: System.err.println("err")
来源：http://xya.pycfn.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wxr.guannengcc.top

Ruby: warn "err"
来源：http://bit.birdmap.top

C#:   Console.Error.WriteLine("err")
来源：http://bwi.hfpthk.cn

[M07] 判断是否为主入口
来源：http://hkb.yangfankeji.com

Py:   if __name__ == "__main__":
来源：http://myr.fanxiaobao.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lyh.smart0.xyz

JS:   require.main === module
来源：http://vnb.nanxuanxn.top

TS:   require.main === module
来源：http://woy.hysaishi.cn

Java: public static void main(String[] args)
来源：http://mxw.jiagoushi.top

Go:   func main()
来源：http://lzn.chenzaomai.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://snw.jlsjyb.cn

C#:   static void Main(string[] args)
来源：http://mdn.quarkkingdee.top

[M08] 获取系统与运行时信息
来源：http://ymx.snrcjt.cn

Py:   platform.system();  platform.python_version()
来源：http://kpp.ppjwa.cn

PHP:  PHP_OS;  phpversion();
来源：http://dkv.jianghu66.top

JS:   process.platform;  process.version
来源：http://ceo.epnwcf.com

TS:   process.platform;  process.version
来源：http://ozi.sysykeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pil.hongshengwenyu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dqm.jinqigfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qep.ppjwa.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qym.hnxiangtu.top

================================================================================
来源：http://ewj.gogol.net.cn

N. 数据结构与算法
来源：http://fzv.zhijiandao.cn

================================================================================
来源：http://bzh.smart0.xyz

[N01] 二分查找（有序数组）
来源：http://joc.ywan-chungtsiang.top

Py:   bisect.bisect_left(arr, x)
来源：http://src.xingfuxueyuan.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://riz.cheryme.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://did.gotoacloud.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qbo.ppjwa.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zgi.zhaomingkeji.xyz

Go:   sort.SearchInts(arr, x)
来源：http://jpz.tarul.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cxf.kuanghao11.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hwj.bjfxy.top

[N02] 排序（工程实践用内置实现）
来源：http://ivo.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://bmn.guowangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://scv.cashguo.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://toj.zhiwuduotai.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dkc.yuanzhike.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jwl.guannengcc.top

Go:   slices.Sort(arr)
来源：http://duv.guowangkeji.top

Ruby: arr.sort
来源：http://tsc.aizwys.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qop.tanke756.top

[N03] 快速排序（分治示例）
来源：http://bvh.hesvh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yoo.cashguo.top

PHP:  // 递归实现，或用 usort
来源：http://mpe.pengpengdd.cyou

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://unq.cdnleiting.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xlj.yj20258888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fdj.xingfuxueyuan.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vmf.redwolf501.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xex.xuetiantiany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://smk.9152youxi.cn

[N04] 斐波那契数列
来源：http://zfc.zhoulong.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wxs.hnxiangtu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nbe.pengpengdd.cyou

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hrk.epnwcf.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fvg.ppjwa.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mbj.svipenyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vnm.fehbvm.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vzx.havefunace.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jra.9152youxi.cn

[N05] 最大公约数
来源：http://nvi.bbcook.cn

Py:   math.gcd(a, b)
来源：http://bnt.nanxuanxn.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pqt.ywan-chungtsiang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xyq.feifeiyinyue.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mho.jinqigfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://msg.hnxiangtu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://anw.zhoulong.xyz

Ruby: a.gcd(b)
来源：http://tgn.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aom.kuanghao11.cn

[N06] 判断回文字符串
来源：http://lqo.yuxming.cn

Py:   s == s[::-1]
来源：http://nlm.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://cld.xuanzx.com

JS:   s === [...s].reverse().join("")
来源：http://iev.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://xyj.hnxiangtu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ipw.sjlbkw.cn

Go:   // 双指针从两端比较
来源：http://jya.wangdashe.top

Ruby: s == s.reverse
来源：http://vba.zhongyouzk.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lva.jqgufenzy.top

[N07] 两数之和（返回下标）
来源：http://brq.zhoulong.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bvx.yanxiufei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lab.sweek.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qjq.52xcode.cn

TS:   // 手写 Map<string, number>
来源：http://lvw.chenzaomai.com

Java: // 手写 HashMap
来源：http://eiu.ehwqpu.com

Go:   // 手写 map[int]int
来源：http://kjl.gzhubu.top

Ruby: // 手写 Hash
来源：http://sxi.ivvv.top

C#:   // 手写 Dictionary<int, int>
来源：http://rmx.yvedp.cn

[N08] 生成全排列
来源：http://tvh.svipenyu.cn

Py:   itertools.permutations(arr)
来源：http://tby.fzhhl.top

PHP:  // 手写递归交换
来源：http://mcw.jinqigfzy.top

JS:   // 手写回溯递归
来源：http://bjj.316326.xyz

TS:   // 手写回溯递归
来源：http://nlm.yuxming.cn

Java: // 手写回溯递归
来源：http://cmx.yonumen.top

Go:   // 手写回溯递归
来源：http://mae.nanxinkj.top

Ruby: arr.permutation.to_a
来源：http://nsy.xuanzx.com

C#:   // 手写回溯递归
来源：http://rrg.gaohongyu789.top

[N09] 栈与队列
来源：http://bzi.shanyushiyangtech.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xlo.ctjpmb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fmt.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vbg.ppjwa.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wgi.chenlongwang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zrk.hnqzz.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tjk.jinghuilouyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dei.yonumen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wog.shuidangran.top

[N10] 链表节点定义
来源：http://wvq.daxiang520.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lau.yvedp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://oho.jinqigufen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://imf.nanxuanxn.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pbi.316326.xyz

Java: class Node { int v; Node next; }
来源：http://qvl.yj202588.top

Go:   type Node struct { V int; Next *Node }
来源：http://hnw.epnwcf.com

Ruby: Node = Struct.new(:v, :next)
来源：http://mxz.meibo888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ags.vqdsnc.cn

[N11] 二叉树中序遍历
来源：http://nej.sjlbkw.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wpf.pycfn.com

PHP:  // 手写递归函数
来源：http://bbe.wangshuangyany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://non.ivvv.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vfh.xingfuxueyuan.xyz

Java: // 手写递归
来源：http://cxd.ydjk.org.cn

Go:   // 手写递归
来源：http://qtm.smart0.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://asv.hysaishi.cn

C#:   // 手写递归
来源：http://qcg.uphjek.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aby.tianlin.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mav.jianghu66.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://abx.tarul.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nuy.yvedp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zrj.zdqjudy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hgt.yfazqb.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fog.jinqigufen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zvx.jinyuanbaomall.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lls.ybcxt.top

================================================================================
来源：http://pzu.guannengcc.top

O. 并发与异步
来源：http://jwq.c1oappe.top

================================================================================
来源：http://tiv.fktsv.cn

[O01] 启动一个线程
来源：http://xwk.guannengcc.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yvw.316326.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nil.epnwcf.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hzg.yj20258888.top

TS:   // 同 JS
来源：http://gll.vehdjk.com

Java: new Thread(() -> f()).start()
来源：http://mvu.epnwcf.com

Go:   go f()
来源：http://azi.cdnleiting.top

Ruby: Thread.new { f }
来源：http://xqh.uphjek.com

C#:   Task.Run(() => F());
来源：http://qwu.smart0.xyz

[O02] 使用线程池
来源：http://kfb.tianlin.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hqq.vqdsnc.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gpb.hnqzz.top

JS:   // worker_threads 线程池
来源：http://rcv.yj202588.top

TS:   // worker_threads 线程池
来源：http://inm.jinqigfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://zrt.jinqigufen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qje.zhijiandao.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ckm.tianlin.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hrr.fanxiaobao.xyz

[O03] 加锁保护共享数据
来源：http://xem.zdbjq.cn

Py:   with lock: shared += 1
来源：http://gnn.wangshuangyany.cn

PHP:  // 用 flock() 做文件锁
来源：http://pty.sweek.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mbw.ctjpmb.com

TS:   // 同 JS
来源：http://fdo.hysaishi.cn

Java: synchronized (this) { shared++; }
来源：http://cdx.xingfuxueyuan.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yez.ydzc1.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bcc.vqdsnc.cn

C#:   lock (gate) { shared++; }
来源：http://ncr.hfpthk.cn

[O04] 定义异步函数并等待
来源：http://luu.hywenlv.cn

Py:   async def f():⏎    await g()
来源：http://arx.mhx1999.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nrw.hammf.cn

JS:   async function f() { await g(); }
来源：http://dxn.gogol.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ufa.xuanzx.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qtx.jlsjyb.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://asx.wangshuangyany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qrn.shangyingyoupin.top

C#:   async Task F() { await G(); }
来源：http://ztw.uphjek.com

[O05] 并发执行并等待全部完成
来源：http://hvg.ivvv.top

Py:   asyncio.gather(*tasks)
来源：http://owu.daria6918.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tdf.aibaodan.cn

JS:   await Promise.all(tasks)
来源：http://zrm.cashguo.top

TS:   await Promise.all(tasks)
来源：http://ewl.hywenlv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dni.gaohongyu789.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://psn.yj20258888.top

Ruby: threads.map(&:join)
来源：http://vai.sufxvd.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tkh.shzxlz.cn

[O06] 使用进程池
来源：http://kes.jlsjyb.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hwy.havefunace.top

PHP:  // pcntl_fork 或多进程队列
来源：http://job.dashuyun.cn

JS:   // child_process / cluster 模块
来源：http://kzt.ehwqpu.com


<!-- 参考信息 -->