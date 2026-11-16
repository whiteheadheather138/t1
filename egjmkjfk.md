代发 wailian999

[K02] JSON 字符串转对象
来源：http://etw.mhx1999.top

Py:   json.loads(s)
来源：http://tcj.tian-w.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ibh.mhx1999.top

JS:   JSON.parse(s)
来源：http://vdh.dashuyun.cn

TS:   JSON.parse(s)
来源：http://ssm.bjfxy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wsh.316326.xyz

Go:   json.Unmarshal(data, &v)
来源：http://pei.hywenlv.cn

Ruby: JSON.parse(s)
来源：http://yrj.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uzi.bbcook.cn

[K03] JSON 美化输出（带缩进）
来源：http://hme.ctjpmb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://okz.52xcode.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cho.nanxinkj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://uvs.xuetiantiany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://boo.zdqjudy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cgt.yj202588.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zth.kuanghao11.cn

Ruby: JSON.pretty_generate(obj)
来源：http://scx.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wep.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://ueo.guannengcc.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qcm.jlsjyb.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fhm.ppjwa.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://inm.zhoulong.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uqu.feifeiyinyue.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aqb.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cbm.smart0.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://xgn.havefunace.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eve.yj20258888.top

[K05] 深拷贝对象
来源：http://ptl.52xcode.cn

Py:   copy.deepcopy(obj)
来源：http://ohi.wangdashe.top

PHP:  unserialize(serialize($obj));
来源：http://clq.jinghuilouyu.cn

JS:   structuredClone(obj)
来源：http://klm.shangyingyoupin.top

TS:   structuredClone(obj)
来源：http://loq.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ypy.hysaishi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rgk.jinqigfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mxj.tarul.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kxh.zhixingplan.top

[K06] 解析 URL 查询串
来源：http://yfo.chenjidiqi.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dgq.yfazqb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dgg.ehwqpu.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fwj.fzhhl.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cpq.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bfx.gotoacloud.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xyc.gzhubu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://epw.ivvv.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mzt.chenlongwang.top

[K07] 进制转换
来源：http://zmr.yuanzhike.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vau.tanke756.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gvl.nwbrower.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gqy.zdqjudy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cpw.fengsongda.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ahk.jinghuilouyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xus.shzxlz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kfc.jqgfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tam.fanxiaobao.xyz

[K08] 二进制序列化（非 JSON）
来源：http://jyh.gzhubu.top

Py:   pickle.dumps(obj)
来源：http://uuv.nwbrower.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mui.guannengcc.top

JS:   v8.serialize(obj)        // Node
来源：http://tgn.shuidangran.top

TS:   v8.serialize(obj)        // Node
来源：http://swy.cdnleiting.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://owm.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://ogb.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://kgf.ctjpmb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zda.zhaomingkeji.xyz

================================================================================
来源：http://hpn.quarkkingdee.top

L. 网络请求
来源：http://rxm.chenlongwang.top

================================================================================
来源：http://qhn.jinyuanbaomall.cn

[L01] 发送 GET 请求
来源：http://dik.nanxuanxn.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lmi.sjlbkw.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gyx.hesvh.cn

JS:   await fetch(url)
来源：http://poy.sysykeji.top

TS:   await fetch(url)
来源：http://tok.shanyushiyangtech.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yro.aibaodan.cn

Go:   resp, err := http.Get(url)
来源：http://vxz.hongshengwenyu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nce.nanxuanxn.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rwf.zhiwuduotai.top

[L02] 发送 POST JSON
来源：http://kvx.cqqwz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mjf.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mzg.52xcode.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oyv.chenzaomai.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tvp.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://har.tarul.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rkx.nanxuanxn.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wjc.yj202588.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ndu.shanyushiyangtech.top

[L03] 设置自定义请求头
来源：http://jwq.ywan-chungtsiang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nee.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jym.guannengcc.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yqq.nanxuanxn.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ryc.pycfn.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cil.sjlbkw.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xaj.wangshuangyany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bot.fehbvm.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://chf.cheryme.top

[L04] 设置超时
来源：http://toj.zycfv.cn

Py:   requests.get(url, timeout=5)
来源：http://ury.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mpj.ydzc1.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kru.zhijiandao.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ouo.guowangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ruy.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://grv.guowangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mdx.nanxinkj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wel.birdmap.top

[L05] 上传文件（multipart）
来源：http://nvh.zhijiandao.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zjp.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fpf.hongshengwenyu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jmn.wangdashe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bdk.52xcode.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pdp.yj20258.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ewq.xinyue.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pot.hesvh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://han.0kj1m.cn

[L06] 解析响应为 JSON
来源：http://xdx.cqqwz.cn

Py:   resp.json()
来源：http://rkr.ybcxt.top

PHP:  json_decode($body, true);
来源：http://ngj.jinyuanbaomall.cn

JS:   await resp.json()
来源：http://ahb.fengsongda.top

TS:   await resp.json()
来源：http://lgd.zhengqikj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bdc.jinqigfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uou.c1oappe.top

Ruby: JSON.parse(resp.body)
来源：http://gpf.c1oappe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mki.hcnkem.com

[L07] 处理 HTTP 状态码
来源：http://orl.52xcode.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jmj.zhijiandao.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://piu.bbcook.cn

JS:   resp.ok;  resp.status
来源：http://ezc.chenzaomai.com

TS:   resp.ok;  resp.status
来源：http://ttt.gzhubu.top

Java: resp.statusCode()
来源：http://mse.xuanzx.com

Go:   resp.StatusCode
来源：http://gxv.dianchejie.cn

Ruby: resp.code.to_i
来源：http://nsb.vqdsnc.cn

C#:   (int)resp.StatusCode
来源：http://ddi.hnxiangtu.top

[L08] 并发请求多个地址
来源：http://wob.ydzc1.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zdf.hnxiangtu.top

PHP:  curl_multi_init() 系列
来源：http://tfd.sufxvd.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pun.sysykeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ltr.cheryme.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sld.daria6918.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qug.xinyue.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://naz.c1oappe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://njs.yonumen.top

================================================================================
来源：http://nme.xinyue.icu

M. 命令行 / 进程 / 环境
来源：http://nry.hnqzz.top

================================================================================
来源：http://mlr.gogol.net.cn

[M01] 读取命令行参数
来源：http://qmp.birdmap.top

Py:   sys.argv[1:]
来源：http://hkx.xuetiantiany.cn

PHP:  $argv;  $argc;
来源：http://oho.fehbvm.com

JS:   process.argv.slice(2)
来源：http://zyq.wangdashe.top

TS:   process.argv.slice(2)
来源：http://xxp.shanyushiyangkeji.top

Java: args 数组（main 方法参数）
来源：http://cwg.redwolf501.top

Go:   os.Args[1:]
来源：http://vsf.sufxvd.cn

Ruby: ARGV
来源：http://zgo.zhixingplan.top

C#:   args 数组（Main 方法参数）
来源：http://ona.mhx1999.top

[M02] 读取环境变量
来源：http://oys.dashuyun.cn

Py:   os.environ.get("HOME")
来源：http://dob.zhixingplan.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xcy.uphjek.com

JS:   process.env.HOME
来源：http://zvv.hcnkem.com

TS:   process.env.HOME
来源：http://blb.zycfv.cn

Java: System.getenv("HOME")
来源：http://hco.xingfuxueyuan.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://brq.pengpengdd.cyou

Ruby: ENV["HOME"]
来源：http://xee.yanxiufei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://txd.cqqwz.cn

[M03] 执行外部命令
来源：http://pjq.redwolf501.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gas.zhixingplan.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nlr.jinqigufen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dzn.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ahd.zhixingplan.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vej.sxryk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uze.gogol.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ovp.zdqjudy.top

C#:   Process.Start("ls", "-l");
来源：http://hvb.vqdsnc.cn

[M04] 获取当前工作目录
来源：http://hpt.tanke756.top

Py:   os.getcwd()
来源：http://toc.chenjidiqi.icu

PHP:  getcwd();
来源：http://wse.yuxming.cn

JS:   process.cwd()
来源：http://gyg.cqqwz.cn

TS:   process.cwd()
来源：http://owt.zhoulong.xyz

Java: Path.of("").toAbsolutePath()
来源：http://wza.yangfankeji.com

Go:   os.Getwd()
来源：http://mjl.hnqzz.top

Ruby: Dir.pwd
来源：http://ggi.shanyushiyangtech.top

C#:   Directory.GetCurrentDirectory()
来源：http://ofa.gogol.net.cn

[M05] 设置退出码
来源：http://fze.havefunace.top

Py:   sys.exit(1)
来源：http://xsp.bjfxy.top

PHP:  exit(1);
来源：http://uex.yanxiufei.cn

JS:   process.exit(1)
来源：http://qie.jlsjyb.cn

TS:   process.exit(1)
来源：http://ijl.guannengcc.top

Java: System.exit(1)
来源：http://jbu.52xcode.cn

Go:   os.Exit(1)
来源：http://ysf.hongshengwenyu.top

Ruby: exit 1
来源：http://xne.c1oappe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bhf.svipenyu.cn

[M06] 向标准错误输出
来源：http://ikh.jyoumei.cn

Py:   print("err", file=sys.stderr)
来源：http://tco.chenlongwang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ayk.hfpthk.cn

JS:   console.error("err")
来源：http://acs.ivvv.top

TS:   console.error("err")
来源：http://ogb.bbcook.cn

Java: System.err.println("err")
来源：http://rmp.ydjk.org.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jwm.wangshuangyany.cn

Ruby: warn "err"
来源：http://brs.52xcode.cn

C#:   Console.Error.WriteLine("err")
来源：http://hpp.316326.xyz

[M07] 判断是否为主入口
来源：http://zep.hnqzz.top

Py:   if __name__ == "__main__":
来源：http://qjt.zdbjq.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ecu.guannengcc.top

JS:   require.main === module
来源：http://pde.jinqigfzy.top

TS:   require.main === module
来源：http://gyv.xylfe.cn

Java: public static void main(String[] args)
来源：http://nns.fanxiaobao.xyz

Go:   func main()
来源：http://tlh.xylfe.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rxf.zdbjq.cn

C#:   static void Main(string[] args)
来源：http://mbc.feifeiyinyue.top

[M08] 获取系统与运行时信息
来源：http://hfb.mhx1999.top

Py:   platform.system();  platform.python_version()
来源：http://pfr.sjlbkw.cn

PHP:  PHP_OS;  phpversion();
来源：http://fwa.jinyuanbaomall.cn

JS:   process.platform;  process.version
来源：http://qzd.hywenlv.cn

TS:   process.platform;  process.version
来源：http://wdx.hfpthk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pmw.zhongyouzk.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ymw.daxiang520.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tao.nanxuanxn.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gli.xinyue.icu

================================================================================
来源：http://kvc.pycfn.com

N. 数据结构与算法
来源：http://ktb.sxryk.cn

================================================================================
来源：http://lwn.jlsjyb.cn

[N01] 二分查找（有序数组）
来源：http://vvu.cucudq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://orh.ydjk.org.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nhb.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cvk.dashuyun.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://csr.shzxlz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nmp.chenzaomai.com

Go:   sort.SearchInts(arr, x)
来源：http://rae.sweek.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://obd.guannengcc.top

C#:   Array.BinarySearch(arr, x)
来源：http://quc.zdbjq.cn

[N02] 排序（工程实践用内置实现）
来源：http://bor.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://nzw.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mzi.xziqi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://csz.cucudq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mja.snrcjt.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hof.ydjk.org.cn

Go:   slices.Sort(arr)
来源：http://oyk.gogol.net.cn

Ruby: arr.sort
来源：http://eum.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://enp.tanke756.top

[N03] 快速排序（分治示例）
来源：http://djb.hywenlv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wsd.yj202588.top

PHP:  // 递归实现，或用 usort
来源：http://oem.andypj.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yde.yangfankeji.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ffy.shzxlz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vji.svipenyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blx.cucudq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nfo.zhijiandao.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yvu.quarkkingdee.top

[N04] 斐波那契数列
来源：http://lqi.yuanzhike.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://drz.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hfb.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dlo.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dzj.yueranfly.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zow.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fyh.snrcjt.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ulh.cdnleiting.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xle.redwolf501.top

[N05] 最大公约数
来源：http://iuv.zycfv.cn

Py:   math.gcd(a, b)
来源：http://qcg.chenjidiqi.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lqr.dashuyun.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://phr.guowangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://evk.xziqi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ybb.hcnkem.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://url.xylfe.cn

Ruby: a.gcd(b)
来源：http://ozq.zhongyouzk.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mht.havefunace.top

[N06] 判断回文字符串
来源：http://tvd.shangyingyoupin.top

Py:   s == s[::-1]
来源：http://bqy.ivvv.top

PHP:  $s === strrev($s);
来源：http://fof.tianlin.xyz

JS:   s === [...s].reverse().join("")
来源：http://apu.yuxming.cn

TS:   s === [...s].reverse().join("")
来源：http://ult.yj20258888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://quv.havefunace.top

Go:   // 双指针从两端比较
来源：http://mkh.meibo888.top

Ruby: s == s.reverse
来源：http://wyr.uphjek.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://yfj.fzhhl.top

[N07] 两数之和（返回下标）
来源：http://oxu.jqgfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sbp.sweek.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://giu.ppjwa.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://csw.dashuyun.cn

TS:   // 手写 Map<string, number>
来源：http://rkx.cqqwz.cn

Java: // 手写 HashMap
来源：http://pgs.52xcode.cn

Go:   // 手写 map[int]int
来源：http://row.quarkkingdee.top

Ruby: // 手写 Hash
来源：http://qka.xuetiantiany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nsk.ydzc1.top

[N08] 生成全排列
来源：http://bty.yuanzhike.top

Py:   itertools.permutations(arr)
来源：http://rks.0kj1m.cn

PHP:  // 手写递归交换
来源：http://pij.0kj1m.cn

JS:   // 手写回溯递归
来源：http://vpp.fktsv.cn

TS:   // 手写回溯递归
来源：http://qdx.9152youxi.cn

Java: // 手写回溯递归
来源：http://hol.jqgufenzy.top

Go:   // 手写回溯递归
来源：http://mzu.52xcode.cn

Ruby: arr.permutation.to_a
来源：http://rhk.jinqigufen.top

C#:   // 手写回溯递归
来源：http://bzn.epnwcf.com

[N09] 栈与队列
来源：http://haj.yj20258888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wug.bjfxy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lqi.zhongyouzk.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iyb.zycfv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pwf.zhiwuduotai.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tnx.gzhubu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mmk.ctjpmb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dtp.tarul.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zgp.pycfn.com

[N10] 链表节点定义
来源：http://vpk.316326.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wje.zhaomingkeji.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://veb.pengpengdd.cyou


<!-- 参考信息 -->