代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://brn.fktsv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wrj.wangdashe.top

[K04] 读取 JSON 文件
来源：http://qar.cashguo.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vpi.wangdashe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qpe.zdbjq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zlw.zhaomingkeji.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fju.zycfv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://myb.hfpthk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uxu.daria6918.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ysv.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://arl.nanxinkj.top

[K05] 深拷贝对象
来源：http://wxt.chenlongwang.top

Py:   copy.deepcopy(obj)
来源：http://vur.ybcxt.top

PHP:  unserialize(serialize($obj));
来源：http://vjt.mhx1999.top

JS:   structuredClone(obj)
来源：http://zxg.jinqigfzy.top

TS:   structuredClone(obj)
来源：http://xyx.hammf.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wck.jianghu66.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jbk.gotoacloud.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://axa.yj20258888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zie.daria6918.cn

[K06] 解析 URL 查询串
来源：http://nui.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ykc.xuetiantiany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uez.shanyushiyangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://inz.havefunace.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bbj.zhiwuduotai.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aly.quarkkingdee.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mtw.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ffm.tianlin.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hbj.ywan-chungtsiang.top

[K07] 进制转换
来源：http://sox.redwolf501.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qcj.316326.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nnx.jqgufenzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dbs.zhongyouzk.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jcd.zhiwuduotai.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bvf.xuanzx.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xgf.sweek.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dep.nanxinkj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zuz.ivvv.top

[K08] 二进制序列化（非 JSON）
来源：http://tzl.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://hhs.guannengcc.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qqs.ppjwa.cn

JS:   v8.serialize(obj)        // Node
来源：http://wiu.cashguo.top

TS:   v8.serialize(obj)        // Node
来源：http://hga.cashguo.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://atc.shuidangran.top

Go:   encoding/gob
来源：http://fws.9152youxi.cn

Ruby: Marshal.dump(obj)
来源：http://iri.guannengcc.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zlr.fzhhl.top

================================================================================
来源：http://qeb.yangfankeji.com

L. 网络请求
来源：http://blg.meibo888.top

================================================================================
来源：http://vwq.hysaishi.cn

[L01] 发送 GET 请求
来源：http://qwj.zhixingplan.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ddq.yanxiufei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dub.wangshuangyany.cn

JS:   await fetch(url)
来源：http://pgh.fanxiaobao.xyz

TS:   await fetch(url)
来源：http://vrj.xylfe.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://udn.yfazqb.com

Go:   resp, err := http.Get(url)
来源：http://qqi.yongpay.top

Ruby: Net::HTTP.get(URI(url))
来源：http://iul.kuanghao11.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sjr.redwolf501.top

[L02] 发送 POST JSON
来源：http://jsh.daxiang520.top

Py:   requests.post(url, json={"a": 1})
来源：http://kld.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dhr.yongpay.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ljp.fengsongda.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ggl.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kri.nwbrower.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ash.ivvv.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ppt.hesvh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gvp.cqqwz.cn

[L03] 设置自定义请求头
来源：http://qms.yangfankeji.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sfc.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mjj.zhengqikj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yoc.cdnleiting.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sht.tarul.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tgt.sjlbkw.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vgc.xinyue.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sso.hnxiangtu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://biq.jiagoushi.top

[L04] 设置超时
来源：http://kpb.fengsongda.top

Py:   requests.get(url, timeout=5)
来源：http://swl.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qow.nwbrower.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gel.ppjwa.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nfy.yuxming.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nob.feifeiyinyue.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bfl.zdbjq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vlr.tarul.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kac.epnwcf.com

[L05] 上传文件（multipart）
来源：http://pxw.uphjek.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fjh.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ydt.316326.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ryf.sjlbkw.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mbk.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lpc.sxryk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cke.xylfe.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lnk.hesvh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nvc.hnqzz.top

[L06] 解析响应为 JSON
来源：http://tds.fzhhl.top

Py:   resp.json()
来源：http://wpl.bbcook.cn

PHP:  json_decode($body, true);
来源：http://ohd.hfpthk.cn

JS:   await resp.json()
来源：http://khw.zdbjq.cn

TS:   await resp.json()
来源：http://ehq.snrcjt.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pwx.epnwcf.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iph.jianghu66.top

Ruby: JSON.parse(resp.body)
来源：http://qwa.ehwqpu.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iaj.andypj.xyz

[L07] 处理 HTTP 状态码
来源：http://wih.andypj.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lkb.yangfankeji.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ayj.zhaomingkeji.xyz

JS:   resp.ok;  resp.status
来源：http://tbn.tarul.cn

TS:   resp.ok;  resp.status
来源：http://wrc.yuanzhike.top

Java: resp.statusCode()
来源：http://xmv.svipenyu.cn

Go:   resp.StatusCode
来源：http://uqy.dianchejie.cn

Ruby: resp.code.to_i
来源：http://gfc.yj20258.top

C#:   (int)resp.StatusCode
来源：http://iue.cheryme.top

[L08] 并发请求多个地址
来源：http://fkh.316326.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ozy.sjlbkw.cn

PHP:  curl_multi_init() 系列
来源：http://zyx.cdnleiting.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ssj.sysykeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cdd.bjfxy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aki.tian-w.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vxm.ydzc1.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ccs.hesvh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ard.jinqigufen.top

================================================================================
来源：http://cdz.quarkkingdee.top

M. 命令行 / 进程 / 环境
来源：http://ubq.jianghu66.top

================================================================================
来源：http://oap.sufxvd.cn

[M01] 读取命令行参数
来源：http://gvg.jqgufenzy.top

Py:   sys.argv[1:]
来源：http://xtl.hywenlv.cn

PHP:  $argv;  $argc;
来源：http://mcd.cqqwz.cn

JS:   process.argv.slice(2)
来源：http://ljx.yonumen.top

TS:   process.argv.slice(2)
来源：http://lqv.316326.xyz

Java: args 数组（main 方法参数）
来源：http://snm.zhijiandao.cn

Go:   os.Args[1:]
来源：http://hjy.ybcxt.top

Ruby: ARGV
来源：http://bho.epnwcf.com

C#:   args 数组（Main 方法参数）
来源：http://jco.316326.xyz

[M02] 读取环境变量
来源：http://wjj.jiagoushi.top

Py:   os.environ.get("HOME")
来源：http://yqb.xingfuxueyuan.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dsv.fktsv.cn

JS:   process.env.HOME
来源：http://ggu.52xcode.cn

TS:   process.env.HOME
来源：http://wdq.yangfankeji.com

Java: System.getenv("HOME")
来源：http://uvu.svipenyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://znq.hnqzz.top

Ruby: ENV["HOME"]
来源：http://qjm.fengsongda.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sqr.nanxuanxn.top

[M03] 执行外部命令
来源：http://mkb.sweek.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rnl.redwolf501.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://adw.yfazqb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://maz.nanxinkj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://arf.ydjk.org.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://btq.gzhubu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://udu.tian-w.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zoe.fengsongda.top

C#:   Process.Start("ls", "-l");
来源：http://wzj.epnwcf.com

[M04] 获取当前工作目录
来源：http://yaz.jinqigufen.top

Py:   os.getcwd()
来源：http://als.gogol.net.cn

PHP:  getcwd();
来源：http://euj.yfazqb.com

JS:   process.cwd()
来源：http://emp.jinqigfzy.top

TS:   process.cwd()
来源：http://mtg.ydzc1.top

Java: Path.of("").toAbsolutePath()
来源：http://uhh.shangyingyoupin.top

Go:   os.Getwd()
来源：http://dsx.shanyushiyangtech.top

Ruby: Dir.pwd
来源：http://wyc.daxiang520.top

C#:   Directory.GetCurrentDirectory()
来源：http://qqb.hfpthk.cn

[M05] 设置退出码
来源：http://joz.shzxlz.cn

Py:   sys.exit(1)
来源：http://qsp.tarul.cn

PHP:  exit(1);
来源：http://vax.ehwqpu.com

JS:   process.exit(1)
来源：http://btg.yj20258888.top

TS:   process.exit(1)
来源：http://use.havefunace.top

Java: System.exit(1)
来源：http://gcq.yueranfly.top

Go:   os.Exit(1)
来源：http://uon.zhixingplan.top

Ruby: exit 1
来源：http://iku.jinqigufen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iwn.hongshengwenyu.top

[M06] 向标准错误输出
来源：http://hnr.ctjpmb.com

Py:   print("err", file=sys.stderr)
来源：http://rnq.hongshengwenyu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://shj.yj202588.top

JS:   console.error("err")
来源：http://loi.vehdjk.com

TS:   console.error("err")
来源：http://iie.yj202588.top

Java: System.err.println("err")
来源：http://fwz.zhiwuduotai.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zjc.sweek.top

Ruby: warn "err"
来源：http://gab.cdnleiting.top

C#:   Console.Error.WriteLine("err")
来源：http://aic.tarul.cn

[M07] 判断是否为主入口
来源：http://klt.bbcook.cn

Py:   if __name__ == "__main__":
来源：http://jel.hesvh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nko.ehwqpu.com

JS:   require.main === module
来源：http://ohf.ivvv.top

TS:   require.main === module
来源：http://yfz.uphjek.com

Java: public static void main(String[] args)
来源：http://omm.ydzc1.top

Go:   func main()
来源：http://xej.aibaodan.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vlu.tianlin.xyz

C#:   static void Main(string[] args)
来源：http://svb.daxiang520.top

[M08] 获取系统与运行时信息
来源：http://syc.haohaochexian.top

Py:   platform.system();  platform.python_version()
来源：http://gpx.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://rpy.haohaochexian.top

JS:   process.platform;  process.version
来源：http://lbh.quarkkingdee.top

TS:   process.platform;  process.version
来源：http://ote.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pmj.redwolf501.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://cui.mhx1999.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dbe.yongpay.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://dos.xuetiantiany.cn

================================================================================
来源：http://olc.sysykeji.top

N. 数据结构与算法
来源：http://xaf.zhengqikj.top

================================================================================
来源：http://rze.dianchejie.cn

[N01] 二分查找（有序数组）
来源：http://isr.yangfankeji.com

Py:   bisect.bisect_left(arr, x)
来源：http://ufs.sufxvd.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://khu.zhoulong.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ixb.tanke756.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nzc.316326.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://del.zhongyouzk.top

Go:   sort.SearchInts(arr, x)
来源：http://qnk.zhiwuduotai.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lyn.ctjpmb.com

C#:   Array.BinarySearch(arr, x)
来源：http://vve.xylfe.cn

[N02] 排序（工程实践用内置实现）
来源：http://uta.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://jkn.meibo888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wng.jinyuanbaomall.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xlp.shanyushiyangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mjp.zhijiandao.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sud.hammf.cn

Go:   slices.Sort(arr)
来源：http://lhm.hysaishi.cn

Ruby: arr.sort
来源：http://mvi.316326.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://gxw.zhongyouzk.top

[N03] 快速排序（分治示例）
来源：http://upc.sufxvd.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ekj.shanyushiyangtech.top

PHP:  // 递归实现，或用 usort
来源：http://gpl.zhaomingkeji.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lhz.shanyushiyangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qst.dianchejie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wzr.hesvh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xmg.ctjpmb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nhn.guowangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://mlx.ybcxt.top

[N04] 斐波那契数列
来源：http://xbb.zycfv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ley.smart0.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pik.zhiwuduotai.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://enu.wangshuangyany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pmz.chenjidiqi.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ccb.iojbl.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cpr.yueranfly.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lim.yj202588.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wrm.ybcxt.top

[N05] 最大公约数
来源：http://hhb.shuidangran.top

Py:   math.gcd(a, b)
来源：http://peh.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://usa.hnqzz.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ycp.shuidangran.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://owy.aizwys.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://abq.fzhhl.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kqr.zhaomingkeji.xyz

Ruby: a.gcd(b)
来源：http://ips.yanxiufei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://alf.nwbrower.top

[N06] 判断回文字符串
来源：http://rgq.zhongyouzk.top

Py:   s == s[::-1]
来源：http://qjc.wangdashe.top

PHP:  $s === strrev($s);
来源：http://xlp.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://din.shzxlz.cn

TS:   s === [...s].reverse().join("")
来源：http://oig.sweek.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xcx.chenzaomai.com

Go:   // 双指针从两端比较
来源：http://nde.epnwcf.com

Ruby: s == s.reverse
来源：http://jmz.xinyue.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://kdw.316326.xyz

[N07] 两数之和（返回下标）
来源：http://kff.aizwys.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vrr.cashguo.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://trp.shanyushiyangtech.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bzt.ydzc1.top

TS:   // 手写 Map<string, number>
来源：http://fpa.cdnleiting.top

Java: // 手写 HashMap
来源：http://hal.snrcjt.cn

Go:   // 手写 map[int]int
来源：http://rkp.9152youxi.cn

Ruby: // 手写 Hash
来源：http://jaq.ydzc1.top

C#:   // 手写 Dictionary<int, int>
来源：http://xed.jqgfzy.top

[N08] 生成全排列
来源：http://wdo.c1oappe.top

Py:   itertools.permutations(arr)
来源：http://bgj.zdbjq.cn

PHP:  // 手写递归交换
来源：http://ppe.xuanzx.com

JS:   // 手写回溯递归
来源：http://ghu.hfpthk.cn

TS:   // 手写回溯递归
来源：http://yzn.wangdashe.top

Java: // 手写回溯递归
来源：http://lkb.xinyue.icu

Go:   // 手写回溯递归
来源：http://upl.fengsongda.top

Ruby: arr.permutation.to_a
来源：http://tfq.cucudq.cn

C#:   // 手写回溯递归
来源：http://syf.316326.xyz

[N09] 栈与队列
来源：http://ywi.bbcook.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ltx.chenlongwang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hlr.yuxming.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vgv.ydjk.org.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xrb.haohaochexian.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://brz.mhx1999.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ujz.shangyingyoupin.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wor.zhengqikj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mnp.jiagoushi.top

[N10] 链表节点定义
来源：http://xsx.kuanghao11.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jfc.nwbrower.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ons.yj202588.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zfl.cdnleiting.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://exx.yonumen.top

Java: class Node { int v; Node next; }
来源：http://bcf.jqgufenzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://jnz.redwolf501.top

Ruby: Node = Struct.new(:v, :next)
来源：http://fzf.zhaomingkeji.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://flx.snrcjt.cn

[N11] 二叉树中序遍历
来源：http://jft.xuanzx.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rzn.jiagoushi.top

PHP:  // 手写递归函数
来源：http://ava.cdnleiting.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wth.jqgfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vfk.aizwys.cn

Java: // 手写递归
来源：http://vtf.c1oappe.top

Go:   // 手写递归
来源：http://aac.hnxiangtu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qim.haohaochexian.top

C#:   // 手写递归
来源：http://ikf.shanyushiyangtech.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://opg.shanyushiyangkeji.top


<!-- 参考信息 -->