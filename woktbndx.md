代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nib.hammf.cn

[K07] 进制转换
来源：http://idt.sweek.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://afd.cqqwz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hul.xinyue.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ufn.sweek.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pbu.shanyushiyangtech.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ski.zhiwuduotai.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oyh.daxiang520.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xpo.hnqzz.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://npj.snrcjt.cn

[K08] 二进制序列化（非 JSON）
来源：http://urb.yongpay.top

Py:   pickle.dumps(obj)
来源：http://ngs.ehwqpu.com

PHP:  serialize($obj);  unserialize($s);
来源：http://gbn.gotoacloud.top

JS:   v8.serialize(obj)        // Node
来源：http://qtu.yj202588.top

TS:   v8.serialize(obj)        // Node
来源：http://acf.tian-w.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://veu.cdnleiting.top

Go:   encoding/gob
来源：http://csk.gzhubu.top

Ruby: Marshal.dump(obj)
来源：http://ybx.shangyingyoupin.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ubm.hnxiangtu.top

================================================================================
来源：http://esn.svipenyu.cn

L. 网络请求
来源：http://tlq.jinghuilouyu.cn

================================================================================
来源：http://hyt.jinqigufen.top

[L01] 发送 GET 请求
来源：http://ded.jinqigufen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mrd.fktsv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dvq.yj20258.top

JS:   await fetch(url)
来源：http://uyu.jlsjyb.cn

TS:   await fetch(url)
来源：http://oyc.zycfv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pqj.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://oat.sxryk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jvv.yvedp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bbt.shanyushiyangtech.top

[L02] 发送 POST JSON
来源：http://fcs.cheryme.top

Py:   requests.post(url, json={"a": 1})
来源：http://dft.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yfz.jyoumei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cgz.hongshengwenyu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tvi.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xwv.jinyuanbaomall.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ulz.hesvh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kim.nwbrower.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jrc.vehdjk.com

[L03] 设置自定义请求头
来源：http://kww.shanyushiyangtech.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://euu.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wvv.havefunace.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ikx.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qqi.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ttw.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://grb.tian-w.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://acz.ehwqpu.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lzu.chenlongwang.top

[L04] 设置超时
来源：http://jor.sufxvd.cn

Py:   requests.get(url, timeout=5)
来源：http://imw.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vqm.zhaomingkeji.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://azk.jianghu66.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ivr.shanyushiyangtech.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tjm.hnxiangtu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ygl.gogol.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bsx.fengsongda.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yrt.zdqjudy.top

[L05] 上传文件（multipart）
来源：http://mjp.zdbjq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eyu.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ihi.xingfuxueyuan.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://luy.epnwcf.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rqc.shuidangran.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fbc.0kj1m.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fog.fktsv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kfc.gzhubu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://osc.zdbjq.cn

[L06] 解析响应为 JSON
来源：http://slm.cucudq.cn

Py:   resp.json()
来源：http://lug.fengsongda.top

PHP:  json_decode($body, true);
来源：http://xee.yueranfly.top

JS:   await resp.json()
来源：http://kyj.ivvv.top

TS:   await resp.json()
来源：http://yef.shzxlz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ata.nanxinkj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mtg.cdnleiting.top

Ruby: JSON.parse(resp.body)
来源：http://awv.shanyushiyangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xox.xuetiantiany.cn

[L07] 处理 HTTP 状态码
来源：http://mbf.gaohongyu789.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://exm.zhixingplan.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lap.gotoacloud.top

JS:   resp.ok;  resp.status
来源：http://wjd.hongshengwenyu.top

TS:   resp.ok;  resp.status
来源：http://cin.zdbjq.cn

Java: resp.statusCode()
来源：http://vsw.zhoulong.xyz

Go:   resp.StatusCode
来源：http://ydp.dianchejie.cn

Ruby: resp.code.to_i
来源：http://pin.uphjek.com

C#:   (int)resp.StatusCode
来源：http://uid.mhx1999.top

[L08] 并发请求多个地址
来源：http://ozu.feifeiyinyue.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bze.sysykeji.top

PHP:  curl_multi_init() 系列
来源：http://jzk.ehwqpu.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fdy.bbcook.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rtl.pycfn.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ylp.mhx1999.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mys.jyoumei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ujh.nanxinkj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xcr.sysykeji.top

================================================================================
来源：http://rlz.fengsongda.top

M. 命令行 / 进程 / 环境
来源：http://qcy.9152youxi.cn

================================================================================
来源：http://var.hcnkem.com

[M01] 读取命令行参数
来源：http://tbt.aibaodan.cn

Py:   sys.argv[1:]
来源：http://xhl.yj202588.top

PHP:  $argv;  $argc;
来源：http://gpg.yj20258.top

JS:   process.argv.slice(2)
来源：http://eaw.chenzaomai.com

TS:   process.argv.slice(2)
来源：http://puv.sjlbkw.cn

Java: args 数组（main 方法参数）
来源：http://svh.yueranfly.top

Go:   os.Args[1:]
来源：http://hsz.dianchejie.cn

Ruby: ARGV
来源：http://wer.tarul.cn

C#:   args 数组（Main 方法参数）
来源：http://qss.quarkkingdee.top

[M02] 读取环境变量
来源：http://ter.sweek.top

Py:   os.environ.get("HOME")
来源：http://iiz.tarul.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wga.feifeiyinyue.top

JS:   process.env.HOME
来源：http://zrz.c1oappe.top

TS:   process.env.HOME
来源：http://nar.chenlongwang.top

Java: System.getenv("HOME")
来源：http://bqe.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://low.svipenyu.cn

Ruby: ENV["HOME"]
来源：http://uwc.xuetiantiany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://efd.snrcjt.cn

[M03] 执行外部命令
来源：http://qty.zhengqikj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://krb.cqqwz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cpt.jianghu66.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cue.ybcxt.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ajv.daria6918.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hfu.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ieb.cashguo.top

Ruby: system("ls -l");  `ls -l`
来源：http://bse.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://lsn.ywan-chungtsiang.top

[M04] 获取当前工作目录
来源：http://pqj.sjlbkw.cn

Py:   os.getcwd()
来源：http://wtb.havefunace.top

PHP:  getcwd();
来源：http://lms.yangfankeji.com

JS:   process.cwd()
来源：http://hpf.jyoumei.cn

TS:   process.cwd()
来源：http://rsh.c1oappe.top

Java: Path.of("").toAbsolutePath()
来源：http://iei.wangdashe.top

Go:   os.Getwd()
来源：http://cts.bjfxy.top

Ruby: Dir.pwd
来源：http://ohc.zhijiandao.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gdv.xylfe.cn

[M05] 设置退出码
来源：http://fzr.ydjk.org.cn

Py:   sys.exit(1)
来源：http://rda.cheryme.top

PHP:  exit(1);
来源：http://etf.zhijiandao.cn

JS:   process.exit(1)
来源：http://nax.hysaishi.cn

TS:   process.exit(1)
来源：http://rly.pengpengdd.cyou

Java: System.exit(1)
来源：http://ciw.gzhubu.top

Go:   os.Exit(1)
来源：http://mea.sxryk.cn

Ruby: exit 1
来源：http://hdl.yj202588.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://goa.yuanzhike.top

[M06] 向标准错误输出
来源：http://oog.hywenlv.cn

Py:   print("err", file=sys.stderr)
来源：http://udl.sjlbkw.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://baa.chenlongwang.top

JS:   console.error("err")
来源：http://bwl.ydzc1.top

TS:   console.error("err")
来源：http://gwg.vehdjk.com

Java: System.err.println("err")
来源：http://sse.smart0.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wga.fktsv.cn

Ruby: warn "err"
来源：http://qxo.nanxuanxn.top

C#:   Console.Error.WriteLine("err")
来源：http://psb.daria6918.cn

[M07] 判断是否为主入口
来源：http://jhw.sufxvd.cn

Py:   if __name__ == "__main__":
来源：http://feo.sufxvd.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://brj.chenjidiqi.icu

JS:   require.main === module
来源：http://fob.ppjwa.cn

TS:   require.main === module
来源：http://zhy.kuanghao11.cn

Java: public static void main(String[] args)
来源：http://gah.hnqzz.top

Go:   func main()
来源：http://vou.tian-w.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://skh.yj20258888.top

C#:   static void Main(string[] args)
来源：http://dix.wangdashe.top

[M08] 获取系统与运行时信息
来源：http://fvb.xylfe.cn

Py:   platform.system();  platform.python_version()
来源：http://ytu.sxryk.cn

PHP:  PHP_OS;  phpversion();
来源：http://zgo.svipenyu.cn

JS:   process.platform;  process.version
来源：http://yus.wangdashe.top

TS:   process.platform;  process.version
来源：http://quu.dianchejie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jba.sjlbkw.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vvn.yfazqb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nma.ivvv.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ctr.pycfn.com

================================================================================
来源：http://ynu.sjlbkw.cn

N. 数据结构与算法
来源：http://xzn.xylfe.cn

================================================================================
来源：http://kxo.hcnkem.com

[N01] 二分查找（有序数组）
来源：http://gcj.epnwcf.com

Py:   bisect.bisect_left(arr, x)
来源：http://fkf.svipenyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://iyv.yongpay.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nac.guowangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xay.zhixingplan.top

Java: Arrays.binarySearch(arr, x)
来源：http://ovl.9152youxi.cn

Go:   sort.SearchInts(arr, x)
来源：http://czu.yangfankeji.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://bok.hysaishi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qtz.yvedp.cn

[N02] 排序（工程实践用内置实现）
来源：http://kte.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://qnl.xingfuxueyuan.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bly.yanxiufei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://akj.wangshuangyany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://opc.yj202588.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tpt.wangdashe.top

Go:   slices.Sort(arr)
来源：http://tjz.meibo888.top

Ruby: arr.sort
来源：http://wpz.vqdsnc.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uop.yuxming.cn

[N03] 快速排序（分治示例）
来源：http://txe.zhijiandao.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://exo.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://cpa.jiagoushi.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lcz.gaohongyu789.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lov.svipenyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vzm.bbcook.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rmo.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://etm.havefunace.top

C#:   // 手写递归，或 Array.Sort
来源：http://gyq.sweek.top

[N04] 斐波那契数列
来源：http://wmz.yuxming.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xby.bbcook.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ere.gogol.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://skc.0kj1m.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uph.meibo888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sbj.xingfuxueyuan.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://txv.9152youxi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://scm.hnqzz.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ovl.316326.xyz

[N05] 最大公约数
来源：http://oyr.yvedp.cn

Py:   math.gcd(a, b)
来源：http://nkq.jinqigfzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gel.gaohongyu789.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zxa.chenlongwang.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ceq.sysykeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cqo.shzxlz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://azf.cashguo.top

Ruby: a.gcd(b)
来源：http://hit.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hmw.svipenyu.cn

[N06] 判断回文字符串
来源：http://cmp.jqgufenzy.top

Py:   s == s[::-1]
来源：http://mgh.epnwcf.com

PHP:  $s === strrev($s);
来源：http://iva.cashguo.top

JS:   s === [...s].reverse().join("")
来源：http://vwt.hywenlv.cn

TS:   s === [...s].reverse().join("")
来源：http://boa.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qhi.zhijiandao.cn

Go:   // 双指针从两端比较
来源：http://myt.0kj1m.cn

Ruby: s == s.reverse
来源：http://fyd.uphjek.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://nai.yuanzhike.top

[N07] 两数之和（返回下标）
来源：http://qoi.bjfxy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zxh.c1oappe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jjw.xinyue.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://gjl.zhongyouzk.top

TS:   // 手写 Map<string, number>
来源：http://fip.bbcook.cn

Java: // 手写 HashMap
来源：http://udb.xziqi.cn

Go:   // 手写 map[int]int
来源：http://tce.c1oappe.top

Ruby: // 手写 Hash
来源：http://ucu.sjlbkw.cn

C#:   // 手写 Dictionary<int, int>
来源：http://scu.ywan-chungtsiang.top

[N08] 生成全排列
来源：http://wej.shzxlz.cn

Py:   itertools.permutations(arr)
来源：http://vzo.dianchejie.cn

PHP:  // 手写递归交换
来源：http://taa.cdnleiting.top

JS:   // 手写回溯递归
来源：http://cvv.svipenyu.cn

TS:   // 手写回溯递归
来源：http://rty.cucudq.cn

Java: // 手写回溯递归
来源：http://mfi.jqgfzy.top

Go:   // 手写回溯递归
来源：http://hek.jiagoushi.top

Ruby: arr.permutation.to_a
来源：http://ljy.snrcjt.cn

C#:   // 手写回溯递归
来源：http://rsj.chenlongwang.top

[N09] 栈与队列
来源：http://tgi.yuanzhike.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bmh.jiagoushi.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://etq.zhiwuduotai.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xuv.gzhubu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hsr.gogol.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://asj.haohaochexian.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ofx.cucudq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://shh.hnqzz.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hgp.vehdjk.com

[N10] 链表节点定义
来源：http://ann.zdbjq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rxo.sjlbkw.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qjl.jqgufenzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://klw.haohaochexian.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dnw.guannengcc.top

Java: class Node { int v; Node next; }
来源：http://kvc.xingfuxueyuan.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://lmw.tanke756.top

Ruby: Node = Struct.new(:v, :next)
来源：http://obh.jinghuilouyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lcn.yongpay.top

[N11] 二叉树中序遍历
来源：http://nwl.tianlin.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kcv.sufxvd.cn

PHP:  // 手写递归函数
来源：http://toy.birdmap.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mte.redwolf501.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://otd.daria6918.cn

Java: // 手写递归
来源：http://bkf.kuanghao11.cn

Go:   // 手写递归
来源：http://svf.daria6918.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wdx.ehwqpu.com

C#:   // 手写递归
来源：http://czb.hfpthk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aok.sweek.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vmn.fktsv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://syp.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pfd.52xcode.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hxq.xingfuxueyuan.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tso.guannengcc.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ftm.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uaz.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vbj.tianlin.xyz

================================================================================
来源：http://koj.hywenlv.cn

O. 并发与异步
来源：http://laq.hnxiangtu.top

================================================================================
来源：http://vsy.yj202588.top

[O01] 启动一个线程
来源：http://che.yj20258.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mpm.hnxiangtu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://arq.daria6918.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gyg.shzxlz.cn

TS:   // 同 JS
来源：http://xjf.xingfuxueyuan.xyz

Java: new Thread(() -> f()).start()
来源：http://nuz.fanxiaobao.xyz

Go:   go f()
来源：http://cux.sysykeji.top

Ruby: Thread.new { f }
来源：http://ddr.jyoumei.cn

C#:   Task.Run(() => F());
来源：http://ffy.wangshuangyany.cn

[O02] 使用线程池
来源：http://zkg.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bdq.gzhubu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wxe.xingfuxueyuan.xyz

JS:   // worker_threads 线程池
来源：http://jww.316326.xyz

TS:   // worker_threads 线程池
来源：http://ipq.daxiang520.top

Java: Executors.newFixedThreadPool(4)
来源：http://khe.hcnkem.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://orp.jqgufenzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qkg.jqgfzy.top


<!-- 参考信息 -->