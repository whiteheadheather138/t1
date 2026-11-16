代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://njg.pycfn.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mbn.xziqi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ltj.9152youxi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bcj.yonumen.top

[K06] 解析 URL 查询串
来源：http://kij.uphjek.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yyj.aizwys.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xni.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jxa.guannengcc.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kuh.wangshuangyany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vdj.ppjwa.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gtt.9152youxi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lrt.yuanzhike.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fhi.xingfuxueyuan.xyz

[K07] 进制转换
来源：http://fij.zhoulong.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://brc.feifeiyinyue.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dsq.hesvh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gjg.vehdjk.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mml.fzhhl.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wfg.chenjidiqi.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ubs.ctjpmb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pqx.zhengqikj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tig.c1oappe.top

[K08] 二进制序列化（非 JSON）
来源：http://nxh.hywenlv.cn

Py:   pickle.dumps(obj)
来源：http://aup.jqgufenzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vii.sysykeji.top

JS:   v8.serialize(obj)        // Node
来源：http://ooi.yj20258888.top

TS:   v8.serialize(obj)        // Node
来源：http://krq.chenjidiqi.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cht.yanxiufei.cn

Go:   encoding/gob
来源：http://roh.wangdashe.top

Ruby: Marshal.dump(obj)
来源：http://eev.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rif.316326.xyz

================================================================================
来源：http://tor.sweek.top

L. 网络请求
来源：http://ixn.shzxlz.cn

================================================================================
来源：http://udf.smart0.xyz

[L01] 发送 GET 请求
来源：http://pob.hesvh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cet.tanke756.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qfa.tianlin.xyz

JS:   await fetch(url)
来源：http://dab.svipenyu.cn

TS:   await fetch(url)
来源：http://gzh.jianghu66.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jvf.yangfankeji.com

Go:   resp, err := http.Get(url)
来源：http://nwi.quarkkingdee.top

Ruby: Net::HTTP.get(URI(url))
来源：http://aau.yangfankeji.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://huu.sjlbkw.cn

[L02] 发送 POST JSON
来源：http://kok.hongshengwenyu.top

Py:   requests.post(url, json={"a": 1})
来源：http://pwc.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kbd.yueranfly.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://icp.svipenyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cue.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://osb.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cbv.yfazqb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uht.sweek.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oso.vehdjk.com

[L03] 设置自定义请求头
来源：http://six.jqgfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qxf.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nur.wangdashe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tdo.guowangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iod.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://avs.feifeiyinyue.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tyv.fengsongda.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zjg.0kj1m.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jlb.zhixingplan.top

[L04] 设置超时
来源：http://ihp.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://unv.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yeu.jinyuanbaomall.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nsp.yongpay.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nyo.vehdjk.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ekq.ydjk.org.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eko.jianghu66.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jlj.havefunace.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jaz.ivvv.top

[L05] 上传文件（multipart）
来源：http://tgs.kuanghao11.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zqc.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://auh.gogol.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mxp.yonumen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lkd.fanxiaobao.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vdp.fzhhl.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iic.9152youxi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oal.fehbvm.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xir.52xcode.cn

[L06] 解析响应为 JSON
来源：http://cgc.ydjk.org.cn

Py:   resp.json()
来源：http://bvd.zhixingplan.top

PHP:  json_decode($body, true);
来源：http://grn.yj20258.top

JS:   await resp.json()
来源：http://snl.sweek.top

TS:   await resp.json()
来源：http://tqr.fengsongda.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sid.dianchejie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cyt.hysaishi.cn

Ruby: JSON.parse(resp.body)
来源：http://eos.fktsv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fao.yvedp.cn

[L07] 处理 HTTP 状态码
来源：http://edr.9152youxi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aem.nanxuanxn.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dsg.zhaomingkeji.xyz

JS:   resp.ok;  resp.status
来源：http://kmx.andypj.xyz

TS:   resp.ok;  resp.status
来源：http://odl.yvedp.cn

Java: resp.statusCode()
来源：http://wdf.yfazqb.com

Go:   resp.StatusCode
来源：http://gcf.hcnkem.com

Ruby: resp.code.to_i
来源：http://kzf.dashuyun.cn

C#:   (int)resp.StatusCode
来源：http://ydz.cashguo.top

[L08] 并发请求多个地址
来源：http://dfm.ydzc1.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zdf.xylfe.cn

PHP:  curl_multi_init() 系列
来源：http://qia.tian-w.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://omp.gogol.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hdi.tanke756.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yrn.hammf.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qkm.shanyushiyangtech.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hgt.cdnleiting.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://avx.xziqi.cn

================================================================================
来源：http://usn.yuanzhike.top

M. 命令行 / 进程 / 环境
来源：http://icw.hongshengwenyu.top

================================================================================
来源：http://hmq.zhongyouzk.top

[M01] 读取命令行参数
来源：http://lxf.jianghu66.top

Py:   sys.argv[1:]
来源：http://grj.hywenlv.cn

PHP:  $argv;  $argc;
来源：http://iiy.yj20258888.top

JS:   process.argv.slice(2)
来源：http://dfx.yvedp.cn

TS:   process.argv.slice(2)
来源：http://xpg.mhx1999.top

Java: args 数组（main 方法参数）
来源：http://xmk.c1oappe.top

Go:   os.Args[1:]
来源：http://xmc.andypj.xyz

Ruby: ARGV
来源：http://syq.vqdsnc.cn

C#:   args 数组（Main 方法参数）
来源：http://qxe.chenjidiqi.icu

[M02] 读取环境变量
来源：http://daz.dianchejie.cn

Py:   os.environ.get("HOME")
来源：http://dkp.tian-w.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://naw.fanxiaobao.xyz

JS:   process.env.HOME
来源：http://tyl.jinyuanbaomall.cn

TS:   process.env.HOME
来源：http://pus.jinqigufen.top

Java: System.getenv("HOME")
来源：http://kzu.zycfv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xlg.gogol.net.cn

Ruby: ENV["HOME"]
来源：http://xvj.smart0.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zgf.nwbrower.top

[M03] 执行外部命令
来源：http://yan.yueranfly.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dxm.havefunace.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yil.yonumen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://oaj.nwbrower.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qrj.yonumen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pkd.jiagoushi.top

Go:   exec.Command("ls", "-l").Output()
来源：http://uej.yj202588.top

Ruby: system("ls -l");  `ls -l`
来源：http://psh.fktsv.cn

C#:   Process.Start("ls", "-l");
来源：http://zkz.sufxvd.cn

[M04] 获取当前工作目录
来源：http://rdy.sysykeji.top

Py:   os.getcwd()
来源：http://pbm.hammf.cn

PHP:  getcwd();
来源：http://udb.c1oappe.top

JS:   process.cwd()
来源：http://vvh.zdqjudy.top

TS:   process.cwd()
来源：http://wes.ctjpmb.com

Java: Path.of("").toAbsolutePath()
来源：http://dqi.xylfe.cn

Go:   os.Getwd()
来源：http://fjw.jqgufenzy.top

Ruby: Dir.pwd
来源：http://rom.hesvh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cvj.hongshengwenyu.top

[M05] 设置退出码
来源：http://tre.bjfxy.top

Py:   sys.exit(1)
来源：http://eyo.feifeiyinyue.top

PHP:  exit(1);
来源：http://hop.tianlin.xyz

JS:   process.exit(1)
来源：http://zzy.fanxiaobao.xyz

TS:   process.exit(1)
来源：http://ete.hcnkem.com

Java: System.exit(1)
来源：http://frg.xziqi.cn

Go:   os.Exit(1)
来源：http://kop.sweek.top

Ruby: exit 1
来源：http://qxc.fanxiaobao.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tax.iojbl.cn

[M06] 向标准错误输出
来源：http://gkg.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://bdj.xuanzx.com

PHP:  fwrite(STDERR, "err\n");
来源：http://wyq.zhoulong.xyz

JS:   console.error("err")
来源：http://clr.sufxvd.cn

TS:   console.error("err")
来源：http://wml.jinyuanbaomall.cn

Java: System.err.println("err")
来源：http://mrd.yj20258.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lsx.vehdjk.com

Ruby: warn "err"
来源：http://kfk.jianghu66.top

C#:   Console.Error.WriteLine("err")
来源：http://vze.yuxming.cn

[M07] 判断是否为主入口
来源：http://zna.yuxming.cn

Py:   if __name__ == "__main__":
来源：http://bus.iojbl.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nhg.bjfxy.top

JS:   require.main === module
来源：http://tmq.jinqigfzy.top

TS:   require.main === module
来源：http://htp.jinqigfzy.top

Java: public static void main(String[] args)
来源：http://lxj.redwolf501.top

Go:   func main()
来源：http://uay.shanyushiyangtech.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uoz.ctjpmb.com

C#:   static void Main(string[] args)
来源：http://whv.svipenyu.cn

[M08] 获取系统与运行时信息
来源：http://bax.shanyushiyangtech.top

Py:   platform.system();  platform.python_version()
来源：http://aqg.smart0.xyz

PHP:  PHP_OS;  phpversion();
来源：http://qne.yueranfly.top

JS:   process.platform;  process.version
来源：http://pcu.feifeiyinyue.top

TS:   process.platform;  process.version
来源：http://oeu.sufxvd.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ydt.zhongyouzk.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ngv.jinghuilouyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dar.zhaomingkeji.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://jfa.tarul.cn

================================================================================
来源：http://wdp.c1oappe.top

N. 数据结构与算法
来源：http://oos.vehdjk.com

================================================================================
来源：http://izs.tianlin.xyz

[N01] 二分查找（有序数组）
来源：http://igs.nanxinkj.top

Py:   bisect.bisect_left(arr, x)
来源：http://njv.zhongyouzk.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://itt.jinghuilouyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://atl.shanyushiyangtech.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qfs.xinyue.icu

Java: Arrays.binarySearch(arr, x)
来源：http://qzk.hesvh.cn

Go:   sort.SearchInts(arr, x)
来源：http://rwe.chenzaomai.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://oxy.fengsongda.top

C#:   Array.BinarySearch(arr, x)
来源：http://hot.gaohongyu789.top

[N02] 排序（工程实践用内置实现）
来源：http://ens.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://utj.nanxinkj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xvx.hfpthk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tey.birdmap.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://nsx.meibo888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ibq.meibo888.top

Go:   slices.Sort(arr)
来源：http://sho.iojbl.cn

Ruby: arr.sort
来源：http://tbj.birdmap.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://otg.haohaochexian.top

[N03] 快速排序（分治示例）
来源：http://gev.zhengqikj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kky.shanyushiyangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://vuh.jianghu66.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ybo.aizwys.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sav.aizwys.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eht.cdnleiting.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nuk.ywan-chungtsiang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ztj.haohaochexian.top

C#:   // 手写递归，或 Array.Sort
来源：http://lei.ydjk.org.cn

[N04] 斐波那契数列
来源：http://lpb.bjfxy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wru.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mpz.fengsongda.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://guf.hywenlv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kpm.quarkkingdee.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mql.sjlbkw.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rvk.sufxvd.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nsu.fzhhl.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ijd.zycfv.cn

[N05] 最大公约数
来源：http://ebx.meibo888.top

Py:   math.gcd(a, b)
来源：http://eeu.meibo888.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wjz.kuanghao11.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mlc.316326.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lfp.fehbvm.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jps.hongshengwenyu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oaf.smart0.xyz

Ruby: a.gcd(b)
来源：http://mgw.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qtp.hesvh.cn

[N06] 判断回文字符串
来源：http://dty.wangshuangyany.cn

Py:   s == s[::-1]
来源：http://oop.ydjk.org.cn

PHP:  $s === strrev($s);
来源：http://ktv.ppjwa.cn

JS:   s === [...s].reverse().join("")
来源：http://vyv.aibaodan.cn

TS:   s === [...s].reverse().join("")
来源：http://apw.birdmap.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fqc.jinghuilouyu.cn

Go:   // 双指针从两端比较
来源：http://erx.zycfv.cn

Ruby: s == s.reverse
来源：http://pup.shangyingyoupin.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ynn.gogol.net.cn

[N07] 两数之和（返回下标）
来源：http://nre.guannengcc.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tsd.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wsu.fehbvm.com

JS:   // 手写 Map：map.set(v, i)
来源：http://siy.zhiwuduotai.top

TS:   // 手写 Map<string, number>
来源：http://ylc.yj20258.top

Java: // 手写 HashMap
来源：http://zza.xylfe.cn

Go:   // 手写 map[int]int
来源：http://hac.hysaishi.cn

Ruby: // 手写 Hash
来源：http://axw.daria6918.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lpe.kuanghao11.cn

[N08] 生成全排列
来源：http://xpq.snrcjt.cn

Py:   itertools.permutations(arr)
来源：http://ykq.guowangkeji.top

PHP:  // 手写递归交换
来源：http://gdl.zycfv.cn

JS:   // 手写回溯递归
来源：http://bmw.hesvh.cn

TS:   // 手写回溯递归
来源：http://eiu.tian-w.cn

Java: // 手写回溯递归
来源：http://znw.gogol.net.cn

Go:   // 手写回溯递归
来源：http://tlv.jinqigfzy.top

Ruby: arr.permutation.to_a
来源：http://mnp.havefunace.top

C#:   // 手写回溯递归
来源：http://iyf.jinqigufen.top

[N09] 栈与队列
来源：http://oyu.xingfuxueyuan.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ijs.yuxming.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iop.xylfe.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://whp.daxiang520.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qsc.zhijiandao.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nph.cdnleiting.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jxl.ctjpmb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qty.aibaodan.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jjg.zhaomingkeji.xyz

[N10] 链表节点定义
来源：http://znm.ivvv.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pfm.wangshuangyany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qyp.andypj.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jnz.ppjwa.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://frk.vehdjk.com

Java: class Node { int v; Node next; }
来源：http://xwx.shzxlz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hog.hcnkem.com

Ruby: Node = Struct.new(:v, :next)
来源：http://wez.daria6918.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lpb.yfazqb.com

[N11] 二叉树中序遍历
来源：http://ulw.316326.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wip.iojbl.cn

PHP:  // 手写递归函数
来源：http://cyn.wangshuangyany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xqx.cheryme.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oxy.nwbrower.top

Java: // 手写递归
来源：http://xjg.shzxlz.cn

Go:   // 手写递归
来源：http://qmr.cheryme.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mep.hongshengwenyu.top

C#:   // 手写递归
来源：http://xbx.bjfxy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nqz.ehwqpu.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://noy.jinghuilouyu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rtl.ehwqpu.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cty.zhijiandao.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kpe.cdnleiting.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ecd.daria6918.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pzx.hnqzz.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://awh.jyoumei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mbn.yangfankeji.com

================================================================================
来源：http://rpw.dashuyun.cn

O. 并发与异步
来源：http://xsb.yvedp.cn

================================================================================
来源：http://wej.gogol.net.cn

[O01] 启动一个线程
来源：http://xtu.vqdsnc.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qpn.yanxiufei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lfw.shanyushiyangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vfo.jianghu66.top

TS:   // 同 JS
来源：http://aia.epnwcf.com


<!-- 参考信息 -->