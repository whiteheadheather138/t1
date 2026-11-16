代发 wailian999

[K02] JSON 字符串转对象
来源：http://vpq.xylfe.cn

Py:   json.loads(s)
来源：http://ocp.nanxuanxn.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vda.zycfv.cn

JS:   JSON.parse(s)
来源：http://wzo.vqdsnc.cn

TS:   JSON.parse(s)
来源：http://hnc.yonumen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vtt.jqgufenzy.top

Go:   json.Unmarshal(data, &v)
来源：http://zwm.yfazqb.com

Ruby: JSON.parse(s)
来源：http://wle.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://byl.yj20258.top

[K03] JSON 美化输出（带缩进）
来源：http://mjm.guowangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ovw.guowangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zbg.guowangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cek.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://dxz.ydjk.org.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://egx.yvedp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://liu.yj20258888.top

Ruby: JSON.pretty_generate(obj)
来源：http://znr.yongpay.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qnr.fehbvm.com

[K04] 读取 JSON 文件
来源：http://ezh.xingfuxueyuan.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zhi.nanxinkj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zst.chenjidiqi.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zpw.yangfankeji.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zoh.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nmo.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jja.guowangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mtb.tanke756.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xmp.fengsongda.top

[K05] 深拷贝对象
来源：http://ocv.yuxming.cn

Py:   copy.deepcopy(obj)
来源：http://xfg.haohaochexian.top

PHP:  unserialize(serialize($obj));
来源：http://gdy.yongpay.top

JS:   structuredClone(obj)
来源：http://nvk.jqgfzy.top

TS:   structuredClone(obj)
来源：http://hsy.gzhubu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ahg.xuanzx.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mga.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kvd.quarkkingdee.top

C#:   // 序列化往返，或自定义 Clone
来源：http://akd.nanxuanxn.top

[K06] 解析 URL 查询串
来源：http://dzh.smart0.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ier.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kdl.zdbjq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qpu.ydzc1.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zgs.yj20258.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qtx.ppjwa.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zik.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fon.shuidangran.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fki.daria6918.cn

[K07] 进制转换
来源：http://xdo.wangshuangyany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zxy.bbcook.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://omy.haohaochexian.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ryz.yvedp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fed.ctjpmb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sjf.xylfe.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wdh.bbcook.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yeg.wangdashe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aas.guowangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://xue.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://jox.hnxiangtu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gbi.mhx1999.top

JS:   v8.serialize(obj)        // Node
来源：http://wep.nwbrower.top

TS:   v8.serialize(obj)        // Node
来源：http://plp.aibaodan.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ryo.snrcjt.cn

Go:   encoding/gob
来源：http://jif.xingfuxueyuan.xyz

Ruby: Marshal.dump(obj)
来源：http://uxb.bjfxy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vqh.yj20258888.top

================================================================================
来源：http://zsg.ydjk.org.cn

L. 网络请求
来源：http://gta.shanyushiyangkeji.top

================================================================================
来源：http://ytm.daria6918.cn

[L01] 发送 GET 请求
来源：http://rpk.wangshuangyany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jlk.gogol.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dsk.shanyushiyangkeji.top

JS:   await fetch(url)
来源：http://zld.yj202588.top

TS:   await fetch(url)
来源：http://cot.zycfv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cqd.xuetiantiany.cn

Go:   resp, err := http.Get(url)
来源：http://fav.ehwqpu.com

Ruby: Net::HTTP.get(URI(url))
来源：http://rtk.tarul.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yoj.gotoacloud.top

[L02] 发送 POST JSON
来源：http://bii.hnqzz.top

Py:   requests.post(url, json={"a": 1})
来源：http://cop.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://anm.smart0.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oze.hysaishi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wss.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nvr.mhx1999.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://chn.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tbo.52xcode.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://boy.epnwcf.com

[L03] 设置自定义请求头
来源：http://evb.epnwcf.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rex.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eoi.chenzaomai.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://txd.9152youxi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fns.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jlf.cucudq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ham.tarul.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hhk.yongpay.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://svo.sxryk.cn

[L04] 设置超时
来源：http://ymj.tianlin.xyz

Py:   requests.get(url, timeout=5)
来源：http://rnq.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ddi.jinghuilouyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://onm.quarkkingdee.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qyq.dashuyun.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fby.xziqi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ywf.fktsv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dhi.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://boe.meibo888.top

[L05] 上传文件（multipart）
来源：http://jvv.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ffh.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lba.fzhhl.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rmr.xuetiantiany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gps.zhongyouzk.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pnm.sxryk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hor.yangfankeji.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://esd.zhixingplan.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bef.jinghuilouyu.cn

[L06] 解析响应为 JSON
来源：http://zsx.yfazqb.com

Py:   resp.json()
来源：http://ibj.xziqi.cn

PHP:  json_decode($body, true);
来源：http://eyh.xinyue.icu

JS:   await resp.json()
来源：http://kwe.ybcxt.top

TS:   await resp.json()
来源：http://ygp.gaohongyu789.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rux.iojbl.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uzp.jyoumei.cn

Ruby: JSON.parse(resp.body)
来源：http://rhs.yangfankeji.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eqp.xuetiantiany.cn

[L07] 处理 HTTP 状态码
来源：http://sew.aibaodan.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ttl.jinqigufen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fgq.tianlin.xyz

JS:   resp.ok;  resp.status
来源：http://xcg.kuanghao11.cn

TS:   resp.ok;  resp.status
来源：http://wal.chenjidiqi.icu

Java: resp.statusCode()
来源：http://wzw.hammf.cn

Go:   resp.StatusCode
来源：http://gth.nanxuanxn.top

Ruby: resp.code.to_i
来源：http://wcd.xinyue.icu

C#:   (int)resp.StatusCode
来源：http://aeo.nanxuanxn.top

[L08] 并发请求多个地址
来源：http://qyj.jlsjyb.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://unx.jqgufenzy.top

PHP:  curl_multi_init() 系列
来源：http://eul.quarkkingdee.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bzg.yongpay.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fjr.tianlin.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qdi.hywenlv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qnn.xingfuxueyuan.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mng.birdmap.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rnw.ctjpmb.com

================================================================================
来源：http://nky.yangfankeji.com

M. 命令行 / 进程 / 环境
来源：http://smy.andypj.xyz

================================================================================
来源：http://eox.jiagoushi.top

[M01] 读取命令行参数
来源：http://bgy.hywenlv.cn

Py:   sys.argv[1:]
来源：http://wjd.ehwqpu.com

PHP:  $argv;  $argc;
来源：http://tdu.aibaodan.cn

JS:   process.argv.slice(2)
来源：http://gme.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://pnt.xuetiantiany.cn

Java: args 数组（main 方法参数）
来源：http://nbg.yvedp.cn

Go:   os.Args[1:]
来源：http://idj.gzhubu.top

Ruby: ARGV
来源：http://las.pycfn.com

C#:   args 数组（Main 方法参数）
来源：http://bye.chenzaomai.com

[M02] 读取环境变量
来源：http://dev.dianchejie.cn

Py:   os.environ.get("HOME")
来源：http://vwi.fktsv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rjq.zhoulong.xyz

JS:   process.env.HOME
来源：http://zxy.fengsongda.top

TS:   process.env.HOME
来源：http://raw.shzxlz.cn

Java: System.getenv("HOME")
来源：http://tau.pengpengdd.cyou

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xbh.ybcxt.top

Ruby: ENV["HOME"]
来源：http://azx.52xcode.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pjk.yanxiufei.cn

[M03] 执行外部命令
来源：http://fpu.haohaochexian.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uqg.chenjidiqi.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://buq.9152youxi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gvm.chenlongwang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wng.shanyushiyangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uyd.hywenlv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://imm.xziqi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://knk.zhoulong.xyz

C#:   Process.Start("ls", "-l");
来源：http://sua.bbcook.cn

[M04] 获取当前工作目录
来源：http://jtr.jiagoushi.top

Py:   os.getcwd()
来源：http://crd.yongpay.top

PHP:  getcwd();
来源：http://xvb.yfazqb.com

JS:   process.cwd()
来源：http://sms.mhx1999.top

TS:   process.cwd()
来源：http://hyl.yvedp.cn

Java: Path.of("").toAbsolutePath()
来源：http://wte.chenlongwang.top

Go:   os.Getwd()
来源：http://vrl.sufxvd.cn

Ruby: Dir.pwd
来源：http://wfb.nwbrower.top

C#:   Directory.GetCurrentDirectory()
来源：http://ayq.ctjpmb.com

[M05] 设置退出码
来源：http://lkq.jinyuanbaomall.cn

Py:   sys.exit(1)
来源：http://xvg.birdmap.top

PHP:  exit(1);
来源：http://qtu.andypj.xyz

JS:   process.exit(1)
来源：http://bng.jqgufenzy.top

TS:   process.exit(1)
来源：http://qey.sjlbkw.cn

Java: System.exit(1)
来源：http://xoz.smart0.xyz

Go:   os.Exit(1)
来源：http://zrp.fengsongda.top

Ruby: exit 1
来源：http://ptt.iojbl.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yne.xuanzx.com

[M06] 向标准错误输出
来源：http://oke.dashuyun.cn

Py:   print("err", file=sys.stderr)
来源：http://bbo.hysaishi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dbl.cqqwz.cn

JS:   console.error("err")
来源：http://wap.xinyue.icu

TS:   console.error("err")
来源：http://rvk.quarkkingdee.top

Java: System.err.println("err")
来源：http://lir.birdmap.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://plr.zhengqikj.top

Ruby: warn "err"
来源：http://pyi.fengsongda.top

C#:   Console.Error.WriteLine("err")
来源：http://qns.hammf.cn

[M07] 判断是否为主入口
来源：http://xnq.shuidangran.top

Py:   if __name__ == "__main__":
来源：http://haa.ybcxt.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://clk.pycfn.com

JS:   require.main === module
来源：http://swe.yongpay.top

TS:   require.main === module
来源：http://nhe.uphjek.com

Java: public static void main(String[] args)
来源：http://qhv.gotoacloud.top

Go:   func main()
来源：http://ugu.c1oappe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://srj.tarul.cn

C#:   static void Main(string[] args)
来源：http://cbw.cucudq.cn

[M08] 获取系统与运行时信息
来源：http://ney.yj202588.top

Py:   platform.system();  platform.python_version()
来源：http://jgt.c1oappe.top

PHP:  PHP_OS;  phpversion();
来源：http://cjl.zhixingplan.top

JS:   process.platform;  process.version
来源：http://bcp.bjfxy.top

TS:   process.platform;  process.version
来源：http://wtw.zdqjudy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wep.pengpengdd.cyou

Go:   runtime.GOOS;  runtime.Version()
来源：http://kxe.birdmap.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gon.ppjwa.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qvo.tianlin.xyz

================================================================================
来源：http://bvi.jyoumei.cn

N. 数据结构与算法
来源：http://oyb.wangdashe.top

================================================================================
来源：http://xxk.xinyue.icu

[N01] 二分查找（有序数组）
来源：http://zhc.shzxlz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://joi.fzhhl.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gtm.nanxinkj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eba.shanyushiyangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dfc.hfpthk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ekt.vehdjk.com

Go:   sort.SearchInts(arr, x)
来源：http://ubs.sjlbkw.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jib.ehwqpu.com

C#:   Array.BinarySearch(arr, x)
来源：http://soy.xylfe.cn

[N02] 排序（工程实践用内置实现）
来源：http://sgt.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://iqp.yueranfly.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zli.gzhubu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mth.daria6918.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lxf.zdbjq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rwq.yonumen.top

Go:   slices.Sort(arr)
来源：http://lwq.cashguo.top

Ruby: arr.sort
来源：http://puy.bbcook.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lqh.dianchejie.cn

[N03] 快速排序（分治示例）
来源：http://uqy.jlsjyb.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://csk.zhixingplan.top

PHP:  // 递归实现，或用 usort
来源：http://dnn.jinyuanbaomall.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rue.epnwcf.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nui.ivvv.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lkc.xylfe.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zzx.zhixingplan.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qlm.andypj.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://gna.tian-w.cn

[N04] 斐波那契数列
来源：http://qox.xingfuxueyuan.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zfv.52xcode.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ptv.nanxinkj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://egh.xziqi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hhp.jinyuanbaomall.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://btf.xuetiantiany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tug.hnxiangtu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mbk.nanxinkj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bbv.guowangkeji.top

[N05] 最大公约数
来源：http://oyy.ctjpmb.com

Py:   math.gcd(a, b)
来源：http://oti.uphjek.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://azq.gotoacloud.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lxz.kuanghao11.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qcd.yuanzhike.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jzy.sxryk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nzj.yongpay.top

Ruby: a.gcd(b)
来源：http://aic.jlsjyb.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://thd.cashguo.top

[N06] 判断回文字符串
来源：http://khz.ydjk.org.cn

Py:   s == s[::-1]
来源：http://knx.andypj.xyz

PHP:  $s === strrev($s);
来源：http://fed.52xcode.cn

JS:   s === [...s].reverse().join("")
来源：http://ytv.ppjwa.cn

TS:   s === [...s].reverse().join("")
来源：http://vme.sysykeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ccb.chenzaomai.com

Go:   // 双指针从两端比较
来源：http://imx.hywenlv.cn

Ruby: s == s.reverse
来源：http://mqc.yuxming.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xaf.iojbl.cn

[N07] 两数之和（返回下标）
来源：http://gdl.hesvh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yba.bbcook.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tvt.xylfe.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tyn.yj20258888.top

TS:   // 手写 Map<string, number>
来源：http://cev.zhijiandao.cn

Java: // 手写 HashMap
来源：http://jzm.hysaishi.cn

Go:   // 手写 map[int]int
来源：http://hem.9152youxi.cn

Ruby: // 手写 Hash
来源：http://cir.ppjwa.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jro.xingfuxueyuan.xyz

[N08] 生成全排列
来源：http://nzd.sysykeji.top

Py:   itertools.permutations(arr)
来源：http://veg.52xcode.cn

PHP:  // 手写递归交换
来源：http://eea.uphjek.com

JS:   // 手写回溯递归
来源：http://jee.aizwys.cn

TS:   // 手写回溯递归
来源：http://tyy.ywan-chungtsiang.top

Java: // 手写回溯递归
来源：http://zna.zhongyouzk.top

Go:   // 手写回溯递归
来源：http://vro.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://xsm.aizwys.cn

C#:   // 手写回溯递归
来源：http://kaj.nwbrower.top

[N09] 栈与队列
来源：http://nds.nanxinkj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://znb.redwolf501.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tzf.xziqi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lrx.andypj.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sql.vehdjk.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pdh.ivvv.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oxg.fzhhl.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tiz.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jrg.shanyushiyangkeji.top

[N10] 链表节点定义
来源：http://wfv.nanxuanxn.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://raz.yuxming.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://slg.316326.xyz


<!-- 参考信息 -->