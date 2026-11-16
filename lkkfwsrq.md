代发 wailian999

[K06] 解析 URL 查询串
来源：http://bve.hfpthk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vdc.tianlin.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://prv.cashguo.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://twl.wangshuangyany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gvk.sufxvd.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pua.yuanzhike.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qhb.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lpt.smart0.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://aso.daria6918.cn

[K07] 进制转换
来源：http://nnb.fengsongda.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rwo.gaohongyu789.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kjl.hfpthk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vtv.redwolf501.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ffb.fengsongda.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xak.yuanzhike.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://msg.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qrg.jqgfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://btu.pycfn.com

[K08] 二进制序列化（非 JSON）
来源：http://uve.hfpthk.cn

Py:   pickle.dumps(obj)
来源：http://gek.aizwys.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pfn.sjlbkw.cn

JS:   v8.serialize(obj)        // Node
来源：http://els.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://typ.meibo888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jsx.zhengqikj.top

Go:   encoding/gob
来源：http://ryg.yj20258888.top

Ruby: Marshal.dump(obj)
来源：http://aoj.wangdashe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://afd.yueranfly.top

================================================================================
来源：http://qep.gotoacloud.top

L. 网络请求
来源：http://fpy.hammf.cn

================================================================================
来源：http://syj.xziqi.cn

[L01] 发送 GET 请求
来源：http://xtz.guannengcc.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qlt.hesvh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://brg.sufxvd.cn

JS:   await fetch(url)
来源：http://cpx.shanyushiyangtech.top

TS:   await fetch(url)
来源：http://kpf.cqqwz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uob.cdnleiting.top

Go:   resp, err := http.Get(url)
来源：http://rlg.aibaodan.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xnj.vehdjk.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mfi.ivvv.top

[L02] 发送 POST JSON
来源：http://ioy.ydzc1.top

Py:   requests.post(url, json={"a": 1})
来源：http://dqi.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nyw.gotoacloud.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bzq.hongshengwenyu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qky.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uvn.hfpthk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fuo.vqdsnc.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xov.wangdashe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ykn.yuanzhike.top

[L03] 设置自定义请求头
来源：http://nel.yangfankeji.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uic.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://atk.0kj1m.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gys.zhaomingkeji.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gkt.jiagoushi.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lwq.0kj1m.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gem.daria6918.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jyf.ctjpmb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://akc.dianchejie.cn

[L04] 设置超时
来源：http://wkl.iojbl.cn

Py:   requests.get(url, timeout=5)
来源：http://juu.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://htq.xingfuxueyuan.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oph.xingfuxueyuan.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ukp.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iwq.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cmr.fehbvm.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://efv.ybcxt.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pao.ctjpmb.com

[L05] 上传文件（multipart）
来源：http://kav.zdbjq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tum.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nkx.ybcxt.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qtu.xinyue.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xjl.jlsjyb.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fzu.aizwys.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vgm.sxryk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://egj.zhoulong.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ntw.c1oappe.top

[L06] 解析响应为 JSON
来源：http://pqh.xuanzx.com

Py:   resp.json()
来源：http://ani.dianchejie.cn

PHP:  json_decode($body, true);
来源：http://trc.tarul.cn

JS:   await resp.json()
来源：http://jig.sxryk.cn

TS:   await resp.json()
来源：http://bti.yj202588.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tpm.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ken.daxiang520.top

Ruby: JSON.parse(resp.body)
来源：http://xqj.smart0.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://otc.vehdjk.com

[L07] 处理 HTTP 状态码
来源：http://pio.hysaishi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://liv.yuxming.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xnv.ehwqpu.com

JS:   resp.ok;  resp.status
来源：http://xwy.zhoulong.xyz

TS:   resp.ok;  resp.status
来源：http://uzs.feifeiyinyue.top

Java: resp.statusCode()
来源：http://frl.zdbjq.cn

Go:   resp.StatusCode
来源：http://wsx.havefunace.top

Ruby: resp.code.to_i
来源：http://tww.nwbrower.top

C#:   (int)resp.StatusCode
来源：http://rza.jinyuanbaomall.cn

[L08] 并发请求多个地址
来源：http://gnw.zhongyouzk.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fth.316326.xyz

PHP:  curl_multi_init() 系列
来源：http://bau.hcnkem.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ycr.yuxming.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://axq.ybcxt.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jkr.hammf.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bmq.shanyushiyangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zmf.yj202588.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://myr.9152youxi.cn

================================================================================
来源：http://ych.ywan-chungtsiang.top

M. 命令行 / 进程 / 环境
来源：http://djv.svipenyu.cn

================================================================================
来源：http://raq.ybcxt.top

[M01] 读取命令行参数
来源：http://wyx.tianlin.xyz

Py:   sys.argv[1:]
来源：http://mtk.fengsongda.top

PHP:  $argv;  $argc;
来源：http://bam.hnqzz.top

JS:   process.argv.slice(2)
来源：http://soq.hywenlv.cn

TS:   process.argv.slice(2)
来源：http://gxo.chenjidiqi.icu

Java: args 数组（main 方法参数）
来源：http://pea.ivvv.top

Go:   os.Args[1:]
来源：http://exl.ydjk.org.cn

Ruby: ARGV
来源：http://vqv.zdqjudy.top

C#:   args 数组（Main 方法参数）
来源：http://dec.hysaishi.cn

[M02] 读取环境变量
来源：http://tfx.cheryme.top

Py:   os.environ.get("HOME")
来源：http://sht.tianlin.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hhd.yangfankeji.com

JS:   process.env.HOME
来源：http://iwz.gotoacloud.top

TS:   process.env.HOME
来源：http://lvm.dashuyun.cn

Java: System.getenv("HOME")
来源：http://dpw.hammf.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tlo.hesvh.cn

Ruby: ENV["HOME"]
来源：http://aua.52xcode.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wsz.ydzc1.top

[M03] 执行外部命令
来源：http://dng.vqdsnc.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zbf.hywenlv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zjt.ivvv.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ard.ivvv.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jkn.chenlongwang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ohf.jinqigfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kdy.cheryme.top

Ruby: system("ls -l");  `ls -l`
来源：http://ywc.redwolf501.top

C#:   Process.Start("ls", "-l");
来源：http://nry.shzxlz.cn

[M04] 获取当前工作目录
来源：http://flf.chenzaomai.com

Py:   os.getcwd()
来源：http://qdv.hammf.cn

PHP:  getcwd();
来源：http://tmk.snrcjt.cn

JS:   process.cwd()
来源：http://uog.yueranfly.top

TS:   process.cwd()
来源：http://kky.haohaochexian.top

Java: Path.of("").toAbsolutePath()
来源：http://dif.jinqigfzy.top

Go:   os.Getwd()
来源：http://tvf.yuxming.cn

Ruby: Dir.pwd
来源：http://bjh.fehbvm.com

C#:   Directory.GetCurrentDirectory()
来源：http://iod.gzhubu.top

[M05] 设置退出码
来源：http://ahg.zhixingplan.top

Py:   sys.exit(1)
来源：http://lgh.shuidangran.top

PHP:  exit(1);
来源：http://zdu.zhaomingkeji.xyz

JS:   process.exit(1)
来源：http://hem.fanxiaobao.xyz

TS:   process.exit(1)
来源：http://kcu.yuanzhike.top

Java: System.exit(1)
来源：http://bcw.aibaodan.cn

Go:   os.Exit(1)
来源：http://mzi.hongshengwenyu.top

Ruby: exit 1
来源：http://lud.xylfe.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ior.daxiang520.top

[M06] 向标准错误输出
来源：http://gbx.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://acc.tanke756.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bij.birdmap.top

JS:   console.error("err")
来源：http://fnq.cdnleiting.top

TS:   console.error("err")
来源：http://pnm.fktsv.cn

Java: System.err.println("err")
来源：http://jbh.gaohongyu789.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zim.hnqzz.top

Ruby: warn "err"
来源：http://ftm.zhaomingkeji.xyz

C#:   Console.Error.WriteLine("err")
来源：http://svh.shanyushiyangkeji.top

[M07] 判断是否为主入口
来源：http://jyl.jqgfzy.top

Py:   if __name__ == "__main__":
来源：http://rre.chenlongwang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lam.sweek.top

JS:   require.main === module
来源：http://txc.yueranfly.top

TS:   require.main === module
来源：http://hsq.quarkkingdee.top

Java: public static void main(String[] args)
来源：http://giv.guowangkeji.top

Go:   func main()
来源：http://bol.mhx1999.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vlx.cashguo.top

C#:   static void Main(string[] args)
来源：http://zhc.vqdsnc.cn

[M08] 获取系统与运行时信息
来源：http://efi.nanxinkj.top

Py:   platform.system();  platform.python_version()
来源：http://oax.dashuyun.cn

PHP:  PHP_OS;  phpversion();
来源：http://bzu.zhaomingkeji.xyz

JS:   process.platform;  process.version
来源：http://pzf.ywan-chungtsiang.top

TS:   process.platform;  process.version
来源：http://nji.jyoumei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://url.zdbjq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vje.yuxming.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vdy.svipenyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gdp.xylfe.cn

================================================================================
来源：http://xsb.9152youxi.cn

N. 数据结构与算法
来源：http://mpa.tarul.cn

================================================================================
来源：http://hph.jinqigfzy.top

[N01] 二分查找（有序数组）
来源：http://lxs.hnxiangtu.top

Py:   bisect.bisect_left(arr, x)
来源：http://spo.hcnkem.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zjm.daria6918.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://stj.bjfxy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tfc.pycfn.com

Java: Arrays.binarySearch(arr, x)
来源：http://mdm.mhx1999.top

Go:   sort.SearchInts(arr, x)
来源：http://ubm.yuanzhike.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ymi.jyoumei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vwq.c1oappe.top

[N02] 排序（工程实践用内置实现）
来源：http://onq.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://ame.shangyingyoupin.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://agy.zhoulong.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://afe.bjfxy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wbs.mhx1999.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://skb.aizwys.cn

Go:   slices.Sort(arr)
来源：http://dcd.wangdashe.top

Ruby: arr.sort
来源：http://fye.yuanzhike.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vvk.dashuyun.cn

[N03] 快速排序（分治示例）
来源：http://buq.snrcjt.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://web.gaohongyu789.top

PHP:  // 递归实现，或用 usort
来源：http://bsa.svipenyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hau.nanxinkj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kcp.c1oappe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ltz.xuanzx.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ibe.zhoulong.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uts.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://ufh.jinyuanbaomall.cn

[N04] 斐波那契数列
来源：http://jua.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vhv.gaohongyu789.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vgl.shanyushiyangtech.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bqx.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rla.yj202588.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jhd.pengpengdd.cyou

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kpr.tarul.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fox.havefunace.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rgm.cdnleiting.top

[N05] 最大公约数
来源：http://ted.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://rhk.zhongyouzk.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ucy.sufxvd.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pmm.gaohongyu789.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ckz.kuanghao11.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cvy.shangyingyoupin.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oyq.yvedp.cn

Ruby: a.gcd(b)
来源：http://dfa.sweek.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fyf.ydjk.org.cn

[N06] 判断回文字符串
来源：http://uyu.tanke756.top

Py:   s == s[::-1]
来源：http://feo.ivvv.top

PHP:  $s === strrev($s);
来源：http://eep.zhengqikj.top

JS:   s === [...s].reverse().join("")
来源：http://qtv.hammf.cn

TS:   s === [...s].reverse().join("")
来源：http://aqe.fengsongda.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gbu.uphjek.com

Go:   // 双指针从两端比较
来源：http://xii.smart0.xyz

Ruby: s == s.reverse
来源：http://ewc.jlsjyb.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vmw.ydjk.org.cn

[N07] 两数之和（返回下标）
来源：http://alh.zhengqikj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://twm.gzhubu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://awk.uphjek.com

JS:   // 手写 Map：map.set(v, i)
来源：http://jqj.hywenlv.cn

TS:   // 手写 Map<string, number>
来源：http://lcw.gzhubu.top

Java: // 手写 HashMap
来源：http://iff.ywan-chungtsiang.top

Go:   // 手写 map[int]int
来源：http://ghc.sjlbkw.cn

Ruby: // 手写 Hash
来源：http://rwa.zhengqikj.top

C#:   // 手写 Dictionary<int, int>
来源：http://icj.0kj1m.cn

[N08] 生成全排列
来源：http://tmv.quarkkingdee.top

Py:   itertools.permutations(arr)
来源：http://uxl.yuanzhike.top

PHP:  // 手写递归交换
来源：http://qxy.mhx1999.top

JS:   // 手写回溯递归
来源：http://uyr.mhx1999.top

TS:   // 手写回溯递归
来源：http://yvj.fktsv.cn

Java: // 手写回溯递归
来源：http://ydp.svipenyu.cn

Go:   // 手写回溯递归
来源：http://wbc.hfpthk.cn

Ruby: arr.permutation.to_a
来源：http://zoy.cheryme.top

C#:   // 手写回溯递归
来源：http://bjh.xylfe.cn

[N09] 栈与队列
来源：http://hab.chenzaomai.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bzc.jinyuanbaomall.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://seq.yuanzhike.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dch.yanxiufei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://coa.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ohe.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xyj.hesvh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eaa.gaohongyu789.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uku.iojbl.cn

[N10] 链表节点定义
来源：http://rwu.hnxiangtu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uta.cheryme.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wdu.cqqwz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wed.daxiang520.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ovt.sweek.top

Java: class Node { int v; Node next; }
来源：http://gqa.pycfn.com

Go:   type Node struct { V int; Next *Node }
来源：http://siv.shanyushiyangtech.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ytd.fehbvm.com

C#:   class Node { public int V; public Node? Next; }
来源：http://fan.gzhubu.top

[N11] 二叉树中序遍历
来源：http://xlt.ehwqpu.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://axe.yongpay.top

PHP:  // 手写递归函数
来源：http://xcn.yuanzhike.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bcl.xylfe.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qqa.jinghuilouyu.cn

Java: // 手写递归
来源：http://dzc.ctjpmb.com

Go:   // 手写递归
来源：http://jtx.sufxvd.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wqe.xylfe.cn

C#:   // 手写递归
来源：http://blp.xylfe.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ofr.bjfxy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ljz.zhoulong.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pow.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fxf.yvedp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vgj.pycfn.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pcw.mhx1999.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://poz.sjlbkw.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wnr.hammf.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yeo.birdmap.top

================================================================================
来源：http://kqq.jinqigfzy.top

O. 并发与异步
来源：http://urb.jinyuanbaomall.cn

================================================================================
来源：http://jjz.svipenyu.cn

[O01] 启动一个线程
来源：http://mla.chenzaomai.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cyv.zhoulong.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://grg.kuanghao11.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fhh.wangshuangyany.cn

TS:   // 同 JS
来源：http://xac.vehdjk.com

Java: new Thread(() -> f()).start()
来源：http://zcu.daxiang520.top

Go:   go f()
来源：http://scc.nwbrower.top

Ruby: Thread.new { f }
来源：http://iul.yj20258.top

C#:   Task.Run(() => F());
来源：http://brg.redwolf501.top


<!-- 参考信息 -->