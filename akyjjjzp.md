代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://doa.yangfankeji.com

[K07] 进制转换
来源：http://cau.yongpay.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fwo.52xcode.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pxg.ywan-chungtsiang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sts.xziqi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bsc.cheryme.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rmv.zycfv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lov.chenlongwang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lwm.wangshuangyany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://avq.jyoumei.cn

[K08] 二进制序列化（非 JSON）
来源：http://gde.jyoumei.cn

Py:   pickle.dumps(obj)
来源：http://bsr.chenjidiqi.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://ajz.aibaodan.cn

JS:   v8.serialize(obj)        // Node
来源：http://ndo.shanyushiyangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://hvf.yvedp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zhm.cdnleiting.top

Go:   encoding/gob
来源：http://mky.hfpthk.cn

Ruby: Marshal.dump(obj)
来源：http://bfx.ydjk.org.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qjh.tanke756.top

================================================================================
来源：http://opj.hfpthk.cn

L. 网络请求
来源：http://bdh.yj20258.top

================================================================================
来源：http://ntf.ydjk.org.cn

[L01] 发送 GET 请求
来源：http://jgr.fengsongda.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eht.haohaochexian.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gro.zhiwuduotai.top

JS:   await fetch(url)
来源：http://tzc.316326.xyz

TS:   await fetch(url)
来源：http://pzq.tanke756.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ucl.yuxming.cn

Go:   resp, err := http.Get(url)
来源：http://dcz.jinqigufen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qhd.tarul.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://grn.cheryme.top

[L02] 发送 POST JSON
来源：http://azp.daxiang520.top

Py:   requests.post(url, json={"a": 1})
来源：http://ppu.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wgk.sysykeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eiv.guowangkeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ini.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jvp.zdqjudy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gff.hywenlv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qfd.cdnleiting.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mec.tarul.cn

[L03] 设置自定义请求头
来源：http://amc.svipenyu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xod.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wjv.bjfxy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vmk.xinyue.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://roo.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lqh.guowangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xlf.zhijiandao.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gfa.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://grk.haohaochexian.top

[L04] 设置超时
来源：http://cvr.aibaodan.cn

Py:   requests.get(url, timeout=5)
来源：http://ojk.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oka.ybcxt.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qhr.zhixingplan.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ffv.meibo888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qgr.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vkn.jlsjyb.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://meg.daxiang520.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wbw.aizwys.cn

[L05] 上传文件（multipart）
来源：http://bpg.yanxiufei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://omd.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uuf.xziqi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://igd.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vqv.yonumen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://naa.xinyue.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fla.yvedp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://axz.mhx1999.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://icn.zhijiandao.cn

[L06] 解析响应为 JSON
来源：http://fdg.birdmap.top

Py:   resp.json()
来源：http://dlk.aizwys.cn

PHP:  json_decode($body, true);
来源：http://iky.epnwcf.com

JS:   await resp.json()
来源：http://sqx.hfpthk.cn

TS:   await resp.json()
来源：http://esw.xuetiantiany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://afp.hywenlv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fic.sufxvd.cn

Ruby: JSON.parse(resp.body)
来源：http://fjk.iojbl.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pqp.nanxinkj.top

[L07] 处理 HTTP 状态码
来源：http://exc.yj202588.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jmt.hywenlv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pxn.c1oappe.top

JS:   resp.ok;  resp.status
来源：http://bsd.yj202588.top

TS:   resp.ok;  resp.status
来源：http://gby.chenlongwang.top

Java: resp.statusCode()
来源：http://woz.cdnleiting.top

Go:   resp.StatusCode
来源：http://yox.zhoulong.xyz

Ruby: resp.code.to_i
来源：http://kwo.bjfxy.top

C#:   (int)resp.StatusCode
来源：http://dyl.aizwys.cn

[L08] 并发请求多个地址
来源：http://yzg.daxiang520.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vlf.nanxinkj.top

PHP:  curl_multi_init() 系列
来源：http://add.chenjidiqi.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ckp.fehbvm.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vrm.epnwcf.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fik.chenjidiqi.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hom.shanyushiyangtech.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zhi.tarul.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yxs.nwbrower.top

================================================================================
来源：http://jev.hammf.cn

M. 命令行 / 进程 / 环境
来源：http://kxv.yj202588.top

================================================================================
来源：http://rwz.hammf.cn

[M01] 读取命令行参数
来源：http://nfb.zdbjq.cn

Py:   sys.argv[1:]
来源：http://ihf.jinqigfzy.top

PHP:  $argv;  $argc;
来源：http://tnj.xuanzx.com

JS:   process.argv.slice(2)
来源：http://xbk.ybcxt.top

TS:   process.argv.slice(2)
来源：http://ksc.gzhubu.top

Java: args 数组（main 方法参数）
来源：http://ows.hnxiangtu.top

Go:   os.Args[1:]
来源：http://ahd.nwbrower.top

Ruby: ARGV
来源：http://vcz.aibaodan.cn

C#:   args 数组（Main 方法参数）
来源：http://mok.pengpengdd.cyou

[M02] 读取环境变量
来源：http://dzx.tarul.cn

Py:   os.environ.get("HOME")
来源：http://hnf.aibaodan.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aht.redwolf501.top

JS:   process.env.HOME
来源：http://iio.jlsjyb.cn

TS:   process.env.HOME
来源：http://zkp.zhiwuduotai.top

Java: System.getenv("HOME")
来源：http://qwj.guannengcc.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hic.52xcode.cn

Ruby: ENV["HOME"]
来源：http://fev.bbcook.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fur.birdmap.top

[M03] 执行外部命令
来源：http://jpq.xziqi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qce.xziqi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nen.hammf.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://eyy.jianghu66.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xow.hongshengwenyu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eno.xuetiantiany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://juz.hnxiangtu.top

Ruby: system("ls -l");  `ls -l`
来源：http://pot.yuanzhike.top

C#:   Process.Start("ls", "-l");
来源：http://unr.zhoulong.xyz

[M04] 获取当前工作目录
来源：http://ann.9152youxi.cn

Py:   os.getcwd()
来源：http://hhu.snrcjt.cn

PHP:  getcwd();
来源：http://ttx.aibaodan.cn

JS:   process.cwd()
来源：http://xok.bjfxy.top

TS:   process.cwd()
来源：http://zsw.zhijiandao.cn

Java: Path.of("").toAbsolutePath()
来源：http://ffz.bjfxy.top

Go:   os.Getwd()
来源：http://hda.nwbrower.top

Ruby: Dir.pwd
来源：http://rnt.jlsjyb.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mcj.yj20258.top

[M05] 设置退出码
来源：http://ibt.zhiwuduotai.top

Py:   sys.exit(1)
来源：http://hot.hysaishi.cn

PHP:  exit(1);
来源：http://bgz.dashuyun.cn

JS:   process.exit(1)
来源：http://kqf.yangfankeji.com

TS:   process.exit(1)
来源：http://jdn.ydjk.org.cn

Java: System.exit(1)
来源：http://hwe.hysaishi.cn

Go:   os.Exit(1)
来源：http://njk.smart0.xyz

Ruby: exit 1
来源：http://snc.cdnleiting.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tvq.guannengcc.top

[M06] 向标准错误输出
来源：http://xse.cheryme.top

Py:   print("err", file=sys.stderr)
来源：http://ofv.chenjidiqi.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://jje.tarul.cn

JS:   console.error("err")
来源：http://hyl.c1oappe.top

TS:   console.error("err")
来源：http://uzt.birdmap.top

Java: System.err.println("err")
来源：http://wjm.snrcjt.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nfe.ivvv.top

Ruby: warn "err"
来源：http://ijl.bjfxy.top

C#:   Console.Error.WriteLine("err")
来源：http://lea.yonumen.top

[M07] 判断是否为主入口
来源：http://zhg.gzhubu.top

Py:   if __name__ == "__main__":
来源：http://aiy.chenlongwang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tcc.ybcxt.top

JS:   require.main === module
来源：http://wcl.zdqjudy.top

TS:   require.main === module
来源：http://wsq.nanxuanxn.top

Java: public static void main(String[] args)
来源：http://jaa.cdnleiting.top

Go:   func main()
来源：http://pwl.havefunace.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ygr.sufxvd.cn

C#:   static void Main(string[] args)
来源：http://xky.sjlbkw.cn

[M08] 获取系统与运行时信息
来源：http://ano.guowangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://ytq.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://mxd.jinyuanbaomall.cn

JS:   process.platform;  process.version
来源：http://xbt.dianchejie.cn

TS:   process.platform;  process.version
来源：http://xzp.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bry.ydzc1.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://utc.chenzaomai.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dkl.jinqigfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://cpk.gogol.net.cn

================================================================================
来源：http://ayj.hnxiangtu.top

N. 数据结构与算法
来源：http://fod.kuanghao11.cn

================================================================================
来源：http://mfm.zhiwuduotai.top

[N01] 二分查找（有序数组）
来源：http://uge.hnqzz.top

Py:   bisect.bisect_left(arr, x)
来源：http://xes.mhx1999.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pfs.jinyuanbaomall.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ftp.zdqjudy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tis.nwbrower.top

Java: Arrays.binarySearch(arr, x)
来源：http://htp.nanxuanxn.top

Go:   sort.SearchInts(arr, x)
来源：http://baw.yanxiufei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gmu.pycfn.com

C#:   Array.BinarySearch(arr, x)
来源：http://wnq.sysykeji.top

[N02] 排序（工程实践用内置实现）
来源：http://xfu.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://sio.c1oappe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ben.meibo888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://sid.xziqi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pwd.daria6918.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://icp.nanxuanxn.top

Go:   slices.Sort(arr)
来源：http://dfz.hongshengwenyu.top

Ruby: arr.sort
来源：http://hbl.yj202588.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ckf.cashguo.top

[N03] 快速排序（分治示例）
来源：http://hsm.zhengqikj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ajr.zhijiandao.cn

PHP:  // 递归实现，或用 usort
来源：http://jqc.xuanzx.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bis.yuxming.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tnj.xuetiantiany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ryf.meibo888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pag.chenzaomai.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cxb.ehwqpu.com

C#:   // 手写递归，或 Array.Sort
来源：http://mze.quarkkingdee.top

[N04] 斐波那契数列
来源：http://kul.zdbjq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qkf.svipenyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://swf.jianghu66.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lhw.chenlongwang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jbb.yuxming.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gjl.svipenyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qkd.jqgufenzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mjb.zycfv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xyz.shanyushiyangkeji.top

[N05] 最大公约数
来源：http://cjz.birdmap.top

Py:   math.gcd(a, b)
来源：http://hpj.vehdjk.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kdp.xuetiantiany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cyd.snrcjt.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zbr.jinghuilouyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oki.birdmap.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lws.uphjek.com

Ruby: a.gcd(b)
来源：http://aaj.dashuyun.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vug.gaohongyu789.top

[N06] 判断回文字符串
来源：http://jfn.yj202588.top

Py:   s == s[::-1]
来源：http://kbs.sufxvd.cn

PHP:  $s === strrev($s);
来源：http://ler.zhaomingkeji.xyz

JS:   s === [...s].reverse().join("")
来源：http://lje.yonumen.top

TS:   s === [...s].reverse().join("")
来源：http://dbn.gaohongyu789.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eai.fengsongda.top

Go:   // 双指针从两端比较
来源：http://guq.sweek.top

Ruby: s == s.reverse
来源：http://nya.dianchejie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sdv.jinghuilouyu.cn

[N07] 两数之和（返回下标）
来源：http://ass.kuanghao11.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jiv.birdmap.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ios.havefunace.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zuj.redwolf501.top

TS:   // 手写 Map<string, number>
来源：http://qpn.chenjidiqi.icu

Java: // 手写 HashMap
来源：http://rrh.vehdjk.com

Go:   // 手写 map[int]int
来源：http://iar.yj20258.top

Ruby: // 手写 Hash
来源：http://yup.tianlin.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://znb.fehbvm.com

[N08] 生成全排列
来源：http://gkj.havefunace.top

Py:   itertools.permutations(arr)
来源：http://emu.haohaochexian.top

PHP:  // 手写递归交换
来源：http://nzo.snrcjt.cn

JS:   // 手写回溯递归
来源：http://rab.chenlongwang.top

TS:   // 手写回溯递归
来源：http://wdy.jinqigufen.top

Java: // 手写回溯递归
来源：http://okg.smart0.xyz

Go:   // 手写回溯递归
来源：http://lpm.zhixingplan.top

Ruby: arr.permutation.to_a
来源：http://kfr.shangyingyoupin.top

C#:   // 手写回溯递归
来源：http://ydc.aizwys.cn

[N09] 栈与队列
来源：http://zmk.iojbl.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dvg.daria6918.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://shs.shzxlz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hxc.vqdsnc.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sbz.jinyuanbaomall.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uny.yongpay.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hmd.sufxvd.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cpw.hesvh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fmr.0kj1m.cn

[N10] 链表节点定义
来源：http://pbg.zdqjudy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hxj.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qzk.sweek.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gdo.hfpthk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mte.daria6918.cn

Java: class Node { int v; Node next; }
来源：http://tvi.cashguo.top

Go:   type Node struct { V int; Next *Node }
来源：http://vzv.chenjidiqi.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://rsm.zdbjq.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lhk.ehwqpu.com

[N11] 二叉树中序遍历
来源：http://jpr.birdmap.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jng.fengsongda.top

PHP:  // 手写递归函数
来源：http://pmy.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lyi.guannengcc.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lof.ctjpmb.com

Java: // 手写递归
来源：http://ecn.hesvh.cn

Go:   // 手写递归
来源：http://kep.xinyue.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rbp.fanxiaobao.xyz

C#:   // 手写递归
来源：http://fib.meibo888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yzk.9152youxi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://psl.0kj1m.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lmq.kuanghao11.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ddt.dianchejie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://odm.hcnkem.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wda.hnxiangtu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cuw.xingfuxueyuan.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://amm.xuanzx.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mue.jianghu66.top

================================================================================
来源：http://zfh.ehwqpu.com

O. 并发与异步
来源：http://bob.jinqigufen.top

================================================================================
来源：http://vil.redwolf501.top

[O01] 启动一个线程
来源：http://dyg.hysaishi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hlh.yuanzhike.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://syk.quarkkingdee.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ntk.c1oappe.top

TS:   // 同 JS
来源：http://fqg.guannengcc.top

Java: new Thread(() -> f()).start()
来源：http://hwi.sufxvd.cn

Go:   go f()
来源：http://jge.jinghuilouyu.cn

Ruby: Thread.new { f }
来源：http://mfp.hysaishi.cn

C#:   Task.Run(() => F());
来源：http://xzp.wangdashe.top

[O02] 使用线程池
来源：http://ltr.gzhubu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ayt.uphjek.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qfs.fzhhl.top

JS:   // worker_threads 线程池
来源：http://zkd.bbcook.cn

TS:   // worker_threads 线程池
来源：http://sxc.chenzaomai.com

Java: Executors.newFixedThreadPool(4)
来源：http://ybi.sjlbkw.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fsh.wangshuangyany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tix.hnqzz.top


<!-- 参考信息 -->