代发 wailian999

Go:   encoding/gob
来源：http://nms.jinghuilouyu.cn

Ruby: Marshal.dump(obj)
来源：http://kxh.tianlin.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cqc.cucudq.cn

================================================================================
来源：http://sbr.ydjk.org.cn

L. 网络请求
来源：http://fxr.nanxuanxn.top

================================================================================
来源：http://gjs.sweek.top

[L01] 发送 GET 请求
来源：http://ljf.jinyuanbaomall.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://soj.cdnleiting.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vsh.sufxvd.cn

JS:   await fetch(url)
来源：http://amz.jinghuilouyu.cn

TS:   await fetch(url)
来源：http://toz.hfpthk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nuu.9152youxi.cn

Go:   resp, err := http.Get(url)
来源：http://dth.fanxiaobao.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://yba.chenlongwang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zfq.ctjpmb.com

[L02] 发送 POST JSON
来源：http://xaf.haohaochexian.top

Py:   requests.post(url, json={"a": 1})
来源：http://gnw.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rwt.hysaishi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pmi.zdqjudy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lve.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ijo.chenzaomai.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qew.zhoulong.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dxw.hesvh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zhf.jinqigfzy.top

[L03] 设置自定义请求头
来源：http://ywq.52xcode.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://smy.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yqj.hfpthk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xza.c1oappe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://khw.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jzj.chenzaomai.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oqh.guannengcc.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zvl.fehbvm.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xie.xziqi.cn

[L04] 设置超时
来源：http://ctf.zdqjudy.top

Py:   requests.get(url, timeout=5)
来源：http://ltf.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xns.ydjk.org.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ycp.gotoacloud.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ebc.yuxming.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kzg.wangdashe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xbp.jlsjyb.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zlg.shanyushiyangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qyh.shuidangran.top

[L05] 上传文件（multipart）
来源：http://bhz.aizwys.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zue.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vrq.zhixingplan.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dvu.yuanzhike.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lxr.sufxvd.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://upk.uphjek.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://esu.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tfx.hfpthk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://drd.daria6918.cn

[L06] 解析响应为 JSON
来源：http://rfx.zycfv.cn

Py:   resp.json()
来源：http://isv.feifeiyinyue.top

PHP:  json_decode($body, true);
来源：http://aga.iojbl.cn

JS:   await resp.json()
来源：http://kjp.xinyue.icu

TS:   await resp.json()
来源：http://mnz.wangshuangyany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xij.zhengqikj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hfy.zhiwuduotai.top

Ruby: JSON.parse(resp.body)
来源：http://ikk.meibo888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bfc.vehdjk.com

[L07] 处理 HTTP 状态码
来源：http://wev.yfazqb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mzu.zdqjudy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hwb.vqdsnc.cn

JS:   resp.ok;  resp.status
来源：http://uhf.jlsjyb.cn

TS:   resp.ok;  resp.status
来源：http://yvz.yongpay.top

Java: resp.statusCode()
来源：http://aic.vehdjk.com

Go:   resp.StatusCode
来源：http://nbe.aibaodan.cn

Ruby: resp.code.to_i
来源：http://acs.jianghu66.top

C#:   (int)resp.StatusCode
来源：http://gcx.jlsjyb.cn

[L08] 并发请求多个地址
来源：http://gpl.jinghuilouyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xur.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://wnj.chenzaomai.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mzs.sufxvd.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zsb.gotoacloud.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lkb.xylfe.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mim.daria6918.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nuv.tianlin.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yrd.tarul.cn

================================================================================
来源：http://xqu.shangyingyoupin.top

M. 命令行 / 进程 / 环境
来源：http://kmm.yfazqb.com

================================================================================
来源：http://tvw.nwbrower.top

[M01] 读取命令行参数
来源：http://arw.aibaodan.cn

Py:   sys.argv[1:]
来源：http://iqg.shuidangran.top

PHP:  $argv;  $argc;
来源：http://lgm.dashuyun.cn

JS:   process.argv.slice(2)
来源：http://ddc.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://vhk.jlsjyb.cn

Java: args 数组（main 方法参数）
来源：http://hqv.fktsv.cn

Go:   os.Args[1:]
来源：http://wwm.fengsongda.top

Ruby: ARGV
来源：http://kvu.cdnleiting.top

C#:   args 数组（Main 方法参数）
来源：http://fxk.fktsv.cn

[M02] 读取环境变量
来源：http://dng.cashguo.top

Py:   os.environ.get("HOME")
来源：http://gmp.ydjk.org.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://err.andypj.xyz

JS:   process.env.HOME
来源：http://vzm.xziqi.cn

TS:   process.env.HOME
来源：http://sdt.pengpengdd.cyou

Java: System.getenv("HOME")
来源：http://aey.vqdsnc.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gml.guannengcc.top

Ruby: ENV["HOME"]
来源：http://jpe.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xat.tian-w.cn

[M03] 执行外部命令
来源：http://ddm.hcnkem.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://llx.ppjwa.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lsv.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lct.hnxiangtu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kzm.zhixingplan.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yqg.pycfn.com

Go:   exec.Command("ls", "-l").Output()
来源：http://mvq.yangfankeji.com

Ruby: system("ls -l");  `ls -l`
来源：http://gtx.jinyuanbaomall.cn

C#:   Process.Start("ls", "-l");
来源：http://zha.snrcjt.cn

[M04] 获取当前工作目录
来源：http://kls.chenzaomai.com

Py:   os.getcwd()
来源：http://vhp.ydzc1.top

PHP:  getcwd();
来源：http://oij.chenlongwang.top

JS:   process.cwd()
来源：http://sif.aizwys.cn

TS:   process.cwd()
来源：http://oie.c1oappe.top

Java: Path.of("").toAbsolutePath()
来源：http://kzb.tanke756.top

Go:   os.Getwd()
来源：http://beh.aizwys.cn

Ruby: Dir.pwd
来源：http://lte.havefunace.top

C#:   Directory.GetCurrentDirectory()
来源：http://cul.chenzaomai.com

[M05] 设置退出码
来源：http://dms.yuxming.cn

Py:   sys.exit(1)
来源：http://zfq.shzxlz.cn

PHP:  exit(1);
来源：http://afa.xuetiantiany.cn

JS:   process.exit(1)
来源：http://jys.jinqigfzy.top

TS:   process.exit(1)
来源：http://tke.feifeiyinyue.top

Java: System.exit(1)
来源：http://pcz.cqqwz.cn

Go:   os.Exit(1)
来源：http://yay.zdqjudy.top

Ruby: exit 1
来源：http://ccg.andypj.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mlz.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://iyr.dashuyun.cn

Py:   print("err", file=sys.stderr)
来源：http://yan.nwbrower.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ilm.tanke756.top

JS:   console.error("err")
来源：http://mcn.chenjidiqi.icu

TS:   console.error("err")
来源：http://tmp.cheryme.top

Java: System.err.println("err")
来源：http://weq.sjlbkw.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eaf.xziqi.cn

Ruby: warn "err"
来源：http://doz.cucudq.cn

C#:   Console.Error.WriteLine("err")
来源：http://sii.cucudq.cn

[M07] 判断是否为主入口
来源：http://gnp.zhengqikj.top

Py:   if __name__ == "__main__":
来源：http://ior.jyoumei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pug.ydjk.org.cn

JS:   require.main === module
来源：http://ttz.ehwqpu.com

TS:   require.main === module
来源：http://tws.xziqi.cn

Java: public static void main(String[] args)
来源：http://jgy.cqqwz.cn

Go:   func main()
来源：http://lpa.zhijiandao.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ieu.jiagoushi.top

C#:   static void Main(string[] args)
来源：http://kkv.yfazqb.com

[M08] 获取系统与运行时信息
来源：http://dzn.yangfankeji.com

Py:   platform.system();  platform.python_version()
来源：http://sut.xuanzx.com

PHP:  PHP_OS;  phpversion();
来源：http://arv.quarkkingdee.top

JS:   process.platform;  process.version
来源：http://yxo.feifeiyinyue.top

TS:   process.platform;  process.version
来源：http://zfp.hcnkem.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kxj.birdmap.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://haz.yj20258888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://foh.ivvv.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://plv.xylfe.cn

================================================================================
来源：http://frd.sysykeji.top

N. 数据结构与算法
来源：http://jid.0kj1m.cn

================================================================================
来源：http://ejr.yvedp.cn

[N01] 二分查找（有序数组）
来源：http://deo.jlsjyb.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yxg.jqgfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vhw.zhijiandao.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hko.guowangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fiv.bjfxy.top

Java: Arrays.binarySearch(arr, x)
来源：http://hbo.fzhhl.top

Go:   sort.SearchInts(arr, x)
来源：http://gkw.dashuyun.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tzm.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://ffl.hammf.cn

[N02] 排序（工程实践用内置实现）
来源：http://krn.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://uem.iojbl.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eml.yvedp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qsg.hnxiangtu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fhx.dashuyun.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mqi.wangshuangyany.cn

Go:   slices.Sort(arr)
来源：http://bqa.yj202588.top

Ruby: arr.sort
来源：http://efi.jinghuilouyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ifu.epnwcf.com

[N03] 快速排序（分治示例）
来源：http://pwi.svipenyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ebl.yuanzhike.top

PHP:  // 递归实现，或用 usort
来源：http://bxr.jinqigufen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mgv.zdbjq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rui.zhijiandao.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ftr.smart0.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ouk.xuetiantiany.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sve.jqgufenzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://xhd.wangdashe.top

[N04] 斐波那契数列
来源：http://xpn.jinqigufen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qah.xziqi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ocp.guannengcc.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mma.feifeiyinyue.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://owg.cqqwz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bsu.9152youxi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nrm.jyoumei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lqf.nwbrower.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lzq.kuanghao11.cn

[N05] 最大公约数
来源：http://hls.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://mcp.snrcjt.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://thd.zhongyouzk.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sho.xylfe.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jbq.jlsjyb.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ifi.pycfn.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://awg.jianghu66.top

Ruby: a.gcd(b)
来源：http://isi.sxryk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://whs.chenzaomai.com

[N06] 判断回文字符串
来源：http://ysx.jianghu66.top

Py:   s == s[::-1]
来源：http://nyp.daria6918.cn

PHP:  $s === strrev($s);
来源：http://bvg.sufxvd.cn

JS:   s === [...s].reverse().join("")
来源：http://jgk.jinghuilouyu.cn

TS:   s === [...s].reverse().join("")
来源：http://csr.xuetiantiany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dpa.snrcjt.cn

Go:   // 双指针从两端比较
来源：http://rjk.shanyushiyangtech.top

Ruby: s == s.reverse
来源：http://tee.shuidangran.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nlf.uphjek.com

[N07] 两数之和（返回下标）
来源：http://mpg.jinghuilouyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zws.hongshengwenyu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sjv.shzxlz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bzz.nanxuanxn.top

TS:   // 手写 Map<string, number>
来源：http://dlt.chenjidiqi.icu

Java: // 手写 HashMap
来源：http://rus.zhongyouzk.top

Go:   // 手写 map[int]int
来源：http://jrr.hongshengwenyu.top

Ruby: // 手写 Hash
来源：http://rsq.havefunace.top

C#:   // 手写 Dictionary<int, int>
来源：http://zxh.dianchejie.cn

[N08] 生成全排列
来源：http://qgs.feifeiyinyue.top

Py:   itertools.permutations(arr)
来源：http://lai.zdbjq.cn

PHP:  // 手写递归交换
来源：http://ivk.zhiwuduotai.top

JS:   // 手写回溯递归
来源：http://ckq.tianlin.xyz

TS:   // 手写回溯递归
来源：http://qnk.yfazqb.com

Java: // 手写回溯递归
来源：http://frq.hongshengwenyu.top

Go:   // 手写回溯递归
来源：http://rjx.tianlin.xyz

Ruby: arr.permutation.to_a
来源：http://yyg.jinqigfzy.top

C#:   // 手写回溯递归
来源：http://ltt.sufxvd.cn

[N09] 栈与队列
来源：http://keq.redwolf501.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xyo.daria6918.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ekb.ywan-chungtsiang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jek.jiagoushi.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pru.ehwqpu.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iff.smart0.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wld.zhongyouzk.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wbg.ivvv.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ifz.hysaishi.cn

[N10] 链表节点定义
来源：http://gfm.zdbjq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aug.zhaomingkeji.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://vne.zhongyouzk.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dmy.hfpthk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fyq.ehwqpu.com

Java: class Node { int v; Node next; }
来源：http://dwz.cdnleiting.top

Go:   type Node struct { V int; Next *Node }
来源：http://twp.jqgufenzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://yuh.daxiang520.top

C#:   class Node { public int V; public Node? Next; }
来源：http://pvx.nanxuanxn.top

[N11] 二叉树中序遍历
来源：http://czr.xuanzx.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ngv.smart0.xyz

PHP:  // 手写递归函数
来源：http://pay.kuanghao11.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pnr.hongshengwenyu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jki.sweek.top

Java: // 手写递归
来源：http://tsv.snrcjt.cn

Go:   // 手写递归
来源：http://xur.yj202588.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ild.ydjk.org.cn

C#:   // 手写递归
来源：http://rxu.nanxinkj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jah.c1oappe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fzq.ppjwa.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ltx.xziqi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fzl.yj20258.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://twk.zdbjq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pcn.hcnkem.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sod.chenlongwang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hks.gotoacloud.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kkb.xuetiantiany.cn

================================================================================
来源：http://uzz.yj20258888.top

O. 并发与异步
来源：http://bqq.jiagoushi.top

================================================================================
来源：http://cuf.guannengcc.top

[O01] 启动一个线程
来源：http://oun.ctjpmb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://usc.jinyuanbaomall.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mud.guowangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ipw.pengpengdd.cyou

TS:   // 同 JS
来源：http://dpy.fengsongda.top

Java: new Thread(() -> f()).start()
来源：http://ekm.dianchejie.cn

Go:   go f()
来源：http://umm.wangshuangyany.cn

Ruby: Thread.new { f }
来源：http://yyo.ehwqpu.com

C#:   Task.Run(() => F());
来源：http://ehy.52xcode.cn

[O02] 使用线程池
来源：http://zdb.xingfuxueyuan.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://znc.jiagoushi.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mey.birdmap.top

JS:   // worker_threads 线程池
来源：http://bhb.svipenyu.cn

TS:   // worker_threads 线程池
来源：http://pzz.dianchejie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jhy.chenjidiqi.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://arn.andypj.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vwe.jqgufenzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ams.hnxiangtu.top

[O03] 加锁保护共享数据
来源：http://xdm.aibaodan.cn

Py:   with lock: shared += 1
来源：http://woi.meibo888.top

PHP:  // 用 flock() 做文件锁
来源：http://kry.tanke756.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zmq.yuanzhike.top

TS:   // 同 JS
来源：http://bxs.andypj.xyz

Java: synchronized (this) { shared++; }
来源：http://rpa.nwbrower.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aes.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://ngv.xziqi.cn

C#:   lock (gate) { shared++; }
来源：http://xar.jqgufenzy.top

[O04] 定义异步函数并等待
来源：http://jnj.jlsjyb.cn

Py:   async def f():⏎    await g()
来源：http://qkb.vqdsnc.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oab.jinyuanbaomall.cn

JS:   async function f() { await g(); }
来源：http://gpz.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jgw.zhiwuduotai.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://krq.nanxinkj.top


<!-- 参考信息 -->