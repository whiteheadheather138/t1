代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://lzc.tianlin.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://pgz.yueranfly.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mxj.sweek.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vpz.zycfv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pto.316326.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iyw.bbcook.cn

[K04] 读取 JSON 文件
来源：http://tfg.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pyn.uphjek.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xjw.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pxu.xuanzx.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jxx.vehdjk.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hmd.jianghu66.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mfh.guannengcc.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sps.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cfc.xylfe.cn

[K05] 深拷贝对象
来源：http://gdq.jinqigufen.top

Py:   copy.deepcopy(obj)
来源：http://pte.tanke756.top

PHP:  unserialize(serialize($obj));
来源：http://tpj.9152youxi.cn

JS:   structuredClone(obj)
来源：http://jqx.hcnkem.com

TS:   structuredClone(obj)
来源：http://pkw.yuanzhike.top

Java: // 手写拷贝构造，或序列化往返
来源：http://kwv.feifeiyinyue.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qak.hysaishi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pks.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fvx.haohaochexian.top

[K06] 解析 URL 查询串
来源：http://mik.quarkkingdee.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hjw.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://org.chenlongwang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bmu.svipenyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jiu.gzhubu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pqj.xuanzx.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://sfe.sysykeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fjp.sjlbkw.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zrn.gaohongyu789.top

[K07] 进制转换
来源：http://tis.nwbrower.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wrq.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vos.gotoacloud.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pao.yueranfly.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vjd.guannengcc.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vwj.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jhg.yj20258.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rec.ehwqpu.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uvk.ywan-chungtsiang.top

[K08] 二进制序列化（非 JSON）
来源：http://ixp.guowangkeji.top

Py:   pickle.dumps(obj)
来源：http://ezm.yvedp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://icl.xylfe.cn

JS:   v8.serialize(obj)        // Node
来源：http://fcf.gogol.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://ldz.snrcjt.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hxd.meibo888.top

Go:   encoding/gob
来源：http://upi.quarkkingdee.top

Ruby: Marshal.dump(obj)
来源：http://fif.uphjek.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nin.hesvh.cn

================================================================================
来源：http://tmw.yueranfly.top

L. 网络请求
来源：http://vnw.zhongyouzk.top

================================================================================
来源：http://igt.zycfv.cn

[L01] 发送 GET 请求
来源：http://mmo.xylfe.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qnr.quarkkingdee.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gmc.hongshengwenyu.top

JS:   await fetch(url)
来源：http://qau.pycfn.com

TS:   await fetch(url)
来源：http://rch.yonumen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pdz.jqgufenzy.top

Go:   resp, err := http.Get(url)
来源：http://krt.redwolf501.top

Ruby: Net::HTTP.get(URI(url))
来源：http://uhh.yanxiufei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ivj.yfazqb.com

[L02] 发送 POST JSON
来源：http://rib.hammf.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vjj.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://krh.cdnleiting.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xlx.aizwys.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hvb.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ndm.svipenyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tqs.tian-w.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zps.hcnkem.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bwx.c1oappe.top

[L03] 设置自定义请求头
来源：http://efn.daria6918.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ayu.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://aue.fzhhl.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kbk.gotoacloud.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xju.havefunace.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xbi.hnxiangtu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zlp.hnxiangtu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mic.chenlongwang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://esd.jqgufenzy.top

[L04] 设置超时
来源：http://arq.xuetiantiany.cn

Py:   requests.get(url, timeout=5)
来源：http://eix.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gya.jlsjyb.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qqv.pycfn.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bvr.tianlin.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://inb.fanxiaobao.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ewa.mhx1999.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uvx.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://beq.jlsjyb.cn

[L05] 上传文件（multipart）
来源：http://hxu.zdbjq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fjr.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xsk.hammf.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xbp.dashuyun.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://awl.jlsjyb.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cte.zhengqikj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tim.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ofx.yvedp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://igu.cqqwz.cn

[L06] 解析响应为 JSON
来源：http://arz.cucudq.cn

Py:   resp.json()
来源：http://lvm.fengsongda.top

PHP:  json_decode($body, true);
来源：http://fxp.yuanzhike.top

JS:   await resp.json()
来源：http://zeo.epnwcf.com

TS:   await resp.json()
来源：http://tpn.hysaishi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oka.ybcxt.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iua.hongshengwenyu.top

Ruby: JSON.parse(resp.body)
来源：http://pha.yj202588.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://giv.havefunace.top

[L07] 处理 HTTP 状态码
来源：http://ale.cheryme.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://axf.xuetiantiany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vde.jinqigfzy.top

JS:   resp.ok;  resp.status
来源：http://ymm.smart0.xyz

TS:   resp.ok;  resp.status
来源：http://zwm.smart0.xyz

Java: resp.statusCode()
来源：http://slh.fzhhl.top

Go:   resp.StatusCode
来源：http://vlr.zhoulong.xyz

Ruby: resp.code.to_i
来源：http://cwd.cqqwz.cn

C#:   (int)resp.StatusCode
来源：http://kls.cashguo.top

[L08] 并发请求多个地址
来源：http://bmk.jinghuilouyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gdc.jinqigfzy.top

PHP:  curl_multi_init() 系列
来源：http://fvd.ppjwa.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ppg.svipenyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yhl.tianlin.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qso.zycfv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eju.wangdashe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rfv.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://prc.aibaodan.cn

================================================================================
来源：http://jhf.chenlongwang.top

M. 命令行 / 进程 / 环境
来源：http://yov.hywenlv.cn

================================================================================
来源：http://enj.shangyingyoupin.top

[M01] 读取命令行参数
来源：http://wap.yj20258888.top

Py:   sys.argv[1:]
来源：http://yhu.ivvv.top

PHP:  $argv;  $argc;
来源：http://lrd.cashguo.top

JS:   process.argv.slice(2)
来源：http://xns.tarul.cn

TS:   process.argv.slice(2)
来源：http://znb.chenlongwang.top

Java: args 数组（main 方法参数）
来源：http://xqj.xziqi.cn

Go:   os.Args[1:]
来源：http://vme.9152youxi.cn

Ruby: ARGV
来源：http://wew.shanyushiyangkeji.top

C#:   args 数组（Main 方法参数）
来源：http://svl.cheryme.top

[M02] 读取环境变量
来源：http://ovd.yj202588.top

Py:   os.environ.get("HOME")
来源：http://nbo.zdbjq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oio.c1oappe.top

JS:   process.env.HOME
来源：http://vwn.hesvh.cn

TS:   process.env.HOME
来源：http://xfg.zhixingplan.top

Java: System.getenv("HOME")
来源：http://eqp.zhijiandao.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aah.hfpthk.cn

Ruby: ENV["HOME"]
来源：http://tzv.shuidangran.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://edu.chenlongwang.top

[M03] 执行外部命令
来源：http://aeu.sufxvd.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zhd.hfpthk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ltl.zhongyouzk.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rug.chenlongwang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hnk.haohaochexian.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uev.nanxuanxn.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qng.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ufn.c1oappe.top

C#:   Process.Start("ls", "-l");
来源：http://fol.jinqigfzy.top

[M04] 获取当前工作目录
来源：http://hhf.haohaochexian.top

Py:   os.getcwd()
来源：http://yvb.ivvv.top

PHP:  getcwd();
来源：http://rdi.316326.xyz

JS:   process.cwd()
来源：http://bbj.mhx1999.top

TS:   process.cwd()
来源：http://wqh.meibo888.top

Java: Path.of("").toAbsolutePath()
来源：http://gef.zhengqikj.top

Go:   os.Getwd()
来源：http://ksq.gaohongyu789.top

Ruby: Dir.pwd
来源：http://fuq.andypj.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://kbq.hywenlv.cn

[M05] 设置退出码
来源：http://top.yanxiufei.cn

Py:   sys.exit(1)
来源：http://mqi.nanxuanxn.top

PHP:  exit(1);
来源：http://xxb.sxryk.cn

JS:   process.exit(1)
来源：http://xty.gaohongyu789.top

TS:   process.exit(1)
来源：http://xvh.tian-w.cn

Java: System.exit(1)
来源：http://gbd.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://yit.sweek.top

Ruby: exit 1
来源：http://mro.xuetiantiany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kar.xuetiantiany.cn

[M06] 向标准错误输出
来源：http://vii.yanxiufei.cn

Py:   print("err", file=sys.stderr)
来源：http://ahf.hnqzz.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rav.ydjk.org.cn

JS:   console.error("err")
来源：http://evg.havefunace.top

TS:   console.error("err")
来源：http://lqk.cdnleiting.top

Java: System.err.println("err")
来源：http://uwy.aizwys.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hti.ybcxt.top

Ruby: warn "err"
来源：http://chm.zdqjudy.top

C#:   Console.Error.WriteLine("err")
来源：http://eqe.mhx1999.top

[M07] 判断是否为主入口
来源：http://pvt.zhaomingkeji.xyz

Py:   if __name__ == "__main__":
来源：http://qsl.ctjpmb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ufn.shanyushiyangkeji.top

JS:   require.main === module
来源：http://cgn.c1oappe.top

TS:   require.main === module
来源：http://gbw.yongpay.top

Java: public static void main(String[] args)
来源：http://dgm.fzhhl.top

Go:   func main()
来源：http://vzv.xuanzx.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://svw.ybcxt.top

C#:   static void Main(string[] args)
来源：http://ccm.chenzaomai.com

[M08] 获取系统与运行时信息
来源：http://hbh.zhiwuduotai.top

Py:   platform.system();  platform.python_version()
来源：http://juf.ywan-chungtsiang.top

PHP:  PHP_OS;  phpversion();
来源：http://faq.gzhubu.top

JS:   process.platform;  process.version
来源：http://dpx.ppjwa.cn

TS:   process.platform;  process.version
来源：http://dlf.0kj1m.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dog.daria6918.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cai.cheryme.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fgz.svipenyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kuf.xinyue.icu

================================================================================
来源：http://elg.sufxvd.cn

N. 数据结构与算法
来源：http://gyk.yj20258888.top

================================================================================
来源：http://qpp.hnxiangtu.top

[N01] 二分查找（有序数组）
来源：http://xct.cqqwz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://etr.ybcxt.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mil.shzxlz.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zuc.xuetiantiany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tsd.fanxiaobao.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://wqe.uphjek.com

Go:   sort.SearchInts(arr, x)
来源：http://xqp.chenjidiqi.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://byt.yvedp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cdb.cqqwz.cn

[N02] 排序（工程实践用内置实现）
来源：http://eeh.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://wxr.xuetiantiany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cfy.meibo888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://wny.chenjidiqi.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://ldh.chenzaomai.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xsm.ybcxt.top

Go:   slices.Sort(arr)
来源：http://lnj.jinqigufen.top

Ruby: arr.sort
来源：http://mjb.cucudq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xis.zhongyouzk.top

[N03] 快速排序（分治示例）
来源：http://mph.aibaodan.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://agl.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://xyv.pycfn.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dbo.shanyushiyangtech.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ehu.daria6918.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://btl.c1oappe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rhy.gotoacloud.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rfg.xinyue.icu

C#:   // 手写递归，或 Array.Sort
来源：http://dtb.andypj.xyz

[N04] 斐波那契数列
来源：http://dfe.andypj.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vng.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vly.9152youxi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cnc.vqdsnc.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vzx.hongshengwenyu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qvw.yj20258.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://acg.dianchejie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rfm.tarul.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ukd.hammf.cn

[N05] 最大公约数
来源：http://dqe.aizwys.cn

Py:   math.gcd(a, b)
来源：http://wgi.zhengqikj.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nir.cheryme.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ilt.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zds.hesvh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ntu.fengsongda.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ehv.fzhhl.top

Ruby: a.gcd(b)
来源：http://cph.zhongyouzk.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rze.hywenlv.cn

[N06] 判断回文字符串
来源：http://fbh.c1oappe.top

Py:   s == s[::-1]
来源：http://jgn.fzhhl.top

PHP:  $s === strrev($s);
来源：http://dvk.zhengqikj.top

JS:   s === [...s].reverse().join("")
来源：http://ytr.jinghuilouyu.cn

TS:   s === [...s].reverse().join("")
来源：http://nim.sjlbkw.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wrx.9152youxi.cn

Go:   // 双指针从两端比较
来源：http://tup.hnxiangtu.top

Ruby: s == s.reverse
来源：http://aef.sufxvd.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rxs.gotoacloud.top

[N07] 两数之和（返回下标）
来源：http://quf.zhiwuduotai.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bph.ctjpmb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gcc.ydjk.org.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sec.yj202588.top

TS:   // 手写 Map<string, number>
来源：http://nyj.shanyushiyangtech.top

Java: // 手写 HashMap
来源：http://lmc.svipenyu.cn

Go:   // 手写 map[int]int
来源：http://gpv.tianlin.xyz

Ruby: // 手写 Hash
来源：http://irv.kuanghao11.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wvk.sysykeji.top

[N08] 生成全排列
来源：http://jcp.nanxinkj.top

Py:   itertools.permutations(arr)
来源：http://erq.nanxuanxn.top

PHP:  // 手写递归交换
来源：http://hew.yj20258888.top

JS:   // 手写回溯递归
来源：http://gfx.zhiwuduotai.top

TS:   // 手写回溯递归
来源：http://emx.jinghuilouyu.cn

Java: // 手写回溯递归
来源：http://emv.guowangkeji.top

Go:   // 手写回溯递归
来源：http://ray.aibaodan.cn

Ruby: arr.permutation.to_a
来源：http://ljm.316326.xyz

C#:   // 手写回溯递归
来源：http://drp.vehdjk.com

[N09] 栈与队列
来源：http://kao.zhoulong.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ysn.chenzaomai.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hmr.chenzaomai.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mgx.aibaodan.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ufz.aizwys.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kbx.9152youxi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wuh.xuanzx.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://suv.nanxinkj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pvq.sjlbkw.cn

[N10] 链表节点定义
来源：http://piz.c1oappe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jvi.gotoacloud.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vmj.yvedp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://znc.guowangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://soc.xuetiantiany.cn

Java: class Node { int v; Node next; }
来源：http://lrp.hywenlv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ngi.uphjek.com

Ruby: Node = Struct.new(:v, :next)
来源：http://iot.jiagoushi.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ikj.tianlin.xyz

[N11] 二叉树中序遍历
来源：http://oue.zycfv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hmx.9152youxi.cn

PHP:  // 手写递归函数
来源：http://piw.fktsv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zxj.jlsjyb.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kll.9152youxi.cn

Java: // 手写递归
来源：http://qgf.svipenyu.cn


<!-- 参考信息 -->