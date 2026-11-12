代发 wailian999

L. 网络请求
来源：http://ioo.bbcook.cn

================================================================================
来源：http://pie.yj202588.top

[L01] 发送 GET 请求
来源：http://gyp.xylfe.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://evi.shangyingyoupin.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sdt.9152youxi.cn

JS:   await fetch(url)
来源：http://whd.andypj.xyz

TS:   await fetch(url)
来源：http://kyx.meibo888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wuw.yonumen.top

Go:   resp, err := http.Get(url)
来源：http://ipe.hnxiangtu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://apx.tianlin.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qxt.cqqwz.cn

[L02] 发送 POST JSON
来源：http://ils.ydzc1.top

Py:   requests.post(url, json={"a": 1})
来源：http://sha.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://svf.jinyuanbaomall.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lsc.zhongyouzk.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://grf.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tkd.yj20258.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://btc.fengsongda.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pge.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ljq.tian-w.cn

[L03] 设置自定义请求头
来源：http://ehs.zycfv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qeq.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yhx.epnwcf.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zge.hesvh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://luk.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dpe.redwolf501.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qch.meibo888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uxv.gaohongyu789.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cvd.ppjwa.cn

[L04] 设置超时
来源：http://wol.jinqigufen.top

Py:   requests.get(url, timeout=5)
来源：http://kjn.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bvy.zhixingplan.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mwe.zhoulong.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://owu.pengpengdd.cyou

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hhg.fanxiaobao.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ylj.hesvh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cqr.ybcxt.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pfy.hysaishi.cn

[L05] 上传文件（multipart）
来源：http://fac.pycfn.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://alo.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bbs.snrcjt.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mdr.feifeiyinyue.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://flw.iojbl.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qyk.zhongyouzk.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://buj.guowangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://isc.zhongyouzk.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hbg.yfazqb.com

[L06] 解析响应为 JSON
来源：http://wih.yvedp.cn

Py:   resp.json()
来源：http://wvm.nanxuanxn.top

PHP:  json_decode($body, true);
来源：http://pwi.jianghu66.top

JS:   await resp.json()
来源：http://ujr.birdmap.top

TS:   await resp.json()
来源：http://vqf.zhijiandao.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://imr.dianchejie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qdm.xinyue.icu

Ruby: JSON.parse(resp.body)
来源：http://zjf.zdbjq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nvt.hysaishi.cn

[L07] 处理 HTTP 状态码
来源：http://maq.aizwys.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://glh.zhixingplan.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uaq.zhixingplan.top

JS:   resp.ok;  resp.status
来源：http://qye.dianchejie.cn

TS:   resp.ok;  resp.status
来源：http://hob.nwbrower.top

Java: resp.statusCode()
来源：http://kny.ywan-chungtsiang.top

Go:   resp.StatusCode
来源：http://opd.xziqi.cn

Ruby: resp.code.to_i
来源：http://qpa.jinqigufen.top

C#:   (int)resp.StatusCode
来源：http://iei.yuxming.cn

[L08] 并发请求多个地址
来源：http://yog.vqdsnc.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lqh.bbcook.cn

PHP:  curl_multi_init() 系列
来源：http://pcq.cdnleiting.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qze.vqdsnc.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://liw.wangdashe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lqp.jinghuilouyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://row.xinyue.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vsr.c1oappe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gvd.zhijiandao.cn

================================================================================
来源：http://dcb.feifeiyinyue.top

M. 命令行 / 进程 / 环境
来源：http://zcp.vqdsnc.cn

================================================================================
来源：http://zxl.yanxiufei.cn

[M01] 读取命令行参数
来源：http://jcp.jyoumei.cn

Py:   sys.argv[1:]
来源：http://ckg.ehwqpu.com

PHP:  $argv;  $argc;
来源：http://vlc.zhixingplan.top

JS:   process.argv.slice(2)
来源：http://oux.daria6918.cn

TS:   process.argv.slice(2)
来源：http://tfo.fzhhl.top

Java: args 数组（main 方法参数）
来源：http://kuq.yonumen.top

Go:   os.Args[1:]
来源：http://kur.hcnkem.com

Ruby: ARGV
来源：http://fnc.yonumen.top

C#:   args 数组（Main 方法参数）
来源：http://pqz.uphjek.com

[M02] 读取环境变量
来源：http://bkw.zdbjq.cn

Py:   os.environ.get("HOME")
来源：http://dnq.pengpengdd.cyou

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ffq.zdbjq.cn

JS:   process.env.HOME
来源：http://vxc.yueranfly.top

TS:   process.env.HOME
来源：http://bvv.uphjek.com

Java: System.getenv("HOME")
来源：http://vac.shzxlz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rwj.dianchejie.cn

Ruby: ENV["HOME"]
来源：http://aax.dashuyun.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dcv.smart0.xyz

[M03] 执行外部命令
来源：http://wue.yanxiufei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xeq.shanyushiyangtech.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bpl.wangshuangyany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gka.ydjk.org.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hmr.haohaochexian.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bvq.ivvv.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ipj.epnwcf.com

Ruby: system("ls -l");  `ls -l`
来源：http://shh.hfpthk.cn

C#:   Process.Start("ls", "-l");
来源：http://iou.sxryk.cn

[M04] 获取当前工作目录
来源：http://vff.jinqigfzy.top

Py:   os.getcwd()
来源：http://ryk.meibo888.top

PHP:  getcwd();
来源：http://gek.ivvv.top

JS:   process.cwd()
来源：http://gdw.yj20258.top

TS:   process.cwd()
来源：http://hxk.hcnkem.com

Java: Path.of("").toAbsolutePath()
来源：http://dds.tanke756.top

Go:   os.Getwd()
来源：http://ila.0kj1m.cn

Ruby: Dir.pwd
来源：http://qzj.pengpengdd.cyou

C#:   Directory.GetCurrentDirectory()
来源：http://kip.iojbl.cn

[M05] 设置退出码
来源：http://urp.vqdsnc.cn

Py:   sys.exit(1)
来源：http://xch.aizwys.cn

PHP:  exit(1);
来源：http://fvk.fzhhl.top

JS:   process.exit(1)
来源：http://crb.vqdsnc.cn

TS:   process.exit(1)
来源：http://xkz.nanxinkj.top

Java: System.exit(1)
来源：http://bkl.9152youxi.cn

Go:   os.Exit(1)
来源：http://nou.feifeiyinyue.top

Ruby: exit 1
来源：http://jiz.bbcook.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vqe.cucudq.cn

[M06] 向标准错误输出
来源：http://kmg.nwbrower.top

Py:   print("err", file=sys.stderr)
来源：http://huu.aizwys.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kji.cashguo.top

JS:   console.error("err")
来源：http://jsa.wangshuangyany.cn

TS:   console.error("err")
来源：http://dvg.gzhubu.top

Java: System.err.println("err")
来源：http://med.ydzc1.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ktd.hywenlv.cn

Ruby: warn "err"
来源：http://tss.shanyushiyangtech.top

C#:   Console.Error.WriteLine("err")
来源：http://fti.nwbrower.top

[M07] 判断是否为主入口
来源：http://zqn.svipenyu.cn

Py:   if __name__ == "__main__":
来源：http://ayu.sysykeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hei.havefunace.top

JS:   require.main === module
来源：http://lrx.snrcjt.cn

TS:   require.main === module
来源：http://yck.ivvv.top

Java: public static void main(String[] args)
来源：http://xwx.zhiwuduotai.top

Go:   func main()
来源：http://bwu.jinqigfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lzy.xinyue.icu

C#:   static void Main(string[] args)
来源：http://bqo.zhixingplan.top

[M08] 获取系统与运行时信息
来源：http://pyz.guannengcc.top

Py:   platform.system();  platform.python_version()
来源：http://loa.cheryme.top

PHP:  PHP_OS;  phpversion();
来源：http://mnh.shanyushiyangtech.top

JS:   process.platform;  process.version
来源：http://clj.sjlbkw.cn

TS:   process.platform;  process.version
来源：http://lll.ivvv.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ifx.yonumen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dnf.gaohongyu789.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dgt.hongshengwenyu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ewx.meibo888.top

================================================================================
来源：http://nto.vehdjk.com

N. 数据结构与算法
来源：http://yaw.tianlin.xyz

================================================================================
来源：http://gfz.jinqigfzy.top

[N01] 二分查找（有序数组）
来源：http://sbn.redwolf501.top

Py:   bisect.bisect_left(arr, x)
来源：http://nqx.zhiwuduotai.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nad.andypj.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jtm.shuidangran.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xeq.xylfe.cn

Java: Arrays.binarySearch(arr, x)
来源：http://iko.dianchejie.cn

Go:   sort.SearchInts(arr, x)
来源：http://pvc.xinyue.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://wfc.fehbvm.com

C#:   Array.BinarySearch(arr, x)
来源：http://ubk.mhx1999.top

[N02] 排序（工程实践用内置实现）
来源：http://nwb.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://def.shanyushiyangtech.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gwx.yangfankeji.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://tur.jinyuanbaomall.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lnr.aizwys.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jww.cheryme.top

Go:   slices.Sort(arr)
来源：http://vez.sysykeji.top

Ruby: arr.sort
来源：http://cmj.bbcook.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xcn.tarul.cn

[N03] 快速排序（分治示例）
来源：http://jms.xinyue.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bli.ydjk.org.cn

PHP:  // 递归实现，或用 usort
来源：http://ssn.guannengcc.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://njf.ydzc1.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qvv.zycfv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jwx.jinqigufen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gpg.zhongyouzk.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kmf.sysykeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://eut.birdmap.top

[N04] 斐波那契数列
来源：http://lxs.ywan-chungtsiang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gkz.zdbjq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pik.epnwcf.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bil.fengsongda.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xwm.ydzc1.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jbl.sjlbkw.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nlm.c1oappe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kgz.jinyuanbaomall.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yzu.svipenyu.cn

[N05] 最大公约数
来源：http://dbb.jinqigufen.top

Py:   math.gcd(a, b)
来源：http://yqw.bjfxy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rpg.snrcjt.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://see.ppjwa.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sta.ctjpmb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://myl.bbcook.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sgw.0kj1m.cn

Ruby: a.gcd(b)
来源：http://vlw.52xcode.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cjc.jinqigufen.top

[N06] 判断回文字符串
来源：http://hqx.fktsv.cn

Py:   s == s[::-1]
来源：http://azg.svipenyu.cn

PHP:  $s === strrev($s);
来源：http://edp.0kj1m.cn

JS:   s === [...s].reverse().join("")
来源：http://lnu.fzhhl.top

TS:   s === [...s].reverse().join("")
来源：http://knt.sweek.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://igm.fanxiaobao.xyz

Go:   // 双指针从两端比较
来源：http://ezh.yueranfly.top

Ruby: s == s.reverse
来源：http://bia.pengpengdd.cyou

C#:   s == new string(s.Reverse().ToArray())
来源：http://vml.sjlbkw.cn

[N07] 两数之和（返回下标）
来源：http://kjv.jqgfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ohs.xuanzx.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dbu.guowangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://axz.yangfankeji.com

TS:   // 手写 Map<string, number>
来源：http://qoe.yj202588.top

Java: // 手写 HashMap
来源：http://lye.fktsv.cn

Go:   // 手写 map[int]int
来源：http://ywm.uphjek.com

Ruby: // 手写 Hash
来源：http://grn.gaohongyu789.top

C#:   // 手写 Dictionary<int, int>
来源：http://zkx.yanxiufei.cn

[N08] 生成全排列
来源：http://wml.shanyushiyangtech.top

Py:   itertools.permutations(arr)
来源：http://uuc.yuanzhike.top

PHP:  // 手写递归交换
来源：http://qay.bjfxy.top

JS:   // 手写回溯递归
来源：http://aef.svipenyu.cn

TS:   // 手写回溯递归
来源：http://fct.jinyuanbaomall.cn

Java: // 手写回溯递归
来源：http://zrv.hesvh.cn

Go:   // 手写回溯递归
来源：http://vkl.sjlbkw.cn

Ruby: arr.permutation.to_a
来源：http://ozi.zhongyouzk.top

C#:   // 手写回溯递归
来源：http://hdp.sysykeji.top

[N09] 栈与队列
来源：http://qat.jiagoushi.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pzm.feifeiyinyue.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vwi.jyoumei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rya.yueranfly.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rph.tarul.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://prf.gaohongyu789.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yys.yanxiufei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://czt.xylfe.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jll.quarkkingdee.top

[N10] 链表节点定义
来源：http://yax.hongshengwenyu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://elh.feifeiyinyue.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ssf.yuanzhike.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dan.zdbjq.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xwh.vehdjk.com

Java: class Node { int v; Node next; }
来源：http://zxf.dashuyun.cn

Go:   type Node struct { V int; Next *Node }
来源：http://edc.fengsongda.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ssu.yvedp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qrq.yuanzhike.top

[N11] 二叉树中序遍历
来源：http://inx.nwbrower.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tlw.zycfv.cn

PHP:  // 手写递归函数
来源：http://oli.wangdashe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iew.aibaodan.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tpg.vehdjk.com

Java: // 手写递归
来源：http://uof.chenjidiqi.icu

Go:   // 手写递归
来源：http://alw.sxryk.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wtl.0kj1m.cn

C#:   // 手写递归
来源：http://qdg.ppjwa.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pqo.c1oappe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gea.nanxuanxn.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ecy.birdmap.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dym.zhiwuduotai.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xog.birdmap.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vie.mhx1999.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ocp.birdmap.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kxr.kuanghao11.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ise.havefunace.top

================================================================================
来源：http://tsm.tanke756.top

O. 并发与异步
来源：http://phs.aizwys.cn

================================================================================
来源：http://ltq.ydjk.org.cn

[O01] 启动一个线程
来源：http://zdw.ywan-chungtsiang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zak.9152youxi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pvg.dashuyun.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ffw.vehdjk.com

TS:   // 同 JS
来源：http://nhn.c1oappe.top

Java: new Thread(() -> f()).start()
来源：http://hyo.sxryk.cn

Go:   go f()
来源：http://rim.andypj.xyz

Ruby: Thread.new { f }
来源：http://gcx.nanxinkj.top

C#:   Task.Run(() => F());
来源：http://gkx.tarul.cn

[O02] 使用线程池
来源：http://nvn.iojbl.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ylo.tarul.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dmb.gotoacloud.top

JS:   // worker_threads 线程池
来源：http://akc.xylfe.cn

TS:   // worker_threads 线程池
来源：http://jdm.chenzaomai.com

Java: Executors.newFixedThreadPool(4)
来源：http://rew.daxiang520.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ygj.hammf.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ivz.ydjk.org.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ysy.shuidangran.top

[O03] 加锁保护共享数据
来源：http://nvg.wangdashe.top

Py:   with lock: shared += 1
来源：http://lku.hywenlv.cn

PHP:  // 用 flock() 做文件锁
来源：http://upr.wangshuangyany.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://aqh.xylfe.cn

TS:   // 同 JS
来源：http://cjl.yuxming.cn

Java: synchronized (this) { shared++; }
来源：http://fcn.zhixingplan.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pce.ehwqpu.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://uze.guannengcc.top

C#:   lock (gate) { shared++; }
来源：http://kah.zhongyouzk.top

[O04] 定义异步函数并等待
来源：http://scq.yueranfly.top

Py:   async def f():⏎    await g()
来源：http://pnm.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kbw.andypj.xyz

JS:   async function f() { await g(); }
来源：http://mvk.sysykeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xzu.vehdjk.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cgb.c1oappe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fzi.vqdsnc.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mpf.ehwqpu.com

C#:   async Task F() { await G(); }
来源：http://jxc.9152youxi.cn

[O05] 并发执行并等待全部完成
来源：http://crl.jqgfzy.top


<!-- 参考信息 -->