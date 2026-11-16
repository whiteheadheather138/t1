代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pzu.chenlongwang.top

[K07] 进制转换
来源：http://qxn.yongpay.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rzn.jlsjyb.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nji.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tfk.jqgfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yvw.dashuyun.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bry.jinghuilouyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yap.tanke756.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zsu.andypj.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xtu.chenzaomai.com

[K08] 二进制序列化（非 JSON）
来源：http://qpk.yongpay.top

Py:   pickle.dumps(obj)
来源：http://ymv.shangyingyoupin.top

PHP:  serialize($obj);  unserialize($s);
来源：http://eyn.bjfxy.top

JS:   v8.serialize(obj)        // Node
来源：http://qpz.hywenlv.cn

TS:   v8.serialize(obj)        // Node
来源：http://uge.zhixingplan.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zmz.uphjek.com

Go:   encoding/gob
来源：http://kmd.zhiwuduotai.top

Ruby: Marshal.dump(obj)
来源：http://gee.jiagoushi.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fwm.yj20258888.top

================================================================================
来源：http://wql.sxryk.cn

L. 网络请求
来源：http://pki.zhiwuduotai.top

================================================================================
来源：http://kem.0kj1m.cn

[L01] 发送 GET 请求
来源：http://bvx.gogol.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pfk.hysaishi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ekt.nanxinkj.top

JS:   await fetch(url)
来源：http://shs.redwolf501.top

TS:   await fetch(url)
来源：http://bpa.nwbrower.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://btb.yuxming.cn

Go:   resp, err := http.Get(url)
来源：http://zeb.birdmap.top

Ruby: Net::HTTP.get(URI(url))
来源：http://elc.shuidangran.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iaf.gaohongyu789.top

[L02] 发送 POST JSON
来源：http://bxn.chenjidiqi.icu

Py:   requests.post(url, json={"a": 1})
来源：http://qvk.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kwy.sxryk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zqv.hfpthk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://put.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sfd.52xcode.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zyj.yvedp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://trf.mhx1999.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wlw.svipenyu.cn

[L03] 设置自定义请求头
来源：http://nfe.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jnd.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://swi.gogol.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://laj.zhijiandao.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mdi.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kbs.guowangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wyf.meibo888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://axi.jiagoushi.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zls.guowangkeji.top

[L04] 设置超时
来源：http://dxi.xuanzx.com

Py:   requests.get(url, timeout=5)
来源：http://zta.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mmh.yueranfly.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zrc.zhengqikj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nli.kuanghao11.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xab.ivvv.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qbg.tianlin.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dgi.pengpengdd.cyou

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://txf.chenzaomai.com

[L05] 上传文件（multipart）
来源：http://uwp.xinyue.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ecj.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rib.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hyf.shuidangran.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tow.tianlin.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gks.0kj1m.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dzu.sxryk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://psx.quarkkingdee.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qqq.jinghuilouyu.cn

[L06] 解析响应为 JSON
来源：http://dim.52xcode.cn

Py:   resp.json()
来源：http://plj.nanxuanxn.top

PHP:  json_decode($body, true);
来源：http://jpf.zhijiandao.cn

JS:   await resp.json()
来源：http://qou.hfpthk.cn

TS:   await resp.json()
来源：http://udj.jlsjyb.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sqx.cucudq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ngd.smart0.xyz

Ruby: JSON.parse(resp.body)
来源：http://jly.sweek.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cnj.havefunace.top

[L07] 处理 HTTP 状态码
来源：http://sxc.chenlongwang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dae.sjlbkw.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jdu.pycfn.com

JS:   resp.ok;  resp.status
来源：http://wac.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://yvf.fehbvm.com

Java: resp.statusCode()
来源：http://rry.zhiwuduotai.top

Go:   resp.StatusCode
来源：http://mhu.jinqigfzy.top

Ruby: resp.code.to_i
来源：http://inm.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://xvb.bbcook.cn

[L08] 并发请求多个地址
来源：http://job.yj20258888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rdo.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://yqc.yvedp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xnp.cashguo.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hgx.tanke756.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bjl.ydzc1.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://snx.yueranfly.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://idj.iojbl.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nrl.ivvv.top

================================================================================
来源：http://sdg.cheryme.top

M. 命令行 / 进程 / 环境
来源：http://kgg.cqqwz.cn

================================================================================
来源：http://qhh.aizwys.cn

[M01] 读取命令行参数
来源：http://cpz.jinyuanbaomall.cn

Py:   sys.argv[1:]
来源：http://gqd.andypj.xyz

PHP:  $argv;  $argc;
来源：http://njb.mhx1999.top

JS:   process.argv.slice(2)
来源：http://ckm.xuanzx.com

TS:   process.argv.slice(2)
来源：http://vmb.ywan-chungtsiang.top

Java: args 数组（main 方法参数）
来源：http://wut.jinqigufen.top

Go:   os.Args[1:]
来源：http://vjr.zdqjudy.top

Ruby: ARGV
来源：http://acv.cqqwz.cn

C#:   args 数组（Main 方法参数）
来源：http://vpi.ydjk.org.cn

[M02] 读取环境变量
来源：http://ptq.snrcjt.cn

Py:   os.environ.get("HOME")
来源：http://wps.jqgufenzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hjw.cheryme.top

JS:   process.env.HOME
来源：http://bcs.zdbjq.cn

TS:   process.env.HOME
来源：http://ahy.guannengcc.top

Java: System.getenv("HOME")
来源：http://xgf.sufxvd.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ajp.9152youxi.cn

Ruby: ENV["HOME"]
来源：http://jvz.hywenlv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://stc.havefunace.top

[M03] 执行外部命令
来源：http://nvm.havefunace.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ldj.yj202588.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tvj.birdmap.top

JS:   child_process.execSync("ls -l").toString()
来源：http://sfx.jinghuilouyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xqc.c1oappe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cqy.shzxlz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lnu.yonumen.top

Ruby: system("ls -l");  `ls -l`
来源：http://lwl.jinqigufen.top

C#:   Process.Start("ls", "-l");
来源：http://mbt.smart0.xyz

[M04] 获取当前工作目录
来源：http://rfw.yueranfly.top

Py:   os.getcwd()
来源：http://mej.vehdjk.com

PHP:  getcwd();
来源：http://glv.gaohongyu789.top

JS:   process.cwd()
来源：http://dit.nanxuanxn.top

TS:   process.cwd()
来源：http://sfe.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://oik.hysaishi.cn

Go:   os.Getwd()
来源：http://lzz.svipenyu.cn

Ruby: Dir.pwd
来源：http://ejo.vehdjk.com

C#:   Directory.GetCurrentDirectory()
来源：http://dsf.shanyushiyangtech.top

[M05] 设置退出码
来源：http://mgg.daxiang520.top

Py:   sys.exit(1)
来源：http://bnp.zhiwuduotai.top

PHP:  exit(1);
来源：http://umi.aibaodan.cn

JS:   process.exit(1)
来源：http://rvy.jiagoushi.top

TS:   process.exit(1)
来源：http://ygl.zhijiandao.cn

Java: System.exit(1)
来源：http://elv.xylfe.cn

Go:   os.Exit(1)
来源：http://feu.yj202588.top

Ruby: exit 1
来源：http://uoh.xingfuxueyuan.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://krz.bbcook.cn

[M06] 向标准错误输出
来源：http://hzg.sysykeji.top

Py:   print("err", file=sys.stderr)
来源：http://wyq.svipenyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://evv.jinyuanbaomall.cn

JS:   console.error("err")
来源：http://brv.yueranfly.top

TS:   console.error("err")
来源：http://jqk.sjlbkw.cn

Java: System.err.println("err")
来源：http://ksw.shangyingyoupin.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vep.kuanghao11.cn

Ruby: warn "err"
来源：http://iba.pengpengdd.cyou

C#:   Console.Error.WriteLine("err")
来源：http://ohy.svipenyu.cn

[M07] 判断是否为主入口
来源：http://wej.zhaomingkeji.xyz

Py:   if __name__ == "__main__":
来源：http://fat.redwolf501.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wrb.cqqwz.cn

JS:   require.main === module
来源：http://pkl.hcnkem.com

TS:   require.main === module
来源：http://xni.chenjidiqi.icu

Java: public static void main(String[] args)
来源：http://iwe.sufxvd.cn

Go:   func main()
来源：http://pda.jinqigfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://neu.jiagoushi.top

C#:   static void Main(string[] args)
来源：http://qol.tarul.cn

[M08] 获取系统与运行时信息
来源：http://pdf.hysaishi.cn

Py:   platform.system();  platform.python_version()
来源：http://ceg.yj202588.top

PHP:  PHP_OS;  phpversion();
来源：http://qgo.zhixingplan.top

JS:   process.platform;  process.version
来源：http://lmv.cucudq.cn

TS:   process.platform;  process.version
来源：http://uor.tian-w.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jps.hysaishi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hnb.yfazqb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ekl.c1oappe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bgf.zdbjq.cn

================================================================================
来源：http://myi.dashuyun.cn

N. 数据结构与算法
来源：http://zit.xylfe.cn

================================================================================
来源：http://fvi.fanxiaobao.xyz

[N01] 二分查找（有序数组）
来源：http://cix.meibo888.top

Py:   bisect.bisect_left(arr, x)
来源：http://mbe.zycfv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qwr.gotoacloud.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vpr.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ztw.tarul.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hyu.bbcook.cn

Go:   sort.SearchInts(arr, x)
来源：http://xue.guannengcc.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rft.haohaochexian.top

C#:   Array.BinarySearch(arr, x)
来源：http://smf.jqgfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://ivf.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://fnc.shuidangran.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://phu.yvedp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ers.sxryk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yof.smart0.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yls.yvedp.cn

Go:   slices.Sort(arr)
来源：http://mno.xuetiantiany.cn

Ruby: arr.sort
来源：http://owv.0kj1m.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nva.zdbjq.cn

[N03] 快速排序（分治示例）
来源：http://tbd.meibo888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://byk.gogol.net.cn

PHP:  // 递归实现，或用 usort
来源：http://xoo.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qva.havefunace.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jwm.52xcode.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pgg.feifeiyinyue.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rzq.hammf.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dzu.zhaomingkeji.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://dnu.fengsongda.top

[N04] 斐波那契数列
来源：http://ypd.shanyushiyangtech.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://efi.hcnkem.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://atn.ehwqpu.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://amr.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qbb.redwolf501.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lqx.guannengcc.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zrd.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ngk.zhijiandao.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uae.nanxuanxn.top

[N05] 最大公约数
来源：http://eeg.zhiwuduotai.top

Py:   math.gcd(a, b)
来源：http://fra.quarkkingdee.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kxa.fehbvm.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://han.wangdashe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pwi.ybcxt.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wmx.jlsjyb.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xnv.ywan-chungtsiang.top

Ruby: a.gcd(b)
来源：http://htv.hywenlv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cxl.chenlongwang.top

[N06] 判断回文字符串
来源：http://uec.xylfe.cn

Py:   s == s[::-1]
来源：http://rut.zhongyouzk.top

PHP:  $s === strrev($s);
来源：http://xfx.ehwqpu.com

JS:   s === [...s].reverse().join("")
来源：http://svw.nwbrower.top

TS:   s === [...s].reverse().join("")
来源：http://psa.gogol.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://euj.ybcxt.top

Go:   // 双指针从两端比较
来源：http://sio.sysykeji.top

Ruby: s == s.reverse
来源：http://xzq.zycfv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jfz.9152youxi.cn

[N07] 两数之和（返回下标）
来源：http://hfa.smart0.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nyh.ppjwa.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rjl.tanke756.top

JS:   // 手写 Map：map.set(v, i)
来源：http://hgs.jiagoushi.top

TS:   // 手写 Map<string, number>
来源：http://scl.hywenlv.cn

Java: // 手写 HashMap
来源：http://gqf.yfazqb.com

Go:   // 手写 map[int]int
来源：http://nua.hammf.cn

Ruby: // 手写 Hash
来源：http://orv.tianlin.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://cej.fzhhl.top

[N08] 生成全排列
来源：http://kep.jinqigufen.top

Py:   itertools.permutations(arr)
来源：http://wnw.zdqjudy.top

PHP:  // 手写递归交换
来源：http://ter.yonumen.top

JS:   // 手写回溯递归
来源：http://hky.daria6918.cn

TS:   // 手写回溯递归
来源：http://ifb.guowangkeji.top

Java: // 手写回溯递归
来源：http://jwq.tanke756.top

Go:   // 手写回溯递归
来源：http://ntu.9152youxi.cn

Ruby: arr.permutation.to_a
来源：http://wky.zdbjq.cn

C#:   // 手写回溯递归
来源：http://wxd.yuanzhike.top

[N09] 栈与队列
来源：http://pya.zdqjudy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vbi.nwbrower.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xay.zdqjudy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jvo.xinyue.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xld.wangshuangyany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mus.hesvh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://npo.hesvh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://aux.dashuyun.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sdg.daxiang520.top

[N10] 链表节点定义
来源：http://etl.hywenlv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dfd.yonumen.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hok.mhx1999.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://scg.pengpengdd.cyou

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mry.xziqi.cn

Java: class Node { int v; Node next; }
来源：http://nha.tian-w.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hvm.shzxlz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://idx.hywenlv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://czx.zhiwuduotai.top

[N11] 二叉树中序遍历
来源：http://lfz.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oza.xylfe.cn

PHP:  // 手写递归函数
来源：http://kdl.redwolf501.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rit.0kj1m.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cro.sxryk.cn

Java: // 手写递归
来源：http://dwt.jinqigfzy.top

Go:   // 手写递归
来源：http://uen.shangyingyoupin.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://esj.snrcjt.cn

C#:   // 手写递归
来源：http://icf.zhijiandao.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ubu.yuanzhike.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ofc.gzhubu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sqt.jinyuanbaomall.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gyc.sweek.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lgt.gotoacloud.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gpm.shuidangran.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ztx.daxiang520.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gqv.wangdashe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://awx.chenlongwang.top

================================================================================
来源：http://zen.yfazqb.com

O. 并发与异步
来源：http://fiq.fengsongda.top

================================================================================
来源：http://exm.nwbrower.top

[O01] 启动一个线程
来源：http://tpm.ppjwa.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lwj.ydzc1.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://skl.aizwys.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pbn.zdbjq.cn

TS:   // 同 JS
来源：http://ybc.yueranfly.top

Java: new Thread(() -> f()).start()
来源：http://cks.yj20258.top

Go:   go f()
来源：http://bcb.iojbl.cn

Ruby: Thread.new { f }
来源：http://etb.yangfankeji.com

C#:   Task.Run(() => F());
来源：http://kch.hammf.cn

[O02] 使用线程池
来源：http://cfk.fehbvm.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://buh.xylfe.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jqr.cqqwz.cn

JS:   // worker_threads 线程池
来源：http://yei.9152youxi.cn

TS:   // worker_threads 线程池
来源：http://kjp.yvedp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bvj.hnqzz.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jgp.iojbl.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xmc.fehbvm.com


<!-- 参考信息 -->