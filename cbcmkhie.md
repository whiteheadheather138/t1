代发 wailian999

Go:   encoding/gob
来源：http://nrv.c1oappe.top

Ruby: Marshal.dump(obj)
来源：http://nos.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aks.yj202588.top

================================================================================
来源：http://blt.shzxlz.cn

L. 网络请求
来源：http://ehr.jianghu66.top

================================================================================
来源：http://zem.andypj.xyz

[L01] 发送 GET 请求
来源：http://jeb.ydjk.org.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oox.nwbrower.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://inf.shangyingyoupin.top

JS:   await fetch(url)
来源：http://mlo.guowangkeji.top

TS:   await fetch(url)
来源：http://qvd.cashguo.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://iqg.ydzc1.top

Go:   resp, err := http.Get(url)
来源：http://thj.ybcxt.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vcr.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yvt.jqgufenzy.top

[L02] 发送 POST JSON
来源：http://gos.ydjk.org.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pmr.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cdb.guannengcc.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://osu.tianlin.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bcp.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ads.xziqi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hzl.hnxiangtu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jhs.yueranfly.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gcd.52xcode.cn

[L03] 设置自定义请求头
来源：http://gid.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iiq.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oob.hnqzz.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gka.xinyue.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qde.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://liq.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cyo.nwbrower.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qjb.0kj1m.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hzf.zhongyouzk.top

[L04] 设置超时
来源：http://zff.epnwcf.com

Py:   requests.get(url, timeout=5)
来源：http://nmj.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wug.nwbrower.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gdd.hammf.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sxg.gotoacloud.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pwh.ehwqpu.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fqk.fktsv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rzh.bjfxy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cbj.zycfv.cn

[L05] 上传文件（multipart）
来源：http://ujn.zhaomingkeji.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dio.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zmg.mhx1999.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sju.feifeiyinyue.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gfd.nwbrower.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fnw.yongpay.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://njf.fanxiaobao.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hld.quarkkingdee.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://btw.hongshengwenyu.top

[L06] 解析响应为 JSON
来源：http://jjm.tian-w.cn

Py:   resp.json()
来源：http://qku.fktsv.cn

PHP:  json_decode($body, true);
来源：http://itn.316326.xyz

JS:   await resp.json()
来源：http://opa.gotoacloud.top

TS:   await resp.json()
来源：http://rwr.tianlin.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cyw.iojbl.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ysh.guowangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://ayj.xinyue.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qhk.nanxinkj.top

[L07] 处理 HTTP 状态码
来源：http://ujv.hesvh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wmb.shanyushiyangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zvu.tanke756.top

JS:   resp.ok;  resp.status
来源：http://upt.nwbrower.top

TS:   resp.ok;  resp.status
来源：http://lgp.jianghu66.top

Java: resp.statusCode()
来源：http://ihl.yvedp.cn

Go:   resp.StatusCode
来源：http://jee.yuxming.cn

Ruby: resp.code.to_i
来源：http://mwm.jinqigfzy.top

C#:   (int)resp.StatusCode
来源：http://wpj.zdqjudy.top

[L08] 并发请求多个地址
来源：http://cpw.bjfxy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://apa.svipenyu.cn

PHP:  curl_multi_init() 系列
来源：http://cha.zycfv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://itj.9152youxi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pbq.shuidangran.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zrl.jinqigufen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fnw.jyoumei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ydh.tian-w.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hhu.sxryk.cn

================================================================================
来源：http://cak.xziqi.cn

M. 命令行 / 进程 / 环境
来源：http://zml.yongpay.top

================================================================================
来源：http://axt.shangyingyoupin.top

[M01] 读取命令行参数
来源：http://kqz.hongshengwenyu.top

Py:   sys.argv[1:]
来源：http://oal.vqdsnc.cn

PHP:  $argv;  $argc;
来源：http://wot.feifeiyinyue.top

JS:   process.argv.slice(2)
来源：http://fsa.feifeiyinyue.top

TS:   process.argv.slice(2)
来源：http://jgm.chenzaomai.com

Java: args 数组（main 方法参数）
来源：http://fzl.sxryk.cn

Go:   os.Args[1:]
来源：http://jki.yanxiufei.cn

Ruby: ARGV
来源：http://hgt.haohaochexian.top

C#:   args 数组（Main 方法参数）
来源：http://pgf.fehbvm.com

[M02] 读取环境变量
来源：http://qjv.nwbrower.top

Py:   os.environ.get("HOME")
来源：http://qvx.yanxiufei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jct.hcnkem.com

JS:   process.env.HOME
来源：http://ifk.tarul.cn

TS:   process.env.HOME
来源：http://pkn.yonumen.top

Java: System.getenv("HOME")
来源：http://ppt.hammf.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hsw.hfpthk.cn

Ruby: ENV["HOME"]
来源：http://yht.shanyushiyangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://eoz.fehbvm.com

[M03] 执行外部命令
来源：http://lsz.shanyushiyangtech.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qkj.ybcxt.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gnu.ctjpmb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://cmb.pycfn.com

TS:   child_process.execSync("ls -l").toString()
来源：http://dew.chenjidiqi.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://znl.tarul.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://eqg.xinyue.icu

Ruby: system("ls -l");  `ls -l`
来源：http://wux.aizwys.cn

C#:   Process.Start("ls", "-l");
来源：http://xaj.zhixingplan.top

[M04] 获取当前工作目录
来源：http://cli.jianghu66.top

Py:   os.getcwd()
来源：http://yyr.guowangkeji.top

PHP:  getcwd();
来源：http://scv.zhongyouzk.top

JS:   process.cwd()
来源：http://cmi.ppjwa.cn

TS:   process.cwd()
来源：http://dtz.jinghuilouyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://afu.kuanghao11.cn

Go:   os.Getwd()
来源：http://jwu.daria6918.cn

Ruby: Dir.pwd
来源：http://jjt.jinyuanbaomall.cn

C#:   Directory.GetCurrentDirectory()
来源：http://quo.xingfuxueyuan.xyz

[M05] 设置退出码
来源：http://jko.tarul.cn

Py:   sys.exit(1)
来源：http://cor.chenjidiqi.icu

PHP:  exit(1);
来源：http://hsx.zhongyouzk.top

JS:   process.exit(1)
来源：http://ttf.zhiwuduotai.top

TS:   process.exit(1)
来源：http://arm.hywenlv.cn

Java: System.exit(1)
来源：http://zwk.ppjwa.cn

Go:   os.Exit(1)
来源：http://tel.gogol.net.cn

Ruby: exit 1
来源：http://cwf.pengpengdd.cyou

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mrk.jqgufenzy.top

[M06] 向标准错误输出
来源：http://bbw.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://iit.yongpay.top

PHP:  fwrite(STDERR, "err\n");
来源：http://loh.nanxinkj.top

JS:   console.error("err")
来源：http://civ.zhaomingkeji.xyz

TS:   console.error("err")
来源：http://gwh.jinyuanbaomall.cn

Java: System.err.println("err")
来源：http://aqy.jinghuilouyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iou.zdbjq.cn

Ruby: warn "err"
来源：http://eur.yj202588.top

C#:   Console.Error.WriteLine("err")
来源：http://idv.jqgfzy.top

[M07] 判断是否为主入口
来源：http://sed.vqdsnc.cn

Py:   if __name__ == "__main__":
来源：http://eit.chenzaomai.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ctg.uphjek.com

JS:   require.main === module
来源：http://vpr.zdbjq.cn

TS:   require.main === module
来源：http://uww.chenzaomai.com

Java: public static void main(String[] args)
来源：http://zrw.hcnkem.com

Go:   func main()
来源：http://ood.cheryme.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xay.fzhhl.top

C#:   static void Main(string[] args)
来源：http://afd.redwolf501.top

[M08] 获取系统与运行时信息
来源：http://qdn.hywenlv.cn

Py:   platform.system();  platform.python_version()
来源：http://hcq.ybcxt.top

PHP:  PHP_OS;  phpversion();
来源：http://yib.jlsjyb.cn

JS:   process.platform;  process.version
来源：http://mis.sjlbkw.cn

TS:   process.platform;  process.version
来源：http://nbr.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gtg.0kj1m.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nvz.jinqigfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vls.yfazqb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://lkk.sufxvd.cn

================================================================================
来源：http://hkx.0kj1m.cn

N. 数据结构与算法
来源：http://nta.pycfn.com

================================================================================
来源：http://scc.yj202588.top

[N01] 二分查找（有序数组）
来源：http://sjn.zhaomingkeji.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://jiy.zhaomingkeji.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://olz.ivvv.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mze.aibaodan.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bwv.bbcook.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lon.ctjpmb.com

Go:   sort.SearchInts(arr, x)
来源：http://yhc.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://tkx.daxiang520.top

C#:   Array.BinarySearch(arr, x)
来源：http://gkg.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://ucd.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://xol.tian-w.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ajx.tanke756.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jas.xuanzx.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://hpr.zhiwuduotai.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pjp.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://apo.kuanghao11.cn

Ruby: arr.sort
来源：http://fln.zdqjudy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nmd.hfpthk.cn

[N03] 快速排序（分治示例）
来源：http://yak.sufxvd.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jdn.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://lsg.zycfv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://paz.jinqigfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aro.zdbjq.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tjp.ppjwa.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bmh.cucudq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://aou.zhoulong.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://wiv.gaohongyu789.top

[N04] 斐波那契数列
来源：http://lmy.shangyingyoupin.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qea.jiagoushi.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ykc.shanyushiyangtech.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jwv.jyoumei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uic.jyoumei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jur.pengpengdd.cyou

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xkv.hysaishi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://com.chenlongwang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hgn.cucudq.cn

[N05] 最大公约数
来源：http://ces.shanyushiyangkeji.top

Py:   math.gcd(a, b)
来源：http://poj.hammf.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wyz.fehbvm.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ohp.hywenlv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nyd.xylfe.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ein.nanxinkj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ldj.daria6918.cn

Ruby: a.gcd(b)
来源：http://ays.zycfv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jet.yanxiufei.cn

[N06] 判断回文字符串
来源：http://swz.zdqjudy.top

Py:   s == s[::-1]
来源：http://ddx.chenzaomai.com

PHP:  $s === strrev($s);
来源：http://jtr.nanxuanxn.top

JS:   s === [...s].reverse().join("")
来源：http://myz.zhiwuduotai.top

TS:   s === [...s].reverse().join("")
来源：http://xxw.mhx1999.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://odl.yj20258888.top

Go:   // 双指针从两端比较
来源：http://ekn.wangshuangyany.cn

Ruby: s == s.reverse
来源：http://dph.zycfv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fld.cheryme.top

[N07] 两数之和（返回下标）
来源：http://nsv.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tzi.haohaochexian.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yqa.316326.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://rkk.haohaochexian.top

TS:   // 手写 Map<string, number>
来源：http://odi.pycfn.com

Java: // 手写 HashMap
来源：http://bem.vqdsnc.cn

Go:   // 手写 map[int]int
来源：http://tki.yongpay.top

Ruby: // 手写 Hash
来源：http://mkm.cashguo.top

C#:   // 手写 Dictionary<int, int>
来源：http://pwa.sxryk.cn

[N08] 生成全排列
来源：http://nty.jlsjyb.cn

Py:   itertools.permutations(arr)
来源：http://cnj.sxryk.cn

PHP:  // 手写递归交换
来源：http://jmy.xuetiantiany.cn

JS:   // 手写回溯递归
来源：http://gcy.hnxiangtu.top

TS:   // 手写回溯递归
来源：http://wlt.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://ncz.yfazqb.com

Go:   // 手写回溯递归
来源：http://xiy.hnxiangtu.top

Ruby: arr.permutation.to_a
来源：http://fvh.fanxiaobao.xyz

C#:   // 手写回溯递归
来源：http://kcx.0kj1m.cn

[N09] 栈与队列
来源：http://tvx.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://srv.tarul.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dlc.sxryk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pin.yj20258.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mbk.jinqigufen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fkt.tanke756.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kzv.zhoulong.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cwz.yanxiufei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ngb.shanyushiyangtech.top

[N10] 链表节点定义
来源：http://nsz.dianchejie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wec.shanyushiyangtech.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ajl.sysykeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xoy.andypj.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jbf.gotoacloud.top

Java: class Node { int v; Node next; }
来源：http://yzs.birdmap.top

Go:   type Node struct { V int; Next *Node }
来源：http://der.shanyushiyangtech.top

Ruby: Node = Struct.new(:v, :next)
来源：http://oiz.jlsjyb.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jxx.shanyushiyangtech.top

[N11] 二叉树中序遍历
来源：http://xdp.yangfankeji.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://czr.sxryk.cn

PHP:  // 手写递归函数
来源：http://zxb.hongshengwenyu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pxb.hfpthk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qfy.nwbrower.top

Java: // 手写递归
来源：http://jtt.52xcode.cn

Go:   // 手写递归
来源：http://ddc.yvedp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xuc.meibo888.top

C#:   // 手写递归
来源：http://rhd.jinqigfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yia.xingfuxueyuan.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qjv.wangshuangyany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://arl.xuetiantiany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rxv.svipenyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zij.fengsongda.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gpe.cdnleiting.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://koh.hammf.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eva.0kj1m.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hwq.hywenlv.cn

================================================================================
来源：http://goj.nanxinkj.top

O. 并发与异步
来源：http://wlo.yueranfly.top

================================================================================
来源：http://ncu.pengpengdd.cyou

[O01] 启动一个线程
来源：http://ifc.aizwys.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mrg.zhiwuduotai.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qpp.chenzaomai.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lru.ydjk.org.cn

TS:   // 同 JS
来源：http://rrn.kuanghao11.cn

Java: new Thread(() -> f()).start()
来源：http://nyt.cheryme.top

Go:   go f()
来源：http://dfl.fengsongda.top

Ruby: Thread.new { f }
来源：http://tat.aibaodan.cn

C#:   Task.Run(() => F());
来源：http://cxz.haohaochexian.top

[O02] 使用线程池
来源：http://oby.9152youxi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gjb.shanyushiyangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rsc.jqgfzy.top

JS:   // worker_threads 线程池
来源：http://ugg.pycfn.com

TS:   // worker_threads 线程池
来源：http://txm.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pbh.316326.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ohy.sysykeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://odm.uphjek.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lqg.jqgufenzy.top

[O03] 加锁保护共享数据
来源：http://gxh.cheryme.top

Py:   with lock: shared += 1
来源：http://dlk.fktsv.cn

PHP:  // 用 flock() 做文件锁
来源：http://rsg.feifeiyinyue.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vja.pycfn.com

TS:   // 同 JS
来源：http://lkl.hesvh.cn

Java: synchronized (this) { shared++; }
来源：http://xqr.jqgufenzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ibr.yuanzhike.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tjd.xuetiantiany.cn

C#:   lock (gate) { shared++; }
来源：http://bvt.zhixingplan.top

[O04] 定义异步函数并等待
来源：http://xrs.ydjk.org.cn

Py:   async def f():⏎    await g()
来源：http://yqj.shangyingyoupin.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hzl.havefunace.top

JS:   async function f() { await g(); }
来源：http://ozv.tianlin.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://bej.hesvh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://red.zhoulong.xyz


<!-- 参考信息 -->