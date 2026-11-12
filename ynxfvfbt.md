代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cqt.gotoacloud.top

[K03] JSON 美化输出（带缩进）
来源：http://yua.52xcode.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://asd.cqqwz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rqk.ppjwa.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://iqs.cheryme.top

TS:   JSON.stringify(obj, null, 2)
来源：http://kog.aibaodan.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qqa.tianlin.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pqw.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://xpg.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xtm.pengpengdd.cyou

[K04] 读取 JSON 文件
来源：http://zmb.ydzc1.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vop.yueranfly.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hvm.fktsv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tds.epnwcf.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dow.yj202588.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iei.tianlin.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://piz.yuxming.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hvm.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bbl.shzxlz.cn

[K05] 深拷贝对象
来源：http://ugf.yvedp.cn

Py:   copy.deepcopy(obj)
来源：http://zzk.fengsongda.top

PHP:  unserialize(serialize($obj));
来源：http://zrq.zycfv.cn

JS:   structuredClone(obj)
来源：http://yes.yj20258888.top

TS:   structuredClone(obj)
来源：http://bii.hongshengwenyu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://uvx.sweek.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://abx.quarkkingdee.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mle.chenlongwang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://aya.jinyuanbaomall.cn

[K06] 解析 URL 查询串
来源：http://eiv.zhaomingkeji.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cgn.ydjk.org.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qkk.epnwcf.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zmg.hesvh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://azr.shuidangran.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://scc.fengsongda.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://shc.mhx1999.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dpi.jianghu66.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://com.sjlbkw.cn

[K07] 进制转换
来源：http://cwm.andypj.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xny.guowangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jem.gaohongyu789.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wfo.fktsv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qhf.cdnleiting.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ypd.jqgufenzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ubh.xinyue.icu

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yqk.tianlin.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rzo.hesvh.cn

[K08] 二进制序列化（非 JSON）
来源：http://wbh.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://yky.iojbl.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gcs.cucudq.cn

JS:   v8.serialize(obj)        // Node
来源：http://oca.hcnkem.com

TS:   v8.serialize(obj)        // Node
来源：http://asw.andypj.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://osu.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://gad.uphjek.com

Ruby: Marshal.dump(obj)
来源：http://wcr.redwolf501.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pps.xuetiantiany.cn

================================================================================
来源：http://qsa.jinqigufen.top

L. 网络请求
来源：http://naj.hnxiangtu.top

================================================================================
来源：http://hll.hnqzz.top

[L01] 发送 GET 请求
来源：http://zhg.zhijiandao.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jlo.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jql.cqqwz.cn

JS:   await fetch(url)
来源：http://cfl.iojbl.cn

TS:   await fetch(url)
来源：http://upy.aibaodan.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wpf.kuanghao11.cn

Go:   resp, err := http.Get(url)
来源：http://iey.sjlbkw.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xft.yj202588.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bnn.ehwqpu.com

[L02] 发送 POST JSON
来源：http://uya.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kdu.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fpg.bbcook.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zcz.kuanghao11.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gtw.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fby.sweek.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lkw.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kfh.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uqp.yj20258.top

[L03] 设置自定义请求头
来源：http://elg.daxiang520.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hzp.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ogq.vehdjk.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jsn.xziqi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nhr.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lxk.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fim.yuanzhike.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qcm.xinyue.icu

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://noa.xingfuxueyuan.xyz

[L04] 设置超时
来源：http://skc.fzhhl.top

Py:   requests.get(url, timeout=5)
来源：http://duh.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mlt.andypj.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://okz.tian-w.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dco.jinyuanbaomall.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://okg.tarul.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iyp.yueranfly.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://prq.cashguo.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://htc.guowangkeji.top

[L05] 上传文件（multipart）
来源：http://fqi.chenzaomai.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://urv.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mff.zhixingplan.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ssj.xinyue.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://llo.zhoulong.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zwa.redwolf501.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qyg.yanxiufei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gap.yuxming.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://orj.zhijiandao.cn

[L06] 解析响应为 JSON
来源：http://eyc.sjlbkw.cn

Py:   resp.json()
来源：http://ztg.yonumen.top

PHP:  json_decode($body, true);
来源：http://zxo.zhengqikj.top

JS:   await resp.json()
来源：http://fpe.jiagoushi.top

TS:   await resp.json()
来源：http://odw.cqqwz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tjk.guowangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gti.xylfe.cn

Ruby: JSON.parse(resp.body)
来源：http://tdp.jlsjyb.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tsu.vqdsnc.cn

[L07] 处理 HTTP 状态码
来源：http://jrd.tanke756.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cpn.jinqigufen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ztw.haohaochexian.top

JS:   resp.ok;  resp.status
来源：http://hrk.ehwqpu.com

TS:   resp.ok;  resp.status
来源：http://frv.xziqi.cn

Java: resp.statusCode()
来源：http://fil.fanxiaobao.xyz

Go:   resp.StatusCode
来源：http://xnn.yangfankeji.com

Ruby: resp.code.to_i
来源：http://esd.yuanzhike.top

C#:   (int)resp.StatusCode
来源：http://joa.dianchejie.cn

[L08] 并发请求多个地址
来源：http://wlm.9152youxi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yhm.cqqwz.cn

PHP:  curl_multi_init() 系列
来源：http://mhw.gzhubu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ugf.redwolf501.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ozw.ppjwa.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://opw.cdnleiting.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cqd.cucudq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dpo.bbcook.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ukq.pycfn.com

================================================================================
来源：http://uga.jqgufenzy.top

M. 命令行 / 进程 / 环境
来源：http://kvh.zhijiandao.cn

================================================================================
来源：http://svy.vehdjk.com

[M01] 读取命令行参数
来源：http://ugx.xuetiantiany.cn

Py:   sys.argv[1:]
来源：http://oea.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://ctf.shanyushiyangkeji.top

JS:   process.argv.slice(2)
来源：http://mvr.fanxiaobao.xyz

TS:   process.argv.slice(2)
来源：http://zzh.yj20258.top

Java: args 数组（main 方法参数）
来源：http://oec.hesvh.cn

Go:   os.Args[1:]
来源：http://gqo.mhx1999.top

Ruby: ARGV
来源：http://brw.ehwqpu.com

C#:   args 数组（Main 方法参数）
来源：http://jev.316326.xyz

[M02] 读取环境变量
来源：http://meh.snrcjt.cn

Py:   os.environ.get("HOME")
来源：http://lqq.tarul.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ckf.jinghuilouyu.cn

JS:   process.env.HOME
来源：http://jns.zhixingplan.top

TS:   process.env.HOME
来源：http://gqr.52xcode.cn

Java: System.getenv("HOME")
来源：http://ulw.jinqigfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lye.mhx1999.top

Ruby: ENV["HOME"]
来源：http://ucj.smart0.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bni.dianchejie.cn

[M03] 执行外部命令
来源：http://txp.wangshuangyany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yuc.cucudq.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vor.sysykeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://yrb.vehdjk.com

TS:   child_process.execSync("ls -l").toString()
来源：http://emy.birdmap.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://brx.ivvv.top

Go:   exec.Command("ls", "-l").Output()
来源：http://eet.hnqzz.top

Ruby: system("ls -l");  `ls -l`
来源：http://nqz.ydjk.org.cn

C#:   Process.Start("ls", "-l");
来源：http://qcw.xziqi.cn

[M04] 获取当前工作目录
来源：http://hzd.yangfankeji.com

Py:   os.getcwd()
来源：http://enj.haohaochexian.top

PHP:  getcwd();
来源：http://jmn.pengpengdd.cyou

JS:   process.cwd()
来源：http://gxe.0kj1m.cn

TS:   process.cwd()
来源：http://yrs.xylfe.cn

Java: Path.of("").toAbsolutePath()
来源：http://ijr.xinyue.icu

Go:   os.Getwd()
来源：http://khq.jinyuanbaomall.cn

Ruby: Dir.pwd
来源：http://wye.zdbjq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jzh.jinghuilouyu.cn

[M05] 设置退出码
来源：http://dzi.nanxuanxn.top

Py:   sys.exit(1)
来源：http://lvb.quarkkingdee.top

PHP:  exit(1);
来源：http://kpg.xuanzx.com

JS:   process.exit(1)
来源：http://pfh.ybcxt.top

TS:   process.exit(1)
来源：http://fiy.jinqigufen.top

Java: System.exit(1)
来源：http://qxe.wangshuangyany.cn

Go:   os.Exit(1)
来源：http://xsc.0kj1m.cn

Ruby: exit 1
来源：http://wnh.shanyushiyangtech.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ien.ivvv.top

[M06] 向标准错误输出
来源：http://acs.jlsjyb.cn

Py:   print("err", file=sys.stderr)
来源：http://tpq.zhixingplan.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ylh.jyoumei.cn

JS:   console.error("err")
来源：http://hxp.jqgufenzy.top

TS:   console.error("err")
来源：http://fzc.vqdsnc.cn

Java: System.err.println("err")
来源：http://fop.fzhhl.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mfq.fktsv.cn

Ruby: warn "err"
来源：http://hak.chenlongwang.top

C#:   Console.Error.WriteLine("err")
来源：http://mwc.dianchejie.cn

[M07] 判断是否为主入口
来源：http://wca.shanyushiyangtech.top

Py:   if __name__ == "__main__":
来源：http://ulr.jqgufenzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pnk.bjfxy.top

JS:   require.main === module
来源：http://hbd.sxryk.cn

TS:   require.main === module
来源：http://ztw.tian-w.cn

Java: public static void main(String[] args)
来源：http://aga.guannengcc.top

Go:   func main()
来源：http://wjs.fengsongda.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tjy.shzxlz.cn

C#:   static void Main(string[] args)
来源：http://bzs.redwolf501.top

[M08] 获取系统与运行时信息
来源：http://lmc.jqgfzy.top

Py:   platform.system();  platform.python_version()
来源：http://ctv.9152youxi.cn

PHP:  PHP_OS;  phpversion();
来源：http://oas.9152youxi.cn

JS:   process.platform;  process.version
来源：http://tmq.fehbvm.com

TS:   process.platform;  process.version
来源：http://ulj.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gud.shangyingyoupin.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://voe.sxryk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bco.meibo888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://pmk.yj20258.top

================================================================================
来源：http://pmx.aibaodan.cn

N. 数据结构与算法
来源：http://ehb.zhixingplan.top

================================================================================
来源：http://nah.wangdashe.top

[N01] 二分查找（有序数组）
来源：http://bqj.zhaomingkeji.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://rfe.hammf.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://crj.cheryme.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qez.ybcxt.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pdr.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://zvy.zhengqikj.top

Go:   sort.SearchInts(arr, x)
来源：http://evw.ydjk.org.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://eiz.hnxiangtu.top

C#:   Array.BinarySearch(arr, x)
来源：http://zvv.tian-w.cn

[N02] 排序（工程实践用内置实现）
来源：http://umr.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://qqd.ivvv.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cyw.fktsv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ohb.jyoumei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dnq.zhiwuduotai.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://svk.snrcjt.cn

Go:   slices.Sort(arr)
来源：http://xlo.0kj1m.cn

Ruby: arr.sort
来源：http://kcv.smart0.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://ljj.cdnleiting.top

[N03] 快速排序（分治示例）
来源：http://uom.fktsv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://twm.nanxinkj.top

PHP:  // 递归实现，或用 usort
来源：http://fin.yvedp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gph.yuanzhike.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hka.yonumen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kdp.yonumen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zjc.ybcxt.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kbs.ydzc1.top

C#:   // 手写递归，或 Array.Sort
来源：http://orl.jqgfzy.top

[N04] 斐波那契数列
来源：http://vgh.yj202588.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ghg.snrcjt.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ydw.zhoulong.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lds.xuanzx.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fwo.9152youxi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ggd.jianghu66.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tus.ydzc1.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rsc.jinyuanbaomall.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qny.shanyushiyangtech.top

[N05] 最大公约数
来源：http://ldx.gzhubu.top

Py:   math.gcd(a, b)
来源：http://mdu.jqgfzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jhj.xuanzx.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ktj.chenlongwang.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hds.smart0.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qlu.chenjidiqi.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mfe.xziqi.cn

Ruby: a.gcd(b)
来源：http://dgi.yj20258.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://usc.jiagoushi.top

[N06] 判断回文字符串
来源：http://sjr.pengpengdd.cyou

Py:   s == s[::-1]
来源：http://zam.mhx1999.top

PHP:  $s === strrev($s);
来源：http://dbp.cqqwz.cn

JS:   s === [...s].reverse().join("")
来源：http://xvo.redwolf501.top

TS:   s === [...s].reverse().join("")
来源：http://oed.feifeiyinyue.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sfa.havefunace.top

Go:   // 双指针从两端比较
来源：http://oqc.yj202588.top

Ruby: s == s.reverse
来源：http://ikx.0kj1m.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kvo.daria6918.cn

[N07] 两数之和（返回下标）
来源：http://mnh.jinqigfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mpu.shanyushiyangtech.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ylc.meibo888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://grf.yangfankeji.com

TS:   // 手写 Map<string, number>
来源：http://mgp.fzhhl.top

Java: // 手写 HashMap
来源：http://mpp.hesvh.cn

Go:   // 手写 map[int]int
来源：http://mja.gzhubu.top

Ruby: // 手写 Hash
来源：http://zxb.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://jlm.yueranfly.top

[N08] 生成全排列
来源：http://pbt.kuanghao11.cn

Py:   itertools.permutations(arr)
来源：http://mgj.cdnleiting.top

PHP:  // 手写递归交换
来源：http://lou.daria6918.cn

JS:   // 手写回溯递归
来源：http://eyb.yj202588.top

TS:   // 手写回溯递归
来源：http://vex.fanxiaobao.xyz

Java: // 手写回溯递归
来源：http://twe.wangdashe.top

Go:   // 手写回溯递归
来源：http://rav.meibo888.top

Ruby: arr.permutation.to_a
来源：http://qxy.shzxlz.cn

C#:   // 手写回溯递归
来源：http://jvh.uphjek.com

[N09] 栈与队列
来源：http://ett.yuanzhike.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ifd.aibaodan.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lqd.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://brn.kuanghao11.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yoe.sjlbkw.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ull.sxryk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tme.c1oappe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sfl.hcnkem.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lfu.wangdashe.top

[N10] 链表节点定义
来源：http://txc.316326.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tqu.ydzc1.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lwi.yj20258.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rjf.sjlbkw.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dio.fehbvm.com

Java: class Node { int v; Node next; }
来源：http://yts.jinyuanbaomall.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fcj.hongshengwenyu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zct.yongpay.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ukw.xylfe.cn

[N11] 二叉树中序遍历
来源：http://lzt.dianchejie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://awu.0kj1m.cn


<!-- 参考信息 -->