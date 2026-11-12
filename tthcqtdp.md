代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jlt.sjlbkw.cn

[K03] JSON 美化输出（带缩进）
来源：http://uxx.zhixingplan.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sws.wangshuangyany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uvs.sjlbkw.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fvz.hnqzz.top

TS:   JSON.stringify(obj, null, 2)
来源：http://kor.sjlbkw.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xee.0kj1m.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hmy.hywenlv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dlk.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tjg.fengsongda.top

[K04] 读取 JSON 文件
来源：http://jqv.shanyushiyangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hnh.zhiwuduotai.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fcn.fengsongda.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://svf.gaohongyu789.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://osu.guannengcc.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xvo.guowangkeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bhf.bbcook.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rvk.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kyd.jqgufenzy.top

[K05] 深拷贝对象
来源：http://tgn.jqgufenzy.top

Py:   copy.deepcopy(obj)
来源：http://snc.yvedp.cn

PHP:  unserialize(serialize($obj));
来源：http://tjl.dianchejie.cn

JS:   structuredClone(obj)
来源：http://xhw.nanxinkj.top

TS:   structuredClone(obj)
来源：http://ocf.quarkkingdee.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ydt.sxryk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vqh.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yun.zdbjq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qnz.hcnkem.com

[K06] 解析 URL 查询串
来源：http://gwk.zhijiandao.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cdm.hysaishi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://adi.snrcjt.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://usx.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zae.smart0.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mem.snrcjt.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://oci.yj20258.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://unb.52xcode.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xyd.gaohongyu789.top

[K07] 进制转换
来源：http://qsq.zhengqikj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wml.sxryk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wcg.ydjk.org.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lok.tian-w.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nxj.vqdsnc.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zki.xinyue.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rjt.jiagoushi.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mzp.jinqigufen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hyz.jyoumei.cn

[K08] 二进制序列化（非 JSON）
来源：http://bsy.0kj1m.cn

Py:   pickle.dumps(obj)
来源：http://jzv.pycfn.com

PHP:  serialize($obj);  unserialize($s);
来源：http://jht.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://bdn.gzhubu.top

TS:   v8.serialize(obj)        // Node
来源：http://psa.meibo888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cro.nanxinkj.top

Go:   encoding/gob
来源：http://rsb.zhaomingkeji.xyz

Ruby: Marshal.dump(obj)
来源：http://gkc.jianghu66.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qcx.yfazqb.com

================================================================================
来源：http://lwu.ehwqpu.com

L. 网络请求
来源：http://lcy.chenzaomai.com

================================================================================
来源：http://wna.sweek.top

[L01] 发送 GET 请求
来源：http://lwf.zhaomingkeji.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cvt.xziqi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cyd.ydjk.org.cn

JS:   await fetch(url)
来源：http://jqs.kuanghao11.cn

TS:   await fetch(url)
来源：http://vmw.jlsjyb.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qgf.jyoumei.cn

Go:   resp, err := http.Get(url)
来源：http://wfn.hcnkem.com

Ruby: Net::HTTP.get(URI(url))
来源：http://blv.tanke756.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ffc.meibo888.top

[L02] 发送 POST JSON
来源：http://skj.jiagoushi.top

Py:   requests.post(url, json={"a": 1})
来源：http://vht.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xip.andypj.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mep.daxiang520.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gvl.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nmo.fengsongda.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vaq.cdnleiting.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hzh.jqgufenzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rsu.kuanghao11.cn

[L03] 设置自定义请求头
来源：http://dfs.ivvv.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://whx.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ask.ywan-chungtsiang.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lhs.zhoulong.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gnf.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wor.wangshuangyany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fft.ehwqpu.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lka.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cwz.52xcode.cn

[L04] 设置超时
来源：http://rzp.ydjk.org.cn

Py:   requests.get(url, timeout=5)
来源：http://aha.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://anp.xuanzx.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://skz.0kj1m.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nmv.jinyuanbaomall.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://all.yangfankeji.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://idr.yuxming.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yec.jqgufenzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nfz.cucudq.cn

[L05] 上传文件（multipart）
来源：http://haa.xuanzx.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://din.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vdo.zhengqikj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://drb.zdqjudy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ogd.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xtc.jinqigfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ypm.iojbl.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zlc.sysykeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pqk.zdqjudy.top

[L06] 解析响应为 JSON
来源：http://kuv.guowangkeji.top

Py:   resp.json()
来源：http://xlv.sysykeji.top

PHP:  json_decode($body, true);
来源：http://ymm.tianlin.xyz

JS:   await resp.json()
来源：http://iar.uphjek.com

TS:   await resp.json()
来源：http://mwx.sufxvd.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nvp.xuetiantiany.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://muu.uphjek.com

Ruby: JSON.parse(resp.body)
来源：http://quh.svipenyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jhs.uphjek.com

[L07] 处理 HTTP 状态码
来源：http://sis.shanyushiyangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mip.vehdjk.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tns.sxryk.cn

JS:   resp.ok;  resp.status
来源：http://xue.jiagoushi.top

TS:   resp.ok;  resp.status
来源：http://dvh.jinghuilouyu.cn

Java: resp.statusCode()
来源：http://hng.yanxiufei.cn

Go:   resp.StatusCode
来源：http://fdx.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://srb.yuanzhike.top

C#:   (int)resp.StatusCode
来源：http://fiv.ctjpmb.com

[L08] 并发请求多个地址
来源：http://esg.9152youxi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dej.yanxiufei.cn

PHP:  curl_multi_init() 系列
来源：http://wlx.fengsongda.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sfk.shanyushiyangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hbx.zhijiandao.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yzn.shanyushiyangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sxz.hnqzz.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jsg.bjfxy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://due.bjfxy.top

================================================================================
来源：http://pyj.yonumen.top

M. 命令行 / 进程 / 环境
来源：http://xlu.hnqzz.top

================================================================================
来源：http://slv.zhixingplan.top

[M01] 读取命令行参数
来源：http://xmu.c1oappe.top

Py:   sys.argv[1:]
来源：http://hqg.316326.xyz

PHP:  $argv;  $argc;
来源：http://oun.bbcook.cn

JS:   process.argv.slice(2)
来源：http://chm.c1oappe.top

TS:   process.argv.slice(2)
来源：http://ikg.tanke756.top

Java: args 数组（main 方法参数）
来源：http://wei.ydzc1.top

Go:   os.Args[1:]
来源：http://khx.xylfe.cn

Ruby: ARGV
来源：http://vmo.dianchejie.cn

C#:   args 数组（Main 方法参数）
来源：http://orf.jianghu66.top

[M02] 读取环境变量
来源：http://crr.yongpay.top

Py:   os.environ.get("HOME")
来源：http://sbs.mhx1999.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://elq.haohaochexian.top

JS:   process.env.HOME
来源：http://lgt.hfpthk.cn

TS:   process.env.HOME
来源：http://afv.gotoacloud.top

Java: System.getenv("HOME")
来源：http://agi.chenzaomai.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vrx.xuanzx.com

Ruby: ENV["HOME"]
来源：http://bxr.xylfe.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zcn.cdnleiting.top

[M03] 执行外部命令
来源：http://dyo.shangyingyoupin.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qpl.hfpthk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wxo.ctjpmb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://emc.xinyue.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://lyy.zhixingplan.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xkn.jinqigufen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nvz.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ofz.xuanzx.com

C#:   Process.Start("ls", "-l");
来源：http://fei.meibo888.top

[M04] 获取当前工作目录
来源：http://pib.yvedp.cn

Py:   os.getcwd()
来源：http://ipm.tanke756.top

PHP:  getcwd();
来源：http://tao.hesvh.cn

JS:   process.cwd()
来源：http://vwc.xuanzx.com

TS:   process.cwd()
来源：http://uxm.chenzaomai.com

Java: Path.of("").toAbsolutePath()
来源：http://gmc.gotoacloud.top

Go:   os.Getwd()
来源：http://qah.jinqigufen.top

Ruby: Dir.pwd
来源：http://vxf.gaohongyu789.top

C#:   Directory.GetCurrentDirectory()
来源：http://woi.epnwcf.com

[M05] 设置退出码
来源：http://luj.vqdsnc.cn

Py:   sys.exit(1)
来源：http://nxm.zhiwuduotai.top

PHP:  exit(1);
来源：http://nna.0kj1m.cn

JS:   process.exit(1)
来源：http://dpy.sweek.top

TS:   process.exit(1)
来源：http://rai.fanxiaobao.xyz

Java: System.exit(1)
来源：http://nit.jinghuilouyu.cn

Go:   os.Exit(1)
来源：http://gxa.jqgfzy.top

Ruby: exit 1
来源：http://qhe.xinyue.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xpw.yj20258.top

[M06] 向标准错误输出
来源：http://dqi.jinghuilouyu.cn

Py:   print("err", file=sys.stderr)
来源：http://igh.wangdashe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ltc.yvedp.cn

JS:   console.error("err")
来源：http://bkc.tarul.cn

TS:   console.error("err")
来源：http://tav.xziqi.cn

Java: System.err.println("err")
来源：http://sqn.sxryk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wdt.jqgfzy.top

Ruby: warn "err"
来源：http://wga.fktsv.cn

C#:   Console.Error.WriteLine("err")
来源：http://mbx.yongpay.top

[M07] 判断是否为主入口
来源：http://hno.nanxinkj.top

Py:   if __name__ == "__main__":
来源：http://rnp.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cnt.wangdashe.top

JS:   require.main === module
来源：http://qop.yvedp.cn

TS:   require.main === module
来源：http://fiu.yj202588.top

Java: public static void main(String[] args)
来源：http://qoo.52xcode.cn

Go:   func main()
来源：http://gsw.sweek.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yae.ywan-chungtsiang.top

C#:   static void Main(string[] args)
来源：http://mdu.gzhubu.top

[M08] 获取系统与运行时信息
来源：http://ndf.hnxiangtu.top

Py:   platform.system();  platform.python_version()
来源：http://rsn.yj20258888.top

PHP:  PHP_OS;  phpversion();
来源：http://uzj.ybcxt.top

JS:   process.platform;  process.version
来源：http://xtk.xylfe.cn

TS:   process.platform;  process.version
来源：http://ptq.dianchejie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sjg.hcnkem.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://fpu.uphjek.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://htp.cheryme.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jbm.jlsjyb.cn

================================================================================
来源：http://ocy.yueranfly.top

N. 数据结构与算法
来源：http://hkf.cashguo.top

================================================================================
来源：http://cym.shanyushiyangtech.top

[N01] 二分查找（有序数组）
来源：http://fxj.jinqigfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://keb.sysykeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://syx.xinyue.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://owo.dashuyun.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fcx.meibo888.top

Java: Arrays.binarySearch(arr, x)
来源：http://jff.fzhhl.top

Go:   sort.SearchInts(arr, x)
来源：http://qjw.mhx1999.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ysf.chenlongwang.top

C#:   Array.BinarySearch(arr, x)
来源：http://ujd.gzhubu.top

[N02] 排序（工程实践用内置实现）
来源：http://qym.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://zyf.yj202588.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sch.haohaochexian.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bsw.sufxvd.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://utm.hfpthk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yhr.yj202588.top

Go:   slices.Sort(arr)
来源：http://usz.mhx1999.top

Ruby: arr.sort
来源：http://yud.daxiang520.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://maw.xinyue.icu

[N03] 快速排序（分治示例）
来源：http://zvw.9152youxi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nsn.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://bwt.hcnkem.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ary.tianlin.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dtz.wangdashe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ljf.xylfe.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://plz.epnwcf.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zlf.xziqi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fjx.chenlongwang.top

[N04] 斐波那契数列
来源：http://wcv.c1oappe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jdv.jqgufenzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wfy.svipenyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ybi.ppjwa.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yhk.meibo888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lak.smart0.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nxd.xziqi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zkv.xinyue.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lqy.hnxiangtu.top

[N05] 最大公约数
来源：http://qli.haohaochexian.top

Py:   math.gcd(a, b)
来源：http://oun.xinyue.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aip.meibo888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lmp.pengpengdd.cyou

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gfg.epnwcf.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rij.gogol.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ern.vqdsnc.cn

Ruby: a.gcd(b)
来源：http://yjo.pycfn.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pbw.aizwys.cn

[N06] 判断回文字符串
来源：http://iot.yuxming.cn

Py:   s == s[::-1]
来源：http://fhh.cheryme.top

PHP:  $s === strrev($s);
来源：http://xcv.yj20258.top

JS:   s === [...s].reverse().join("")
来源：http://xvt.yj20258888.top

TS:   s === [...s].reverse().join("")
来源：http://ivg.jyoumei.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nbr.yueranfly.top

Go:   // 双指针从两端比较
来源：http://pfi.aibaodan.cn

Ruby: s == s.reverse
来源：http://zry.nanxuanxn.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://baw.fzhhl.top

[N07] 两数之和（返回下标）
来源：http://ypm.tarul.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bqr.daxiang520.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uik.yvedp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sif.svipenyu.cn

TS:   // 手写 Map<string, number>
来源：http://lkt.wangshuangyany.cn

Java: // 手写 HashMap
来源：http://twu.zhoulong.xyz

Go:   // 手写 map[int]int
来源：http://ulq.feifeiyinyue.top

Ruby: // 手写 Hash
来源：http://mow.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gtq.shzxlz.cn

[N08] 生成全排列
来源：http://wvg.cqqwz.cn

Py:   itertools.permutations(arr)
来源：http://gmw.xinyue.icu

PHP:  // 手写递归交换
来源：http://hfe.cucudq.cn

JS:   // 手写回溯递归
来源：http://tkh.yongpay.top

TS:   // 手写回溯递归
来源：http://jdh.ybcxt.top

Java: // 手写回溯递归
来源：http://wyd.bbcook.cn

Go:   // 手写回溯递归
来源：http://mfl.shuidangran.top

Ruby: arr.permutation.to_a
来源：http://hin.aibaodan.cn

C#:   // 手写回溯递归
来源：http://wzt.yfazqb.com

[N09] 栈与队列
来源：http://wgk.sysykeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xtl.jianghu66.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mjy.gzhubu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fjw.yj20258888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iyu.hysaishi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xyg.shuidangran.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ihu.kuanghao11.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wwc.ybcxt.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ieb.hesvh.cn

[N10] 链表节点定义
来源：http://uji.hnqzz.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://slq.yj202588.top

PHP:  class Node { public $v; public $next = null; }
来源：http://oka.9152youxi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://byl.jlsjyb.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://utu.wangshuangyany.cn

Java: class Node { int v; Node next; }
来源：http://qhw.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://myt.jinqigufen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ivd.cqqwz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ybx.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://iow.ivvv.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eiv.ivvv.top


<!-- 参考信息 -->