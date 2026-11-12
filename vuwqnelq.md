代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://ywv.bbcook.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vof.yvedp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pkw.uphjek.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vgi.redwolf501.top

Ruby: JSON.pretty_generate(obj)
来源：http://chb.chenlongwang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vvz.yfazqb.com

[K04] 读取 JSON 文件
来源：http://dzf.xylfe.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xfv.zhaomingkeji.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tqo.c1oappe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vyg.yvedp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eil.yongpay.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yof.uphjek.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yow.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://elq.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zid.nwbrower.top

[K05] 深拷贝对象
来源：http://iqc.ywan-chungtsiang.top

Py:   copy.deepcopy(obj)
来源：http://oty.smart0.xyz

PHP:  unserialize(serialize($obj));
来源：http://edm.bbcook.cn

JS:   structuredClone(obj)
来源：http://jiv.hesvh.cn

TS:   structuredClone(obj)
来源：http://kor.52xcode.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gqf.sjlbkw.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dej.jlsjyb.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ypu.vehdjk.com

C#:   // 序列化往返，或自定义 Clone
来源：http://wgr.0kj1m.cn

[K06] 解析 URL 查询串
来源：http://axu.jqgufenzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pxa.9152youxi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ddw.vehdjk.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ofz.cdnleiting.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mwq.snrcjt.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pwk.dianchejie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vot.c1oappe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wfh.jinyuanbaomall.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ban.tanke756.top

[K07] 进制转换
来源：http://dsc.nwbrower.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://phh.tanke756.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fwo.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yks.gotoacloud.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sck.daria6918.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gwf.gotoacloud.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wbw.fanxiaobao.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fif.zdqjudy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gdd.aizwys.cn

[K08] 二进制序列化（非 JSON）
来源：http://jgx.fengsongda.top

Py:   pickle.dumps(obj)
来源：http://nzk.ydjk.org.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://abe.zycfv.cn

JS:   v8.serialize(obj)        // Node
来源：http://jnf.yuxming.cn

TS:   v8.serialize(obj)        // Node
来源：http://lja.chenlongwang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nyg.fanxiaobao.xyz

Go:   encoding/gob
来源：http://lgb.sjlbkw.cn

Ruby: Marshal.dump(obj)
来源：http://jgx.chenzaomai.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://onx.hnxiangtu.top

================================================================================
来源：http://dzo.chenjidiqi.icu

L. 网络请求
来源：http://aly.ehwqpu.com

================================================================================
来源：http://ryt.fengsongda.top

[L01] 发送 GET 请求
来源：http://cza.dianchejie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pmw.shanyushiyangtech.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wxn.haohaochexian.top

JS:   await fetch(url)
来源：http://pbq.yj20258888.top

TS:   await fetch(url)
来源：http://uez.zhiwuduotai.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hul.yanxiufei.cn

Go:   resp, err := http.Get(url)
来源：http://qua.yj202588.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jeb.xuanzx.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pwh.hongshengwenyu.top

[L02] 发送 POST JSON
来源：http://ixg.gaohongyu789.top

Py:   requests.post(url, json={"a": 1})
来源：http://cnv.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xum.wangshuangyany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bto.yangfankeji.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pdr.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nnc.uphjek.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://neq.feifeiyinyue.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ntw.fzhhl.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rsv.jlsjyb.cn

[L03] 设置自定义请求头
来源：http://tyi.fktsv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cwl.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://frf.zhengqikj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tjz.sjlbkw.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tsx.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ikv.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qrf.ivvv.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wfi.birdmap.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yqg.xziqi.cn

[L04] 设置超时
来源：http://xkc.jinghuilouyu.cn

Py:   requests.get(url, timeout=5)
来源：http://fhl.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nsq.chenzaomai.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lgt.epnwcf.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wmh.c1oappe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gpp.gzhubu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nkr.hongshengwenyu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hqr.nwbrower.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://som.ybcxt.top

[L05] 上传文件（multipart）
来源：http://ena.zdqjudy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qfc.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ruf.zdbjq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pee.nanxuanxn.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hrn.yonumen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lde.cqqwz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vay.jinyuanbaomall.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ngq.tianlin.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gvw.hnxiangtu.top

[L06] 解析响应为 JSON
来源：http://epd.wangshuangyany.cn

Py:   resp.json()
来源：http://mng.snrcjt.cn

PHP:  json_decode($body, true);
来源：http://wdj.316326.xyz

JS:   await resp.json()
来源：http://tnw.pycfn.com

TS:   await resp.json()
来源：http://ota.chenjidiqi.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pda.dianchejie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://aqr.yuanzhike.top

Ruby: JSON.parse(resp.body)
来源：http://fjf.meibo888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ako.chenlongwang.top

[L07] 处理 HTTP 状态码
来源：http://yyo.jinqigufen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://exu.cucudq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aia.shuidangran.top

JS:   resp.ok;  resp.status
来源：http://cfn.cashguo.top

TS:   resp.ok;  resp.status
来源：http://xoe.yvedp.cn

Java: resp.statusCode()
来源：http://exa.hongshengwenyu.top

Go:   resp.StatusCode
来源：http://yon.yonumen.top

Ruby: resp.code.to_i
来源：http://jri.zhiwuduotai.top

C#:   (int)resp.StatusCode
来源：http://stz.daria6918.cn

[L08] 并发请求多个地址
来源：http://ttu.hnqzz.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gno.tianlin.xyz

PHP:  curl_multi_init() 系列
来源：http://bpr.quarkkingdee.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bzk.hcnkem.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://idt.daria6918.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dkg.jinyuanbaomall.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aqg.yvedp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zyr.jiagoushi.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://soq.yuxming.cn

================================================================================
来源：http://zpu.hesvh.cn

M. 命令行 / 进程 / 环境
来源：http://pwn.fanxiaobao.xyz

================================================================================
来源：http://lqw.dianchejie.cn

[M01] 读取命令行参数
来源：http://vdv.nwbrower.top

Py:   sys.argv[1:]
来源：http://nag.tarul.cn

PHP:  $argv;  $argc;
来源：http://hzl.xinyue.icu

JS:   process.argv.slice(2)
来源：http://vov.shuidangran.top

TS:   process.argv.slice(2)
来源：http://yml.gogol.net.cn

Java: args 数组（main 方法参数）
来源：http://vlr.dianchejie.cn

Go:   os.Args[1:]
来源：http://dtj.vehdjk.com

Ruby: ARGV
来源：http://qkq.gogol.net.cn

C#:   args 数组（Main 方法参数）
来源：http://tmm.bbcook.cn

[M02] 读取环境变量
来源：http://eya.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://zcz.snrcjt.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lry.0kj1m.cn

JS:   process.env.HOME
来源：http://ecp.zhengqikj.top

TS:   process.env.HOME
来源：http://uwg.andypj.xyz

Java: System.getenv("HOME")
来源：http://txk.mhx1999.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bhi.xziqi.cn

Ruby: ENV["HOME"]
来源：http://bxh.yangfankeji.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mfy.316326.xyz

[M03] 执行外部命令
来源：http://vus.gzhubu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oih.shuidangran.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hoo.sjlbkw.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://awr.yanxiufei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bdr.yueranfly.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ohp.hysaishi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dij.sweek.top

Ruby: system("ls -l");  `ls -l`
来源：http://gwl.chenlongwang.top

C#:   Process.Start("ls", "-l");
来源：http://oko.uphjek.com

[M04] 获取当前工作目录
来源：http://laj.zhixingplan.top

Py:   os.getcwd()
来源：http://xty.jyoumei.cn

PHP:  getcwd();
来源：http://kxa.sjlbkw.cn

JS:   process.cwd()
来源：http://bfg.xziqi.cn

TS:   process.cwd()
来源：http://lhz.shanyushiyangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://gzo.jyoumei.cn

Go:   os.Getwd()
来源：http://wwg.aibaodan.cn

Ruby: Dir.pwd
来源：http://wuc.c1oappe.top

C#:   Directory.GetCurrentDirectory()
来源：http://kde.cashguo.top

[M05] 设置退出码
来源：http://dwr.redwolf501.top

Py:   sys.exit(1)
来源：http://xpn.svipenyu.cn

PHP:  exit(1);
来源：http://tpz.zhaomingkeji.xyz

JS:   process.exit(1)
来源：http://hpf.havefunace.top

TS:   process.exit(1)
来源：http://mzp.jlsjyb.cn

Java: System.exit(1)
来源：http://gge.zhongyouzk.top

Go:   os.Exit(1)
来源：http://gcj.yonumen.top

Ruby: exit 1
来源：http://unc.zhaomingkeji.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ygf.zhengqikj.top

[M06] 向标准错误输出
来源：http://xyr.aizwys.cn

Py:   print("err", file=sys.stderr)
来源：http://bjy.cqqwz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://khk.epnwcf.com

JS:   console.error("err")
来源：http://dnc.ybcxt.top

TS:   console.error("err")
来源：http://ezh.shzxlz.cn

Java: System.err.println("err")
来源：http://hfl.nwbrower.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vkx.dianchejie.cn

Ruby: warn "err"
来源：http://ovu.aizwys.cn

C#:   Console.Error.WriteLine("err")
来源：http://yvf.sweek.top

[M07] 判断是否为主入口
来源：http://cbv.ydzc1.top

Py:   if __name__ == "__main__":
来源：http://nrc.hcnkem.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jlw.yonumen.top

JS:   require.main === module
来源：http://kft.zhengqikj.top

TS:   require.main === module
来源：http://slw.jlsjyb.cn

Java: public static void main(String[] args)
来源：http://dgd.sysykeji.top

Go:   func main()
来源：http://eej.havefunace.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bcl.hysaishi.cn

C#:   static void Main(string[] args)
来源：http://gfi.xinyue.icu

[M08] 获取系统与运行时信息
来源：http://bwc.haohaochexian.top

Py:   platform.system();  platform.python_version()
来源：http://jer.shzxlz.cn

PHP:  PHP_OS;  phpversion();
来源：http://nym.vehdjk.com

JS:   process.platform;  process.version
来源：http://gez.iojbl.cn

TS:   process.platform;  process.version
来源：http://esk.tarul.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ycs.ydzc1.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pyu.jinyuanbaomall.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://clf.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://fcw.epnwcf.com

================================================================================
来源：http://xdu.shanyushiyangtech.top

N. 数据结构与算法
来源：http://kse.guowangkeji.top

================================================================================
来源：http://wmq.zhongyouzk.top

[N01] 二分查找（有序数组）
来源：http://vjw.jqgfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://tpp.bjfxy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://erd.iojbl.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fzd.vqdsnc.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ouw.chenjidiqi.icu

Java: Arrays.binarySearch(arr, x)
来源：http://tzg.uphjek.com

Go:   sort.SearchInts(arr, x)
来源：http://yco.sxryk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ipk.gotoacloud.top

C#:   Array.BinarySearch(arr, x)
来源：http://dvk.yj202588.top

[N02] 排序（工程实践用内置实现）
来源：http://mkt.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://ddj.chenlongwang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kzh.fktsv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bhj.jinqigfzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://aej.chenlongwang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ryf.bbcook.cn

Go:   slices.Sort(arr)
来源：http://lyp.nanxinkj.top

Ruby: arr.sort
来源：http://lle.bbcook.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ziw.yj20258.top

[N03] 快速排序（分治示例）
来源：http://jwt.iojbl.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zxw.bjfxy.top

PHP:  // 递归实现，或用 usort
来源：http://qzs.shangyingyoupin.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mou.cqqwz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wkh.ydjk.org.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://spa.cashguo.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rso.bbcook.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jtc.nwbrower.top

C#:   // 手写递归，或 Array.Sort
来源：http://ggm.birdmap.top

[N04] 斐波那契数列
来源：http://hvk.jinqigufen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bpb.zhoulong.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fly.ydjk.org.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wjf.smart0.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jnk.dashuyun.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rrh.jyoumei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hte.nanxinkj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kbc.vehdjk.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://czd.vehdjk.com

[N05] 最大公约数
来源：http://vag.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://srd.yueranfly.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ziz.yj202588.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lkn.zhixingplan.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rfc.aibaodan.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sgr.zhoulong.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zth.cashguo.top

Ruby: a.gcd(b)
来源：http://dtn.zhijiandao.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nit.yueranfly.top

[N06] 判断回文字符串
来源：http://coh.fzhhl.top

Py:   s == s[::-1]
来源：http://wup.xingfuxueyuan.xyz

PHP:  $s === strrev($s);
来源：http://qcw.bbcook.cn

JS:   s === [...s].reverse().join("")
来源：http://gja.xuetiantiany.cn

TS:   s === [...s].reverse().join("")
来源：http://vmu.hnqzz.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kmo.hammf.cn

Go:   // 双指针从两端比较
来源：http://idt.xuetiantiany.cn

Ruby: s == s.reverse
来源：http://gso.hesvh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://iee.jqgfzy.top

[N07] 两数之和（返回下标）
来源：http://gva.cashguo.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tua.ppjwa.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ufl.zhijiandao.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://syf.sysykeji.top

TS:   // 手写 Map<string, number>
来源：http://kzv.zhongyouzk.top

Java: // 手写 HashMap
来源：http://ehr.zhijiandao.cn

Go:   // 手写 map[int]int
来源：http://cgw.bjfxy.top

Ruby: // 手写 Hash
来源：http://cvg.feifeiyinyue.top

C#:   // 手写 Dictionary<int, int>
来源：http://rwd.chenzaomai.com

[N08] 生成全排列
来源：http://psi.tianlin.xyz

Py:   itertools.permutations(arr)
来源：http://say.aizwys.cn

PHP:  // 手写递归交换
来源：http://dak.shzxlz.cn

JS:   // 手写回溯递归
来源：http://vfp.guannengcc.top

TS:   // 手写回溯递归
来源：http://nvi.fktsv.cn

Java: // 手写回溯递归
来源：http://hfq.tanke756.top

Go:   // 手写回溯递归
来源：http://ose.guowangkeji.top

Ruby: arr.permutation.to_a
来源：http://tbz.xziqi.cn

C#:   // 手写回溯递归
来源：http://bsd.bbcook.cn

[N09] 栈与队列
来源：http://isp.xingfuxueyuan.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dsu.jyoumei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ara.sweek.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zmy.nanxinkj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pzp.ctjpmb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://liy.chenjidiqi.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uxv.hnxiangtu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://thl.ehwqpu.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pvl.yuanzhike.top

[N10] 链表节点定义
来源：http://fll.nwbrower.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uyb.ehwqpu.com

PHP:  class Node { public $v; public $next = null; }
来源：http://wnx.zdqjudy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qnq.tanke756.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mfg.aibaodan.cn

Java: class Node { int v; Node next; }
来源：http://pck.xuetiantiany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rat.guowangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mwo.kuanghao11.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dmd.xylfe.cn

[N11] 二叉树中序遍历
来源：http://mhj.shanyushiyangtech.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hpg.zycfv.cn

PHP:  // 手写递归函数
来源：http://csy.yonumen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hwo.gaohongyu789.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zpd.hongshengwenyu.top

Java: // 手写递归
来源：http://zac.meibo888.top


<!-- 参考信息 -->