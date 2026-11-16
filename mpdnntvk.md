代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://otx.zdbjq.cn

[K03] JSON 美化输出（带缩进）
来源：http://mki.jqgfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hlo.c1oappe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ulk.vqdsnc.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gik.xingfuxueyuan.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://kdv.daria6918.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://opb.iojbl.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wxq.pycfn.com

Ruby: JSON.pretty_generate(obj)
来源：http://lum.ivvv.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yqe.vehdjk.com

[K04] 读取 JSON 文件
来源：http://gvv.yanxiufei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://htn.nanxuanxn.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xvm.yongpay.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fsb.xylfe.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://buv.dianchejie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wwx.52xcode.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ixn.zhijiandao.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hqf.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dmq.xylfe.cn

[K05] 深拷贝对象
来源：http://uin.gogol.net.cn

Py:   copy.deepcopy(obj)
来源：http://ryp.xuetiantiany.cn

PHP:  unserialize(serialize($obj));
来源：http://csv.epnwcf.com

JS:   structuredClone(obj)
来源：http://yyb.shanyushiyangkeji.top

TS:   structuredClone(obj)
来源：http://rfv.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://izi.gzhubu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kae.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cyv.hysaishi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xut.52xcode.cn

[K06] 解析 URL 查询串
来源：http://cpn.guannengcc.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zdf.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nas.yuxming.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jkw.c1oappe.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bdn.hnxiangtu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fqy.nwbrower.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jou.yonumen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mpz.uphjek.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ogk.hesvh.cn

[K07] 进制转换
来源：http://bxz.gzhubu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gfc.gogol.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dvk.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dbs.chenjidiqi.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bmk.hcnkem.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ybn.iojbl.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ewj.hcnkem.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lex.0kj1m.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pcj.shanyushiyangtech.top

[K08] 二进制序列化（非 JSON）
来源：http://yng.iojbl.cn

Py:   pickle.dumps(obj)
来源：http://cyc.mhx1999.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qdl.hysaishi.cn

JS:   v8.serialize(obj)        // Node
来源：http://zga.cucudq.cn

TS:   v8.serialize(obj)        // Node
来源：http://okf.yj20258888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jqp.epnwcf.com

Go:   encoding/gob
来源：http://ayi.pycfn.com

Ruby: Marshal.dump(obj)
来源：http://mxq.hongshengwenyu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rsu.xziqi.cn

================================================================================
来源：http://exp.havefunace.top

L. 网络请求
来源：http://tul.fengsongda.top

================================================================================
来源：http://bfd.gaohongyu789.top

[L01] 发送 GET 请求
来源：http://bnc.zhixingplan.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xrd.zycfv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zpk.ydjk.org.cn

JS:   await fetch(url)
来源：http://ymz.gotoacloud.top

TS:   await fetch(url)
来源：http://jlo.yj202588.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://heo.dianchejie.cn

Go:   resp, err := http.Get(url)
来源：http://rsf.zhaomingkeji.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://ojc.zycfv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yrr.fanxiaobao.xyz

[L02] 发送 POST JSON
来源：http://imb.gzhubu.top

Py:   requests.post(url, json={"a": 1})
来源：http://frr.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bpf.zhiwuduotai.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eid.zhiwuduotai.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jfp.cheryme.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pnb.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rrf.yonumen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tlu.jlsjyb.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rre.havefunace.top

[L03] 设置自定义请求头
来源：http://nbd.fehbvm.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wpk.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pvu.vqdsnc.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ywz.tarul.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fdk.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rbo.hcnkem.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gjm.cqqwz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://osq.chenlongwang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yti.cdnleiting.top

[L04] 设置超时
来源：http://qzy.bbcook.cn

Py:   requests.get(url, timeout=5)
来源：http://heg.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://osa.hammf.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pmz.hnqzz.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ulw.cheryme.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://buy.yuxming.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://emt.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bcf.sufxvd.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fsv.zhiwuduotai.top

[L05] 上传文件（multipart）
来源：http://kyj.mhx1999.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://myt.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://law.mhx1999.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zmq.kuanghao11.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sgi.fktsv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bwt.guowangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fgz.sxryk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ilr.nanxuanxn.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wor.cucudq.cn

[L06] 解析响应为 JSON
来源：http://bfm.yangfankeji.com

Py:   resp.json()
来源：http://adf.hongshengwenyu.top

PHP:  json_decode($body, true);
来源：http://sim.jinqigfzy.top

JS:   await resp.json()
来源：http://xhm.pycfn.com

TS:   await resp.json()
来源：http://vps.shangyingyoupin.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sma.xinyue.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kmh.yongpay.top

Ruby: JSON.parse(resp.body)
来源：http://poh.yonumen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mex.jyoumei.cn

[L07] 处理 HTTP 状态码
来源：http://xvj.wangdashe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qku.cashguo.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://efx.jinqigfzy.top

JS:   resp.ok;  resp.status
来源：http://vhq.shzxlz.cn

TS:   resp.ok;  resp.status
来源：http://bbt.zhiwuduotai.top

Java: resp.statusCode()
来源：http://iym.cashguo.top

Go:   resp.StatusCode
来源：http://szb.yj20258888.top

Ruby: resp.code.to_i
来源：http://cbq.cheryme.top

C#:   (int)resp.StatusCode
来源：http://yxw.andypj.xyz

[L08] 并发请求多个地址
来源：http://snm.smart0.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tux.cheryme.top

PHP:  curl_multi_init() 系列
来源：http://iwc.tanke756.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yry.ybcxt.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ggv.zhengqikj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vab.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://unb.bjfxy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hxj.snrcjt.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zbu.guannengcc.top

================================================================================
来源：http://hqs.ivvv.top

M. 命令行 / 进程 / 环境
来源：http://jgx.wangshuangyany.cn

================================================================================
来源：http://npl.chenzaomai.com

[M01] 读取命令行参数
来源：http://sou.jinghuilouyu.cn

Py:   sys.argv[1:]
来源：http://ikt.daxiang520.top

PHP:  $argv;  $argc;
来源：http://zbb.52xcode.cn

JS:   process.argv.slice(2)
来源：http://cwt.ivvv.top

TS:   process.argv.slice(2)
来源：http://gqt.mhx1999.top

Java: args 数组（main 方法参数）
来源：http://jql.pengpengdd.cyou

Go:   os.Args[1:]
来源：http://xmg.dianchejie.cn

Ruby: ARGV
来源：http://ufs.ehwqpu.com

C#:   args 数组（Main 方法参数）
来源：http://mys.fehbvm.com

[M02] 读取环境变量
来源：http://wze.cdnleiting.top

Py:   os.environ.get("HOME")
来源：http://wrq.dashuyun.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rzu.xinyue.icu

JS:   process.env.HOME
来源：http://bke.jianghu66.top

TS:   process.env.HOME
来源：http://vko.epnwcf.com

Java: System.getenv("HOME")
来源：http://set.yj202588.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lzc.zycfv.cn

Ruby: ENV["HOME"]
来源：http://nwx.yanxiufei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qgx.mhx1999.top

[M03] 执行外部命令
来源：http://lzh.zdbjq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uei.quarkkingdee.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://aab.xuetiantiany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jwt.zhijiandao.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mxf.aibaodan.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://enm.jiagoushi.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yjl.wangshuangyany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://aaq.xingfuxueyuan.xyz

C#:   Process.Start("ls", "-l");
来源：http://yvp.guowangkeji.top

[M04] 获取当前工作目录
来源：http://cfe.jianghu66.top

Py:   os.getcwd()
来源：http://hec.gzhubu.top

PHP:  getcwd();
来源：http://yvd.bjfxy.top

JS:   process.cwd()
来源：http://dgp.dianchejie.cn

TS:   process.cwd()
来源：http://fil.tian-w.cn

Java: Path.of("").toAbsolutePath()
来源：http://nsg.tarul.cn

Go:   os.Getwd()
来源：http://sjx.c1oappe.top

Ruby: Dir.pwd
来源：http://poo.ybcxt.top

C#:   Directory.GetCurrentDirectory()
来源：http://hgf.mhx1999.top

[M05] 设置退出码
来源：http://vmg.gogol.net.cn

Py:   sys.exit(1)
来源：http://fob.redwolf501.top

PHP:  exit(1);
来源：http://zzd.dianchejie.cn

JS:   process.exit(1)
来源：http://llt.vehdjk.com

TS:   process.exit(1)
来源：http://tls.birdmap.top

Java: System.exit(1)
来源：http://lnq.jyoumei.cn

Go:   os.Exit(1)
来源：http://ylu.zhongyouzk.top

Ruby: exit 1
来源：http://vzv.zhengqikj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://crz.316326.xyz

[M06] 向标准错误输出
来源：http://tbh.yvedp.cn

Py:   print("err", file=sys.stderr)
来源：http://awc.ctjpmb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://pon.aibaodan.cn

JS:   console.error("err")
来源：http://cgo.wangdashe.top

TS:   console.error("err")
来源：http://tpe.yfazqb.com

Java: System.err.println("err")
来源：http://wlg.pengpengdd.cyou

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ogh.xuetiantiany.cn

Ruby: warn "err"
来源：http://srz.cheryme.top

C#:   Console.Error.WriteLine("err")
来源：http://ont.bjfxy.top

[M07] 判断是否为主入口
来源：http://urd.epnwcf.com

Py:   if __name__ == "__main__":
来源：http://cfe.ivvv.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tbx.cucudq.cn

JS:   require.main === module
来源：http://yjq.hysaishi.cn

TS:   require.main === module
来源：http://yrt.shanyushiyangkeji.top

Java: public static void main(String[] args)
来源：http://eil.dianchejie.cn

Go:   func main()
来源：http://hve.pycfn.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bsk.birdmap.top

C#:   static void Main(string[] args)
来源：http://lhd.hongshengwenyu.top

[M08] 获取系统与运行时信息
来源：http://myg.pycfn.com

Py:   platform.system();  platform.python_version()
来源：http://efe.gogol.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://qhq.iojbl.cn

JS:   process.platform;  process.version
来源：http://hst.jinqigufen.top

TS:   process.platform;  process.version
来源：http://nff.xylfe.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bjd.nwbrower.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vos.smart0.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pvf.zhongyouzk.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jas.9152youxi.cn

================================================================================
来源：http://xxx.cdnleiting.top

N. 数据结构与算法
来源：http://opq.ydjk.org.cn

================================================================================
来源：http://wsv.daxiang520.top

[N01] 二分查找（有序数组）
来源：http://agi.pengpengdd.cyou

Py:   bisect.bisect_left(arr, x)
来源：http://fej.ctjpmb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ino.cheryme.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gln.jyoumei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lif.havefunace.top

Java: Arrays.binarySearch(arr, x)
来源：http://gbs.pengpengdd.cyou

Go:   sort.SearchInts(arr, x)
来源：http://zvp.fehbvm.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://fsz.fehbvm.com

C#:   Array.BinarySearch(arr, x)
来源：http://ijv.aibaodan.cn

[N02] 排序（工程实践用内置实现）
来源：http://rop.sweek.top

Py:   sorted(arr);  arr.sort()
来源：http://lxt.xylfe.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ukn.sufxvd.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://syj.jinghuilouyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yih.zdqjudy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gow.hnqzz.top

Go:   slices.Sort(arr)
来源：http://mel.hammf.cn

Ruby: arr.sort
来源：http://xfj.fengsongda.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://moh.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://fag.sysykeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jjj.epnwcf.com

PHP:  // 递归实现，或用 usort
来源：http://qlz.ehwqpu.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wuy.yvedp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mbr.nanxuanxn.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hft.fzhhl.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ehu.bjfxy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://imu.jinyuanbaomall.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ylu.hcnkem.com

[N04] 斐波那契数列
来源：http://nwf.fehbvm.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jbn.sweek.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ipd.gzhubu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vrh.0kj1m.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oxl.hnqzz.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ngv.shanyushiyangtech.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zye.yfazqb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://iyo.yonumen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bdp.nanxinkj.top

[N05] 最大公约数
来源：http://usn.zhoulong.xyz

Py:   math.gcd(a, b)
来源：http://pmd.tianlin.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://miw.daria6918.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nls.sysykeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vbn.fzhhl.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fog.yangfankeji.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uqn.epnwcf.com

Ruby: a.gcd(b)
来源：http://zog.jianghu66.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pio.zhixingplan.top

[N06] 判断回文字符串
来源：http://vpp.yfazqb.com

Py:   s == s[::-1]
来源：http://rfu.wangdashe.top

PHP:  $s === strrev($s);
来源：http://lub.c1oappe.top

JS:   s === [...s].reverse().join("")
来源：http://hre.tarul.cn

TS:   s === [...s].reverse().join("")
来源：http://qxu.ydzc1.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kfy.hesvh.cn

Go:   // 双指针从两端比较
来源：http://mtg.bjfxy.top

Ruby: s == s.reverse
来源：http://qgb.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://rom.c1oappe.top

[N07] 两数之和（返回下标）
来源：http://kfp.zdqjudy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://miu.tarul.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cqc.jinqigufen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://hud.dianchejie.cn

TS:   // 手写 Map<string, number>
来源：http://iiu.gaohongyu789.top

Java: // 手写 HashMap
来源：http://uqd.wangdashe.top

Go:   // 手写 map[int]int
来源：http://pwq.sxryk.cn

Ruby: // 手写 Hash
来源：http://eys.xylfe.cn

C#:   // 手写 Dictionary<int, int>
来源：http://euz.xuanzx.com

[N08] 生成全排列
来源：http://ndr.9152youxi.cn

Py:   itertools.permutations(arr)
来源：http://ftd.dashuyun.cn

PHP:  // 手写递归交换
来源：http://zcf.9152youxi.cn

JS:   // 手写回溯递归
来源：http://gsj.shanyushiyangtech.top

TS:   // 手写回溯递归
来源：http://jsz.zdqjudy.top

Java: // 手写回溯递归
来源：http://dww.hnqzz.top

Go:   // 手写回溯递归
来源：http://non.mhx1999.top

Ruby: arr.permutation.to_a
来源：http://rgu.mhx1999.top

C#:   // 手写回溯递归
来源：http://zfc.tianlin.xyz

[N09] 栈与队列
来源：http://ppu.yonumen.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ltw.hesvh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bld.chenjidiqi.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aze.chenlongwang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://han.cdnleiting.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lka.feifeiyinyue.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bdb.jinqigufen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pfn.yj20258.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eyg.redwolf501.top

[N10] 链表节点定义
来源：http://mih.zhixingplan.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://igw.pycfn.com

PHP:  class Node { public $v; public $next = null; }
来源：http://syw.jqgfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vfl.ppjwa.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jnl.jinqigfzy.top

Java: class Node { int v; Node next; }
来源：http://qyz.yj20258888.top

Go:   type Node struct { V int; Next *Node }
来源：http://diu.316326.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://ogd.shanyushiyangtech.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lab.gzhubu.top

[N11] 二叉树中序遍历
来源：http://cxn.cashguo.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wig.hnxiangtu.top


<!-- 参考信息 -->