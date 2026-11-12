代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kcq.hammf.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dmu.uphjek.com

[K08] 二进制序列化（非 JSON）
来源：http://ove.fehbvm.com

Py:   pickle.dumps(obj)
来源：http://meh.chenzaomai.com

PHP:  serialize($obj);  unserialize($s);
来源：http://qax.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://hnm.jlsjyb.cn

TS:   v8.serialize(obj)        // Node
来源：http://upe.gogol.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://udu.kuanghao11.cn

Go:   encoding/gob
来源：http://xzp.uphjek.com

Ruby: Marshal.dump(obj)
来源：http://trn.jinyuanbaomall.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://omv.fzhhl.top

================================================================================
来源：http://sfm.sysykeji.top

L. 网络请求
来源：http://rzf.iojbl.cn

================================================================================
来源：http://ufo.aibaodan.cn

[L01] 发送 GET 请求
来源：http://lqd.jqgfzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ewp.xziqi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://inp.shanyushiyangkeji.top

JS:   await fetch(url)
来源：http://gxp.dianchejie.cn

TS:   await fetch(url)
来源：http://vlk.jianghu66.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gmy.tanke756.top

Go:   resp, err := http.Get(url)
来源：http://iro.snrcjt.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tkh.mhx1999.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ijn.birdmap.top

[L02] 发送 POST JSON
来源：http://tev.havefunace.top

Py:   requests.post(url, json={"a": 1})
来源：http://bjd.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xmo.hnxiangtu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vps.xylfe.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pmm.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eqr.pycfn.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qxd.jlsjyb.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eme.fktsv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zbl.sysykeji.top

[L03] 设置自定义请求头
来源：http://ape.pengpengdd.cyou

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cbf.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ecd.shzxlz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://frq.smart0.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sdc.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ayx.hongshengwenyu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yso.hywenlv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sel.hfpthk.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dms.chenlongwang.top

[L04] 设置超时
来源：http://hlb.zhiwuduotai.top

Py:   requests.get(url, timeout=5)
来源：http://qpz.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bjo.zdbjq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qia.zhiwuduotai.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vwl.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jrf.pengpengdd.cyou

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xle.zhongyouzk.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pqt.fzhhl.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sye.gzhubu.top

[L05] 上传文件（multipart）
来源：http://wyw.zhongyouzk.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gze.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ugd.ywan-chungtsiang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://slz.hfpthk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://upo.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pac.shanyushiyangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://irz.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iui.hcnkem.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gav.sjlbkw.cn

[L06] 解析响应为 JSON
来源：http://ezk.vqdsnc.cn

Py:   resp.json()
来源：http://xaf.shzxlz.cn

PHP:  json_decode($body, true);
来源：http://ynq.birdmap.top

JS:   await resp.json()
来源：http://ngg.hywenlv.cn

TS:   await resp.json()
来源：http://bqn.daxiang520.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xmr.snrcjt.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lpt.jinqigfzy.top

Ruby: JSON.parse(resp.body)
来源：http://mld.sysykeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://afp.ydzc1.top

[L07] 处理 HTTP 状态码
来源：http://jwk.vehdjk.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wkp.gogol.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rwc.yfazqb.com

JS:   resp.ok;  resp.status
来源：http://cqs.jqgfzy.top

TS:   resp.ok;  resp.status
来源：http://ccw.sufxvd.cn

Java: resp.statusCode()
来源：http://tfc.vehdjk.com

Go:   resp.StatusCode
来源：http://ote.zhoulong.xyz

Ruby: resp.code.to_i
来源：http://unn.aizwys.cn

C#:   (int)resp.StatusCode
来源：http://hrm.zycfv.cn

[L08] 并发请求多个地址
来源：http://wwy.jinqigufen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rkk.zhixingplan.top

PHP:  curl_multi_init() 系列
来源：http://tvs.jinqigufen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ptq.birdmap.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xkr.sufxvd.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bus.jinyuanbaomall.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qnd.chenlongwang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dxz.dianchejie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zay.svipenyu.cn

================================================================================
来源：http://bda.9152youxi.cn

M. 命令行 / 进程 / 环境
来源：http://taq.feifeiyinyue.top

================================================================================
来源：http://vik.0kj1m.cn

[M01] 读取命令行参数
来源：http://wix.fengsongda.top

Py:   sys.argv[1:]
来源：http://kmu.yongpay.top

PHP:  $argv;  $argc;
来源：http://ren.ybcxt.top

JS:   process.argv.slice(2)
来源：http://vtg.hcnkem.com

TS:   process.argv.slice(2)
来源：http://deu.zhaomingkeji.xyz

Java: args 数组（main 方法参数）
来源：http://ozl.zhaomingkeji.xyz

Go:   os.Args[1:]
来源：http://sjc.snrcjt.cn

Ruby: ARGV
来源：http://dda.gaohongyu789.top

C#:   args 数组（Main 方法参数）
来源：http://ynh.tarul.cn

[M02] 读取环境变量
来源：http://tli.hywenlv.cn

Py:   os.environ.get("HOME")
来源：http://jrs.zdbjq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kbe.hywenlv.cn

JS:   process.env.HOME
来源：http://mdd.haohaochexian.top

TS:   process.env.HOME
来源：http://tub.sxryk.cn

Java: System.getenv("HOME")
来源：http://kjs.gzhubu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aqb.fehbvm.com

Ruby: ENV["HOME"]
来源：http://vgm.epnwcf.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oqz.gogol.net.cn

[M03] 执行外部命令
来源：http://mdc.tarul.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ofn.xuanzx.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nqu.9152youxi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bak.aibaodan.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xiw.xylfe.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xys.jinqigfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://tkl.yongpay.top

Ruby: system("ls -l");  `ls -l`
来源：http://zjj.tianlin.xyz

C#:   Process.Start("ls", "-l");
来源：http://nsk.jinyuanbaomall.cn

[M04] 获取当前工作目录
来源：http://zso.yonumen.top

Py:   os.getcwd()
来源：http://xnv.fengsongda.top

PHP:  getcwd();
来源：http://fer.svipenyu.cn

JS:   process.cwd()
来源：http://ohh.hysaishi.cn

TS:   process.cwd()
来源：http://csu.ehwqpu.com

Java: Path.of("").toAbsolutePath()
来源：http://sgw.hnxiangtu.top

Go:   os.Getwd()
来源：http://tis.jinqigufen.top

Ruby: Dir.pwd
来源：http://lqv.yueranfly.top

C#:   Directory.GetCurrentDirectory()
来源：http://trl.nwbrower.top

[M05] 设置退出码
来源：http://ltp.hywenlv.cn

Py:   sys.exit(1)
来源：http://rfy.tian-w.cn

PHP:  exit(1);
来源：http://hha.xuetiantiany.cn

JS:   process.exit(1)
来源：http://pkw.sysykeji.top

TS:   process.exit(1)
来源：http://irm.zhoulong.xyz

Java: System.exit(1)
来源：http://ups.0kj1m.cn

Go:   os.Exit(1)
来源：http://tmc.shuidangran.top

Ruby: exit 1
来源：http://sex.fengsongda.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ymk.jyoumei.cn

[M06] 向标准错误输出
来源：http://nuo.xinyue.icu

Py:   print("err", file=sys.stderr)
来源：http://xwv.yj202588.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kxm.daria6918.cn

JS:   console.error("err")
来源：http://huc.zhoulong.xyz

TS:   console.error("err")
来源：http://ynz.sweek.top

Java: System.err.println("err")
来源：http://dwr.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://joh.jinqigfzy.top

Ruby: warn "err"
来源：http://gtr.316326.xyz

C#:   Console.Error.WriteLine("err")
来源：http://fzc.vehdjk.com

[M07] 判断是否为主入口
来源：http://xjg.yj20258888.top

Py:   if __name__ == "__main__":
来源：http://fga.hongshengwenyu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aqh.epnwcf.com

JS:   require.main === module
来源：http://ufk.iojbl.cn

TS:   require.main === module
来源：http://gan.pycfn.com

Java: public static void main(String[] args)
来源：http://ygx.daria6918.cn

Go:   func main()
来源：http://xjv.cheryme.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bir.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://xsg.sxryk.cn

[M08] 获取系统与运行时信息
来源：http://xgz.hysaishi.cn

Py:   platform.system();  platform.python_version()
来源：http://xbo.cheryme.top

PHP:  PHP_OS;  phpversion();
来源：http://jmh.zhiwuduotai.top

JS:   process.platform;  process.version
来源：http://onk.tianlin.xyz

TS:   process.platform;  process.version
来源：http://yxx.wangshuangyany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zie.smart0.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://rny.cheryme.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jme.cdnleiting.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://moh.zhengqikj.top

================================================================================
来源：http://nak.0kj1m.cn

N. 数据结构与算法
来源：http://pio.ywan-chungtsiang.top

================================================================================
来源：http://pcs.jqgfzy.top

[N01] 二分查找（有序数组）
来源：http://she.yonumen.top

Py:   bisect.bisect_left(arr, x)
来源：http://wvx.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qhe.xingfuxueyuan.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ipj.ydjk.org.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kan.ybcxt.top

Java: Arrays.binarySearch(arr, x)
来源：http://jgx.hywenlv.cn

Go:   sort.SearchInts(arr, x)
来源：http://ccv.xylfe.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xii.daxiang520.top

C#:   Array.BinarySearch(arr, x)
来源：http://zqq.yuxming.cn

[N02] 排序（工程实践用内置实现）
来源：http://beo.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://qcw.jianghu66.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eyk.chenlongwang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vga.sufxvd.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xdm.sysykeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://urd.fzhhl.top

Go:   slices.Sort(arr)
来源：http://dpk.shanyushiyangtech.top

Ruby: arr.sort
来源：http://ode.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vqb.jqgufenzy.top

[N03] 快速排序（分治示例）
来源：http://rqo.birdmap.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yjl.sysykeji.top

PHP:  // 递归实现，或用 usort
来源：http://erp.0kj1m.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ynz.ivvv.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hxm.snrcjt.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vgf.shangyingyoupin.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dsb.zhaomingkeji.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ngt.zhengqikj.top

C#:   // 手写递归，或 Array.Sort
来源：http://tzl.ybcxt.top

[N04] 斐波那契数列
来源：http://hnq.bjfxy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://chg.hnqzz.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zwr.jinqigufen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pmo.jqgufenzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://deo.zhiwuduotai.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://twb.svipenyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xhd.gogol.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://klh.yueranfly.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kfb.vehdjk.com

[N05] 最大公约数
来源：http://dff.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://ggv.uphjek.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jmw.aizwys.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zgl.yuxming.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uon.shanyushiyangtech.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://crr.kuanghao11.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sie.sjlbkw.cn

Ruby: a.gcd(b)
来源：http://xkw.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qxa.yanxiufei.cn

[N06] 判断回文字符串
来源：http://ely.shanyushiyangtech.top

Py:   s == s[::-1]
来源：http://hze.dianchejie.cn

PHP:  $s === strrev($s);
来源：http://bti.ppjwa.cn

JS:   s === [...s].reverse().join("")
来源：http://vza.havefunace.top

TS:   s === [...s].reverse().join("")
来源：http://zby.guowangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pbd.tarul.cn

Go:   // 双指针从两端比较
来源：http://wio.aibaodan.cn

Ruby: s == s.reverse
来源：http://ien.hywenlv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://leb.vqdsnc.cn

[N07] 两数之和（返回下标）
来源：http://mgg.fzhhl.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zxr.gzhubu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aeo.jianghu66.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zvn.haohaochexian.top

TS:   // 手写 Map<string, number>
来源：http://jqz.dianchejie.cn

Java: // 手写 HashMap
来源：http://enl.cdnleiting.top

Go:   // 手写 map[int]int
来源：http://tqj.hesvh.cn

Ruby: // 手写 Hash
来源：http://njb.jyoumei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tdp.xinyue.icu

[N08] 生成全排列
来源：http://ozx.ydjk.org.cn

Py:   itertools.permutations(arr)
来源：http://hmq.cdnleiting.top

PHP:  // 手写递归交换
来源：http://bzq.ydzc1.top

JS:   // 手写回溯递归
来源：http://szd.ctjpmb.com

TS:   // 手写回溯递归
来源：http://hvh.jiagoushi.top

Java: // 手写回溯递归
来源：http://hrx.yj202588.top

Go:   // 手写回溯递归
来源：http://fsi.ppjwa.cn

Ruby: arr.permutation.to_a
来源：http://mfm.sysykeji.top

C#:   // 手写回溯递归
来源：http://not.xinyue.icu

[N09] 栈与队列
来源：http://ftu.meibo888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ppc.hcnkem.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ddg.guowangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ate.hongshengwenyu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rjy.yueranfly.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ykd.52xcode.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ckj.zhixingplan.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tsb.yonumen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nbj.chenlongwang.top

[N10] 链表节点定义
来源：http://zea.tanke756.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yls.9152youxi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://luo.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dqw.nwbrower.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://phi.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://fpu.jqgufenzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://evm.chenzaomai.com

Ruby: Node = Struct.new(:v, :next)
来源：http://umy.cashguo.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dvx.daxiang520.top

[N11] 二叉树中序遍历
来源：http://zxh.jqgufenzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pnu.hysaishi.cn

PHP:  // 手写递归函数
来源：http://jfi.guannengcc.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pir.yj202588.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gup.kuanghao11.cn

Java: // 手写递归
来源：http://rtm.jinqigfzy.top

Go:   // 手写递归
来源：http://ddu.cashguo.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vjk.9152youxi.cn

C#:   // 手写递归
来源：http://nbj.hammf.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fcu.redwolf501.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rwg.cdnleiting.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://acv.fehbvm.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jej.guannengcc.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tso.52xcode.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tyd.sweek.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jto.fktsv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ova.zhijiandao.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ltx.fehbvm.com

================================================================================
来源：http://bek.yfazqb.com

O. 并发与异步
来源：http://gaq.hesvh.cn

================================================================================
来源：http://nbq.gzhubu.top

[O01] 启动一个线程
来源：http://ejt.wangdashe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ehr.bbcook.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tbr.nwbrower.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xsv.haohaochexian.top

TS:   // 同 JS
来源：http://qte.zhongyouzk.top

Java: new Thread(() -> f()).start()
来源：http://imx.zhoulong.xyz

Go:   go f()
来源：http://eaa.jinghuilouyu.cn

Ruby: Thread.new { f }
来源：http://dnv.zhongyouzk.top

C#:   Task.Run(() => F());
来源：http://gxk.svipenyu.cn

[O02] 使用线程池
来源：http://nfq.guowangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oty.zhongyouzk.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xyj.shuidangran.top

JS:   // worker_threads 线程池
来源：http://wyu.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://erw.epnwcf.com

Java: Executors.newFixedThreadPool(4)
来源：http://ezw.zhoulong.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://aun.hesvh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kpi.guowangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zir.yuxming.cn

[O03] 加锁保护共享数据
来源：http://veq.guannengcc.top

Py:   with lock: shared += 1
来源：http://xwk.tian-w.cn

PHP:  // 用 flock() 做文件锁
来源：http://ads.ybcxt.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hfj.zdqjudy.top

TS:   // 同 JS
来源：http://xyn.nanxuanxn.top

Java: synchronized (this) { shared++; }
来源：http://plv.yj202588.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://slb.meibo888.top


<!-- 参考信息 -->