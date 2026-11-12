代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://fhs.aizwys.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wof.cucudq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://amc.yangfankeji.com

C#:   // 序列化往返，或自定义 Clone
来源：http://tgq.cqqwz.cn

[K06] 解析 URL 查询串
来源：http://zme.wangshuangyany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bmr.mhx1999.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bam.cucudq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qqa.xinyue.icu

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://haw.mhx1999.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pts.gaohongyu789.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jhp.yonumen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gjh.zycfv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mna.epnwcf.com

[K07] 进制转换
来源：http://rqr.ydjk.org.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://faf.yangfankeji.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://myj.xuetiantiany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xnj.jyoumei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ydw.wangdashe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wwy.xuanzx.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jhg.aibaodan.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://grj.wangshuangyany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oaq.tian-w.cn

[K08] 二进制序列化（非 JSON）
来源：http://uyr.bbcook.cn

Py:   pickle.dumps(obj)
来源：http://clw.ydjk.org.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ovo.zhixingplan.top

JS:   v8.serialize(obj)        // Node
来源：http://pvk.sweek.top

TS:   v8.serialize(obj)        // Node
来源：http://vxz.aibaodan.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ohp.yj20258888.top

Go:   encoding/gob
来源：http://mru.yj20258.top

Ruby: Marshal.dump(obj)
来源：http://jnt.shuidangran.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ain.mhx1999.top

================================================================================
来源：http://wur.hesvh.cn

L. 网络请求
来源：http://drt.pengpengdd.cyou

================================================================================
来源：http://cdo.hfpthk.cn

[L01] 发送 GET 请求
来源：http://ulj.sweek.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qbl.tianlin.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pdg.svipenyu.cn

JS:   await fetch(url)
来源：http://afk.fengsongda.top

TS:   await fetch(url)
来源：http://wqe.feifeiyinyue.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://trs.xingfuxueyuan.xyz

Go:   resp, err := http.Get(url)
来源：http://ody.xuetiantiany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://aoj.fengsongda.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://him.ybcxt.top

[L02] 发送 POST JSON
来源：http://qqb.haohaochexian.top

Py:   requests.post(url, json={"a": 1})
来源：http://upk.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ety.fanxiaobao.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ads.ydjk.org.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fft.yj20258.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ekk.ivvv.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jni.ehwqpu.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dbm.sysykeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eri.bbcook.cn

[L03] 设置自定义请求头
来源：http://okv.wangdashe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jbt.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lnh.guannengcc.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zcm.fehbvm.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ylb.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gmn.yj202588.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jtd.jinyuanbaomall.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qdu.jiagoushi.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lss.andypj.xyz

[L04] 设置超时
来源：http://ppq.hesvh.cn

Py:   requests.get(url, timeout=5)
来源：http://qqh.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fsy.epnwcf.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qsi.tianlin.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xat.sysykeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uho.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://otw.c1oappe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ycq.yfazqb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ezc.vehdjk.com

[L05] 上传文件（multipart）
来源：http://grs.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rae.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vpp.9152youxi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qtv.yueranfly.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eko.316326.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kzq.zhijiandao.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ecw.cdnleiting.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ydl.kuanghao11.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yql.ybcxt.top

[L06] 解析响应为 JSON
来源：http://upq.nwbrower.top

Py:   resp.json()
来源：http://wle.bjfxy.top

PHP:  json_decode($body, true);
来源：http://yct.yj20258.top

JS:   await resp.json()
来源：http://lpf.tian-w.cn

TS:   await resp.json()
来源：http://say.haohaochexian.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dgh.fzhhl.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ifc.daria6918.cn

Ruby: JSON.parse(resp.body)
来源：http://hjl.zdbjq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bun.fanxiaobao.xyz

[L07] 处理 HTTP 状态码
来源：http://wcx.hywenlv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xjv.redwolf501.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://abw.cqqwz.cn

JS:   resp.ok;  resp.status
来源：http://zwr.jqgufenzy.top

TS:   resp.ok;  resp.status
来源：http://prv.hammf.cn

Java: resp.statusCode()
来源：http://vdt.ppjwa.cn

Go:   resp.StatusCode
来源：http://ozr.tianlin.xyz

Ruby: resp.code.to_i
来源：http://ahr.gotoacloud.top

C#:   (int)resp.StatusCode
来源：http://lul.fktsv.cn

[L08] 并发请求多个地址
来源：http://uov.daxiang520.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://amx.zhixingplan.top

PHP:  curl_multi_init() 系列
来源：http://hyj.xinyue.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://shp.yj20258.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bix.cdnleiting.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lbj.yueranfly.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fuh.vqdsnc.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zvq.tian-w.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jmo.zhongyouzk.top

================================================================================
来源：http://gsl.andypj.xyz

M. 命令行 / 进程 / 环境
来源：http://rev.jqgufenzy.top

================================================================================
来源：http://mrz.andypj.xyz

[M01] 读取命令行参数
来源：http://vrt.yuanzhike.top

Py:   sys.argv[1:]
来源：http://vyl.pycfn.com

PHP:  $argv;  $argc;
来源：http://wfk.jinyuanbaomall.cn

JS:   process.argv.slice(2)
来源：http://ona.yangfankeji.com

TS:   process.argv.slice(2)
来源：http://yjp.ywan-chungtsiang.top

Java: args 数组（main 方法参数）
来源：http://vel.feifeiyinyue.top

Go:   os.Args[1:]
来源：http://hrp.52xcode.cn

Ruby: ARGV
来源：http://iir.jqgfzy.top

C#:   args 数组（Main 方法参数）
来源：http://zvx.haohaochexian.top

[M02] 读取环境变量
来源：http://mif.yj202588.top

Py:   os.environ.get("HOME")
来源：http://zfl.daxiang520.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://btg.jlsjyb.cn

JS:   process.env.HOME
来源：http://ngb.cdnleiting.top

TS:   process.env.HOME
来源：http://maz.andypj.xyz

Java: System.getenv("HOME")
来源：http://wth.quarkkingdee.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vgb.cdnleiting.top

Ruby: ENV["HOME"]
来源：http://eda.gaohongyu789.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tsu.hywenlv.cn

[M03] 执行外部命令
来源：http://mvc.hnqzz.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wvi.jinqigufen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gxs.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gde.guowangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vwd.redwolf501.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cdg.yuanzhike.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jnu.pycfn.com

Ruby: system("ls -l");  `ls -l`
来源：http://pkf.yangfankeji.com

C#:   Process.Start("ls", "-l");
来源：http://guv.aibaodan.cn

[M04] 获取当前工作目录
来源：http://blw.yangfankeji.com

Py:   os.getcwd()
来源：http://ort.shanyushiyangtech.top

PHP:  getcwd();
来源：http://cwt.jianghu66.top

JS:   process.cwd()
来源：http://akg.gotoacloud.top

TS:   process.cwd()
来源：http://ryo.svipenyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://jif.xuanzx.com

Go:   os.Getwd()
来源：http://agy.ehwqpu.com

Ruby: Dir.pwd
来源：http://oos.sjlbkw.cn

C#:   Directory.GetCurrentDirectory()
来源：http://siq.0kj1m.cn

[M05] 设置退出码
来源：http://cis.hfpthk.cn

Py:   sys.exit(1)
来源：http://ihx.tian-w.cn

PHP:  exit(1);
来源：http://hzq.yj202588.top

JS:   process.exit(1)
来源：http://rvt.jqgufenzy.top

TS:   process.exit(1)
来源：http://cag.9152youxi.cn

Java: System.exit(1)
来源：http://kvp.yangfankeji.com

Go:   os.Exit(1)
来源：http://mlr.jianghu66.top

Ruby: exit 1
来源：http://tnv.sysykeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zcs.yanxiufei.cn

[M06] 向标准错误输出
来源：http://oir.cqqwz.cn

Py:   print("err", file=sys.stderr)
来源：http://vzb.jinyuanbaomall.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dcc.hongshengwenyu.top

JS:   console.error("err")
来源：http://aiz.xuetiantiany.cn

TS:   console.error("err")
来源：http://xpc.haohaochexian.top

Java: System.err.println("err")
来源：http://wpq.guannengcc.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vfs.epnwcf.com

Ruby: warn "err"
来源：http://qts.yanxiufei.cn

C#:   Console.Error.WriteLine("err")
来源：http://jqw.9152youxi.cn

[M07] 判断是否为主入口
来源：http://qjw.xuanzx.com

Py:   if __name__ == "__main__":
来源：http://ygx.xuetiantiany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://szx.xziqi.cn

JS:   require.main === module
来源：http://ozd.shangyingyoupin.top

TS:   require.main === module
来源：http://gis.wangdashe.top

Java: public static void main(String[] args)
来源：http://uxn.nanxuanxn.top

Go:   func main()
来源：http://mng.chenjidiqi.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rmu.hywenlv.cn

C#:   static void Main(string[] args)
来源：http://mch.fzhhl.top

[M08] 获取系统与运行时信息
来源：http://jap.bbcook.cn

Py:   platform.system();  platform.python_version()
来源：http://xgp.52xcode.cn

PHP:  PHP_OS;  phpversion();
来源：http://nyp.316326.xyz

JS:   process.platform;  process.version
来源：http://qgf.birdmap.top

TS:   process.platform;  process.version
来源：http://kwf.wangdashe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gkn.chenjidiqi.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://hpv.uphjek.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://utw.daxiang520.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gey.316326.xyz

================================================================================
来源：http://tng.ppjwa.cn

N. 数据结构与算法
来源：http://azb.gaohongyu789.top

================================================================================
来源：http://veg.gotoacloud.top

[N01] 二分查找（有序数组）
来源：http://vdq.dianchejie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://msz.iojbl.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nxy.fehbvm.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://viw.birdmap.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hxt.fehbvm.com

Java: Arrays.binarySearch(arr, x)
来源：http://upl.hysaishi.cn

Go:   sort.SearchInts(arr, x)
来源：http://bkk.vqdsnc.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qpr.c1oappe.top

C#:   Array.BinarySearch(arr, x)
来源：http://kag.0kj1m.cn

[N02] 排序（工程实践用内置实现）
来源：http://iba.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://fuh.yfazqb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zlu.yonumen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lgx.gotoacloud.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ohj.hesvh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jyg.zhiwuduotai.top

Go:   slices.Sort(arr)
来源：http://qqz.wangdashe.top

Ruby: arr.sort
来源：http://mpc.hesvh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dpx.smart0.xyz

[N03] 快速排序（分治示例）
来源：http://svn.chenjidiqi.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pjh.wangshuangyany.cn

PHP:  // 递归实现，或用 usort
来源：http://rsw.pycfn.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zjl.ctjpmb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tcx.iojbl.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ika.jyoumei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://urg.fktsv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dch.birdmap.top

C#:   // 手写递归，或 Array.Sort
来源：http://bhx.xuanzx.com

[N04] 斐波那契数列
来源：http://fap.tian-w.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zrf.hesvh.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://spd.yj202588.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uax.fktsv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vrr.guowangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uvd.guannengcc.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rje.havefunace.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gsl.sjlbkw.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jik.hcnkem.com

[N05] 最大公约数
来源：http://nxd.sjlbkw.cn

Py:   math.gcd(a, b)
来源：http://htr.hammf.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tdj.yfazqb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jha.hysaishi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cwd.jinghuilouyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zwe.316326.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://efo.52xcode.cn

Ruby: a.gcd(b)
来源：http://xxm.chenlongwang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://asl.chenlongwang.top

[N06] 判断回文字符串
来源：http://vhk.sweek.top

Py:   s == s[::-1]
来源：http://hrb.jinyuanbaomall.cn

PHP:  $s === strrev($s);
来源：http://bed.yonumen.top

JS:   s === [...s].reverse().join("")
来源：http://rux.aizwys.cn

TS:   s === [...s].reverse().join("")
来源：http://bhf.cdnleiting.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rnx.uphjek.com

Go:   // 双指针从两端比较
来源：http://hlm.guowangkeji.top

Ruby: s == s.reverse
来源：http://pop.quarkkingdee.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qwu.fanxiaobao.xyz

[N07] 两数之和（返回下标）
来源：http://gtz.xingfuxueyuan.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cvr.yangfankeji.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uey.zhixingplan.top

JS:   // 手写 Map：map.set(v, i)
来源：http://uou.vehdjk.com

TS:   // 手写 Map<string, number>
来源：http://wij.hysaishi.cn

Java: // 手写 HashMap
来源：http://sth.iojbl.cn

Go:   // 手写 map[int]int
来源：http://gyx.yj20258888.top

Ruby: // 手写 Hash
来源：http://kma.ehwqpu.com

C#:   // 手写 Dictionary<int, int>
来源：http://zpz.andypj.xyz

[N08] 生成全排列
来源：http://knm.jlsjyb.cn

Py:   itertools.permutations(arr)
来源：http://dos.52xcode.cn

PHP:  // 手写递归交换
来源：http://jrn.316326.xyz

JS:   // 手写回溯递归
来源：http://hwd.aibaodan.cn

TS:   // 手写回溯递归
来源：http://xwj.hesvh.cn

Java: // 手写回溯递归
来源：http://yaw.smart0.xyz

Go:   // 手写回溯递归
来源：http://wnk.uphjek.com

Ruby: arr.permutation.to_a
来源：http://quj.dashuyun.cn

C#:   // 手写回溯递归
来源：http://mfe.ydjk.org.cn

[N09] 栈与队列
来源：http://nvt.smart0.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wfs.yvedp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gmy.ydjk.org.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sak.mhx1999.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mwf.dianchejie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rpj.snrcjt.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wxm.cdnleiting.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ccy.9152youxi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eqk.mhx1999.top

[N10] 链表节点定义
来源：http://mhm.cqqwz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pui.smart0.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://drm.tianlin.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hpn.shanyushiyangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nci.nwbrower.top

Java: class Node { int v; Node next; }
来源：http://knq.aizwys.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ait.zdqjudy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tfm.gaohongyu789.top

C#:   class Node { public int V; public Node? Next; }
来源：http://pxc.chenjidiqi.icu

[N11] 二叉树中序遍历
来源：http://pto.ywan-chungtsiang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aok.ctjpmb.com

PHP:  // 手写递归函数
来源：http://xyv.ivvv.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vhr.aizwys.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dyf.vqdsnc.cn

Java: // 手写递归
来源：http://vdy.zhongyouzk.top

Go:   // 手写递归
来源：http://ktn.yj20258888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vsv.zhengqikj.top

C#:   // 手写递归
来源：http://cnj.guannengcc.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qrf.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rdi.xuetiantiany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sey.zhixingplan.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bnx.zycfv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rwo.tanke756.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://swj.zhengqikj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yku.xinyue.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://znv.fktsv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ejb.zhaomingkeji.xyz

================================================================================
来源：http://ylm.xylfe.cn

O. 并发与异步
来源：http://vjd.sweek.top

================================================================================
来源：http://vst.chenlongwang.top

[O01] 启动一个线程
来源：http://iqj.yuxming.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://frl.yj20258.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jdk.smart0.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://adb.xuanzx.com

TS:   // 同 JS
来源：http://oit.havefunace.top


<!-- 参考信息 -->