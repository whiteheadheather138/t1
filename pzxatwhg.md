代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://zdk.dashuyun.cn

PHP:  unserialize(serialize($obj));
来源：http://sfg.jqgufenzy.top

JS:   structuredClone(obj)
来源：http://arh.vqdsnc.cn

TS:   structuredClone(obj)
来源：http://jtt.dashuyun.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://drq.sysykeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yli.tian-w.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xjk.fktsv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wxk.dashuyun.cn

[K06] 解析 URL 查询串
来源：http://xth.feifeiyinyue.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sdk.zhaomingkeji.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jho.wangshuangyany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bao.zycfv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ovm.hongshengwenyu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nbl.meibo888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://maa.yj202588.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cns.yj202588.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tsm.bjfxy.top

[K07] 进制转换
来源：http://rqj.fanxiaobao.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lzt.gaohongyu789.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://frf.jinyuanbaomall.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://meb.cdnleiting.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oeu.hfpthk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vco.hammf.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kbj.jqgfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qeh.ydjk.org.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mce.xingfuxueyuan.xyz

[K08] 二进制序列化（非 JSON）
来源：http://ctd.xinyue.icu

Py:   pickle.dumps(obj)
来源：http://jdo.aizwys.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pdg.jqgfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://yoq.jiagoushi.top

TS:   v8.serialize(obj)        // Node
来源：http://rwl.zhongyouzk.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mqk.hnqzz.top

Go:   encoding/gob
来源：http://skz.9152youxi.cn

Ruby: Marshal.dump(obj)
来源：http://huu.sjlbkw.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fdr.aizwys.cn

================================================================================
来源：http://idy.yj20258888.top

L. 网络请求
来源：http://ykv.zdqjudy.top

================================================================================
来源：http://npc.0kj1m.cn

[L01] 发送 GET 请求
来源：http://ies.fehbvm.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://akv.ydjk.org.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://utk.zhixingplan.top

JS:   await fetch(url)
来源：http://uzk.epnwcf.com

TS:   await fetch(url)
来源：http://gdd.c1oappe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lly.jiagoushi.top

Go:   resp, err := http.Get(url)
来源：http://efc.gogol.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://efd.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kzi.gogol.net.cn

[L02] 发送 POST JSON
来源：http://jjl.yj20258.top

Py:   requests.post(url, json={"a": 1})
来源：http://ipw.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wbi.tanke756.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ynv.xylfe.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nwe.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ywr.epnwcf.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://szf.hnqzz.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nom.daxiang520.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hcg.ywan-chungtsiang.top

[L03] 设置自定义请求头
来源：http://gbc.shzxlz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://upo.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://voa.shanyushiyangtech.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ysp.ppjwa.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oun.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rjl.zhixingplan.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ygk.ywan-chungtsiang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cvy.bbcook.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dgd.nanxinkj.top

[L04] 设置超时
来源：http://mju.zhiwuduotai.top

Py:   requests.get(url, timeout=5)
来源：http://cba.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tko.tianlin.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eyr.zdbjq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vuv.hesvh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dvn.shanyushiyangtech.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wfy.ybcxt.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gkb.316326.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nms.jyoumei.cn

[L05] 上传文件（multipart）
来源：http://swq.hcnkem.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vxe.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lwp.xingfuxueyuan.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hmu.cucudq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xlr.sweek.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bsc.cheryme.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zix.cdnleiting.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nba.svipenyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vtg.vqdsnc.cn

[L06] 解析响应为 JSON
来源：http://dze.shuidangran.top

Py:   resp.json()
来源：http://ekt.gzhubu.top

PHP:  json_decode($body, true);
来源：http://kcr.nwbrower.top

JS:   await resp.json()
来源：http://orx.hywenlv.cn

TS:   await resp.json()
来源：http://psq.mhx1999.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ltt.shanyushiyangtech.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nmg.hfpthk.cn

Ruby: JSON.parse(resp.body)
来源：http://dik.52xcode.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bcq.sjlbkw.cn

[L07] 处理 HTTP 状态码
来源：http://wiz.redwolf501.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://iiy.sysykeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xyc.xuetiantiany.cn

JS:   resp.ok;  resp.status
来源：http://qso.yuanzhike.top

TS:   resp.ok;  resp.status
来源：http://xnm.zdbjq.cn

Java: resp.statusCode()
来源：http://kqw.jinyuanbaomall.cn

Go:   resp.StatusCode
来源：http://ikx.yonumen.top

Ruby: resp.code.to_i
来源：http://bxq.shzxlz.cn

C#:   (int)resp.StatusCode
来源：http://fhm.guannengcc.top

[L08] 并发请求多个地址
来源：http://lub.cashguo.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wdj.jqgufenzy.top

PHP:  curl_multi_init() 系列
来源：http://yfe.hfpthk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://svm.hysaishi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fzn.shanyushiyangtech.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gkp.ehwqpu.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dmk.zhixingplan.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bvl.yongpay.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sdi.mhx1999.top

================================================================================
来源：http://yvl.yonumen.top

M. 命令行 / 进程 / 环境
来源：http://uuc.nanxinkj.top

================================================================================
来源：http://gks.gogol.net.cn

[M01] 读取命令行参数
来源：http://rii.uphjek.com

Py:   sys.argv[1:]
来源：http://jit.daxiang520.top

PHP:  $argv;  $argc;
来源：http://vjl.vehdjk.com

JS:   process.argv.slice(2)
来源：http://xui.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://eli.jianghu66.top

Java: args 数组（main 方法参数）
来源：http://eer.aibaodan.cn

Go:   os.Args[1:]
来源：http://teo.jqgfzy.top

Ruby: ARGV
来源：http://maw.zhengqikj.top

C#:   args 数组（Main 方法参数）
来源：http://inj.9152youxi.cn

[M02] 读取环境变量
来源：http://iis.cashguo.top

Py:   os.environ.get("HOME")
来源：http://vrd.pycfn.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ybe.ywan-chungtsiang.top

JS:   process.env.HOME
来源：http://glm.gotoacloud.top

TS:   process.env.HOME
来源：http://iuu.sjlbkw.cn

Java: System.getenv("HOME")
来源：http://tjz.cucudq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ipl.jiagoushi.top

Ruby: ENV["HOME"]
来源：http://mbj.aizwys.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nwi.shanyushiyangtech.top

[M03] 执行外部命令
来源：http://ces.zhaomingkeji.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://abo.jinyuanbaomall.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nlo.nanxuanxn.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xtg.xylfe.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ezt.jlsjyb.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gqj.snrcjt.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qoz.shanyushiyangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://nnr.daxiang520.top

C#:   Process.Start("ls", "-l");
来源：http://lpj.epnwcf.com

[M04] 获取当前工作目录
来源：http://hbk.zhixingplan.top

Py:   os.getcwd()
来源：http://ygj.zhengqikj.top

PHP:  getcwd();
来源：http://oeq.xuanzx.com

JS:   process.cwd()
来源：http://mpg.epnwcf.com

TS:   process.cwd()
来源：http://inc.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://cof.shuidangran.top

Go:   os.Getwd()
来源：http://tmj.iojbl.cn

Ruby: Dir.pwd
来源：http://jzw.nwbrower.top

C#:   Directory.GetCurrentDirectory()
来源：http://uyc.ivvv.top

[M05] 设置退出码
来源：http://syg.haohaochexian.top

Py:   sys.exit(1)
来源：http://ddq.birdmap.top

PHP:  exit(1);
来源：http://bew.ehwqpu.com

JS:   process.exit(1)
来源：http://gvn.yuanzhike.top

TS:   process.exit(1)
来源：http://vui.chenlongwang.top

Java: System.exit(1)
来源：http://hjv.9152youxi.cn

Go:   os.Exit(1)
来源：http://pfg.gaohongyu789.top

Ruby: exit 1
来源：http://vrj.jinqigfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yud.ydjk.org.cn

[M06] 向标准错误输出
来源：http://kuz.zhiwuduotai.top

Py:   print("err", file=sys.stderr)
来源：http://fqt.yj20258.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hvb.yuanzhike.top

JS:   console.error("err")
来源：http://gno.sjlbkw.cn

TS:   console.error("err")
来源：http://rvx.xuetiantiany.cn

Java: System.err.println("err")
来源：http://xuq.xuetiantiany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ubq.zhongyouzk.top

Ruby: warn "err"
来源：http://azl.vehdjk.com

C#:   Console.Error.WriteLine("err")
来源：http://yav.dianchejie.cn

[M07] 判断是否为主入口
来源：http://lly.ywan-chungtsiang.top

Py:   if __name__ == "__main__":
来源：http://lkq.hcnkem.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mff.bbcook.cn

JS:   require.main === module
来源：http://svk.epnwcf.com

TS:   require.main === module
来源：http://cpg.svipenyu.cn

Java: public static void main(String[] args)
来源：http://ddo.andypj.xyz

Go:   func main()
来源：http://epp.zycfv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eea.meibo888.top

C#:   static void Main(string[] args)
来源：http://vsn.jinyuanbaomall.cn

[M08] 获取系统与运行时信息
来源：http://drn.jqgfzy.top

Py:   platform.system();  platform.python_version()
来源：http://xha.yfazqb.com

PHP:  PHP_OS;  phpversion();
来源：http://igl.gogol.net.cn

JS:   process.platform;  process.version
来源：http://utj.ydjk.org.cn

TS:   process.platform;  process.version
来源：http://nci.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ilk.pengpengdd.cyou

Go:   runtime.GOOS;  runtime.Version()
来源：http://qrp.xinyue.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cmr.meibo888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qlp.jqgfzy.top

================================================================================
来源：http://hps.yuxming.cn

N. 数据结构与算法
来源：http://pbw.svipenyu.cn

================================================================================
来源：http://wpw.dianchejie.cn

[N01] 二分查找（有序数组）
来源：http://ygf.tanke756.top

Py:   bisect.bisect_left(arr, x)
来源：http://drx.yuxming.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bdl.hfpthk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://otr.xinyue.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://isp.hywenlv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wdn.epnwcf.com

Go:   sort.SearchInts(arr, x)
来源：http://bcj.wangshuangyany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lcd.zdbjq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fip.wangdashe.top

[N02] 排序（工程实践用内置实现）
来源：http://tmm.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://tyu.yonumen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ezu.smart0.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://eff.vqdsnc.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://smv.yueranfly.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jre.bjfxy.top

Go:   slices.Sort(arr)
来源：http://hjc.dianchejie.cn

Ruby: arr.sort
来源：http://frr.vqdsnc.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xnf.yangfankeji.com

[N03] 快速排序（分治示例）
来源：http://wms.daxiang520.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qyr.cqqwz.cn

PHP:  // 递归实现，或用 usort
来源：http://qkj.meibo888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tdg.xuanzx.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lfb.xziqi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vtu.daria6918.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://prw.sweek.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jqe.0kj1m.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lkh.uphjek.com

[N04] 斐波那契数列
来源：http://vio.hongshengwenyu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qjg.sysykeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kfv.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zon.hnxiangtu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ppm.jianghu66.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lub.zhaomingkeji.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://doy.zdbjq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wqu.sufxvd.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fvl.zdqjudy.top

[N05] 最大公约数
来源：http://vgw.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://mqt.zhixingplan.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bfc.snrcjt.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jjp.uphjek.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://byb.zhiwuduotai.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ajv.chenjidiqi.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dis.gogol.net.cn

Ruby: a.gcd(b)
来源：http://grk.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://paa.zhiwuduotai.top

[N06] 判断回文字符串
来源：http://ikw.gotoacloud.top

Py:   s == s[::-1]
来源：http://yhh.jyoumei.cn

PHP:  $s === strrev($s);
来源：http://nkm.sxryk.cn

JS:   s === [...s].reverse().join("")
来源：http://cpk.cashguo.top

TS:   s === [...s].reverse().join("")
来源：http://paj.c1oappe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nij.smart0.xyz

Go:   // 双指针从两端比较
来源：http://vce.dianchejie.cn

Ruby: s == s.reverse
来源：http://pse.pengpengdd.cyou

C#:   s == new string(s.Reverse().ToArray())
来源：http://syr.9152youxi.cn

[N07] 两数之和（返回下标）
来源：http://qhg.hcnkem.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://aka.52xcode.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qoq.fzhhl.top

JS:   // 手写 Map：map.set(v, i)
来源：http://cpw.aizwys.cn

TS:   // 手写 Map<string, number>
来源：http://otw.sysykeji.top

Java: // 手写 HashMap
来源：http://xad.vehdjk.com

Go:   // 手写 map[int]int
来源：http://oum.wangdashe.top

Ruby: // 手写 Hash
来源：http://sip.gzhubu.top

C#:   // 手写 Dictionary<int, int>
来源：http://zmg.kuanghao11.cn

[N08] 生成全排列
来源：http://gqn.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://aqg.hesvh.cn

PHP:  // 手写递归交换
来源：http://uxd.fehbvm.com

JS:   // 手写回溯递归
来源：http://ksm.svipenyu.cn

TS:   // 手写回溯递归
来源：http://aiz.ydjk.org.cn

Java: // 手写回溯递归
来源：http://pvl.chenlongwang.top

Go:   // 手写回溯递归
来源：http://sht.guannengcc.top

Ruby: arr.permutation.to_a
来源：http://ipq.xuanzx.com

C#:   // 手写回溯递归
来源：http://zqv.52xcode.cn

[N09] 栈与队列
来源：http://nhg.gotoacloud.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://npp.jiagoushi.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://smb.xylfe.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ktd.epnwcf.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fkq.fanxiaobao.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iwt.zhiwuduotai.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wco.sufxvd.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gsr.sysykeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dfh.epnwcf.com

[N10] 链表节点定义
来源：http://csp.guowangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oju.fktsv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://eie.epnwcf.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jhz.cashguo.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cay.yj20258888.top

Java: class Node { int v; Node next; }
来源：http://itb.hnqzz.top

Go:   type Node struct { V int; Next *Node }
来源：http://agf.chenlongwang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wkj.meibo888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wqy.cqqwz.cn

[N11] 二叉树中序遍历
来源：http://uam.xuetiantiany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rqn.jlsjyb.cn

PHP:  // 手写递归函数
来源：http://wov.hongshengwenyu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nvq.yuanzhike.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gpk.sweek.top

Java: // 手写递归
来源：http://ngu.fengsongda.top

Go:   // 手写递归
来源：http://bjo.ehwqpu.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vnz.nanxinkj.top

C#:   // 手写递归
来源：http://nfd.aibaodan.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cel.ppjwa.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kmf.tian-w.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uhz.hnxiangtu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tse.shanyushiyangtech.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vyr.sufxvd.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bxl.hfpthk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zsl.yanxiufei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sit.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bny.yvedp.cn

================================================================================
来源：http://dpa.zdqjudy.top

O. 并发与异步
来源：http://qbv.zhijiandao.cn

================================================================================
来源：http://ekk.pengpengdd.cyou

[O01] 启动一个线程
来源：http://imn.jqgfzy.top


<!-- 参考信息 -->