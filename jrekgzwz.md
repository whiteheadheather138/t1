代发 wailian999

Go:   encoding/gob
来源：http://lyt.52xcode.cn

Ruby: Marshal.dump(obj)
来源：http://znt.yuxming.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gcm.smart0.xyz

================================================================================
来源：http://hap.cucudq.cn

L. 网络请求
来源：http://rzs.yongpay.top

================================================================================
来源：http://ugu.daria6918.cn

[L01] 发送 GET 请求
来源：http://zxq.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://obl.gogol.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xaf.snrcjt.cn

JS:   await fetch(url)
来源：http://qgb.fzhhl.top

TS:   await fetch(url)
来源：http://cza.vehdjk.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zta.vqdsnc.cn

Go:   resp, err := http.Get(url)
来源：http://qho.jinqigfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rwm.feifeiyinyue.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vvd.yuxming.cn

[L02] 发送 POST JSON
来源：http://vgg.epnwcf.com

Py:   requests.post(url, json={"a": 1})
来源：http://hmy.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tol.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hmw.hongshengwenyu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://svg.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rmm.yj20258.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oey.zhengqikj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xot.hnqzz.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qaa.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://cra.hfpthk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fzs.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lfl.guannengcc.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://crm.tianlin.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://via.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pgf.aibaodan.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xng.haohaochexian.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bxf.smart0.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dbo.jlsjyb.cn

[L04] 设置超时
来源：http://erh.yj202588.top

Py:   requests.get(url, timeout=5)
来源：http://jjr.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gju.yanxiufei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xup.jinqigfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dnk.jianghu66.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bbj.zhixingplan.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pti.aibaodan.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wpd.zhaomingkeji.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mek.tian-w.cn

[L05] 上传文件（multipart）
来源：http://zxv.smart0.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rds.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zbe.jinghuilouyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tzj.aibaodan.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ozi.haohaochexian.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iua.ppjwa.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nuh.nanxuanxn.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qbc.jinghuilouyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sfn.mhx1999.top

[L06] 解析响应为 JSON
来源：http://zwt.sufxvd.cn

Py:   resp.json()
来源：http://zyx.nanxuanxn.top

PHP:  json_decode($body, true);
来源：http://ldp.jinqigfzy.top

JS:   await resp.json()
来源：http://pwd.dashuyun.cn

TS:   await resp.json()
来源：http://rfn.wangshuangyany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tly.fzhhl.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://htn.sweek.top

Ruby: JSON.parse(resp.body)
来源：http://fxz.0kj1m.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nfv.zdbjq.cn

[L07] 处理 HTTP 状态码
来源：http://nrn.shangyingyoupin.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xat.ivvv.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lul.zhiwuduotai.top

JS:   resp.ok;  resp.status
来源：http://nwl.nanxuanxn.top

TS:   resp.ok;  resp.status
来源：http://fmq.haohaochexian.top

Java: resp.statusCode()
来源：http://crf.52xcode.cn

Go:   resp.StatusCode
来源：http://wzo.yanxiufei.cn

Ruby: resp.code.to_i
来源：http://oqb.guowangkeji.top

C#:   (int)resp.StatusCode
来源：http://fkg.jqgfzy.top

[L08] 并发请求多个地址
来源：http://ogl.aizwys.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nrm.tanke756.top

PHP:  curl_multi_init() 系列
来源：http://ncz.gaohongyu789.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ugx.nanxuanxn.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://azg.chenzaomai.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eva.tianlin.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ctr.shzxlz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fvi.hfpthk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fyj.jinqigfzy.top

================================================================================
来源：http://ump.ehwqpu.com

M. 命令行 / 进程 / 环境
来源：http://waf.fanxiaobao.xyz

================================================================================
来源：http://mcw.tarul.cn

[M01] 读取命令行参数
来源：http://wyo.shanyushiyangkeji.top

Py:   sys.argv[1:]
来源：http://jnd.yj20258.top

PHP:  $argv;  $argc;
来源：http://vvk.ctjpmb.com

JS:   process.argv.slice(2)
来源：http://nwp.ydjk.org.cn

TS:   process.argv.slice(2)
来源：http://jvc.gotoacloud.top

Java: args 数组（main 方法参数）
来源：http://ryt.yfazqb.com

Go:   os.Args[1:]
来源：http://die.bjfxy.top

Ruby: ARGV
来源：http://ler.xylfe.cn

C#:   args 数组（Main 方法参数）
来源：http://vwj.tarul.cn

[M02] 读取环境变量
来源：http://khz.ydjk.org.cn

Py:   os.environ.get("HOME")
来源：http://rsd.xinyue.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rhh.zycfv.cn

JS:   process.env.HOME
来源：http://hoz.kuanghao11.cn

TS:   process.env.HOME
来源：http://pha.hcnkem.com

Java: System.getenv("HOME")
来源：http://haw.zdbjq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lgx.vehdjk.com

Ruby: ENV["HOME"]
来源：http://nwl.xuetiantiany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://waq.andypj.xyz

[M03] 执行外部命令
来源：http://ovp.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hta.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nyr.gogol.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vxh.zhiwuduotai.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lqr.zhengqikj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ylo.hysaishi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wse.smart0.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://ono.aibaodan.cn

C#:   Process.Start("ls", "-l");
来源：http://kec.jinyuanbaomall.cn

[M04] 获取当前工作目录
来源：http://hhz.yuanzhike.top

Py:   os.getcwd()
来源：http://jhy.chenjidiqi.icu

PHP:  getcwd();
来源：http://lnk.yfazqb.com

JS:   process.cwd()
来源：http://hkr.haohaochexian.top

TS:   process.cwd()
来源：http://ubj.meibo888.top

Java: Path.of("").toAbsolutePath()
来源：http://cna.sweek.top

Go:   os.Getwd()
来源：http://mus.epnwcf.com

Ruby: Dir.pwd
来源：http://xkz.jinyuanbaomall.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fyp.aibaodan.cn

[M05] 设置退出码
来源：http://jqb.cqqwz.cn

Py:   sys.exit(1)
来源：http://mvg.cdnleiting.top

PHP:  exit(1);
来源：http://ftb.zhongyouzk.top

JS:   process.exit(1)
来源：http://ayv.jinqigfzy.top

TS:   process.exit(1)
来源：http://swl.cheryme.top

Java: System.exit(1)
来源：http://fnu.feifeiyinyue.top

Go:   os.Exit(1)
来源：http://ekv.yj202588.top

Ruby: exit 1
来源：http://tac.yueranfly.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fbw.cucudq.cn

[M06] 向标准错误输出
来源：http://aqo.yuxming.cn

Py:   print("err", file=sys.stderr)
来源：http://xvn.xinyue.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://pba.gotoacloud.top

JS:   console.error("err")
来源：http://qvj.feifeiyinyue.top

TS:   console.error("err")
来源：http://vkn.epnwcf.com

Java: System.err.println("err")
来源：http://yfv.jiagoushi.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mlx.sxryk.cn

Ruby: warn "err"
来源：http://ezq.wangdashe.top

C#:   Console.Error.WriteLine("err")
来源：http://eje.dashuyun.cn

[M07] 判断是否为主入口
来源：http://jot.aibaodan.cn

Py:   if __name__ == "__main__":
来源：http://pag.yanxiufei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hfm.kuanghao11.cn

JS:   require.main === module
来源：http://xmv.smart0.xyz

TS:   require.main === module
来源：http://hyw.zhixingplan.top

Java: public static void main(String[] args)
来源：http://ysh.gogol.net.cn

Go:   func main()
来源：http://yyp.jqgfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gnd.snrcjt.cn

C#:   static void Main(string[] args)
来源：http://lsi.zdqjudy.top

[M08] 获取系统与运行时信息
来源：http://odn.zhengqikj.top

Py:   platform.system();  platform.python_version()
来源：http://sre.chenjidiqi.icu

PHP:  PHP_OS;  phpversion();
来源：http://djj.xinyue.icu

JS:   process.platform;  process.version
来源：http://zjv.epnwcf.com

TS:   process.platform;  process.version
来源：http://gaw.hnxiangtu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qug.yanxiufei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nqo.zhijiandao.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zwy.ydjk.org.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://oea.jinyuanbaomall.cn

================================================================================
来源：http://uni.xziqi.cn

N. 数据结构与算法
来源：http://sfq.shanyushiyangkeji.top

================================================================================
来源：http://kdi.xylfe.cn

[N01] 二分查找（有序数组）
来源：http://tur.cashguo.top

Py:   bisect.bisect_left(arr, x)
来源：http://qeg.ppjwa.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bzp.jiagoushi.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kbg.aizwys.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://web.yvedp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://obo.hysaishi.cn

Go:   sort.SearchInts(arr, x)
来源：http://xby.zhaomingkeji.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://xfj.chenzaomai.com

C#:   Array.BinarySearch(arr, x)
来源：http://ysm.meibo888.top

[N02] 排序（工程实践用内置实现）
来源：http://spb.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://ypg.shanyushiyangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jia.zhaomingkeji.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://ufc.redwolf501.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://iiq.pengpengdd.cyou

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gle.yangfankeji.com

Go:   slices.Sort(arr)
来源：http://wna.cucudq.cn

Ruby: arr.sort
来源：http://jbp.smart0.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://qcd.fktsv.cn

[N03] 快速排序（分治示例）
来源：http://rjx.xingfuxueyuan.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dtd.dashuyun.cn

PHP:  // 递归实现，或用 usort
来源：http://wzg.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://foj.zdqjudy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fsl.dashuyun.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jdz.yuanzhike.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ioz.feifeiyinyue.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uyf.shanyushiyangtech.top

C#:   // 手写递归，或 Array.Sort
来源：http://ttb.hesvh.cn

[N04] 斐波那契数列
来源：http://qbh.xylfe.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zon.ydjk.org.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cua.ybcxt.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xuu.zdqjudy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://azx.hywenlv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qnk.jinqigfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qiv.birdmap.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hjz.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qit.yj202588.top

[N05] 最大公约数
来源：http://rae.gogol.net.cn

Py:   math.gcd(a, b)
来源：http://rfo.yfazqb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uxu.0kj1m.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ema.iojbl.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nih.gogol.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://atm.yj20258.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eme.wangdashe.top

Ruby: a.gcd(b)
来源：http://iih.aibaodan.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yhy.gogol.net.cn

[N06] 判断回文字符串
来源：http://nql.bjfxy.top

Py:   s == s[::-1]
来源：http://iku.wangdashe.top

PHP:  $s === strrev($s);
来源：http://bnx.quarkkingdee.top

JS:   s === [...s].reverse().join("")
来源：http://stg.hongshengwenyu.top

TS:   s === [...s].reverse().join("")
来源：http://ezz.guowangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wer.vehdjk.com

Go:   // 双指针从两端比较
来源：http://piu.xinyue.icu

Ruby: s == s.reverse
来源：http://fal.guowangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rzk.xziqi.cn

[N07] 两数之和（返回下标）
来源：http://apg.gaohongyu789.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jvz.316326.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fin.chenlongwang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://uep.snrcjt.cn

TS:   // 手写 Map<string, number>
来源：http://lld.yuxming.cn

Java: // 手写 HashMap
来源：http://unj.nwbrower.top

Go:   // 手写 map[int]int
来源：http://sjd.yfazqb.com

Ruby: // 手写 Hash
来源：http://swz.yuanzhike.top

C#:   // 手写 Dictionary<int, int>
来源：http://uql.jianghu66.top

[N08] 生成全排列
来源：http://jne.kuanghao11.cn

Py:   itertools.permutations(arr)
来源：http://fpe.c1oappe.top

PHP:  // 手写递归交换
来源：http://mof.0kj1m.cn

JS:   // 手写回溯递归
来源：http://edo.jqgfzy.top

TS:   // 手写回溯递归
来源：http://pem.yueranfly.top

Java: // 手写回溯递归
来源：http://tbf.pycfn.com

Go:   // 手写回溯递归
来源：http://uxz.tanke756.top

Ruby: arr.permutation.to_a
来源：http://ado.wangdashe.top

C#:   // 手写回溯递归
来源：http://yao.xinyue.icu

[N09] 栈与队列
来源：http://yxr.sjlbkw.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wyr.c1oappe.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nve.tarul.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lld.guowangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hjp.vehdjk.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jrq.hesvh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yzs.tarul.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zpb.0kj1m.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mad.jianghu66.top

[N10] 链表节点定义
来源：http://ird.yangfankeji.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aho.yj20258888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gxt.meibo888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jxw.smart0.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mqg.tianlin.xyz

Java: class Node { int v; Node next; }
来源：http://ofh.zhongyouzk.top

Go:   type Node struct { V int; Next *Node }
来源：http://rxm.nanxinkj.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rbs.hnqzz.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mpm.hesvh.cn

[N11] 二叉树中序遍历
来源：http://bej.yonumen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wpw.gzhubu.top

PHP:  // 手写递归函数
来源：http://qwf.cashguo.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tzx.shzxlz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hne.guowangkeji.top

Java: // 手写递归
来源：http://dbd.9152youxi.cn

Go:   // 手写递归
来源：http://ezo.kuanghao11.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://den.shangyingyoupin.top

C#:   // 手写递归
来源：http://foi.hnqzz.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vql.yj202588.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jfy.ydzc1.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xtj.xingfuxueyuan.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bbw.ctjpmb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://job.shuidangran.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ccu.wangdashe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mzj.gaohongyu789.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ccj.yangfankeji.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mis.vehdjk.com

================================================================================
来源：http://phl.ctjpmb.com

O. 并发与异步
来源：http://rpv.xziqi.cn

================================================================================
来源：http://njg.zhengqikj.top

[O01] 启动一个线程
来源：http://yev.shuidangran.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tde.xziqi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jhg.nanxinkj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hkv.yj20258888.top

TS:   // 同 JS
来源：http://jqk.ydjk.org.cn

Java: new Thread(() -> f()).start()
来源：http://ydx.zhaomingkeji.xyz

Go:   go f()
来源：http://vnj.jqgfzy.top

Ruby: Thread.new { f }
来源：http://gxm.zhoulong.xyz

C#:   Task.Run(() => F());
来源：http://qle.bbcook.cn

[O02] 使用线程池
来源：http://ilh.jinqigufen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bam.xinyue.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hxl.redwolf501.top

JS:   // worker_threads 线程池
来源：http://hfk.kuanghao11.cn

TS:   // worker_threads 线程池
来源：http://awu.vehdjk.com

Java: Executors.newFixedThreadPool(4)
来源：http://jnm.smart0.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qyf.hesvh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://umi.birdmap.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qyq.zhixingplan.top

[O03] 加锁保护共享数据
来源：http://ydg.hongshengwenyu.top

Py:   with lock: shared += 1
来源：http://byf.birdmap.top

PHP:  // 用 flock() 做文件锁
来源：http://ytk.wangdashe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pyx.yj20258888.top

TS:   // 同 JS
来源：http://kym.epnwcf.com

Java: synchronized (this) { shared++; }
来源：http://fbf.bjfxy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vzx.jqgfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wsj.tian-w.cn

C#:   lock (gate) { shared++; }
来源：http://hzq.epnwcf.com

[O04] 定义异步函数并等待
来源：http://jwu.hnqzz.top

Py:   async def f():⏎    await g()
来源：http://amz.jqgufenzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hxj.chenlongwang.top

JS:   async function f() { await g(); }
来源：http://kgb.hnqzz.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://nju.fktsv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sfr.zhixingplan.top


<!-- 参考信息 -->