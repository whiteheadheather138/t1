代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://lqs.redwolf501.top

TS:   JSON.stringify(obj, null, 2)
来源：http://uwt.ydjk.org.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://typ.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ayk.zycfv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://edd.vehdjk.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jch.jqgufenzy.top

[K04] 读取 JSON 文件
来源：http://vcn.shangyingyoupin.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yhf.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kih.daria6918.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iou.ctjpmb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ehv.tianlin.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xba.316326.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lgz.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kzp.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yfz.52xcode.cn

[K05] 深拷贝对象
来源：http://iqs.fehbvm.com

Py:   copy.deepcopy(obj)
来源：http://tcl.ywan-chungtsiang.top

PHP:  unserialize(serialize($obj));
来源：http://uaz.quarkkingdee.top

JS:   structuredClone(obj)
来源：http://qna.quarkkingdee.top

TS:   structuredClone(obj)
来源：http://dkl.guowangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jpc.nanxinkj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://olb.hysaishi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zlx.jianghu66.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jqh.zhijiandao.cn

[K06] 解析 URL 查询串
来源：http://sbs.redwolf501.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ymq.guowangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vxb.vqdsnc.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ndt.andypj.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://maq.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ujz.jinyuanbaomall.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nao.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cdd.zdqjudy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wzh.yonumen.top

[K07] 进制转换
来源：http://pun.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yxa.ydzc1.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yul.mhx1999.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gof.iojbl.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cqu.hcnkem.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aas.hywenlv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ixd.yvedp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jkv.epnwcf.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ajq.uphjek.com

[K08] 二进制序列化（非 JSON）
来源：http://zzo.jinyuanbaomall.cn

Py:   pickle.dumps(obj)
来源：http://rcp.guannengcc.top

PHP:  serialize($obj);  unserialize($s);
来源：http://uyc.zycfv.cn

JS:   v8.serialize(obj)        // Node
来源：http://pmx.sjlbkw.cn

TS:   v8.serialize(obj)        // Node
来源：http://gac.yuxming.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kpq.gaohongyu789.top

Go:   encoding/gob
来源：http://frp.jinqigufen.top

Ruby: Marshal.dump(obj)
来源：http://fun.fzhhl.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gal.hnxiangtu.top

================================================================================
来源：http://mqp.cqqwz.cn

L. 网络请求
来源：http://fbz.sxryk.cn

================================================================================
来源：http://czu.vqdsnc.cn

[L01] 发送 GET 请求
来源：http://bml.jinqigufen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ewy.smart0.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fvg.nwbrower.top

JS:   await fetch(url)
来源：http://twi.pengpengdd.cyou

TS:   await fetch(url)
来源：http://afs.aizwys.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kce.yueranfly.top

Go:   resp, err := http.Get(url)
来源：http://hrz.snrcjt.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hdr.cucudq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mgm.zhixingplan.top

[L02] 发送 POST JSON
来源：http://qee.52xcode.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kiw.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qkp.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lay.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zwh.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zwu.hcnkem.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fbt.haohaochexian.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wum.jinyuanbaomall.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uwx.tanke756.top

[L03] 设置自定义请求头
来源：http://lob.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fub.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cva.meibo888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lhz.yj20258888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dih.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nkf.hammf.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pbc.hnxiangtu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ply.havefunace.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lke.quarkkingdee.top

[L04] 设置超时
来源：http://ypk.tian-w.cn

Py:   requests.get(url, timeout=5)
来源：http://yeu.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://isu.vehdjk.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vad.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cio.316326.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dpv.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dce.nwbrower.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pni.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://quk.jqgfzy.top

[L05] 上传文件（multipart）
来源：http://aex.yuanzhike.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dml.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://evh.0kj1m.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mnc.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ivx.svipenyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bkw.hywenlv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jiu.shanyushiyangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qyp.zhaomingkeji.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zih.sufxvd.cn

[L06] 解析响应为 JSON
来源：http://yrx.hysaishi.cn

Py:   resp.json()
来源：http://tvk.tarul.cn

PHP:  json_decode($body, true);
来源：http://def.kuanghao11.cn

JS:   await resp.json()
来源：http://eaq.yonumen.top

TS:   await resp.json()
来源：http://wee.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zik.guannengcc.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ieh.cashguo.top

Ruby: JSON.parse(resp.body)
来源：http://rah.zhijiandao.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sry.chenzaomai.com

[L07] 处理 HTTP 状态码
来源：http://vla.9152youxi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uot.fengsongda.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tnf.yj20258888.top

JS:   resp.ok;  resp.status
来源：http://xnw.gaohongyu789.top

TS:   resp.ok;  resp.status
来源：http://sgq.fehbvm.com

Java: resp.statusCode()
来源：http://itr.zdqjudy.top

Go:   resp.StatusCode
来源：http://dog.hongshengwenyu.top

Ruby: resp.code.to_i
来源：http://pmt.zhengqikj.top

C#:   (int)resp.StatusCode
来源：http://def.gogol.net.cn

[L08] 并发请求多个地址
来源：http://hgx.xinyue.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ckc.gzhubu.top

PHP:  curl_multi_init() 系列
来源：http://orj.xylfe.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ikr.aizwys.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zwk.quarkkingdee.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://skc.xingfuxueyuan.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://msd.sweek.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mpr.0kj1m.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qjz.shangyingyoupin.top

================================================================================
来源：http://ttg.mhx1999.top

M. 命令行 / 进程 / 环境
来源：http://kvt.hongshengwenyu.top

================================================================================
来源：http://pbr.yonumen.top

[M01] 读取命令行参数
来源：http://qfx.xylfe.cn

Py:   sys.argv[1:]
来源：http://yvw.gzhubu.top

PHP:  $argv;  $argc;
来源：http://wxk.zhoulong.xyz

JS:   process.argv.slice(2)
来源：http://tja.aibaodan.cn

TS:   process.argv.slice(2)
来源：http://msp.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://xjk.mhx1999.top

Go:   os.Args[1:]
来源：http://urx.0kj1m.cn

Ruby: ARGV
来源：http://kil.birdmap.top

C#:   args 数组（Main 方法参数）
来源：http://whc.gzhubu.top

[M02] 读取环境变量
来源：http://vju.shanyushiyangtech.top

Py:   os.environ.get("HOME")
来源：http://jkx.aizwys.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gur.yj20258888.top

JS:   process.env.HOME
来源：http://utu.jqgfzy.top

TS:   process.env.HOME
来源：http://vak.ppjwa.cn

Java: System.getenv("HOME")
来源：http://pcn.zhiwuduotai.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hpr.jqgfzy.top

Ruby: ENV["HOME"]
来源：http://zme.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fyo.feifeiyinyue.top

[M03] 执行外部命令
来源：http://vtk.fehbvm.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jes.uphjek.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lxh.yonumen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://eip.hysaishi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tvv.birdmap.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tjp.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://ayj.havefunace.top

Ruby: system("ls -l");  `ls -l`
来源：http://jez.andypj.xyz

C#:   Process.Start("ls", "-l");
来源：http://khx.xuanzx.com

[M04] 获取当前工作目录
来源：http://fvc.aizwys.cn

Py:   os.getcwd()
来源：http://rvn.redwolf501.top

PHP:  getcwd();
来源：http://jhq.shuidangran.top

JS:   process.cwd()
来源：http://bpg.yfazqb.com

TS:   process.cwd()
来源：http://vyw.zhoulong.xyz

Java: Path.of("").toAbsolutePath()
来源：http://sfu.jiagoushi.top

Go:   os.Getwd()
来源：http://wju.jyoumei.cn

Ruby: Dir.pwd
来源：http://iia.zhongyouzk.top

C#:   Directory.GetCurrentDirectory()
来源：http://lds.jqgufenzy.top

[M05] 设置退出码
来源：http://luo.ppjwa.cn

Py:   sys.exit(1)
来源：http://kee.aizwys.cn

PHP:  exit(1);
来源：http://cvm.cqqwz.cn

JS:   process.exit(1)
来源：http://qku.ivvv.top

TS:   process.exit(1)
来源：http://bdx.hammf.cn

Java: System.exit(1)
来源：http://esi.gogol.net.cn

Go:   os.Exit(1)
来源：http://von.yanxiufei.cn

Ruby: exit 1
来源：http://jof.yj202588.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dih.yongpay.top

[M06] 向标准错误输出
来源：http://zvm.smart0.xyz

Py:   print("err", file=sys.stderr)
来源：http://zxg.tarul.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ibz.ppjwa.cn

JS:   console.error("err")
来源：http://jyb.quarkkingdee.top

TS:   console.error("err")
来源：http://gjb.jqgufenzy.top

Java: System.err.println("err")
来源：http://ksl.kuanghao11.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ske.zhongyouzk.top

Ruby: warn "err"
来源：http://ddn.9152youxi.cn

C#:   Console.Error.WriteLine("err")
来源：http://grj.bjfxy.top

[M07] 判断是否为主入口
来源：http://mdp.vehdjk.com

Py:   if __name__ == "__main__":
来源：http://dul.kuanghao11.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uwq.yonumen.top

JS:   require.main === module
来源：http://crl.dashuyun.cn

TS:   require.main === module
来源：http://hfr.c1oappe.top

Java: public static void main(String[] args)
来源：http://qsr.yangfankeji.com

Go:   func main()
来源：http://tyv.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ath.feifeiyinyue.top

C#:   static void Main(string[] args)
来源：http://lbv.sjlbkw.cn

[M08] 获取系统与运行时信息
来源：http://ndt.chenlongwang.top

Py:   platform.system();  platform.python_version()
来源：http://gfp.nanxinkj.top

PHP:  PHP_OS;  phpversion();
来源：http://uwh.cqqwz.cn

JS:   process.platform;  process.version
来源：http://zcv.hysaishi.cn

TS:   process.platform;  process.version
来源：http://msq.hcnkem.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://moq.mhx1999.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wdw.quarkkingdee.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qty.mhx1999.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fdn.gotoacloud.top

================================================================================
来源：http://uqx.havefunace.top

N. 数据结构与算法
来源：http://lbe.tianlin.xyz

================================================================================
来源：http://zpi.52xcode.cn

[N01] 二分查找（有序数组）
来源：http://mwd.yanxiufei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qal.zhengqikj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://usg.gzhubu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pwx.kuanghao11.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://slp.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://yjq.vqdsnc.cn

Go:   sort.SearchInts(arr, x)
来源：http://kbp.yvedp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://swl.yangfankeji.com

C#:   Array.BinarySearch(arr, x)
来源：http://dnc.yj20258888.top

[N02] 排序（工程实践用内置实现）
来源：http://udk.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://vsa.zdbjq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zfv.svipenyu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wwx.shanyushiyangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ieb.sjlbkw.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lxg.tianlin.xyz

Go:   slices.Sort(arr)
来源：http://tkg.chenlongwang.top

Ruby: arr.sort
来源：http://mvu.yangfankeji.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://fgn.sweek.top

[N03] 快速排序（分治示例）
来源：http://voi.wangdashe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fee.zhijiandao.cn

PHP:  // 递归实现，或用 usort
来源：http://hxh.zhijiandao.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bwp.iojbl.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vvf.yangfankeji.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pxt.cqqwz.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zcr.jlsjyb.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dms.epnwcf.com

C#:   // 手写递归，或 Array.Sort
来源：http://ode.havefunace.top

[N04] 斐波那契数列
来源：http://zmt.aibaodan.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ymg.chenzaomai.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://usi.tanke756.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rtt.hongshengwenyu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qcf.yangfankeji.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hfd.hammf.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rid.chenlongwang.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eai.daxiang520.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ggf.shanyushiyangtech.top

[N05] 最大公约数
来源：http://jae.tianlin.xyz

Py:   math.gcd(a, b)
来源：http://hdk.shuidangran.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://szr.sweek.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rxq.zhengqikj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bbk.xinyue.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://asa.andypj.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zsi.316326.xyz

Ruby: a.gcd(b)
来源：http://pga.mhx1999.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kyf.zhengqikj.top

[N06] 判断回文字符串
来源：http://bbx.tian-w.cn

Py:   s == s[::-1]
来源：http://mgo.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://mns.iojbl.cn

JS:   s === [...s].reverse().join("")
来源：http://stc.ydzc1.top

TS:   s === [...s].reverse().join("")
来源：http://wor.fanxiaobao.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dhv.hongshengwenyu.top

Go:   // 双指针从两端比较
来源：http://flk.fzhhl.top

Ruby: s == s.reverse
来源：http://ajs.ywan-chungtsiang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gfd.gotoacloud.top

[N07] 两数之和（返回下标）
来源：http://lir.ivvv.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sub.jinqigufen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://urp.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tin.yfazqb.com

TS:   // 手写 Map<string, number>
来源：http://ife.hesvh.cn

Java: // 手写 HashMap
来源：http://sna.zhongyouzk.top

Go:   // 手写 map[int]int
来源：http://nnm.yongpay.top

Ruby: // 手写 Hash
来源：http://qkx.birdmap.top

C#:   // 手写 Dictionary<int, int>
来源：http://kss.yuanzhike.top

[N08] 生成全排列
来源：http://hql.vehdjk.com

Py:   itertools.permutations(arr)
来源：http://cde.xziqi.cn

PHP:  // 手写递归交换
来源：http://lig.yanxiufei.cn

JS:   // 手写回溯递归
来源：http://jtl.daria6918.cn

TS:   // 手写回溯递归
来源：http://pbz.jiagoushi.top

Java: // 手写回溯递归
来源：http://ifb.zhongyouzk.top

Go:   // 手写回溯递归
来源：http://rsa.ydzc1.top

Ruby: arr.permutation.to_a
来源：http://oyi.kuanghao11.cn

C#:   // 手写回溯递归
来源：http://hia.aizwys.cn

[N09] 栈与队列
来源：http://wmu.jqgufenzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oik.ctjpmb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oci.smart0.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gah.snrcjt.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lmi.zycfv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fln.cqqwz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uew.ybcxt.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://smu.aizwys.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yja.yuanzhike.top

[N10] 链表节点定义
来源：http://mds.ybcxt.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://smi.yj20258.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dkq.quarkkingdee.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bst.quarkkingdee.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tsv.bjfxy.top

Java: class Node { int v; Node next; }
来源：http://xht.gotoacloud.top

Go:   type Node struct { V int; Next *Node }
来源：http://qsw.ctjpmb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://egu.nanxinkj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://yxk.cheryme.top

[N11] 二叉树中序遍历
来源：http://vws.fktsv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gdt.vqdsnc.cn

PHP:  // 手写递归函数
来源：http://lue.yongpay.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lzx.cheryme.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mog.birdmap.top

Java: // 手写递归
来源：http://wzd.jlsjyb.cn


<!-- 参考信息 -->