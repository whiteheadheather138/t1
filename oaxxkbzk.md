代发 wailian999

L. 网络请求
来源：http://qww.sjlbkw.cn

================================================================================
来源：http://qlf.jianghu66.top

[L01] 发送 GET 请求
来源：http://zyg.cucudq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fqe.cdnleiting.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cgu.meibo888.top

JS:   await fetch(url)
来源：http://vez.jyoumei.cn

TS:   await fetch(url)
来源：http://qbq.yfazqb.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://evr.uphjek.com

Go:   resp, err := http.Get(url)
来源：http://vkj.daria6918.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jrg.zhiwuduotai.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nir.ydjk.org.cn

[L02] 发送 POST JSON
来源：http://tbm.shuidangran.top

Py:   requests.post(url, json={"a": 1})
来源：http://eat.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uvl.jqgufenzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jqz.jlsjyb.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://stt.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rvv.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zki.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iih.vqdsnc.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ctr.guannengcc.top

[L03] 设置自定义请求头
来源：http://jmg.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kqv.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vij.yongpay.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zns.yj20258888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ghd.pycfn.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bmh.chenjidiqi.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dtk.uphjek.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yhn.redwolf501.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bqq.ydjk.org.cn

[L04] 设置超时
来源：http://vza.hnqzz.top

Py:   requests.get(url, timeout=5)
来源：http://zcf.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dve.andypj.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ulr.shanyushiyangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sph.nwbrower.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jcc.gzhubu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sey.ehwqpu.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wty.snrcjt.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://frk.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://wsd.jinghuilouyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cxs.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jgk.zhengqikj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ptj.hammf.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dba.zhengqikj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hct.jyoumei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kyv.jianghu66.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bzk.ctjpmb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mmf.fanxiaobao.xyz

[L06] 解析响应为 JSON
来源：http://khj.shzxlz.cn

Py:   resp.json()
来源：http://cwk.jinyuanbaomall.cn

PHP:  json_decode($body, true);
来源：http://khs.sjlbkw.cn

JS:   await resp.json()
来源：http://pet.gotoacloud.top

TS:   await resp.json()
来源：http://gfb.jiagoushi.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kik.hnqzz.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uqj.zhiwuduotai.top

Ruby: JSON.parse(resp.body)
来源：http://rzw.zhongyouzk.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://obs.nanxinkj.top

[L07] 处理 HTTP 状态码
来源：http://bki.zhengqikj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pvz.zhengqikj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kec.pycfn.com

JS:   resp.ok;  resp.status
来源：http://bkf.ydzc1.top

TS:   resp.ok;  resp.status
来源：http://lxa.gzhubu.top

Java: resp.statusCode()
来源：http://dlt.jinqigufen.top

Go:   resp.StatusCode
来源：http://yrv.vqdsnc.cn

Ruby: resp.code.to_i
来源：http://bob.yongpay.top

C#:   (int)resp.StatusCode
来源：http://dhn.hnxiangtu.top

[L08] 并发请求多个地址
来源：http://tpb.gaohongyu789.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oeu.nwbrower.top

PHP:  curl_multi_init() 系列
来源：http://hmi.hammf.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qpc.cashguo.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://itx.sweek.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zyt.zhijiandao.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tge.ybcxt.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ejj.svipenyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oks.ydjk.org.cn

================================================================================
来源：http://efm.hongshengwenyu.top

M. 命令行 / 进程 / 环境
来源：http://qxr.fzhhl.top

================================================================================
来源：http://wam.tian-w.cn

[M01] 读取命令行参数
来源：http://qgk.zhaomingkeji.xyz

Py:   sys.argv[1:]
来源：http://bpd.mhx1999.top

PHP:  $argv;  $argc;
来源：http://mzh.andypj.xyz

JS:   process.argv.slice(2)
来源：http://mfk.daxiang520.top

TS:   process.argv.slice(2)
来源：http://uxr.fengsongda.top

Java: args 数组（main 方法参数）
来源：http://peb.hcnkem.com

Go:   os.Args[1:]
来源：http://vid.gotoacloud.top

Ruby: ARGV
来源：http://oda.sweek.top

C#:   args 数组（Main 方法参数）
来源：http://mre.ywan-chungtsiang.top

[M02] 读取环境变量
来源：http://baq.xziqi.cn

Py:   os.environ.get("HOME")
来源：http://etk.zdbjq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yfo.jqgfzy.top

JS:   process.env.HOME
来源：http://iam.chenlongwang.top

TS:   process.env.HOME
来源：http://yam.gogol.net.cn

Java: System.getenv("HOME")
来源：http://auj.yonumen.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rkm.sxryk.cn

Ruby: ENV["HOME"]
来源：http://tpy.feifeiyinyue.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pbd.chenlongwang.top

[M03] 执行外部命令
来源：http://ave.yj20258.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zxl.jiagoushi.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vbp.yj20258.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wer.yueranfly.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jtg.zdbjq.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kat.mhx1999.top

Go:   exec.Command("ls", "-l").Output()
来源：http://plu.meibo888.top

Ruby: system("ls -l");  `ls -l`
来源：http://ecp.daxiang520.top

C#:   Process.Start("ls", "-l");
来源：http://ltm.sxryk.cn

[M04] 获取当前工作目录
来源：http://fwh.mhx1999.top

Py:   os.getcwd()
来源：http://nun.birdmap.top

PHP:  getcwd();
来源：http://ugj.bbcook.cn

JS:   process.cwd()
来源：http://dhr.hcnkem.com

TS:   process.cwd()
来源：http://ush.jianghu66.top

Java: Path.of("").toAbsolutePath()
来源：http://dur.hfpthk.cn

Go:   os.Getwd()
来源：http://hdn.yonumen.top

Ruby: Dir.pwd
来源：http://iul.ydjk.org.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sli.gogol.net.cn

[M05] 设置退出码
来源：http://nhf.nanxuanxn.top

Py:   sys.exit(1)
来源：http://lbk.cucudq.cn

PHP:  exit(1);
来源：http://yce.0kj1m.cn

JS:   process.exit(1)
来源：http://puj.bbcook.cn

TS:   process.exit(1)
来源：http://ett.hcnkem.com

Java: System.exit(1)
来源：http://zwk.aibaodan.cn

Go:   os.Exit(1)
来源：http://wri.zhoulong.xyz

Ruby: exit 1
来源：http://kac.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pky.yfazqb.com

[M06] 向标准错误输出
来源：http://vbe.sufxvd.cn

Py:   print("err", file=sys.stderr)
来源：http://osu.hfpthk.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wjn.yuxming.cn

JS:   console.error("err")
来源：http://npk.shanyushiyangtech.top

TS:   console.error("err")
来源：http://erz.ppjwa.cn

Java: System.err.println("err")
来源：http://yjs.meibo888.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mmk.zhixingplan.top

Ruby: warn "err"
来源：http://edw.guowangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://red.chenjidiqi.icu

[M07] 判断是否为主入口
来源：http://kaw.hysaishi.cn

Py:   if __name__ == "__main__":
来源：http://nbb.hesvh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jde.redwolf501.top

JS:   require.main === module
来源：http://yua.zhixingplan.top

TS:   require.main === module
来源：http://sxv.yj20258888.top

Java: public static void main(String[] args)
来源：http://qwv.sxryk.cn

Go:   func main()
来源：http://kzb.ehwqpu.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xum.jiagoushi.top

C#:   static void Main(string[] args)
来源：http://rdl.zhoulong.xyz

[M08] 获取系统与运行时信息
来源：http://tin.yj20258888.top

Py:   platform.system();  platform.python_version()
来源：http://iip.havefunace.top

PHP:  PHP_OS;  phpversion();
来源：http://uas.zdbjq.cn

JS:   process.platform;  process.version
来源：http://fiz.zdbjq.cn

TS:   process.platform;  process.version
来源：http://pab.xylfe.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qkf.jinqigfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://klo.shuidangran.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eiw.0kj1m.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ufh.zhijiandao.cn

================================================================================
来源：http://ffo.cheryme.top

N. 数据结构与算法
来源：http://hiy.jinqigufen.top

================================================================================
来源：http://dbg.yuxming.cn

[N01] 二分查找（有序数组）
来源：http://vdo.zhoulong.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://epd.hesvh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uui.feifeiyinyue.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jxm.ivvv.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ekn.zycfv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jph.cdnleiting.top

Go:   sort.SearchInts(arr, x)
来源：http://cbe.cheryme.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://udi.bbcook.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rza.ybcxt.top

[N02] 排序（工程实践用内置实现）
来源：http://wvr.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://wtz.jianghu66.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nof.svipenyu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xia.cheryme.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yzl.sufxvd.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sir.cheryme.top

Go:   slices.Sort(arr)
来源：http://hyq.pycfn.com

Ruby: arr.sort
来源：http://twv.sufxvd.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xnk.zhiwuduotai.top

[N03] 快速排序（分治示例）
来源：http://sxi.yj202588.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lkf.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://ndb.fktsv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pak.pengpengdd.cyou

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yxf.9152youxi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cgb.jinyuanbaomall.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://reu.xziqi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hgu.hcnkem.com

C#:   // 手写递归，或 Array.Sort
来源：http://pzr.tarul.cn

[N04] 斐波那契数列
来源：http://gkv.shzxlz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rwo.tian-w.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zyu.daxiang520.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gbm.ydzc1.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sxb.xuetiantiany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kbx.hongshengwenyu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jrt.jqgfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hmk.hammf.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://iaf.jlsjyb.cn

[N05] 最大公约数
来源：http://xzf.ydzc1.top

Py:   math.gcd(a, b)
来源：http://mgq.cashguo.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hev.gotoacloud.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zfa.yuanzhike.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hxw.chenzaomai.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eeb.xziqi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kpn.meibo888.top

Ruby: a.gcd(b)
来源：http://hqp.chenlongwang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lvv.hongshengwenyu.top

[N06] 判断回文字符串
来源：http://lgn.ybcxt.top

Py:   s == s[::-1]
来源：http://vlm.aizwys.cn

PHP:  $s === strrev($s);
来源：http://jaa.jyoumei.cn

JS:   s === [...s].reverse().join("")
来源：http://lrn.cqqwz.cn

TS:   s === [...s].reverse().join("")
来源：http://xtk.redwolf501.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ekz.dianchejie.cn

Go:   // 双指针从两端比较
来源：http://kxu.jinghuilouyu.cn

Ruby: s == s.reverse
来源：http://kpv.tarul.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uos.yj20258888.top

[N07] 两数之和（返回下标）
来源：http://qui.sufxvd.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ute.pengpengdd.cyou

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kmj.sufxvd.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zlg.yueranfly.top

TS:   // 手写 Map<string, number>
来源：http://ijr.ywan-chungtsiang.top

Java: // 手写 HashMap
来源：http://qnw.hongshengwenyu.top

Go:   // 手写 map[int]int
来源：http://nxf.tian-w.cn

Ruby: // 手写 Hash
来源：http://dii.gotoacloud.top

C#:   // 手写 Dictionary<int, int>
来源：http://xbx.gotoacloud.top

[N08] 生成全排列
来源：http://ilw.316326.xyz

Py:   itertools.permutations(arr)
来源：http://amj.fzhhl.top

PHP:  // 手写递归交换
来源：http://bqo.nanxinkj.top

JS:   // 手写回溯递归
来源：http://weo.shzxlz.cn

TS:   // 手写回溯递归
来源：http://twa.mhx1999.top

Java: // 手写回溯递归
来源：http://lmv.sxryk.cn

Go:   // 手写回溯递归
来源：http://tjj.hcnkem.com

Ruby: arr.permutation.to_a
来源：http://lun.pengpengdd.cyou

C#:   // 手写回溯递归
来源：http://pws.andypj.xyz

[N09] 栈与队列
来源：http://coz.chenjidiqi.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bis.feifeiyinyue.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://alz.shuidangran.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://upq.fehbvm.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iov.zdqjudy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nlt.daxiang520.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mdb.dianchejie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sde.cqqwz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://toz.yueranfly.top

[N10] 链表节点定义
来源：http://qye.sufxvd.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ixk.zhoulong.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://vek.xingfuxueyuan.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vgb.iojbl.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vlt.pengpengdd.cyou

Java: class Node { int v; Node next; }
来源：http://knb.kuanghao11.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vez.chenzaomai.com

Ruby: Node = Struct.new(:v, :next)
来源：http://hmo.chenzaomai.com

C#:   class Node { public int V; public Node? Next; }
来源：http://xjk.zdbjq.cn

[N11] 二叉树中序遍历
来源：http://prw.hfpthk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ksy.yj20258888.top

PHP:  // 手写递归函数
来源：http://hxa.feifeiyinyue.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nln.haohaochexian.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ifv.yj20258888.top

Java: // 手写递归
来源：http://ogk.chenzaomai.com

Go:   // 手写递归
来源：http://iwb.yangfankeji.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://olz.xuanzx.com

C#:   // 手写递归
来源：http://shv.xuanzx.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rnv.haohaochexian.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wha.52xcode.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://szr.xinyue.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dvg.iojbl.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://igl.guannengcc.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rye.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lum.mhx1999.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jbg.hysaishi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vhb.fanxiaobao.xyz

================================================================================
来源：http://dhs.hfpthk.cn

O. 并发与异步
来源：http://djp.daxiang520.top

================================================================================
来源：http://mxh.zhoulong.xyz

[O01] 启动一个线程
来源：http://yys.yj20258888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rzx.yj202588.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rqs.zdqjudy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lwq.tanke756.top

TS:   // 同 JS
来源：http://pyk.epnwcf.com

Java: new Thread(() -> f()).start()
来源：http://bsi.vehdjk.com

Go:   go f()
来源：http://lbf.cheryme.top

Ruby: Thread.new { f }
来源：http://ufu.nanxinkj.top

C#:   Task.Run(() => F());
来源：http://mps.xuanzx.com

[O02] 使用线程池
来源：http://yvf.yuanzhike.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wwr.yonumen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hvu.gaohongyu789.top

JS:   // worker_threads 线程池
来源：http://gnu.jqgfzy.top

TS:   // worker_threads 线程池
来源：http://ejz.vqdsnc.cn

Java: Executors.newFixedThreadPool(4)
来源：http://caa.jqgufenzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kwu.daxiang520.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vqt.sufxvd.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sas.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://rdb.jiagoushi.top

Py:   with lock: shared += 1
来源：http://bwj.jiagoushi.top

PHP:  // 用 flock() 做文件锁
来源：http://qlr.quarkkingdee.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://brz.cheryme.top

TS:   // 同 JS
来源：http://aau.c1oappe.top

Java: synchronized (this) { shared++; }
来源：http://fkk.jianghu66.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vfh.0kj1m.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://iul.jinqigufen.top

C#:   lock (gate) { shared++; }
来源：http://ddp.bjfxy.top

[O04] 定义异步函数并等待
来源：http://vbg.9152youxi.cn

Py:   async def f():⏎    await g()
来源：http://jvx.bjfxy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mgc.ydzc1.top

JS:   async function f() { await g(); }
来源：http://etu.gzhubu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lil.jqgufenzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tgf.ehwqpu.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eqx.zdqjudy.top

Ruby: # 用 Fiber 或 async gem
来源：http://wfv.xziqi.cn

C#:   async Task F() { await G(); }
来源：http://nnc.uphjek.com

[O05] 并发执行并等待全部完成
来源：http://ije.jinqigfzy.top


<!-- 参考信息 -->