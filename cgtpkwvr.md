代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://ymw.hcnkem.com

TS:   JSON.stringify(obj, null, 2)
来源：http://wbn.nwbrower.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dpu.tianlin.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tyv.chenzaomai.com

Ruby: JSON.pretty_generate(obj)
来源：http://xvk.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fpk.redwolf501.top

[K04] 读取 JSON 文件
来源：http://tbx.sufxvd.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vfj.0kj1m.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fxw.jiagoushi.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nah.daxiang520.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fbm.0kj1m.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pix.vehdjk.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dmh.mhx1999.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qqj.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xwh.zycfv.cn

[K05] 深拷贝对象
来源：http://wyz.jqgfzy.top

Py:   copy.deepcopy(obj)
来源：http://hks.haohaochexian.top

PHP:  unserialize(serialize($obj));
来源：http://uxe.iojbl.cn

JS:   structuredClone(obj)
来源：http://aco.fehbvm.com

TS:   structuredClone(obj)
来源：http://tej.cheryme.top

Java: // 手写拷贝构造，或序列化往返
来源：http://etd.316326.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ugw.cucudq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ejz.sxryk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lte.vqdsnc.cn

[K06] 解析 URL 查询串
来源：http://jxa.snrcjt.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bfw.pengpengdd.cyou

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yvq.ppjwa.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tih.ppjwa.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dgk.epnwcf.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kue.snrcjt.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gua.cucudq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eva.cheryme.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zhb.ybcxt.top

[K07] 进制转换
来源：http://syi.jyoumei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vfh.yangfankeji.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pzo.andypj.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://azf.cucudq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cgn.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ain.zhiwuduotai.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sze.kuanghao11.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sdz.nwbrower.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://klo.hywenlv.cn

[K08] 二进制序列化（非 JSON）
来源：http://uas.ehwqpu.com

Py:   pickle.dumps(obj)
来源：http://rqo.pengpengdd.cyou

PHP:  serialize($obj);  unserialize($s);
来源：http://hyx.quarkkingdee.top

JS:   v8.serialize(obj)        // Node
来源：http://flu.xylfe.cn

TS:   v8.serialize(obj)        // Node
来源：http://fxc.yj20258.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://phe.quarkkingdee.top

Go:   encoding/gob
来源：http://ahk.meibo888.top

Ruby: Marshal.dump(obj)
来源：http://blw.yj20258888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gea.ivvv.top

================================================================================
来源：http://dru.gotoacloud.top

L. 网络请求
来源：http://bbn.bjfxy.top

================================================================================
来源：http://hvx.xuanzx.com

[L01] 发送 GET 请求
来源：http://zof.gotoacloud.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iry.jyoumei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jvu.nanxinkj.top

JS:   await fetch(url)
来源：http://ccv.jianghu66.top

TS:   await fetch(url)
来源：http://ysc.gaohongyu789.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rgm.yongpay.top

Go:   resp, err := http.Get(url)
来源：http://kat.gaohongyu789.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nlf.tanke756.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gqc.daxiang520.top

[L02] 发送 POST JSON
来源：http://lno.hnxiangtu.top

Py:   requests.post(url, json={"a": 1})
来源：http://pav.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://del.hywenlv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uux.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iaf.316326.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qcm.dashuyun.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ast.shangyingyoupin.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pgo.hongshengwenyu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://znr.zhaomingkeji.xyz

[L03] 设置自定义请求头
来源：http://zyw.sweek.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ecg.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jik.meibo888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bdw.hammf.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dai.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://avn.ppjwa.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zna.jqgfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eiz.sxryk.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zym.sysykeji.top

[L04] 设置超时
来源：http://twq.ivvv.top

Py:   requests.get(url, timeout=5)
来源：http://erb.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vik.ivvv.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sxi.snrcjt.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://njv.tianlin.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jbf.yongpay.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xkk.fktsv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://svy.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mee.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://rel.andypj.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vib.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vaz.aizwys.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://izb.yongpay.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ilx.zhaomingkeji.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kpc.yfazqb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gbm.ydjk.org.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vuj.sxryk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rgc.quarkkingdee.top

[L06] 解析响应为 JSON
来源：http://lod.yj20258.top

Py:   resp.json()
来源：http://eie.jianghu66.top

PHP:  json_decode($body, true);
来源：http://vvv.tarul.cn

JS:   await resp.json()
来源：http://nwe.jinqigfzy.top

TS:   await resp.json()
来源：http://ocv.tian-w.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kmx.c1oappe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ykq.jqgufenzy.top

Ruby: JSON.parse(resp.body)
来源：http://way.hywenlv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ggf.fehbvm.com

[L07] 处理 HTTP 状态码
来源：http://amv.hammf.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kmm.vqdsnc.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dns.guannengcc.top

JS:   resp.ok;  resp.status
来源：http://tnw.hesvh.cn

TS:   resp.ok;  resp.status
来源：http://jgi.xylfe.cn

Java: resp.statusCode()
来源：http://mfr.jinyuanbaomall.cn

Go:   resp.StatusCode
来源：http://bvo.xuetiantiany.cn

Ruby: resp.code.to_i
来源：http://wxa.jinqigufen.top

C#:   (int)resp.StatusCode
来源：http://yaa.yvedp.cn

[L08] 并发请求多个地址
来源：http://pqz.birdmap.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ohl.52xcode.cn

PHP:  curl_multi_init() 系列
来源：http://ulo.yanxiufei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yiv.ywan-chungtsiang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ydi.jinghuilouyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wvi.ybcxt.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://juc.0kj1m.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://elz.zdbjq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mga.sjlbkw.cn

================================================================================
来源：http://qfo.zhixingplan.top

M. 命令行 / 进程 / 环境
来源：http://evg.haohaochexian.top

================================================================================
来源：http://pvi.dashuyun.cn

[M01] 读取命令行参数
来源：http://unu.tanke756.top

Py:   sys.argv[1:]
来源：http://pbg.tian-w.cn

PHP:  $argv;  $argc;
来源：http://jga.ppjwa.cn

JS:   process.argv.slice(2)
来源：http://dzb.chenzaomai.com

TS:   process.argv.slice(2)
来源：http://crk.shanyushiyangtech.top

Java: args 数组（main 方法参数）
来源：http://pql.jlsjyb.cn

Go:   os.Args[1:]
来源：http://xmz.ybcxt.top

Ruby: ARGV
来源：http://wrw.zhengqikj.top

C#:   args 数组（Main 方法参数）
来源：http://wha.yfazqb.com

[M02] 读取环境变量
来源：http://nyf.ydzc1.top

Py:   os.environ.get("HOME")
来源：http://nlu.chenlongwang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dfy.ywan-chungtsiang.top

JS:   process.env.HOME
来源：http://vjz.snrcjt.cn

TS:   process.env.HOME
来源：http://bou.fktsv.cn

Java: System.getenv("HOME")
来源：http://tnb.zhiwuduotai.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aio.shanyushiyangtech.top

Ruby: ENV["HOME"]
来源：http://ylr.andypj.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cwc.ppjwa.cn

[M03] 执行外部命令
来源：http://ysv.nwbrower.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rvi.hnxiangtu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rjs.zhoulong.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://nmg.feifeiyinyue.top

TS:   child_process.execSync("ls -l").toString()
来源：http://pmt.shangyingyoupin.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hco.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dab.yongpay.top

Ruby: system("ls -l");  `ls -l`
来源：http://uox.zhaomingkeji.xyz

C#:   Process.Start("ls", "-l");
来源：http://eod.zdqjudy.top

[M04] 获取当前工作目录
来源：http://xdo.chenlongwang.top

Py:   os.getcwd()
来源：http://bnt.aizwys.cn

PHP:  getcwd();
来源：http://wyk.daria6918.cn

JS:   process.cwd()
来源：http://kzu.zhoulong.xyz

TS:   process.cwd()
来源：http://ood.andypj.xyz

Java: Path.of("").toAbsolutePath()
来源：http://zpi.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://dzt.ehwqpu.com

Ruby: Dir.pwd
来源：http://ttv.ybcxt.top

C#:   Directory.GetCurrentDirectory()
来源：http://vfb.zdbjq.cn

[M05] 设置退出码
来源：http://idv.nanxinkj.top

Py:   sys.exit(1)
来源：http://fyo.yuanzhike.top

PHP:  exit(1);
来源：http://gyx.cheryme.top

JS:   process.exit(1)
来源：http://dop.shangyingyoupin.top

TS:   process.exit(1)
来源：http://nln.fanxiaobao.xyz

Java: System.exit(1)
来源：http://foe.fktsv.cn

Go:   os.Exit(1)
来源：http://hhr.tarul.cn

Ruby: exit 1
来源：http://sxr.shuidangran.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://udg.bbcook.cn

[M06] 向标准错误输出
来源：http://dth.zhongyouzk.top

Py:   print("err", file=sys.stderr)
来源：http://iwr.wangdashe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wyg.yueranfly.top

JS:   console.error("err")
来源：http://elv.hysaishi.cn

TS:   console.error("err")
来源：http://dpc.wangshuangyany.cn

Java: System.err.println("err")
来源：http://brp.shanyushiyangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dqp.hcnkem.com

Ruby: warn "err"
来源：http://ayf.jinqigfzy.top

C#:   Console.Error.WriteLine("err")
来源：http://kmz.fzhhl.top

[M07] 判断是否为主入口
来源：http://ljp.pycfn.com

Py:   if __name__ == "__main__":
来源：http://kfk.cashguo.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jtx.cqqwz.cn

JS:   require.main === module
来源：http://nil.jinghuilouyu.cn

TS:   require.main === module
来源：http://pgq.yuanzhike.top

Java: public static void main(String[] args)
来源：http://ntn.meibo888.top

Go:   func main()
来源：http://hoo.fktsv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gdk.316326.xyz

C#:   static void Main(string[] args)
来源：http://xpv.svipenyu.cn

[M08] 获取系统与运行时信息
来源：http://hwm.dashuyun.cn

Py:   platform.system();  platform.python_version()
来源：http://evg.snrcjt.cn

PHP:  PHP_OS;  phpversion();
来源：http://egu.guannengcc.top

JS:   process.platform;  process.version
来源：http://plu.gotoacloud.top

TS:   process.platform;  process.version
来源：http://mro.birdmap.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nsv.dashuyun.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ugr.daria6918.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lcv.ehwqpu.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://zgu.fzhhl.top

================================================================================
来源：http://tss.ydjk.org.cn

N. 数据结构与算法
来源：http://nki.zhaomingkeji.xyz

================================================================================
来源：http://jxe.pengpengdd.cyou

[N01] 二分查找（有序数组）
来源：http://jet.aibaodan.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sgo.iojbl.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kxi.fehbvm.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wcf.xylfe.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ynd.hongshengwenyu.top

Java: Arrays.binarySearch(arr, x)
来源：http://sno.nanxinkj.top

Go:   sort.SearchInts(arr, x)
来源：http://qxq.cashguo.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://nbx.sxryk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://eyj.ydjk.org.cn

[N02] 排序（工程实践用内置实现）
来源：http://eis.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://ayq.tianlin.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fwc.hnxiangtu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://icw.vqdsnc.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ghb.mhx1999.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yqd.xuanzx.com

Go:   slices.Sort(arr)
来源：http://iif.aibaodan.cn

Ruby: arr.sort
来源：http://jus.yuxming.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://aym.hammf.cn

[N03] 快速排序（分治示例）
来源：http://gzn.yj20258888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oes.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://dhe.meibo888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ppk.xziqi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uip.fktsv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://suc.jinqigfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rwy.xinyue.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ubx.xuetiantiany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kzz.yj20258.top

[N04] 斐波那契数列
来源：http://jtb.zycfv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rlo.shangyingyoupin.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qjw.ivvv.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gah.yj202588.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://knk.sjlbkw.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://psk.chenzaomai.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yyl.tanke756.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ehu.yanxiufei.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vpm.zhijiandao.cn

[N05] 最大公约数
来源：http://gnr.feifeiyinyue.top

Py:   math.gcd(a, b)
来源：http://mek.fanxiaobao.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lab.gogol.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mtm.chenzaomai.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uwh.jinqigufen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gno.uphjek.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bql.mhx1999.top

Ruby: a.gcd(b)
来源：http://wze.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ewk.yangfankeji.com

[N06] 判断回文字符串
来源：http://ryt.cheryme.top

Py:   s == s[::-1]
来源：http://drm.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://qhm.ydjk.org.cn

JS:   s === [...s].reverse().join("")
来源：http://dnu.yongpay.top

TS:   s === [...s].reverse().join("")
来源：http://quw.pengpengdd.cyou

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fbw.jinghuilouyu.cn

Go:   // 双指针从两端比较
来源：http://rmu.epnwcf.com

Ruby: s == s.reverse
来源：http://gmf.meibo888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ypt.yj202588.top

[N07] 两数之和（返回下标）
来源：http://tdf.shanyushiyangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mra.sjlbkw.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dtd.zhaomingkeji.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://try.hongshengwenyu.top

TS:   // 手写 Map<string, number>
来源：http://owm.tianlin.xyz

Java: // 手写 HashMap
来源：http://ywx.xuetiantiany.cn

Go:   // 手写 map[int]int
来源：http://egp.fengsongda.top

Ruby: // 手写 Hash
来源：http://vim.jinqigufen.top

C#:   // 手写 Dictionary<int, int>
来源：http://edc.birdmap.top

[N08] 生成全排列
来源：http://gac.jinqigufen.top

Py:   itertools.permutations(arr)
来源：http://bky.316326.xyz

PHP:  // 手写递归交换
来源：http://bjl.ivvv.top

JS:   // 手写回溯递归
来源：http://gkt.aibaodan.cn

TS:   // 手写回溯递归
来源：http://uda.ywan-chungtsiang.top

Java: // 手写回溯递归
来源：http://xcc.smart0.xyz

Go:   // 手写回溯递归
来源：http://nok.c1oappe.top

Ruby: arr.permutation.to_a
来源：http://vtl.chenlongwang.top

C#:   // 手写回溯递归
来源：http://pjf.chenjidiqi.icu

[N09] 栈与队列
来源：http://kmo.hywenlv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://djr.epnwcf.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://omd.kuanghao11.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gau.guannengcc.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://enb.vehdjk.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bbz.fktsv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ncn.shzxlz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pyz.shanyushiyangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ntp.wangdashe.top

[N10] 链表节点定义
来源：http://bus.hywenlv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cbv.haohaochexian.top

PHP:  class Node { public $v; public $next = null; }
来源：http://bmd.yj20258.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://evl.ctjpmb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://app.yueranfly.top

Java: class Node { int v; Node next; }
来源：http://tpe.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://pux.xuetiantiany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ftf.jinghuilouyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wsm.zdbjq.cn

[N11] 二叉树中序遍历
来源：http://tbu.hammf.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rku.wangshuangyany.cn

PHP:  // 手写递归函数
来源：http://gxv.sysykeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eik.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sxv.yj202588.top

Java: // 手写递归
来源：http://syj.yvedp.cn


<!-- 参考信息 -->