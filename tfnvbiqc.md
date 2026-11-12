代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://bri.redwolf501.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tdi.haohaochexian.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tls.nanxuanxn.top

[L02] 发送 POST JSON
来源：http://lwn.sweek.top

Py:   requests.post(url, json={"a": 1})
来源：http://jhz.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uam.andypj.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oek.jinqigufen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nxe.yj202588.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://epw.yonumen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bji.vqdsnc.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hti.ywan-chungtsiang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wbc.wangshuangyany.cn

[L03] 设置自定义请求头
来源：http://xgk.daxiang520.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://erl.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vtb.bjfxy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rej.fehbvm.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qke.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rhk.havefunace.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bzn.feifeiyinyue.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eyj.svipenyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jvx.yonumen.top

[L04] 设置超时
来源：http://cmn.mhx1999.top

Py:   requests.get(url, timeout=5)
来源：http://wyv.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://euq.yuxming.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tvn.xingfuxueyuan.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://axf.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sjw.tianlin.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jfp.cashguo.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sih.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://poo.kuanghao11.cn

[L05] 上传文件（multipart）
来源：http://zpx.jinghuilouyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://itu.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xdl.pycfn.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://aax.fengsongda.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zwm.hnxiangtu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vnv.zhixingplan.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uxi.aibaodan.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vup.daria6918.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xcl.jinyuanbaomall.cn

[L06] 解析响应为 JSON
来源：http://zqz.yueranfly.top

Py:   resp.json()
来源：http://ksc.ydzc1.top

PHP:  json_decode($body, true);
来源：http://xfs.cqqwz.cn

JS:   await resp.json()
来源：http://zvr.zdqjudy.top

TS:   await resp.json()
来源：http://xka.gzhubu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gkp.snrcjt.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iky.yvedp.cn

Ruby: JSON.parse(resp.body)
来源：http://gxx.birdmap.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qho.nwbrower.top

[L07] 处理 HTTP 状态码
来源：http://hsr.wangdashe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kzf.uphjek.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://byi.chenzaomai.com

JS:   resp.ok;  resp.status
来源：http://mcy.gaohongyu789.top

TS:   resp.ok;  resp.status
来源：http://rzf.zhongyouzk.top

Java: resp.statusCode()
来源：http://yoc.shuidangran.top

Go:   resp.StatusCode
来源：http://exn.yuanzhike.top

Ruby: resp.code.to_i
来源：http://rah.pengpengdd.cyou

C#:   (int)resp.StatusCode
来源：http://bca.zhixingplan.top

[L08] 并发请求多个地址
来源：http://pyn.9152youxi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fyb.meibo888.top

PHP:  curl_multi_init() 系列
来源：http://eoq.tanke756.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wpk.dashuyun.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gsw.sweek.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tky.sjlbkw.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kwk.ivvv.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://klc.andypj.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aus.aibaodan.cn

================================================================================
来源：http://plj.epnwcf.com

M. 命令行 / 进程 / 环境
来源：http://rfu.wangshuangyany.cn

================================================================================
来源：http://nnk.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://khx.yueranfly.top

Py:   sys.argv[1:]
来源：http://iuu.gotoacloud.top

PHP:  $argv;  $argc;
来源：http://lzc.dianchejie.cn

JS:   process.argv.slice(2)
来源：http://xlz.ybcxt.top

TS:   process.argv.slice(2)
来源：http://bdx.nanxinkj.top

Java: args 数组（main 方法参数）
来源：http://qxz.ydzc1.top

Go:   os.Args[1:]
来源：http://tkr.jiagoushi.top

Ruby: ARGV
来源：http://hnt.chenlongwang.top

C#:   args 数组（Main 方法参数）
来源：http://vec.guowangkeji.top

[M02] 读取环境变量
来源：http://shm.guowangkeji.top

Py:   os.environ.get("HOME")
来源：http://bte.tarul.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jjz.0kj1m.cn

JS:   process.env.HOME
来源：http://zyr.sweek.top

TS:   process.env.HOME
来源：http://abo.redwolf501.top

Java: System.getenv("HOME")
来源：http://cyp.svipenyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fzn.fzhhl.top

Ruby: ENV["HOME"]
来源：http://oap.hcnkem.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xdm.jianghu66.top

[M03] 执行外部命令
来源：http://tdi.xingfuxueyuan.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cmx.sxryk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gpk.tian-w.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nfs.wangdashe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hhh.yangfankeji.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rcd.yuxming.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://prf.daxiang520.top

Ruby: system("ls -l");  `ls -l`
来源：http://yxp.zhengqikj.top

C#:   Process.Start("ls", "-l");
来源：http://gso.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://jho.zhoulong.xyz

Py:   os.getcwd()
来源：http://ydm.guannengcc.top

PHP:  getcwd();
来源：http://qeu.jqgufenzy.top

JS:   process.cwd()
来源：http://swp.hfpthk.cn

TS:   process.cwd()
来源：http://ubq.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://rat.sxryk.cn

Go:   os.Getwd()
来源：http://vup.zhixingplan.top

Ruby: Dir.pwd
来源：http://tmw.xziqi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ssq.chenjidiqi.icu

[M05] 设置退出码
来源：http://wuo.yonumen.top

Py:   sys.exit(1)
来源：http://ckc.zhijiandao.cn

PHP:  exit(1);
来源：http://xxu.xuetiantiany.cn

JS:   process.exit(1)
来源：http://rqg.zdbjq.cn

TS:   process.exit(1)
来源：http://gco.52xcode.cn

Java: System.exit(1)
来源：http://hwj.tanke756.top

Go:   os.Exit(1)
来源：http://crf.tianlin.xyz

Ruby: exit 1
来源：http://zok.hnqzz.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dxu.tanke756.top

[M06] 向标准错误输出
来源：http://npq.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://pme.jinghuilouyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nbt.zdqjudy.top

JS:   console.error("err")
来源：http://kei.zhaomingkeji.xyz

TS:   console.error("err")
来源：http://ssz.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://mas.wangshuangyany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://txp.cdnleiting.top

Ruby: warn "err"
来源：http://qej.bjfxy.top

C#:   Console.Error.WriteLine("err")
来源：http://ngt.ydzc1.top

[M07] 判断是否为主入口
来源：http://frc.xziqi.cn

Py:   if __name__ == "__main__":
来源：http://wda.fzhhl.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://amj.smart0.xyz

JS:   require.main === module
来源：http://kjv.xziqi.cn

TS:   require.main === module
来源：http://fiy.ydjk.org.cn

Java: public static void main(String[] args)
来源：http://cgg.xziqi.cn

Go:   func main()
来源：http://qiq.nanxuanxn.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://byu.zhixingplan.top

C#:   static void Main(string[] args)
来源：http://izh.dashuyun.cn

[M08] 获取系统与运行时信息
来源：http://wyn.nanxinkj.top

Py:   platform.system();  platform.python_version()
来源：http://xxu.0kj1m.cn

PHP:  PHP_OS;  phpversion();
来源：http://gnr.tianlin.xyz

JS:   process.platform;  process.version
来源：http://nia.zhixingplan.top

TS:   process.platform;  process.version
来源：http://upc.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fhn.shanyushiyangtech.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jeb.iojbl.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yeg.ywan-chungtsiang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hry.cashguo.top

================================================================================
来源：http://aqs.uphjek.com

N. 数据结构与算法
来源：http://ehw.jyoumei.cn

================================================================================
来源：http://ceq.jyoumei.cn

[N01] 二分查找（有序数组）
来源：http://fmc.guannengcc.top

Py:   bisect.bisect_left(arr, x)
来源：http://uxy.cashguo.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://auy.jqgfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://csn.cashguo.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gks.mhx1999.top

Java: Arrays.binarySearch(arr, x)
来源：http://uzq.nwbrower.top

Go:   sort.SearchInts(arr, x)
来源：http://tck.zhoulong.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://qrl.jianghu66.top

C#:   Array.BinarySearch(arr, x)
来源：http://wiz.bjfxy.top

[N02] 排序（工程实践用内置实现）
来源：http://hce.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://eib.sysykeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fto.zhixingplan.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://eui.meibo888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ipx.jinghuilouyu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mhp.jlsjyb.cn

Go:   slices.Sort(arr)
来源：http://ftu.gzhubu.top

Ruby: arr.sort
来源：http://qpi.andypj.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://ygg.tianlin.xyz

[N03] 快速排序（分治示例）
来源：http://atc.fengsongda.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vqy.uphjek.com

PHP:  // 递归实现，或用 usort
来源：http://abp.xziqi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ker.jqgufenzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dfu.jiagoushi.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xgp.hammf.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nxg.zhixingplan.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://img.fktsv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vmd.cqqwz.cn

[N04] 斐波那契数列
来源：http://fsz.hnqzz.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zgn.jinqigufen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://myp.birdmap.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xce.9152youxi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pca.ehwqpu.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://msc.xingfuxueyuan.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mkt.meibo888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kln.cashguo.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rrs.havefunace.top

[N05] 最大公约数
来源：http://sla.c1oappe.top

Py:   math.gcd(a, b)
来源：http://muj.redwolf501.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jpo.bbcook.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kwk.zhoulong.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://itw.shzxlz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pow.ywan-chungtsiang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zgl.fanxiaobao.xyz

Ruby: a.gcd(b)
来源：http://ywt.shanyushiyangtech.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kbz.sxryk.cn

[N06] 判断回文字符串
来源：http://fes.yangfankeji.com

Py:   s == s[::-1]
来源：http://avm.cashguo.top

PHP:  $s === strrev($s);
来源：http://nnf.daxiang520.top

JS:   s === [...s].reverse().join("")
来源：http://zxu.jinqigufen.top

TS:   s === [...s].reverse().join("")
来源：http://zgj.bbcook.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://opp.nwbrower.top

Go:   // 双指针从两端比较
来源：http://clz.chenzaomai.com

Ruby: s == s.reverse
来源：http://fib.hongshengwenyu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://eeo.andypj.xyz

[N07] 两数之和（返回下标）
来源：http://dsi.uphjek.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ybl.redwolf501.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kwz.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jhs.hysaishi.cn

TS:   // 手写 Map<string, number>
来源：http://itq.chenlongwang.top

Java: // 手写 HashMap
来源：http://jyj.zdqjudy.top

Go:   // 手写 map[int]int
来源：http://ems.meibo888.top

Ruby: // 手写 Hash
来源：http://qfu.xuetiantiany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dgo.sxryk.cn

[N08] 生成全排列
来源：http://lkc.sweek.top

Py:   itertools.permutations(arr)
来源：http://nbe.jyoumei.cn

PHP:  // 手写递归交换
来源：http://exg.bbcook.cn

JS:   // 手写回溯递归
来源：http://mcg.haohaochexian.top

TS:   // 手写回溯递归
来源：http://lqn.jiagoushi.top

Java: // 手写回溯递归
来源：http://jfq.cdnleiting.top

Go:   // 手写回溯递归
来源：http://kiu.daria6918.cn

Ruby: arr.permutation.to_a
来源：http://gqh.shanyushiyangtech.top

C#:   // 手写回溯递归
来源：http://wph.ydjk.org.cn

[N09] 栈与队列
来源：http://oeg.jinyuanbaomall.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ury.shzxlz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gwe.yvedp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dvu.daxiang520.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uxp.uphjek.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qrm.xingfuxueyuan.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qtv.jqgufenzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eys.chenlongwang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dny.feifeiyinyue.top

[N10] 链表节点定义
来源：http://gql.hfpthk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aej.aizwys.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dog.cqqwz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://unc.sufxvd.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wyq.gogol.net.cn

Java: class Node { int v; Node next; }
来源：http://ayi.yangfankeji.com

Go:   type Node struct { V int; Next *Node }
来源：http://wfr.zhiwuduotai.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tmj.nanxuanxn.top

C#:   class Node { public int V; public Node? Next; }
来源：http://nxp.fktsv.cn

[N11] 二叉树中序遍历
来源：http://qtu.xuanzx.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://emx.316326.xyz

PHP:  // 手写递归函数
来源：http://nnl.nanxuanxn.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wdy.yangfankeji.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wui.cheryme.top

Java: // 手写递归
来源：http://tuk.xziqi.cn

Go:   // 手写递归
来源：http://bjc.hfpthk.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hcp.xingfuxueyuan.xyz

C#:   // 手写递归
来源：http://jdi.jinyuanbaomall.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://byr.xuetiantiany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cmt.yanxiufei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://eri.jinghuilouyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sws.yuxming.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yhr.kuanghao11.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wdk.daria6918.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://anf.chenzaomai.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mts.jqgufenzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://syq.zhoulong.xyz

================================================================================
来源：http://bgf.guannengcc.top

O. 并发与异步
来源：http://tbp.guannengcc.top

================================================================================
来源：http://sfg.jyoumei.cn

[O01] 启动一个线程
来源：http://ymk.fehbvm.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://brr.yongpay.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xdx.yfazqb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ueu.wangdashe.top

TS:   // 同 JS
来源：http://irb.yfazqb.com

Java: new Thread(() -> f()).start()
来源：http://pby.fzhhl.top

Go:   go f()
来源：http://gqi.chenjidiqi.icu

Ruby: Thread.new { f }
来源：http://rtv.ppjwa.cn

C#:   Task.Run(() => F());
来源：http://qyy.ppjwa.cn

[O02] 使用线程池
来源：http://ohi.hongshengwenyu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ait.cdnleiting.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kuh.fanxiaobao.xyz

JS:   // worker_threads 线程池
来源：http://kbt.shanyushiyangkeji.top

TS:   // worker_threads 线程池
来源：http://iqi.uphjek.com

Java: Executors.newFixedThreadPool(4)
来源：http://ila.jinghuilouyu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nns.fengsongda.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wad.zhoulong.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tlt.iojbl.cn

[O03] 加锁保护共享数据
来源：http://hmn.chenjidiqi.icu

Py:   with lock: shared += 1
来源：http://bry.jqgufenzy.top

PHP:  // 用 flock() 做文件锁
来源：http://ejm.hywenlv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xjm.hnqzz.top

TS:   // 同 JS
来源：http://jma.yj20258.top

Java: synchronized (this) { shared++; }
来源：http://ahh.xinyue.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iih.jlsjyb.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xho.yj202588.top

C#:   lock (gate) { shared++; }
来源：http://lrd.dashuyun.cn

[O04] 定义异步函数并等待
来源：http://coj.guannengcc.top

Py:   async def f():⏎    await g()
来源：http://eas.gogol.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eil.smart0.xyz

JS:   async function f() { await g(); }
来源：http://djx.ivvv.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jro.dashuyun.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xpw.bjfxy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zni.sufxvd.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ifr.sufxvd.cn

C#:   async Task F() { await G(); }
来源：http://huy.yongpay.top

[O05] 并发执行并等待全部完成
来源：http://zth.cashguo.top

Py:   asyncio.gather(*tasks)
来源：http://wvv.zhixingplan.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kbs.9152youxi.cn

JS:   await Promise.all(tasks)
来源：http://wmj.yonumen.top

TS:   await Promise.all(tasks)
来源：http://hux.pycfn.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kgj.hongshengwenyu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eoi.wangdashe.top

Ruby: threads.map(&:join)
来源：http://jux.redwolf501.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ric.fehbvm.com


<!-- 参考信息 -->