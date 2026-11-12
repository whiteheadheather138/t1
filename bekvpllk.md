代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://szw.hywenlv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kbo.mhx1999.top

[K04] 读取 JSON 文件
来源：http://nlq.ydzc1.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vru.pycfn.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wrn.epnwcf.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ohh.ppjwa.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kab.yfazqb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bul.fengsongda.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gyy.fzhhl.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://slr.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://viu.havefunace.top

[K05] 深拷贝对象
来源：http://ybt.vqdsnc.cn

Py:   copy.deepcopy(obj)
来源：http://jqq.yanxiufei.cn

PHP:  unserialize(serialize($obj));
来源：http://hsu.tian-w.cn

JS:   structuredClone(obj)
来源：http://xcg.hesvh.cn

TS:   structuredClone(obj)
来源：http://nzu.vqdsnc.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://viw.bjfxy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pej.jyoumei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nyo.gogol.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gba.sxryk.cn

[K06] 解析 URL 查询串
来源：http://erp.nanxuanxn.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://awh.shangyingyoupin.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hpu.sysykeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zod.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bdm.haohaochexian.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rhd.hnqzz.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ojj.gotoacloud.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fgm.quarkkingdee.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://olu.xziqi.cn

[K07] 进制转换
来源：http://kvl.nanxuanxn.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cqb.xuetiantiany.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tok.ctjpmb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ren.jinghuilouyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ciy.jinqigfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dym.zhongyouzk.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://enb.zhengqikj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bsr.zhengqikj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qjp.zhijiandao.cn

[K08] 二进制序列化（非 JSON）
来源：http://avm.aibaodan.cn

Py:   pickle.dumps(obj)
来源：http://pfb.yongpay.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xob.yonumen.top

JS:   v8.serialize(obj)        // Node
来源：http://mec.xingfuxueyuan.xyz

TS:   v8.serialize(obj)        // Node
来源：http://anv.sxryk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://obx.zhongyouzk.top

Go:   encoding/gob
来源：http://axe.dashuyun.cn

Ruby: Marshal.dump(obj)
来源：http://eas.sufxvd.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lfq.cashguo.top

================================================================================
来源：http://quf.zhoulong.xyz

L. 网络请求
来源：http://acx.sxryk.cn

================================================================================
来源：http://ifh.birdmap.top

[L01] 发送 GET 请求
来源：http://kcx.zhengqikj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://utn.shangyingyoupin.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vlq.xuanzx.com

JS:   await fetch(url)
来源：http://rnq.shangyingyoupin.top

TS:   await fetch(url)
来源：http://gzz.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zct.wangshuangyany.cn

Go:   resp, err := http.Get(url)
来源：http://gfg.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gyy.zhengqikj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wpa.shzxlz.cn

[L02] 发送 POST JSON
来源：http://cvn.jlsjyb.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wnb.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gxi.yuxming.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wun.tanke756.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rjm.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zfk.wangshuangyany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oeo.gaohongyu789.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pms.birdmap.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vvc.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://cvl.guowangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uti.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cde.andypj.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://alk.chenlongwang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jvn.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lgq.sysykeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kdo.sweek.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lvr.yanxiufei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dgf.jyoumei.cn

[L04] 设置超时
来源：http://qfo.xuanzx.com

Py:   requests.get(url, timeout=5)
来源：http://shx.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dkl.jinqigfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fvg.feifeiyinyue.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kdk.yonumen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rbp.gogol.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qqo.fengsongda.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iys.zhijiandao.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sak.wangdashe.top

[L05] 上传文件（multipart）
来源：http://tum.havefunace.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zul.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jps.gzhubu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dhq.zdqjudy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://taf.yj20258888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lfo.jqgfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dzy.pycfn.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sun.zhijiandao.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cmn.haohaochexian.top

[L06] 解析响应为 JSON
来源：http://oae.xylfe.cn

Py:   resp.json()
来源：http://ftu.bjfxy.top

PHP:  json_decode($body, true);
来源：http://dtz.ehwqpu.com

JS:   await resp.json()
来源：http://vak.yonumen.top

TS:   await resp.json()
来源：http://vap.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rkw.chenlongwang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rdd.shzxlz.cn

Ruby: JSON.parse(resp.body)
来源：http://sqo.zycfv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wks.guowangkeji.top

[L07] 处理 HTTP 状态码
来源：http://gsp.nanxuanxn.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pbr.bbcook.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tjv.ydzc1.top

JS:   resp.ok;  resp.status
来源：http://izp.vqdsnc.cn

TS:   resp.ok;  resp.status
来源：http://doq.chenjidiqi.icu

Java: resp.statusCode()
来源：http://uzi.xingfuxueyuan.xyz

Go:   resp.StatusCode
来源：http://mbv.shangyingyoupin.top

Ruby: resp.code.to_i
来源：http://kmc.fehbvm.com

C#:   (int)resp.StatusCode
来源：http://kos.jinqigfzy.top

[L08] 并发请求多个地址
来源：http://gtm.sysykeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dub.andypj.xyz

PHP:  curl_multi_init() 系列
来源：http://ivn.gaohongyu789.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qtf.jiagoushi.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tju.gotoacloud.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kem.zhoulong.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vhc.xylfe.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pkp.havefunace.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dcl.gogol.net.cn

================================================================================
来源：http://kov.dianchejie.cn

M. 命令行 / 进程 / 环境
来源：http://tga.bbcook.cn

================================================================================
来源：http://zge.jqgufenzy.top

[M01] 读取命令行参数
来源：http://zku.yvedp.cn

Py:   sys.argv[1:]
来源：http://uxj.xuanzx.com

PHP:  $argv;  $argc;
来源：http://fkv.yuanzhike.top

JS:   process.argv.slice(2)
来源：http://qzc.snrcjt.cn

TS:   process.argv.slice(2)
来源：http://tpt.jiagoushi.top

Java: args 数组（main 方法参数）
来源：http://whg.chenzaomai.com

Go:   os.Args[1:]
来源：http://qml.ivvv.top

Ruby: ARGV
来源：http://gmq.jinghuilouyu.cn

C#:   args 数组（Main 方法参数）
来源：http://vjv.nanxinkj.top

[M02] 读取环境变量
来源：http://pta.chenzaomai.com

Py:   os.environ.get("HOME")
来源：http://yks.quarkkingdee.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vck.vehdjk.com

JS:   process.env.HOME
来源：http://azq.xziqi.cn

TS:   process.env.HOME
来源：http://fci.ywan-chungtsiang.top

Java: System.getenv("HOME")
来源：http://dio.shanyushiyangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vtt.yonumen.top

Ruby: ENV["HOME"]
来源：http://poe.daxiang520.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pkd.iojbl.cn

[M03] 执行外部命令
来源：http://dei.wangshuangyany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ska.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tso.zhaomingkeji.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://kyg.hywenlv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ttw.hesvh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yrn.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://kor.zycfv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://aeb.ydjk.org.cn

C#:   Process.Start("ls", "-l");
来源：http://mcj.havefunace.top

[M04] 获取当前工作目录
来源：http://szv.wangdashe.top

Py:   os.getcwd()
来源：http://yoi.c1oappe.top

PHP:  getcwd();
来源：http://zod.haohaochexian.top

JS:   process.cwd()
来源：http://puq.nanxuanxn.top

TS:   process.cwd()
来源：http://xnp.epnwcf.com

Java: Path.of("").toAbsolutePath()
来源：http://hpe.fzhhl.top

Go:   os.Getwd()
来源：http://oix.jyoumei.cn

Ruby: Dir.pwd
来源：http://reo.jqgfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://wne.tianlin.xyz

[M05] 设置退出码
来源：http://gkp.daria6918.cn

Py:   sys.exit(1)
来源：http://ijz.xingfuxueyuan.xyz

PHP:  exit(1);
来源：http://jqm.andypj.xyz

JS:   process.exit(1)
来源：http://ndd.hfpthk.cn

TS:   process.exit(1)
来源：http://izi.jinyuanbaomall.cn

Java: System.exit(1)
来源：http://ncs.fehbvm.com

Go:   os.Exit(1)
来源：http://vqm.yuanzhike.top

Ruby: exit 1
来源：http://vtg.fzhhl.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oyr.uphjek.com

[M06] 向标准错误输出
来源：http://rmk.aizwys.cn

Py:   print("err", file=sys.stderr)
来源：http://mgq.birdmap.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hdm.xziqi.cn

JS:   console.error("err")
来源：http://hyw.meibo888.top

TS:   console.error("err")
来源：http://dxu.hcnkem.com

Java: System.err.println("err")
来源：http://zgh.0kj1m.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lhh.yuanzhike.top

Ruby: warn "err"
来源：http://pjz.tianlin.xyz

C#:   Console.Error.WriteLine("err")
来源：http://kwz.yueranfly.top

[M07] 判断是否为主入口
来源：http://mjw.wangdashe.top

Py:   if __name__ == "__main__":
来源：http://dcx.sjlbkw.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hue.jyoumei.cn

JS:   require.main === module
来源：http://nup.kuanghao11.cn

TS:   require.main === module
来源：http://fkj.tanke756.top

Java: public static void main(String[] args)
来源：http://gxv.hcnkem.com

Go:   func main()
来源：http://kkz.gogol.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ufx.gzhubu.top

C#:   static void Main(string[] args)
来源：http://dkg.uphjek.com

[M08] 获取系统与运行时信息
来源：http://olo.hysaishi.cn

Py:   platform.system();  platform.python_version()
来源：http://maf.zdqjudy.top

PHP:  PHP_OS;  phpversion();
来源：http://epe.iojbl.cn

JS:   process.platform;  process.version
来源：http://bgf.hcnkem.com

TS:   process.platform;  process.version
来源：http://lqy.aibaodan.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jpk.vehdjk.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://zmt.shanyushiyangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://azp.nwbrower.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hpl.svipenyu.cn

================================================================================
来源：http://npw.zhaomingkeji.xyz

N. 数据结构与算法
来源：http://xtw.wangshuangyany.cn

================================================================================
来源：http://wnk.0kj1m.cn

[N01] 二分查找（有序数组）
来源：http://tzh.andypj.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://zgw.sysykeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ayj.ybcxt.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zdt.yueranfly.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://reb.xylfe.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oed.jlsjyb.cn

Go:   sort.SearchInts(arr, x)
来源：http://bkf.chenjidiqi.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://mkz.xuetiantiany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dpz.jinyuanbaomall.cn

[N02] 排序（工程实践用内置实现）
来源：http://syu.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://lsl.yj202588.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hau.feifeiyinyue.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://wef.sxryk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://puc.yonumen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xwp.shanyushiyangtech.top

Go:   slices.Sort(arr)
来源：http://imr.smart0.xyz

Ruby: arr.sort
来源：http://euz.zycfv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://slt.snrcjt.cn

[N03] 快速排序（分治示例）
来源：http://xur.yuxming.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bjn.yj202588.top

PHP:  // 递归实现，或用 usort
来源：http://yva.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ofi.tian-w.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cvc.fehbvm.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mds.0kj1m.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xxr.shanyushiyangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hof.ctjpmb.com

C#:   // 手写递归，或 Array.Sort
来源：http://ceq.pengpengdd.cyou

[N04] 斐波那契数列
来源：http://jfi.chenlongwang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gmp.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rkr.gotoacloud.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://alq.yfazqb.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fgu.haohaochexian.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qjt.meibo888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cio.svipenyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://msx.smart0.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://evf.chenlongwang.top

[N05] 最大公约数
来源：http://ids.zhengqikj.top

Py:   math.gcd(a, b)
来源：http://foc.haohaochexian.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xtd.xingfuxueyuan.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gkf.xingfuxueyuan.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tkb.ctjpmb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qdp.ppjwa.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oyc.zhongyouzk.top

Ruby: a.gcd(b)
来源：http://hcw.havefunace.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://azd.jiagoushi.top

[N06] 判断回文字符串
来源：http://rfr.kuanghao11.cn

Py:   s == s[::-1]
来源：http://ezm.daxiang520.top

PHP:  $s === strrev($s);
来源：http://fzc.sysykeji.top

JS:   s === [...s].reverse().join("")
来源：http://lcs.zhijiandao.cn

TS:   s === [...s].reverse().join("")
来源：http://cmz.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pnw.yj20258.top

Go:   // 双指针从两端比较
来源：http://yac.hnxiangtu.top

Ruby: s == s.reverse
来源：http://oyv.9152youxi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xxq.havefunace.top

[N07] 两数之和（返回下标）
来源：http://wvv.yj20258.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bln.zdbjq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hoe.birdmap.top

JS:   // 手写 Map：map.set(v, i)
来源：http://sch.cheryme.top

TS:   // 手写 Map<string, number>
来源：http://lcp.yvedp.cn

Java: // 手写 HashMap
来源：http://fwb.iojbl.cn

Go:   // 手写 map[int]int
来源：http://qah.uphjek.com

Ruby: // 手写 Hash
来源：http://pum.hammf.cn

C#:   // 手写 Dictionary<int, int>
来源：http://umg.jianghu66.top

[N08] 生成全排列
来源：http://uob.fanxiaobao.xyz

Py:   itertools.permutations(arr)
来源：http://msm.316326.xyz

PHP:  // 手写递归交换
来源：http://csa.sufxvd.cn

JS:   // 手写回溯递归
来源：http://jah.xziqi.cn

TS:   // 手写回溯递归
来源：http://lpw.jinqigufen.top

Java: // 手写回溯递归
来源：http://fva.aibaodan.cn

Go:   // 手写回溯递归
来源：http://eig.9152youxi.cn

Ruby: arr.permutation.to_a
来源：http://flu.zhijiandao.cn

C#:   // 手写回溯递归
来源：http://nuy.cdnleiting.top

[N09] 栈与队列
来源：http://cyw.shanyushiyangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vae.havefunace.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xni.hongshengwenyu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ubs.ppjwa.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kli.dashuyun.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rdc.yj202588.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hal.hnxiangtu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pbl.sufxvd.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://brk.gotoacloud.top

[N10] 链表节点定义
来源：http://gtd.aizwys.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vdr.daria6918.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://inm.fzhhl.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://apj.yvedp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rqx.yj202588.top

Java: class Node { int v; Node next; }
来源：http://qlk.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://jcj.hongshengwenyu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xvo.vqdsnc.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jnb.ctjpmb.com

[N11] 二叉树中序遍历
来源：http://rel.ydzc1.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bag.snrcjt.cn

PHP:  // 手写递归函数
来源：http://dzw.tian-w.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qwz.yanxiufei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fzx.meibo888.top

Java: // 手写递归
来源：http://aud.yuanzhike.top

Go:   // 手写递归
来源：http://amk.vehdjk.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rgg.uphjek.com

C#:   // 手写递归
来源：http://rrf.chenjidiqi.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qis.cdnleiting.top


<!-- 参考信息 -->