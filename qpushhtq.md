代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://osa.jinqigufen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nqx.cdnleiting.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://yed.nanxuanxn.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ykv.hysaishi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uoy.jlsjyb.cn

[K07] 进制转换
来源：http://bdc.aizwys.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vzf.zhijiandao.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mhs.aizwys.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kpv.jqgufenzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tcm.ehwqpu.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xfs.yongpay.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gyf.hfpthk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uqk.yanxiufei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://huw.pycfn.com

[K08] 二进制序列化（非 JSON）
来源：http://ilb.zhijiandao.cn

Py:   pickle.dumps(obj)
来源：http://gjl.52xcode.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nqw.yuxming.cn

JS:   v8.serialize(obj)        // Node
来源：http://qhg.gzhubu.top

TS:   v8.serialize(obj)        // Node
来源：http://bet.jyoumei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ibw.ydjk.org.cn

Go:   encoding/gob
来源：http://ajh.zdqjudy.top

Ruby: Marshal.dump(obj)
来源：http://rpw.zdbjq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fbs.zdbjq.cn

================================================================================
来源：http://iyk.ivvv.top

L. 网络请求
来源：http://wvl.yj20258888.top

================================================================================
来源：http://uwh.shanyushiyangtech.top

[L01] 发送 GET 请求
来源：http://hrk.aizwys.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mqf.havefunace.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wvg.wangdashe.top

JS:   await fetch(url)
来源：http://nvs.epnwcf.com

TS:   await fetch(url)
来源：http://eqt.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jzm.gotoacloud.top

Go:   resp, err := http.Get(url)
来源：http://hfr.yvedp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pib.snrcjt.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vae.xylfe.cn

[L02] 发送 POST JSON
来源：http://xfu.shanyushiyangtech.top

Py:   requests.post(url, json={"a": 1})
来源：http://xgr.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ysq.ydjk.org.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://avi.jinqigufen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cnr.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://asp.hnqzz.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://svi.nanxinkj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oal.yanxiufei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dsn.wangshuangyany.cn

[L03] 设置自定义请求头
来源：http://wrp.wangshuangyany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nrx.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iic.jianghu66.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tfq.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bfp.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hje.xziqi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jga.jinqigfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tpu.cdnleiting.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kjk.shangyingyoupin.top

[L04] 设置超时
来源：http://dlj.gogol.net.cn

Py:   requests.get(url, timeout=5)
来源：http://htq.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mwj.hongshengwenyu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lru.zhaomingkeji.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ref.sweek.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://don.yuxming.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bki.sufxvd.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wpn.yanxiufei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dhu.tarul.cn

[L05] 上传文件（multipart）
来源：http://qge.sxryk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fia.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tfe.cqqwz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pih.zhengqikj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://atr.zhoulong.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zlu.jinqigfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zbq.smart0.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eht.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uiw.cucudq.cn

[L06] 解析响应为 JSON
来源：http://ayn.ivvv.top

Py:   resp.json()
来源：http://gfv.tanke756.top

PHP:  json_decode($body, true);
来源：http://zls.xylfe.cn

JS:   await resp.json()
来源：http://xnm.xylfe.cn

TS:   await resp.json()
来源：http://zsq.9152youxi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lmp.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blb.ydzc1.top

Ruby: JSON.parse(resp.body)
来源：http://emn.jqgfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nyv.vehdjk.com

[L07] 处理 HTTP 状态码
来源：http://let.jqgufenzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qtk.dianchejie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ebx.birdmap.top

JS:   resp.ok;  resp.status
来源：http://xhn.jiagoushi.top

TS:   resp.ok;  resp.status
来源：http://okc.yuxming.cn

Java: resp.statusCode()
来源：http://oxz.yj20258.top

Go:   resp.StatusCode
来源：http://hlh.yanxiufei.cn

Ruby: resp.code.to_i
来源：http://jgm.chenjidiqi.icu

C#:   (int)resp.StatusCode
来源：http://efr.yuxming.cn

[L08] 并发请求多个地址
来源：http://dbm.gogol.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zlo.nwbrower.top

PHP:  curl_multi_init() 系列
来源：http://jlw.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dgg.yj202588.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ahz.fzhhl.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uzr.hongshengwenyu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ywf.iojbl.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rhr.daria6918.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qzi.xinyue.icu

================================================================================
来源：http://oib.zhongyouzk.top

M. 命令行 / 进程 / 环境
来源：http://udf.wangshuangyany.cn

================================================================================
来源：http://ejr.yj20258888.top

[M01] 读取命令行参数
来源：http://ywn.hcnkem.com

Py:   sys.argv[1:]
来源：http://zdj.kuanghao11.cn

PHP:  $argv;  $argc;
来源：http://gdt.cucudq.cn

JS:   process.argv.slice(2)
来源：http://vpl.zhijiandao.cn

TS:   process.argv.slice(2)
来源：http://ikz.tian-w.cn

Java: args 数组（main 方法参数）
来源：http://gaj.gogol.net.cn

Go:   os.Args[1:]
来源：http://uox.tian-w.cn

Ruby: ARGV
来源：http://dvp.hywenlv.cn

C#:   args 数组（Main 方法参数）
来源：http://hcn.nwbrower.top

[M02] 读取环境变量
来源：http://udc.nwbrower.top

Py:   os.environ.get("HOME")
来源：http://jci.ppjwa.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://adr.havefunace.top

JS:   process.env.HOME
来源：http://cpm.redwolf501.top

TS:   process.env.HOME
来源：http://jrf.fktsv.cn

Java: System.getenv("HOME")
来源：http://poi.cucudq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nwt.ydzc1.top

Ruby: ENV["HOME"]
来源：http://vwh.gotoacloud.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nfy.bbcook.cn

[M03] 执行外部命令
来源：http://yhe.chenlongwang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jmv.sweek.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rdk.zhiwuduotai.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vew.nanxinkj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qaq.gaohongyu789.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://isz.cdnleiting.top

Go:   exec.Command("ls", "-l").Output()
来源：http://web.quarkkingdee.top

Ruby: system("ls -l");  `ls -l`
来源：http://dpk.jinghuilouyu.cn

C#:   Process.Start("ls", "-l");
来源：http://dkg.sxryk.cn

[M04] 获取当前工作目录
来源：http://cvt.yj20258888.top

Py:   os.getcwd()
来源：http://fub.sxryk.cn

PHP:  getcwd();
来源：http://vdg.cheryme.top

JS:   process.cwd()
来源：http://son.zhiwuduotai.top

TS:   process.cwd()
来源：http://jum.bbcook.cn

Java: Path.of("").toAbsolutePath()
来源：http://epv.dianchejie.cn

Go:   os.Getwd()
来源：http://cil.fengsongda.top

Ruby: Dir.pwd
来源：http://frw.shanyushiyangtech.top

C#:   Directory.GetCurrentDirectory()
来源：http://vxo.yangfankeji.com

[M05] 设置退出码
来源：http://xmz.haohaochexian.top

Py:   sys.exit(1)
来源：http://rfo.shanyushiyangtech.top

PHP:  exit(1);
来源：http://huy.jqgfzy.top

JS:   process.exit(1)
来源：http://krm.yonumen.top

TS:   process.exit(1)
来源：http://dsr.xylfe.cn

Java: System.exit(1)
来源：http://wsu.andypj.xyz

Go:   os.Exit(1)
来源：http://caz.yongpay.top

Ruby: exit 1
来源：http://get.sweek.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vmg.hysaishi.cn

[M06] 向标准错误输出
来源：http://lcu.guowangkeji.top

Py:   print("err", file=sys.stderr)
来源：http://ndg.ctjpmb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://fvj.feifeiyinyue.top

JS:   console.error("err")
来源：http://sbz.bbcook.cn

TS:   console.error("err")
来源：http://hhn.tarul.cn

Java: System.err.println("err")
来源：http://ahu.zhixingplan.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xqa.xylfe.cn

Ruby: warn "err"
来源：http://orl.snrcjt.cn

C#:   Console.Error.WriteLine("err")
来源：http://nsh.nwbrower.top

[M07] 判断是否为主入口
来源：http://oon.cqqwz.cn

Py:   if __name__ == "__main__":
来源：http://wqb.shanyushiyangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hpg.shuidangran.top

JS:   require.main === module
来源：http://fhp.yongpay.top

TS:   require.main === module
来源：http://jbz.daxiang520.top

Java: public static void main(String[] args)
来源：http://xcs.jqgufenzy.top

Go:   func main()
来源：http://wbm.cqqwz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kzd.xziqi.cn

C#:   static void Main(string[] args)
来源：http://zwi.aibaodan.cn

[M08] 获取系统与运行时信息
来源：http://phk.hammf.cn

Py:   platform.system();  platform.python_version()
来源：http://etn.jqgufenzy.top

PHP:  PHP_OS;  phpversion();
来源：http://hhj.52xcode.cn

JS:   process.platform;  process.version
来源：http://agc.ehwqpu.com

TS:   process.platform;  process.version
来源：http://nzo.zhiwuduotai.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mqt.cdnleiting.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gfc.gotoacloud.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://efe.redwolf501.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vmu.cqqwz.cn

================================================================================
来源：http://bki.52xcode.cn

N. 数据结构与算法
来源：http://bwy.yj20258888.top

================================================================================
来源：http://vea.hesvh.cn

[N01] 二分查找（有序数组）
来源：http://hoi.yj20258888.top

Py:   bisect.bisect_left(arr, x)
来源：http://ydk.yj20258888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dqw.jinyuanbaomall.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mub.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tlj.jinqigufen.top

Java: Arrays.binarySearch(arr, x)
来源：http://lut.yj20258888.top

Go:   sort.SearchInts(arr, x)
来源：http://xqx.ywan-chungtsiang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hfq.sysykeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://cml.zhongyouzk.top

[N02] 排序（工程实践用内置实现）
来源：http://sfy.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://rxg.cqqwz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ohz.zhoulong.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://gfe.pengpengdd.cyou

TS:   [...arr].sort((a, b) => a - b)
来源：http://tie.birdmap.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://asn.mhx1999.top

Go:   slices.Sort(arr)
来源：http://cak.zhongyouzk.top

Ruby: arr.sort
来源：http://emt.xuanzx.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://kex.hesvh.cn

[N03] 快速排序（分治示例）
来源：http://uhy.feifeiyinyue.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nwy.jianghu66.top

PHP:  // 递归实现，或用 usort
来源：http://hnx.zycfv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xgk.ydzc1.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fvt.ivvv.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kdy.pycfn.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qja.hesvh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wgx.smart0.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://moc.xziqi.cn

[N04] 斐波那契数列
来源：http://qrc.smart0.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://emr.jinghuilouyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://spx.haohaochexian.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jqh.52xcode.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://plr.nanxuanxn.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dar.zdqjudy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fvn.gzhubu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://heb.yj202588.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ord.daxiang520.top

[N05] 最大公约数
来源：http://rla.shzxlz.cn

Py:   math.gcd(a, b)
来源：http://xhl.ydjk.org.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rzq.aizwys.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xnl.hfpthk.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hyd.shuidangran.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eaz.meibo888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jve.jiagoushi.top

Ruby: a.gcd(b)
来源：http://mry.jinghuilouyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mwm.yueranfly.top

[N06] 判断回文字符串
来源：http://juz.mhx1999.top

Py:   s == s[::-1]
来源：http://cgx.sweek.top

PHP:  $s === strrev($s);
来源：http://mif.zdbjq.cn

JS:   s === [...s].reverse().join("")
来源：http://cbm.ehwqpu.com

TS:   s === [...s].reverse().join("")
来源：http://vsn.jinqigufen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vdy.jianghu66.top

Go:   // 双指针从两端比较
来源：http://xag.shanyushiyangtech.top

Ruby: s == s.reverse
来源：http://dqr.ehwqpu.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://ybs.iojbl.cn

[N07] 两数之和（返回下标）
来源：http://den.wangshuangyany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mvu.zdbjq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wtc.c1oappe.top

JS:   // 手写 Map：map.set(v, i)
来源：http://uwu.zdbjq.cn

TS:   // 手写 Map<string, number>
来源：http://dtl.jyoumei.cn

Java: // 手写 HashMap
来源：http://vro.vehdjk.com

Go:   // 手写 map[int]int
来源：http://cnw.yj202588.top

Ruby: // 手写 Hash
来源：http://pdf.zhongyouzk.top

C#:   // 手写 Dictionary<int, int>
来源：http://dir.andypj.xyz

[N08] 生成全排列
来源：http://amm.bbcook.cn

Py:   itertools.permutations(arr)
来源：http://ytg.feifeiyinyue.top

PHP:  // 手写递归交换
来源：http://ely.meibo888.top

JS:   // 手写回溯递归
来源：http://vcv.zhengqikj.top

TS:   // 手写回溯递归
来源：http://ghl.wangdashe.top

Java: // 手写回溯递归
来源：http://fhs.jlsjyb.cn

Go:   // 手写回溯递归
来源：http://gta.hesvh.cn

Ruby: arr.permutation.to_a
来源：http://ivx.havefunace.top

C#:   // 手写回溯递归
来源：http://znd.yj202588.top

[N09] 栈与队列
来源：http://vpv.wangdashe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tgt.ctjpmb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gzm.hysaishi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dun.yanxiufei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ibv.andypj.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ney.zhixingplan.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://opu.jqgufenzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fed.ydjk.org.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wum.ppjwa.cn

[N10] 链表节点定义
来源：http://twz.ctjpmb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uyz.daria6918.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ezi.yangfankeji.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://klm.zhaomingkeji.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lhv.tian-w.cn

Java: class Node { int v; Node next; }
来源：http://vnd.sysykeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://gwc.yueranfly.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dqz.jinqigfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bdx.xylfe.cn

[N11] 二叉树中序遍历
来源：http://rwj.jinqigfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://axh.sxryk.cn

PHP:  // 手写递归函数
来源：http://vsr.aibaodan.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://geq.hfpthk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yxz.jinqigfzy.top

Java: // 手写递归
来源：http://xlu.jiagoushi.top

Go:   // 手写递归
来源：http://nkp.jinyuanbaomall.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yqr.smart0.xyz

C#:   // 手写递归
来源：http://fki.haohaochexian.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yij.shzxlz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pqj.hnxiangtu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uyb.hammf.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rjg.yanxiufei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hbu.shanyushiyangtech.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://klx.shzxlz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yyl.andypj.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zsd.zhongyouzk.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kei.gogol.net.cn

================================================================================
来源：http://tdr.tian-w.cn

O. 并发与异步
来源：http://vdr.hfpthk.cn

================================================================================
来源：http://vcu.cashguo.top

[O01] 启动一个线程
来源：http://muv.dashuyun.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xgw.hnqzz.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://per.guannengcc.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://duh.mhx1999.top

TS:   // 同 JS
来源：http://nvi.cqqwz.cn

Java: new Thread(() -> f()).start()
来源：http://kks.ivvv.top

Go:   go f()
来源：http://wxn.daria6918.cn

Ruby: Thread.new { f }
来源：http://tvm.ppjwa.cn

C#:   Task.Run(() => F());
来源：http://jzn.feifeiyinyue.top

[O02] 使用线程池
来源：http://thl.zdbjq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eqs.fktsv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qnd.nanxinkj.top

JS:   // worker_threads 线程池
来源：http://zxs.c1oappe.top


<!-- 参考信息 -->