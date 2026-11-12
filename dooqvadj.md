代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://dbs.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oen.cashguo.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ujn.haohaochexian.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ist.redwolf501.top

[K06] 解析 URL 查询串
来源：http://abo.zhaomingkeji.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kaa.zhijiandao.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zek.ybcxt.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://box.vqdsnc.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dci.fktsv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vhl.yangfankeji.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://ftf.fktsv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eua.gogol.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wrr.316326.xyz

[K07] 进制转换
来源：http://xhr.birdmap.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bui.wangdashe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ojz.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cat.hongshengwenyu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hmp.mhx1999.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hcb.xingfuxueyuan.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rty.wangshuangyany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wut.bjfxy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rbz.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://wmh.cdnleiting.top

Py:   pickle.dumps(obj)
来源：http://hxp.sxryk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xrk.hysaishi.cn

JS:   v8.serialize(obj)        // Node
来源：http://gbu.yj20258.top

TS:   v8.serialize(obj)        // Node
来源：http://hvb.xuetiantiany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oxm.yanxiufei.cn

Go:   encoding/gob
来源：http://qvy.tianlin.xyz

Ruby: Marshal.dump(obj)
来源：http://osn.bjfxy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zkk.gaohongyu789.top

================================================================================
来源：http://vta.hcnkem.com

L. 网络请求
来源：http://hia.yuanzhike.top

================================================================================
来源：http://kgt.xuetiantiany.cn

[L01] 发送 GET 请求
来源：http://lfr.hnxiangtu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vmx.cdnleiting.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xdi.zhaomingkeji.xyz

JS:   await fetch(url)
来源：http://wul.mhx1999.top

TS:   await fetch(url)
来源：http://vam.jqgufenzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://udw.shanyushiyangkeji.top

Go:   resp, err := http.Get(url)
来源：http://vjz.ybcxt.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fzk.meibo888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pll.zdbjq.cn

[L02] 发送 POST JSON
来源：http://odj.chenzaomai.com

Py:   requests.post(url, json={"a": 1})
来源：http://vpe.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xxk.jinqigfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://frj.bjfxy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zjc.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bep.fktsv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lkq.0kj1m.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iug.zdqjudy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yve.sysykeji.top

[L03] 设置自定义请求头
来源：http://gey.shanyushiyangtech.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wag.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://utc.bjfxy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sxz.hongshengwenyu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://okk.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ckx.yuxming.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ate.birdmap.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qfi.yvedp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fyu.0kj1m.cn

[L04] 设置超时
来源：http://ggm.nwbrower.top

Py:   requests.get(url, timeout=5)
来源：http://nzd.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vyv.daxiang520.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zxg.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aoi.smart0.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bto.fzhhl.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fqd.epnwcf.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vfp.xziqi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mdq.yuxming.cn

[L05] 上传文件（multipart）
来源：http://tcm.xuetiantiany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qsv.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jjq.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oks.zdbjq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blk.jiagoushi.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ofn.haohaochexian.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hlq.dianchejie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://equ.smart0.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bjh.yuanzhike.top

[L06] 解析响应为 JSON
来源：http://rva.sjlbkw.cn

Py:   resp.json()
来源：http://bex.nanxinkj.top

PHP:  json_decode($body, true);
来源：http://ohd.yanxiufei.cn

JS:   await resp.json()
来源：http://ptx.52xcode.cn

TS:   await resp.json()
来源：http://vie.bbcook.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zus.cdnleiting.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://glf.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://nhj.xuanzx.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sqb.yj20258888.top

[L07] 处理 HTTP 状态码
来源：http://ies.jiagoushi.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qvi.daxiang520.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://epw.haohaochexian.top

JS:   resp.ok;  resp.status
来源：http://eps.pycfn.com

TS:   resp.ok;  resp.status
来源：http://wqt.xuanzx.com

Java: resp.statusCode()
来源：http://kct.tianlin.xyz

Go:   resp.StatusCode
来源：http://mnt.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://iyt.chenzaomai.com

C#:   (int)resp.StatusCode
来源：http://etn.ehwqpu.com

[L08] 并发请求多个地址
来源：http://sry.ydjk.org.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://geq.xuanzx.com

PHP:  curl_multi_init() 系列
来源：http://tse.mhx1999.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rsg.jqgufenzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vor.birdmap.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://csk.bbcook.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rdy.ybcxt.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ogw.hcnkem.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hlz.jianghu66.top

================================================================================
来源：http://zeb.yongpay.top

M. 命令行 / 进程 / 环境
来源：http://egz.uphjek.com

================================================================================
来源：http://tur.bjfxy.top

[M01] 读取命令行参数
来源：http://mjt.gzhubu.top

Py:   sys.argv[1:]
来源：http://fvf.zhiwuduotai.top

PHP:  $argv;  $argc;
来源：http://qff.yanxiufei.cn

JS:   process.argv.slice(2)
来源：http://vsw.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://njl.c1oappe.top

Java: args 数组（main 方法参数）
来源：http://gaw.zhengqikj.top

Go:   os.Args[1:]
来源：http://cvk.quarkkingdee.top

Ruby: ARGV
来源：http://aho.sxryk.cn

C#:   args 数组（Main 方法参数）
来源：http://rvu.xziqi.cn

[M02] 读取环境变量
来源：http://zgj.ivvv.top

Py:   os.environ.get("HOME")
来源：http://grl.jyoumei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xme.jinqigufen.top

JS:   process.env.HOME
来源：http://cvy.snrcjt.cn

TS:   process.env.HOME
来源：http://wsj.ydzc1.top

Java: System.getenv("HOME")
来源：http://yuv.gaohongyu789.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rtc.chenjidiqi.icu

Ruby: ENV["HOME"]
来源：http://kab.nwbrower.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wes.yangfankeji.com

[M03] 执行外部命令
来源：http://yuh.cdnleiting.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pba.wangshuangyany.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zzl.sjlbkw.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fsm.yuxming.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gtr.daxiang520.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ugf.xingfuxueyuan.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://kmz.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ovo.zhengqikj.top

C#:   Process.Start("ls", "-l");
来源：http://qcd.xziqi.cn

[M04] 获取当前工作目录
来源：http://dlv.svipenyu.cn

Py:   os.getcwd()
来源：http://xhx.yueranfly.top

PHP:  getcwd();
来源：http://eap.svipenyu.cn

JS:   process.cwd()
来源：http://wli.jinqigfzy.top

TS:   process.cwd()
来源：http://rof.jinghuilouyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://qob.yangfankeji.com

Go:   os.Getwd()
来源：http://bqk.hongshengwenyu.top

Ruby: Dir.pwd
来源：http://upe.ctjpmb.com

C#:   Directory.GetCurrentDirectory()
来源：http://rwc.bbcook.cn

[M05] 设置退出码
来源：http://jor.jinyuanbaomall.cn

Py:   sys.exit(1)
来源：http://kby.yvedp.cn

PHP:  exit(1);
来源：http://nqb.havefunace.top

JS:   process.exit(1)
来源：http://lzm.bjfxy.top

TS:   process.exit(1)
来源：http://qeu.sufxvd.cn

Java: System.exit(1)
来源：http://oxl.9152youxi.cn

Go:   os.Exit(1)
来源：http://bsy.dashuyun.cn

Ruby: exit 1
来源：http://irz.yueranfly.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tjv.dianchejie.cn

[M06] 向标准错误输出
来源：http://usm.birdmap.top

Py:   print("err", file=sys.stderr)
来源：http://jsw.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xxx.pycfn.com

JS:   console.error("err")
来源：http://ylp.daria6918.cn

TS:   console.error("err")
来源：http://mpf.mhx1999.top

Java: System.err.println("err")
来源：http://fnx.aibaodan.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rja.52xcode.cn

Ruby: warn "err"
来源：http://pkc.zhongyouzk.top

C#:   Console.Error.WriteLine("err")
来源：http://rjm.ehwqpu.com

[M07] 判断是否为主入口
来源：http://vgt.fzhhl.top

Py:   if __name__ == "__main__":
来源：http://xdb.feifeiyinyue.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rti.fehbvm.com

JS:   require.main === module
来源：http://xyb.fanxiaobao.xyz

TS:   require.main === module
来源：http://qtn.guannengcc.top

Java: public static void main(String[] args)
来源：http://lpi.aibaodan.cn

Go:   func main()
来源：http://cgm.hywenlv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mjk.ydjk.org.cn

C#:   static void Main(string[] args)
来源：http://xkm.zhixingplan.top

[M08] 获取系统与运行时信息
来源：http://xvv.jqgufenzy.top

Py:   platform.system();  platform.python_version()
来源：http://xwd.jinqigufen.top

PHP:  PHP_OS;  phpversion();
来源：http://gzl.zhijiandao.cn

JS:   process.platform;  process.version
来源：http://vvt.bbcook.cn

TS:   process.platform;  process.version
来源：http://iaf.dashuyun.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mbe.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://guq.zhoulong.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rim.hnqzz.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fsf.9152youxi.cn

================================================================================
来源：http://itl.yongpay.top

N. 数据结构与算法
来源：http://qab.chenlongwang.top

================================================================================
来源：http://izc.hysaishi.cn

[N01] 二分查找（有序数组）
来源：http://xny.vqdsnc.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wsi.jinqigufen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sgt.hfpthk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vrn.gotoacloud.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://our.shanyushiyangtech.top

Java: Arrays.binarySearch(arr, x)
来源：http://zso.aibaodan.cn

Go:   sort.SearchInts(arr, x)
来源：http://btn.kuanghao11.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sot.hnxiangtu.top

C#:   Array.BinarySearch(arr, x)
来源：http://nwi.uphjek.com

[N02] 排序（工程实践用内置实现）
来源：http://qvb.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://ofm.hongshengwenyu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gdn.hcnkem.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://deh.andypj.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://uhi.zdbjq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://phl.xziqi.cn

Go:   slices.Sort(arr)
来源：http://zrz.ivvv.top

Ruby: arr.sort
来源：http://djh.daxiang520.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pjz.cashguo.top

[N03] 快速排序（分治示例）
来源：http://pma.gotoacloud.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dit.hesvh.cn

PHP:  // 递归实现，或用 usort
来源：http://vnp.iojbl.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mol.9152youxi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ckh.zhijiandao.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eza.tanke756.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yul.fehbvm.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://spt.svipenyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zrt.hfpthk.cn

[N04] 斐波那契数列
来源：http://fuf.yvedp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://skg.gotoacloud.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tvx.hammf.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pmk.yj20258.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fmv.hongshengwenyu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xea.smart0.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nwm.zhongyouzk.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yji.hnxiangtu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cjr.nwbrower.top

[N05] 最大公约数
来源：http://qex.yfazqb.com

Py:   math.gcd(a, b)
来源：http://itx.c1oappe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ffv.shanyushiyangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dbj.fengsongda.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cyl.yj20258888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://miw.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uqg.hywenlv.cn

Ruby: a.gcd(b)
来源：http://ecz.fktsv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kca.xziqi.cn

[N06] 判断回文字符串
来源：http://qvh.ydjk.org.cn

Py:   s == s[::-1]
来源：http://cas.dashuyun.cn

PHP:  $s === strrev($s);
来源：http://ylq.havefunace.top

JS:   s === [...s].reverse().join("")
来源：http://vrs.tianlin.xyz

TS:   s === [...s].reverse().join("")
来源：http://xdl.yfazqb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://psi.daxiang520.top

Go:   // 双指针从两端比较
来源：http://yck.dashuyun.cn

Ruby: s == s.reverse
来源：http://wvt.tarul.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rum.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://fes.zhaomingkeji.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hwt.smart0.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://slz.hongshengwenyu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xom.sysykeji.top

TS:   // 手写 Map<string, number>
来源：http://vix.yongpay.top

Java: // 手写 HashMap
来源：http://rur.zhixingplan.top

Go:   // 手写 map[int]int
来源：http://kji.yj20258888.top

Ruby: // 手写 Hash
来源：http://yjx.sjlbkw.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rfd.daria6918.cn

[N08] 生成全排列
来源：http://nfb.andypj.xyz

Py:   itertools.permutations(arr)
来源：http://xfb.hongshengwenyu.top

PHP:  // 手写递归交换
来源：http://pmy.c1oappe.top

JS:   // 手写回溯递归
来源：http://oyz.yj20258888.top

TS:   // 手写回溯递归
来源：http://wif.redwolf501.top

Java: // 手写回溯递归
来源：http://ewc.mhx1999.top

Go:   // 手写回溯递归
来源：http://ctv.316326.xyz

Ruby: arr.permutation.to_a
来源：http://icn.feifeiyinyue.top

C#:   // 手写回溯递归
来源：http://opq.cucudq.cn

[N09] 栈与队列
来源：http://ugf.quarkkingdee.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vuo.hywenlv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://opb.snrcjt.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://clm.ehwqpu.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uzd.gaohongyu789.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qwt.sweek.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eqe.zhijiandao.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pcn.hnqzz.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kjx.guowangkeji.top

[N10] 链表节点定义
来源：http://bnm.xziqi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qsy.shuidangran.top

PHP:  class Node { public $v; public $next = null; }
来源：http://nlg.andypj.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kjj.gzhubu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vne.fanxiaobao.xyz

Java: class Node { int v; Node next; }
来源：http://oix.kuanghao11.cn

Go:   type Node struct { V int; Next *Node }
来源：http://biz.fengsongda.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zdj.guannengcc.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zxh.yangfankeji.com

[N11] 二叉树中序遍历
来源：http://fmk.yvedp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sld.daria6918.cn

PHP:  // 手写递归函数
来源：http://svq.nanxinkj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://niq.bbcook.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ffp.havefunace.top

Java: // 手写递归
来源：http://mho.316326.xyz

Go:   // 手写递归
来源：http://iej.zycfv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://elw.vehdjk.com

C#:   // 手写递归
来源：http://sfm.shangyingyoupin.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gwi.jinqigfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mjz.ywan-chungtsiang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jbe.dianchejie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wzr.ydzc1.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://smz.hammf.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mlo.hysaishi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zgk.xingfuxueyuan.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://neu.tanke756.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://miw.fanxiaobao.xyz

================================================================================
来源：http://bxg.mhx1999.top

O. 并发与异步
来源：http://muj.yj20258888.top

================================================================================
来源：http://cnb.yvedp.cn

[O01] 启动一个线程
来源：http://rrn.zycfv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ojm.ydjk.org.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://abg.smart0.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dxi.haohaochexian.top

TS:   // 同 JS
来源：http://cin.ybcxt.top


<!-- 参考信息 -->