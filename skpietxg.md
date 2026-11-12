代发 wailian999

[K06] 解析 URL 查询串
来源：http://dpr.tianlin.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hzk.daria6918.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lob.smart0.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ltc.zhengqikj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rmg.jqgufenzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rkb.jinyuanbaomall.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bxd.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kkp.zhiwuduotai.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sjs.andypj.xyz

[K07] 进制转换
来源：http://eag.jyoumei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cpb.jyoumei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xjy.zhaomingkeji.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uzn.xuanzx.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dql.yonumen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ofd.chenjidiqi.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://exz.snrcjt.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kra.xinyue.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://obr.jinqigufen.top

[K08] 二进制序列化（非 JSON）
来源：http://vov.pycfn.com

Py:   pickle.dumps(obj)
来源：http://hqz.vqdsnc.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qkv.jyoumei.cn

JS:   v8.serialize(obj)        // Node
来源：http://aju.sufxvd.cn

TS:   v8.serialize(obj)        // Node
来源：http://okz.cheryme.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qom.xziqi.cn

Go:   encoding/gob
来源：http://ccd.yj202588.top

Ruby: Marshal.dump(obj)
来源：http://tju.daria6918.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hzb.cdnleiting.top

================================================================================
来源：http://eei.havefunace.top

L. 网络请求
来源：http://jye.daria6918.cn

================================================================================
来源：http://ruv.zdqjudy.top

[L01] 发送 GET 请求
来源：http://lzv.zhaomingkeji.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nxm.ydjk.org.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nqx.ppjwa.cn

JS:   await fetch(url)
来源：http://eke.snrcjt.cn

TS:   await fetch(url)
来源：http://luk.wangdashe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fnh.aizwys.cn

Go:   resp, err := http.Get(url)
来源：http://qlv.jqgufenzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fld.vehdjk.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oae.pycfn.com

[L02] 发送 POST JSON
来源：http://mvr.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dqc.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uny.cucudq.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://seu.birdmap.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rrs.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://agc.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://num.zdqjudy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tbo.jianghu66.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vix.fengsongda.top

[L03] 设置自定义请求头
来源：http://xag.sxryk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oeq.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rnt.yvedp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cxk.cdnleiting.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zcu.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wes.guannengcc.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hfh.yueranfly.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nzw.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kyv.ctjpmb.com

[L04] 设置超时
来源：http://lzm.sufxvd.cn

Py:   requests.get(url, timeout=5)
来源：http://sqj.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aht.xinyue.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jfi.bjfxy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dwk.shuidangran.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ews.bjfxy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zwd.haohaochexian.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pxj.mhx1999.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://adc.ehwqpu.com

[L05] 上传文件（multipart）
来源：http://hle.uphjek.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vvb.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://diu.yuanzhike.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kbc.hnqzz.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ubd.wangshuangyany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fwe.sufxvd.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rrn.hfpthk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tjh.hongshengwenyu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://alz.shanyushiyangtech.top

[L06] 解析响应为 JSON
来源：http://qka.yvedp.cn

Py:   resp.json()
来源：http://ktb.daxiang520.top

PHP:  json_decode($body, true);
来源：http://vij.svipenyu.cn

JS:   await resp.json()
来源：http://kgi.mhx1999.top

TS:   await resp.json()
来源：http://wob.zhoulong.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uqu.yangfankeji.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vsp.vqdsnc.cn

Ruby: JSON.parse(resp.body)
来源：http://kkv.feifeiyinyue.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://atw.gaohongyu789.top

[L07] 处理 HTTP 状态码
来源：http://oqu.bbcook.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://agy.hcnkem.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hnc.fktsv.cn

JS:   resp.ok;  resp.status
来源：http://cjq.shangyingyoupin.top

TS:   resp.ok;  resp.status
来源：http://qkj.hcnkem.com

Java: resp.statusCode()
来源：http://lnj.birdmap.top

Go:   resp.StatusCode
来源：http://uoy.redwolf501.top

Ruby: resp.code.to_i
来源：http://qzh.316326.xyz

C#:   (int)resp.StatusCode
来源：http://lui.chenzaomai.com

[L08] 并发请求多个地址
来源：http://lwb.shangyingyoupin.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rus.dashuyun.cn

PHP:  curl_multi_init() 系列
来源：http://gjf.yvedp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://imi.jinqigufen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://che.yonumen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vpm.uphjek.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://arw.shanyushiyangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://isu.sweek.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yqc.fktsv.cn

================================================================================
来源：http://gfh.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境
来源：http://fgk.yanxiufei.cn

================================================================================
来源：http://dzb.tian-w.cn

[M01] 读取命令行参数
来源：http://ila.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://vqi.zhijiandao.cn

PHP:  $argv;  $argc;
来源：http://zuv.zhongyouzk.top

JS:   process.argv.slice(2)
来源：http://abh.fehbvm.com

TS:   process.argv.slice(2)
来源：http://fvs.9152youxi.cn

Java: args 数组（main 方法参数）
来源：http://bmz.daxiang520.top

Go:   os.Args[1:]
来源：http://vls.pycfn.com

Ruby: ARGV
来源：http://phk.dianchejie.cn

C#:   args 数组（Main 方法参数）
来源：http://pkq.shuidangran.top

[M02] 读取环境变量
来源：http://zey.nwbrower.top

Py:   os.environ.get("HOME")
来源：http://khx.nanxinkj.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sap.daxiang520.top

JS:   process.env.HOME
来源：http://qix.hesvh.cn

TS:   process.env.HOME
来源：http://zya.snrcjt.cn

Java: System.getenv("HOME")
来源：http://umo.shangyingyoupin.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ulo.hesvh.cn

Ruby: ENV["HOME"]
来源：http://sww.yvedp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vlv.jiagoushi.top

[M03] 执行外部命令
来源：http://juf.xziqi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gpd.jianghu66.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oue.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sml.hnxiangtu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://pli.bbcook.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yzs.zhoulong.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://fvd.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pme.hfpthk.cn

C#:   Process.Start("ls", "-l");
来源：http://bsk.iojbl.cn

[M04] 获取当前工作目录
来源：http://knj.jqgufenzy.top

Py:   os.getcwd()
来源：http://got.jianghu66.top

PHP:  getcwd();
来源：http://pzh.zhaomingkeji.xyz

JS:   process.cwd()
来源：http://ijq.gzhubu.top

TS:   process.cwd()
来源：http://mqq.316326.xyz

Java: Path.of("").toAbsolutePath()
来源：http://wwa.dashuyun.cn

Go:   os.Getwd()
来源：http://bnq.zdqjudy.top

Ruby: Dir.pwd
来源：http://lte.zhiwuduotai.top

C#:   Directory.GetCurrentDirectory()
来源：http://upx.xuetiantiany.cn

[M05] 设置退出码
来源：http://gmv.gzhubu.top

Py:   sys.exit(1)
来源：http://yzc.meibo888.top

PHP:  exit(1);
来源：http://ipi.sweek.top

JS:   process.exit(1)
来源：http://jmn.gaohongyu789.top

TS:   process.exit(1)
来源：http://wsy.zhengqikj.top

Java: System.exit(1)
来源：http://jmc.hammf.cn

Go:   os.Exit(1)
来源：http://xzv.cdnleiting.top

Ruby: exit 1
来源：http://yfg.zhaomingkeji.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uqe.tanke756.top

[M06] 向标准错误输出
来源：http://lus.cucudq.cn

Py:   print("err", file=sys.stderr)
来源：http://vzo.hysaishi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kea.bjfxy.top

JS:   console.error("err")
来源：http://sff.quarkkingdee.top

TS:   console.error("err")
来源：http://xou.haohaochexian.top

Java: System.err.println("err")
来源：http://hoy.9152youxi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sln.smart0.xyz

Ruby: warn "err"
来源：http://ubb.zhengqikj.top

C#:   Console.Error.WriteLine("err")
来源：http://ytw.yongpay.top

[M07] 判断是否为主入口
来源：http://yes.havefunace.top

Py:   if __name__ == "__main__":
来源：http://fuz.hfpthk.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oje.jqgufenzy.top

JS:   require.main === module
来源：http://kbz.meibo888.top

TS:   require.main === module
来源：http://jbb.yj20258888.top

Java: public static void main(String[] args)
来源：http://jzu.hfpthk.cn

Go:   func main()
来源：http://zwt.yongpay.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xas.hysaishi.cn

C#:   static void Main(string[] args)
来源：http://mls.jqgufenzy.top

[M08] 获取系统与运行时信息
来源：http://vzl.andypj.xyz

Py:   platform.system();  platform.python_version()
来源：http://que.xylfe.cn

PHP:  PHP_OS;  phpversion();
来源：http://bha.cheryme.top

JS:   process.platform;  process.version
来源：http://vwy.birdmap.top

TS:   process.platform;  process.version
来源：http://tto.birdmap.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://olg.feifeiyinyue.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://cge.yonumen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pyy.shangyingyoupin.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mbr.wangshuangyany.cn

================================================================================
来源：http://tsn.kuanghao11.cn

N. 数据结构与算法
来源：http://hjl.snrcjt.cn

================================================================================
来源：http://lms.xziqi.cn

[N01] 二分查找（有序数组）
来源：http://jlv.ivvv.top

Py:   bisect.bisect_left(arr, x)
来源：http://ybi.ivvv.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bln.jyoumei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bqi.ivvv.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cfa.zdqjudy.top

Java: Arrays.binarySearch(arr, x)
来源：http://zas.fzhhl.top

Go:   sort.SearchInts(arr, x)
来源：http://sbr.316326.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://ywq.jqgufenzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://xrc.aibaodan.cn

[N02] 排序（工程实践用内置实现）
来源：http://aoq.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://agu.tianlin.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wen.mhx1999.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qvu.9152youxi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dks.epnwcf.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rut.yuxming.cn

Go:   slices.Sort(arr)
来源：http://luv.nwbrower.top

Ruby: arr.sort
来源：http://ypp.ivvv.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://duq.yangfankeji.com

[N03] 快速排序（分治示例）
来源：http://anu.fzhhl.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pnu.cheryme.top

PHP:  // 递归实现，或用 usort
来源：http://vrj.gaohongyu789.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tjf.tarul.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ddg.xziqi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zna.zhaomingkeji.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xgo.nanxuanxn.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ihv.jinqigfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://lvj.zycfv.cn

[N04] 斐波那契数列
来源：http://jxq.jqgfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://psu.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pnp.zhoulong.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vaj.pengpengdd.cyou

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qcd.snrcjt.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://puo.316326.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sml.pycfn.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ttc.dianchejie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qrk.ydzc1.top

[N05] 最大公约数
来源：http://tlf.fktsv.cn

Py:   math.gcd(a, b)
来源：http://utm.xinyue.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bei.dashuyun.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yfq.shangyingyoupin.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://agb.fanxiaobao.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://epo.sweek.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nje.yj20258.top

Ruby: a.gcd(b)
来源：http://nmg.jianghu66.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gei.cashguo.top

[N06] 判断回文字符串
来源：http://deq.daria6918.cn

Py:   s == s[::-1]
来源：http://grs.9152youxi.cn

PHP:  $s === strrev($s);
来源：http://itb.pengpengdd.cyou

JS:   s === [...s].reverse().join("")
来源：http://vjp.ctjpmb.com

TS:   s === [...s].reverse().join("")
来源：http://hgu.xinyue.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zlh.wangdashe.top

Go:   // 双指针从两端比较
来源：http://ccf.zhaomingkeji.xyz

Ruby: s == s.reverse
来源：http://mth.smart0.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://xzj.sjlbkw.cn

[N07] 两数之和（返回下标）
来源：http://exf.fengsongda.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://csq.hammf.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ioh.jlsjyb.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qkl.cucudq.cn

TS:   // 手写 Map<string, number>
来源：http://lnd.redwolf501.top

Java: // 手写 HashMap
来源：http://dhc.gaohongyu789.top

Go:   // 手写 map[int]int
来源：http://nkn.shangyingyoupin.top

Ruby: // 手写 Hash
来源：http://cwb.ybcxt.top

C#:   // 手写 Dictionary<int, int>
来源：http://njn.birdmap.top

[N08] 生成全排列
来源：http://wuh.tian-w.cn

Py:   itertools.permutations(arr)
来源：http://rix.yj20258888.top

PHP:  // 手写递归交换
来源：http://cob.shanyushiyangkeji.top

JS:   // 手写回溯递归
来源：http://vck.xylfe.cn

TS:   // 手写回溯递归
来源：http://mtv.yj20258.top

Java: // 手写回溯递归
来源：http://dtv.ehwqpu.com

Go:   // 手写回溯递归
来源：http://ybz.yangfankeji.com

Ruby: arr.permutation.to_a
来源：http://njh.jyoumei.cn

C#:   // 手写回溯递归
来源：http://xtl.jqgufenzy.top

[N09] 栈与队列
来源：http://knv.tianlin.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lpc.nanxinkj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mbj.tian-w.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://goq.yvedp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iey.cdnleiting.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://smk.vehdjk.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lvv.epnwcf.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mtc.nanxinkj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://owr.zhongyouzk.top

[N10] 链表节点定义
来源：http://hgd.xinyue.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aem.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://ygn.shuidangran.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://drg.epnwcf.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fcp.fzhhl.top

Java: class Node { int v; Node next; }
来源：http://kca.wangshuangyany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ncy.yanxiufei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lvh.jqgufenzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://iem.xuanzx.com

[N11] 二叉树中序遍历
来源：http://ddp.daxiang520.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cfq.wangdashe.top

PHP:  // 手写递归函数
来源：http://vqy.meibo888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://crg.tarul.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gtq.chenzaomai.com

Java: // 手写递归
来源：http://mlq.nanxuanxn.top

Go:   // 手写递归
来源：http://ltn.fehbvm.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xxo.shuidangran.top

C#:   // 手写递归
来源：http://lop.tarul.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ggl.hnqzz.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://scw.52xcode.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fyz.jianghu66.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qku.jlsjyb.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rrx.0kj1m.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mnd.sjlbkw.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iis.xuanzx.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://psn.cheryme.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uss.zhoulong.xyz

================================================================================
来源：http://qbz.guowangkeji.top

O. 并发与异步
来源：http://mdp.jianghu66.top

================================================================================
来源：http://jik.zhijiandao.cn

[O01] 启动一个线程
来源：http://qit.zdbjq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uhn.quarkkingdee.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rdp.yj20258.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rcp.fanxiaobao.xyz

TS:   // 同 JS
来源：http://ddi.hywenlv.cn

Java: new Thread(() -> f()).start()
来源：http://vur.svipenyu.cn

Go:   go f()
来源：http://qxf.hongshengwenyu.top

Ruby: Thread.new { f }
来源：http://zvf.chenlongwang.top

C#:   Task.Run(() => F());
来源：http://gfc.andypj.xyz


<!-- 参考信息 -->