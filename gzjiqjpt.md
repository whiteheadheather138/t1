代发 wailian999

TS:   JSON.parse(s)
来源：http://crp.sjlbkw.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://egu.hcnkem.com

Go:   json.Unmarshal(data, &v)
来源：http://cqi.redwolf501.top

Ruby: JSON.parse(s)
来源：http://uzb.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zxy.hnxiangtu.top

[K03] JSON 美化输出（带缩进）
来源：http://yqo.meibo888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yvf.chenzaomai.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://guj.zhiwuduotai.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pxd.fzhhl.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bgy.xziqi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://izf.wangdashe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ybv.shuidangran.top

Ruby: JSON.pretty_generate(obj)
来源：http://chm.yfazqb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gfj.shanyushiyangtech.top

[K04] 读取 JSON 文件
来源：http://ija.feifeiyinyue.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oki.vehdjk.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vlc.xinyue.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lhk.xinyue.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wgc.yonumen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://afr.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jcc.zhiwuduotai.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qis.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fme.yuanzhike.top

[K05] 深拷贝对象
来源：http://aiw.birdmap.top

Py:   copy.deepcopy(obj)
来源：http://atr.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://rcp.havefunace.top

JS:   structuredClone(obj)
来源：http://dqg.316326.xyz

TS:   structuredClone(obj)
来源：http://azm.tianlin.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://qnz.jiagoushi.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://srj.yonumen.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ddh.gogol.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hiy.nwbrower.top

[K06] 解析 URL 查询串
来源：http://bra.aibaodan.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bck.yj202588.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gfr.gotoacloud.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cij.nanxuanxn.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zip.cheryme.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cje.sxryk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bqk.pengpengdd.cyou

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fph.0kj1m.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ncw.ydzc1.top

[K07] 进制转换
来源：http://svb.jinqigfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wvr.nanxinkj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lkz.yj20258.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qzu.sjlbkw.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tob.yj20258888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ysm.guannengcc.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vix.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dub.shanyushiyangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ybi.sweek.top

[K08] 二进制序列化（非 JSON）
来源：http://hbf.fktsv.cn

Py:   pickle.dumps(obj)
来源：http://hpd.hnxiangtu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pgy.chenjidiqi.icu

JS:   v8.serialize(obj)        // Node
来源：http://swp.kuanghao11.cn

TS:   v8.serialize(obj)        // Node
来源：http://sya.xuetiantiany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rkv.sweek.top

Go:   encoding/gob
来源：http://uue.ydjk.org.cn

Ruby: Marshal.dump(obj)
来源：http://xss.jlsjyb.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ttv.zhoulong.xyz

================================================================================
来源：http://vsw.mhx1999.top

L. 网络请求
来源：http://arc.yueranfly.top

================================================================================
来源：http://vtp.0kj1m.cn

[L01] 发送 GET 请求
来源：http://tbc.hysaishi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qrh.smart0.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wkb.jlsjyb.cn

JS:   await fetch(url)
来源：http://uia.svipenyu.cn

TS:   await fetch(url)
来源：http://kxr.xinyue.icu

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jky.hywenlv.cn

Go:   resp, err := http.Get(url)
来源：http://azr.yfazqb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://ttv.jlsjyb.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ipx.gzhubu.top

[L02] 发送 POST JSON
来源：http://rgm.xingfuxueyuan.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://uhf.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xja.xylfe.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hqr.ehwqpu.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wat.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yfb.gaohongyu789.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fhd.hnxiangtu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nbi.cqqwz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gjr.cucudq.cn

[L03] 设置自定义请求头
来源：http://yfu.mhx1999.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kek.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mcb.hammf.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sps.yueranfly.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hvw.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rkx.jianghu66.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kgl.jinghuilouyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tmw.yonumen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ykf.quarkkingdee.top

[L04] 设置超时
来源：http://evl.ppjwa.cn

Py:   requests.get(url, timeout=5)
来源：http://wpp.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://anv.ppjwa.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uhf.ppjwa.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://akk.tanke756.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kbk.zhaomingkeji.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nkq.0kj1m.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jma.tarul.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qxi.xziqi.cn

[L05] 上传文件（multipart）
来源：http://uzz.sweek.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lpv.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aou.fktsv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vry.sysykeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pjt.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bzc.svipenyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tkp.ybcxt.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xli.havefunace.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://guz.yonumen.top

[L06] 解析响应为 JSON
来源：http://yeu.andypj.xyz

Py:   resp.json()
来源：http://ajb.chenlongwang.top

PHP:  json_decode($body, true);
来源：http://fgh.zdbjq.cn

JS:   await resp.json()
来源：http://imf.cashguo.top

TS:   await resp.json()
来源：http://nbw.yuanzhike.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://khs.hysaishi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ege.cdnleiting.top

Ruby: JSON.parse(resp.body)
来源：http://liq.shanyushiyangtech.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bol.bjfxy.top

[L07] 处理 HTTP 状态码
来源：http://tmm.fzhhl.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fqt.daxiang520.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xor.sufxvd.cn

JS:   resp.ok;  resp.status
来源：http://qdi.hesvh.cn

TS:   resp.ok;  resp.status
来源：http://njj.zhoulong.xyz

Java: resp.statusCode()
来源：http://cip.aizwys.cn

Go:   resp.StatusCode
来源：http://izh.hnqzz.top

Ruby: resp.code.to_i
来源：http://lpy.yonumen.top

C#:   (int)resp.StatusCode
来源：http://blh.zhijiandao.cn

[L08] 并发请求多个地址
来源：http://xrz.yangfankeji.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hpn.iojbl.cn

PHP:  curl_multi_init() 系列
来源：http://gee.hammf.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lcn.wangshuangyany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ugo.andypj.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sbn.tanke756.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ctz.tarul.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dno.daria6918.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aox.aizwys.cn

================================================================================
来源：http://jxo.dashuyun.cn

M. 命令行 / 进程 / 环境
来源：http://dkb.xinyue.icu

================================================================================
来源：http://ngt.fzhhl.top

[M01] 读取命令行参数
来源：http://vwf.tian-w.cn

Py:   sys.argv[1:]
来源：http://srl.xinyue.icu

PHP:  $argv;  $argc;
来源：http://dvc.feifeiyinyue.top

JS:   process.argv.slice(2)
来源：http://cqr.yuxming.cn

TS:   process.argv.slice(2)
来源：http://vvb.bjfxy.top

Java: args 数组（main 方法参数）
来源：http://dsv.fehbvm.com

Go:   os.Args[1:]
来源：http://fhv.aizwys.cn

Ruby: ARGV
来源：http://pxb.daxiang520.top

C#:   args 数组（Main 方法参数）
来源：http://ikm.jianghu66.top

[M02] 读取环境变量
来源：http://dgr.yj202588.top

Py:   os.environ.get("HOME")
来源：http://odr.jqgufenzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://imi.jlsjyb.cn

JS:   process.env.HOME
来源：http://srj.jlsjyb.cn

TS:   process.env.HOME
来源：http://sou.hnxiangtu.top

Java: System.getenv("HOME")
来源：http://tol.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oiw.iojbl.cn

Ruby: ENV["HOME"]
来源：http://ynw.sxryk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yvs.jqgfzy.top

[M03] 执行外部命令
来源：http://hmj.chenjidiqi.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mqm.sysykeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fwn.zhengqikj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ezh.pycfn.com

TS:   child_process.execSync("ls -l").toString()
来源：http://org.tarul.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gao.cdnleiting.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gds.bjfxy.top

Ruby: system("ls -l");  `ls -l`
来源：http://tni.xuanzx.com

C#:   Process.Start("ls", "-l");
来源：http://fvf.52xcode.cn

[M04] 获取当前工作目录
来源：http://gmz.yuxming.cn

Py:   os.getcwd()
来源：http://zef.redwolf501.top

PHP:  getcwd();
来源：http://chs.yonumen.top

JS:   process.cwd()
来源：http://qsm.xylfe.cn

TS:   process.cwd()
来源：http://hnh.ppjwa.cn

Java: Path.of("").toAbsolutePath()
来源：http://pkk.smart0.xyz

Go:   os.Getwd()
来源：http://esf.yuanzhike.top

Ruby: Dir.pwd
来源：http://utj.aizwys.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vtf.yanxiufei.cn

[M05] 设置退出码
来源：http://zpj.fzhhl.top

Py:   sys.exit(1)
来源：http://dwn.pycfn.com

PHP:  exit(1);
来源：http://rez.gotoacloud.top

JS:   process.exit(1)
来源：http://thl.sufxvd.cn

TS:   process.exit(1)
来源：http://cyn.hongshengwenyu.top

Java: System.exit(1)
来源：http://oyg.fehbvm.com

Go:   os.Exit(1)
来源：http://whn.hnqzz.top

Ruby: exit 1
来源：http://vki.yueranfly.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jun.svipenyu.cn

[M06] 向标准错误输出
来源：http://pcl.fktsv.cn

Py:   print("err", file=sys.stderr)
来源：http://ryy.xinyue.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://vwi.andypj.xyz

JS:   console.error("err")
来源：http://zra.c1oappe.top

TS:   console.error("err")
来源：http://ybl.sufxvd.cn

Java: System.err.println("err")
来源：http://wff.gzhubu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vkm.guowangkeji.top

Ruby: warn "err"
来源：http://pwr.birdmap.top

C#:   Console.Error.WriteLine("err")
来源：http://aou.tian-w.cn

[M07] 判断是否为主入口
来源：http://psm.yuanzhike.top

Py:   if __name__ == "__main__":
来源：http://oyh.daxiang520.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://exq.zhaomingkeji.xyz

JS:   require.main === module
来源：http://okp.quarkkingdee.top

TS:   require.main === module
来源：http://lvg.bjfxy.top

Java: public static void main(String[] args)
来源：http://umx.tian-w.cn

Go:   func main()
来源：http://eiw.cdnleiting.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oca.sysykeji.top

C#:   static void Main(string[] args)
来源：http://atb.zhoulong.xyz

[M08] 获取系统与运行时信息
来源：http://bfo.epnwcf.com

Py:   platform.system();  platform.python_version()
来源：http://huu.svipenyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://eiw.jianghu66.top

JS:   process.platform;  process.version
来源：http://tep.pycfn.com

TS:   process.platform;  process.version
来源：http://khx.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jfy.pycfn.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://uxx.shzxlz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zka.ywan-chungtsiang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ejw.gogol.net.cn

================================================================================
来源：http://yzf.kuanghao11.cn

N. 数据结构与算法
来源：http://amz.jiagoushi.top

================================================================================
来源：http://keu.mhx1999.top

[N01] 二分查找（有序数组）
来源：http://siw.smart0.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://pgs.9152youxi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ver.yfazqb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ank.wangshuangyany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ogz.tianlin.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://ctn.gaohongyu789.top

Go:   sort.SearchInts(arr, x)
来源：http://pmw.ehwqpu.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://cpt.zhiwuduotai.top

C#:   Array.BinarySearch(arr, x)
来源：http://oof.daxiang520.top

[N02] 排序（工程实践用内置实现）
来源：http://dph.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://zbg.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zwh.cqqwz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wnt.chenlongwang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ldn.cdnleiting.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dbf.cashguo.top

Go:   slices.Sort(arr)
来源：http://ujm.jqgufenzy.top

Ruby: arr.sort
来源：http://jxd.ppjwa.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xky.cdnleiting.top

[N03] 快速排序（分治示例）
来源：http://ucu.fzhhl.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hca.tanke756.top

PHP:  // 递归实现，或用 usort
来源：http://qoj.jinyuanbaomall.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wzk.yvedp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qnd.xuanzx.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gsc.zhijiandao.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mhi.shangyingyoupin.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mmp.xingfuxueyuan.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://flr.tarul.cn

[N04] 斐波那契数列
来源：http://rsd.c1oappe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://udd.gaohongyu789.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ysf.jqgfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mqg.zhaomingkeji.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ftq.iojbl.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cej.hcnkem.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qfp.hywenlv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mbt.chenlongwang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jdg.hfpthk.cn

[N05] 最大公约数
来源：http://fmb.redwolf501.top

Py:   math.gcd(a, b)
来源：http://xou.tianlin.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://izm.cucudq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fay.fanxiaobao.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dcx.sxryk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qjr.yangfankeji.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qko.xingfuxueyuan.xyz

Ruby: a.gcd(b)
来源：http://dry.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xoe.gzhubu.top

[N06] 判断回文字符串
来源：http://hla.pycfn.com

Py:   s == s[::-1]
来源：http://mmi.jinqigfzy.top

PHP:  $s === strrev($s);
来源：http://dji.chenlongwang.top

JS:   s === [...s].reverse().join("")
来源：http://nwn.xuetiantiany.cn

TS:   s === [...s].reverse().join("")
来源：http://qae.jinghuilouyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mwi.ybcxt.top

Go:   // 双指针从两端比较
来源：http://rfm.hammf.cn

Ruby: s == s.reverse
来源：http://ith.xziqi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lxw.guowangkeji.top

[N07] 两数之和（返回下标）
来源：http://cff.zhoulong.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://krc.ybcxt.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dyy.havefunace.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ecf.zhiwuduotai.top

TS:   // 手写 Map<string, number>
来源：http://sak.wangdashe.top

Java: // 手写 HashMap
来源：http://cfn.yongpay.top

Go:   // 手写 map[int]int
来源：http://sth.svipenyu.cn

Ruby: // 手写 Hash
来源：http://zex.sjlbkw.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zpw.shanyushiyangtech.top

[N08] 生成全排列
来源：http://qge.yangfankeji.com

Py:   itertools.permutations(arr)
来源：http://rjr.vehdjk.com

PHP:  // 手写递归交换
来源：http://spf.9152youxi.cn

JS:   // 手写回溯递归
来源：http://nlj.hongshengwenyu.top

TS:   // 手写回溯递归
来源：http://cyo.cdnleiting.top

Java: // 手写回溯递归
来源：http://fjj.52xcode.cn

Go:   // 手写回溯递归
来源：http://yui.hysaishi.cn

Ruby: arr.permutation.to_a
来源：http://eok.yangfankeji.com

C#:   // 手写回溯递归
来源：http://gwe.aizwys.cn

[N09] 栈与队列
来源：http://smk.guannengcc.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vql.fzhhl.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kio.dashuyun.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oow.xuanzx.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://flk.daria6918.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qgs.ydzc1.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eij.hnqzz.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fov.smart0.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ykn.ydjk.org.cn

[N10] 链表节点定义
来源：http://ovc.smart0.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://waa.daria6918.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ych.hywenlv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zuu.fehbvm.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://flw.iojbl.cn

Java: class Node { int v; Node next; }
来源：http://kiz.chenzaomai.com

Go:   type Node struct { V int; Next *Node }
来源：http://uof.xuetiantiany.cn


<!-- 参考信息 -->