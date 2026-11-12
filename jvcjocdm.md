代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://ojh.c1oappe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rvr.ydjk.org.cn

[K04] 读取 JSON 文件
来源：http://khz.yvedp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lmt.chenlongwang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jul.sweek.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gdq.yongpay.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://khb.guowangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://muv.hywenlv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vsn.hnxiangtu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lak.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ztn.sufxvd.cn

[K05] 深拷贝对象
来源：http://yma.316326.xyz

Py:   copy.deepcopy(obj)
来源：http://ziy.xingfuxueyuan.xyz

PHP:  unserialize(serialize($obj));
来源：http://igk.shangyingyoupin.top

JS:   structuredClone(obj)
来源：http://iyj.quarkkingdee.top

TS:   structuredClone(obj)
来源：http://vax.hnxiangtu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://rgg.vehdjk.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nro.meibo888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zmr.jiagoushi.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jaa.zhengqikj.top

[K06] 解析 URL 查询串
来源：http://wmp.cdnleiting.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://apb.pengpengdd.cyou

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://psi.zhoulong.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://whz.vqdsnc.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xwf.wangdashe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yaa.zycfv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gvl.birdmap.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ixg.cashguo.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mzv.xziqi.cn

[K07] 进制转换
来源：http://bla.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://phz.jiagoushi.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fhv.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dvq.shuidangran.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://njs.iojbl.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rog.aibaodan.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://apo.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://aud.gogol.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ogg.xuetiantiany.cn

[K08] 二进制序列化（非 JSON）
来源：http://qfr.tarul.cn

Py:   pickle.dumps(obj)
来源：http://tna.sxryk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lhc.nanxuanxn.top

JS:   v8.serialize(obj)        // Node
来源：http://evj.bbcook.cn

TS:   v8.serialize(obj)        // Node
来源：http://okl.hnqzz.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qlk.sxryk.cn

Go:   encoding/gob
来源：http://mgd.epnwcf.com

Ruby: Marshal.dump(obj)
来源：http://zie.ybcxt.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bkx.chenlongwang.top

================================================================================
来源：http://nlk.fehbvm.com

L. 网络请求
来源：http://ypv.jqgufenzy.top

================================================================================
来源：http://mpi.yonumen.top

[L01] 发送 GET 请求
来源：http://xum.guannengcc.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://isq.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xqh.redwolf501.top

JS:   await fetch(url)
来源：http://isf.chenlongwang.top

TS:   await fetch(url)
来源：http://bxd.xylfe.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pyj.shangyingyoupin.top

Go:   resp, err := http.Get(url)
来源：http://rrm.zdqjudy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ola.ydzc1.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nab.zycfv.cn

[L02] 发送 POST JSON
来源：http://gyn.hnxiangtu.top

Py:   requests.post(url, json={"a": 1})
来源：http://qca.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uxp.yonumen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wmi.jinqigufen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://skw.yj20258.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rvf.hysaishi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zig.0kj1m.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qdq.ehwqpu.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xxo.wangdashe.top

[L03] 设置自定义请求头
来源：http://mrq.bjfxy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nis.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bzu.jianghu66.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uxr.ywan-chungtsiang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xdg.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ech.ydzc1.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hmq.zhongyouzk.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hal.nwbrower.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fti.zhixingplan.top

[L04] 设置超时
来源：http://btr.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://ono.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hma.fehbvm.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://goc.cqqwz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://llb.sufxvd.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nwm.nwbrower.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eys.hfpthk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qfx.52xcode.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ehj.fktsv.cn

[L05] 上传文件（multipart）
来源：http://ndp.xziqi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rqq.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ldp.feifeiyinyue.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ccv.chenzaomai.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://spx.jqgufenzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bwx.daria6918.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pkd.wangshuangyany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qhr.hywenlv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kbd.fzhhl.top

[L06] 解析响应为 JSON
来源：http://sin.bbcook.cn

Py:   resp.json()
来源：http://wcg.iojbl.cn

PHP:  json_decode($body, true);
来源：http://eqt.cashguo.top

JS:   await resp.json()
来源：http://yee.yfazqb.com

TS:   await resp.json()
来源：http://nrd.jinqigfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qog.gotoacloud.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hwz.yueranfly.top

Ruby: JSON.parse(resp.body)
来源：http://wow.kuanghao11.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://okm.yuanzhike.top

[L07] 处理 HTTP 状态码
来源：http://jeb.zhijiandao.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qmd.hywenlv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xft.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://jgr.cucudq.cn

TS:   resp.ok;  resp.status
来源：http://toy.shanyushiyangtech.top

Java: resp.statusCode()
来源：http://ffb.tianlin.xyz

Go:   resp.StatusCode
来源：http://mpe.jlsjyb.cn

Ruby: resp.code.to_i
来源：http://xpr.zhiwuduotai.top

C#:   (int)resp.StatusCode
来源：http://tyj.ehwqpu.com

[L08] 并发请求多个地址
来源：http://qva.jianghu66.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jpm.ydzc1.top

PHP:  curl_multi_init() 系列
来源：http://eaj.jlsjyb.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bos.epnwcf.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ofc.chenzaomai.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jeq.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ojf.nanxinkj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nvq.hongshengwenyu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nhi.haohaochexian.top

================================================================================
来源：http://xrp.yfazqb.com

M. 命令行 / 进程 / 环境
来源：http://xmf.guannengcc.top

================================================================================
来源：http://kek.xinyue.icu

[M01] 读取命令行参数
来源：http://uhf.yueranfly.top

Py:   sys.argv[1:]
来源：http://qji.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://kka.hnxiangtu.top

JS:   process.argv.slice(2)
来源：http://gky.zhongyouzk.top

TS:   process.argv.slice(2)
来源：http://jch.ppjwa.cn

Java: args 数组（main 方法参数）
来源：http://tql.aizwys.cn

Go:   os.Args[1:]
来源：http://hhl.epnwcf.com

Ruby: ARGV
来源：http://ybu.jyoumei.cn

C#:   args 数组（Main 方法参数）
来源：http://pgs.ppjwa.cn

[M02] 读取环境变量
来源：http://jpn.jinghuilouyu.cn

Py:   os.environ.get("HOME")
来源：http://zom.mhx1999.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cik.dianchejie.cn

JS:   process.env.HOME
来源：http://pni.gzhubu.top

TS:   process.env.HOME
来源：http://zdq.gzhubu.top

Java: System.getenv("HOME")
来源：http://arh.sjlbkw.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://spt.hnxiangtu.top

Ruby: ENV["HOME"]
来源：http://swl.jyoumei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ilf.hysaishi.cn

[M03] 执行外部命令
来源：http://goe.jianghu66.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xul.tian-w.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bti.hnqzz.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qws.shanyushiyangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://baf.haohaochexian.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dhz.shanyushiyangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://buw.meibo888.top

Ruby: system("ls -l");  `ls -l`
来源：http://ypn.yvedp.cn

C#:   Process.Start("ls", "-l");
来源：http://fxo.sysykeji.top

[M04] 获取当前工作目录
来源：http://voo.snrcjt.cn

Py:   os.getcwd()
来源：http://uqx.cashguo.top

PHP:  getcwd();
来源：http://qkc.xinyue.icu

JS:   process.cwd()
来源：http://tts.jinghuilouyu.cn

TS:   process.cwd()
来源：http://isq.yj20258.top

Java: Path.of("").toAbsolutePath()
来源：http://wzo.jqgfzy.top

Go:   os.Getwd()
来源：http://tte.birdmap.top

Ruby: Dir.pwd
来源：http://fal.wangshuangyany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://aae.quarkkingdee.top

[M05] 设置退出码
来源：http://kii.zhijiandao.cn

Py:   sys.exit(1)
来源：http://lhg.yfazqb.com

PHP:  exit(1);
来源：http://eux.xylfe.cn

JS:   process.exit(1)
来源：http://nzy.fanxiaobao.xyz

TS:   process.exit(1)
来源：http://cok.shanyushiyangkeji.top

Java: System.exit(1)
来源：http://mzi.yuanzhike.top

Go:   os.Exit(1)
来源：http://jtn.0kj1m.cn

Ruby: exit 1
来源：http://vuq.cdnleiting.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yud.shzxlz.cn

[M06] 向标准错误输出
来源：http://qcn.jqgufenzy.top

Py:   print("err", file=sys.stderr)
来源：http://ves.mhx1999.top

PHP:  fwrite(STDERR, "err\n");
来源：http://eib.jqgfzy.top

JS:   console.error("err")
来源：http://adj.haohaochexian.top

TS:   console.error("err")
来源：http://llf.jqgfzy.top

Java: System.err.println("err")
来源：http://qng.52xcode.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cvs.wangshuangyany.cn

Ruby: warn "err"
来源：http://jgf.zhoulong.xyz

C#:   Console.Error.WriteLine("err")
来源：http://shs.chenzaomai.com

[M07] 判断是否为主入口
来源：http://kra.shzxlz.cn

Py:   if __name__ == "__main__":
来源：http://msc.sweek.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ukx.haohaochexian.top

JS:   require.main === module
来源：http://ztg.ehwqpu.com

TS:   require.main === module
来源：http://hgm.zdqjudy.top

Java: public static void main(String[] args)
来源：http://dbb.meibo888.top

Go:   func main()
来源：http://kcl.0kj1m.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eoq.zhoulong.xyz

C#:   static void Main(string[] args)
来源：http://onu.tanke756.top

[M08] 获取系统与运行时信息
来源：http://qmd.fktsv.cn

Py:   platform.system();  platform.python_version()
来源：http://ezw.yongpay.top

PHP:  PHP_OS;  phpversion();
来源：http://bii.hammf.cn

JS:   process.platform;  process.version
来源：http://yxx.cdnleiting.top

TS:   process.platform;  process.version
来源：http://hdw.aibaodan.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iqy.pycfn.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://zeu.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nmb.jinyuanbaomall.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rqg.shuidangran.top

================================================================================
来源：http://gis.fktsv.cn

N. 数据结构与算法
来源：http://hin.daxiang520.top

================================================================================
来源：http://mye.ehwqpu.com

[N01] 二分查找（有序数组）
来源：http://plf.dianchejie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wgt.zhoulong.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vvq.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://boj.tanke756.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ipr.pengpengdd.cyou

Java: Arrays.binarySearch(arr, x)
来源：http://tqz.zdbjq.cn

Go:   sort.SearchInts(arr, x)
来源：http://teo.shanyushiyangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://wvs.yuanzhike.top

C#:   Array.BinarySearch(arr, x)
来源：http://cri.hongshengwenyu.top

[N02] 排序（工程实践用内置实现）
来源：http://ydq.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://irm.zdbjq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zup.ydzc1.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xwq.ywan-chungtsiang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mqo.jiagoushi.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sjz.hammf.cn

Go:   slices.Sort(arr)
来源：http://vsw.fehbvm.com

Ruby: arr.sort
来源：http://pgj.xuanzx.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://rdi.wangdashe.top

[N03] 快速排序（分治示例）
来源：http://jwh.sjlbkw.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://awz.0kj1m.cn

PHP:  // 递归实现，或用 usort
来源：http://zmo.zhoulong.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xqd.sweek.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cyh.uphjek.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wkn.xinyue.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hgl.vehdjk.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lve.svipenyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qjb.zhiwuduotai.top

[N04] 斐波那契数列
来源：http://ioy.gzhubu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://deg.jianghu66.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nio.yvedp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xek.jinqigufen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://npj.yuxming.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rqz.tian-w.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pkw.zycfv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://usa.hongshengwenyu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ehr.bbcook.cn

[N05] 最大公约数
来源：http://lnb.aibaodan.cn

Py:   math.gcd(a, b)
来源：http://haz.jlsjyb.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ozf.zhengqikj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ktm.gzhubu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ctk.jinqigfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kxl.yongpay.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://aes.c1oappe.top

Ruby: a.gcd(b)
来源：http://oaf.quarkkingdee.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mlh.bjfxy.top

[N06] 判断回文字符串
来源：http://yoh.wangshuangyany.cn

Py:   s == s[::-1]
来源：http://zfc.yangfankeji.com

PHP:  $s === strrev($s);
来源：http://mhv.shuidangran.top

JS:   s === [...s].reverse().join("")
来源：http://hur.cheryme.top

TS:   s === [...s].reverse().join("")
来源：http://zoq.pengpengdd.cyou

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ubo.jyoumei.cn

Go:   // 双指针从两端比较
来源：http://kbv.shangyingyoupin.top

Ruby: s == s.reverse
来源：http://izi.yvedp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lge.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://bji.sweek.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lmv.shangyingyoupin.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ryd.9152youxi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jbh.sjlbkw.cn

TS:   // 手写 Map<string, number>
来源：http://vuq.zhiwuduotai.top

Java: // 手写 HashMap
来源：http://wuv.zhoulong.xyz

Go:   // 手写 map[int]int
来源：http://gut.epnwcf.com

Ruby: // 手写 Hash
来源：http://ucm.gzhubu.top

C#:   // 手写 Dictionary<int, int>
来源：http://hfr.andypj.xyz

[N08] 生成全排列
来源：http://zrv.fehbvm.com

Py:   itertools.permutations(arr)
来源：http://qkv.tarul.cn

PHP:  // 手写递归交换
来源：http://dur.aizwys.cn

JS:   // 手写回溯递归
来源：http://zwi.sxryk.cn

TS:   // 手写回溯递归
来源：http://dnd.gzhubu.top

Java: // 手写回溯递归
来源：http://rqq.zhengqikj.top

Go:   // 手写回溯递归
来源：http://qda.gzhubu.top

Ruby: arr.permutation.to_a
来源：http://xmy.meibo888.top

C#:   // 手写回溯递归
来源：http://bps.zdbjq.cn

[N09] 栈与队列
来源：http://cnz.cashguo.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zfh.quarkkingdee.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://szj.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://apt.52xcode.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lpu.zdqjudy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vzo.epnwcf.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qbb.meibo888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iao.hysaishi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uvu.chenlongwang.top

[N10] 链表节点定义
来源：http://dzi.epnwcf.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bts.bbcook.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qow.shanyushiyangkeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cbd.zycfv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tck.yj202588.top

Java: class Node { int v; Node next; }
来源：http://onc.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://vmp.dashuyun.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gxc.epnwcf.com

C#:   class Node { public int V; public Node? Next; }
来源：http://mkz.pycfn.com

[N11] 二叉树中序遍历
来源：http://mah.yangfankeji.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ard.yfazqb.com

PHP:  // 手写递归函数
来源：http://qfx.hfpthk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://etk.guannengcc.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yln.epnwcf.com

Java: // 手写递归
来源：http://gca.vqdsnc.cn

Go:   // 手写递归
来源：http://cnq.pengpengdd.cyou

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hwy.hcnkem.com

C#:   // 手写递归
来源：http://cuo.yangfankeji.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jcx.jqgufenzy.top


<!-- 参考信息 -->