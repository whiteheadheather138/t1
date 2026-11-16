代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://epb.iojbl.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mcz.hammf.cn

JS:   JSON.stringify(obj)
来源：http://kxv.hywenlv.cn

TS:   JSON.stringify(obj)
来源：http://wkt.meibo888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jte.yongpay.top

Go:   json.Marshal(obj)
来源：http://axx.9152youxi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://miq.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jgv.c1oappe.top

[K02] JSON 字符串转对象
来源：http://npr.zycfv.cn

Py:   json.loads(s)
来源：http://qqh.gotoacloud.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cyt.9152youxi.cn

JS:   JSON.parse(s)
来源：http://mzs.hammf.cn

TS:   JSON.parse(s)
来源：http://fgx.bjfxy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tlk.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://zus.birdmap.top

Ruby: JSON.parse(s)
来源：http://dsm.meibo888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qxs.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://oxm.sysykeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bit.cdnleiting.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://end.gogol.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://atf.ydzc1.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bhe.zhongyouzk.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eqh.52xcode.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://svm.birdmap.top

Ruby: JSON.pretty_generate(obj)
来源：http://rdq.fzhhl.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uvl.bjfxy.top

[K04] 读取 JSON 文件
来源：http://tag.cdnleiting.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ddq.jiagoushi.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pqs.snrcjt.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cgr.yfazqb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bfe.ybcxt.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://avl.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uwq.yvedp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lpa.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cuq.hnxiangtu.top

[K05] 深拷贝对象
来源：http://qqq.yongpay.top

Py:   copy.deepcopy(obj)
来源：http://rrj.chenlongwang.top

PHP:  unserialize(serialize($obj));
来源：http://ant.0kj1m.cn

JS:   structuredClone(obj)
来源：http://xhh.hnqzz.top

TS:   structuredClone(obj)
来源：http://uig.chenzaomai.com

Java: // 手写拷贝构造，或序列化往返
来源：http://qvt.gzhubu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uov.sxryk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vyf.ydzc1.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gxo.yuanzhike.top

[K06] 解析 URL 查询串
来源：http://giz.bbcook.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mho.tian-w.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://snj.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ayb.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mrz.chenjidiqi.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wku.yonumen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ffi.yanxiufei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vsf.xziqi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://haj.ehwqpu.com

[K07] 进制转换
来源：http://omw.shuidangran.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rvp.gotoacloud.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lan.tian-w.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dtu.jinqigufen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ein.fanxiaobao.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rts.fengsongda.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ixx.fengsongda.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ark.sufxvd.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eni.fengsongda.top

[K08] 二进制序列化（非 JSON）
来源：http://trz.shzxlz.cn

Py:   pickle.dumps(obj)
来源：http://haz.iojbl.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lgk.gzhubu.top

JS:   v8.serialize(obj)        // Node
来源：http://kux.cucudq.cn

TS:   v8.serialize(obj)        // Node
来源：http://kly.tianlin.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wit.yonumen.top

Go:   encoding/gob
来源：http://wov.meibo888.top

Ruby: Marshal.dump(obj)
来源：http://mlf.xingfuxueyuan.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://msu.ydjk.org.cn

================================================================================
来源：http://yme.yangfankeji.com

L. 网络请求
来源：http://dnt.xingfuxueyuan.xyz

================================================================================
来源：http://yom.zhiwuduotai.top

[L01] 发送 GET 请求
来源：http://fmk.yvedp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pwr.zhoulong.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zib.sxryk.cn

JS:   await fetch(url)
来源：http://omg.cheryme.top

TS:   await fetch(url)
来源：http://orj.hfpthk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rqk.kuanghao11.cn

Go:   resp, err := http.Get(url)
来源：http://rko.sysykeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qvl.guannengcc.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pkg.birdmap.top

[L02] 发送 POST JSON
来源：http://rhj.dashuyun.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yqx.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dej.yonumen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://erh.guowangkeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vpb.yj20258.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kvk.jyoumei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tso.sweek.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hbe.jqgufenzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kwr.chenlongwang.top

[L03] 设置自定义请求头
来源：http://wgk.zhijiandao.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ouy.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gvn.shanyushiyangtech.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mvv.bbcook.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rqe.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uuq.iojbl.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gej.vehdjk.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yub.xylfe.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yew.hcnkem.com

[L04] 设置超时
来源：http://wkl.yonumen.top

Py:   requests.get(url, timeout=5)
来源：http://hvl.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yqz.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yhj.shanyushiyangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ctk.yongpay.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://doj.zhoulong.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ozl.zdqjudy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zve.jinqigufen.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ivb.yueranfly.top

[L05] 上传文件（multipart）
来源：http://lao.0kj1m.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xtq.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xjh.sxryk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eax.yvedp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gij.yvedp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://owu.wangdashe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ddk.shuidangran.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bxb.hcnkem.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ozy.birdmap.top

[L06] 解析响应为 JSON
来源：http://vgg.9152youxi.cn

Py:   resp.json()
来源：http://xjf.guannengcc.top

PHP:  json_decode($body, true);
来源：http://xlr.ppjwa.cn

JS:   await resp.json()
来源：http://efx.sxryk.cn

TS:   await resp.json()
来源：http://rtb.dashuyun.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vpd.bjfxy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dxl.jlsjyb.cn

Ruby: JSON.parse(resp.body)
来源：http://wfe.aibaodan.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qem.dianchejie.cn

[L07] 处理 HTTP 状态码
来源：http://zwm.tanke756.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ugq.chenlongwang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yoa.bjfxy.top

JS:   resp.ok;  resp.status
来源：http://sre.zhiwuduotai.top

TS:   resp.ok;  resp.status
来源：http://xxf.gzhubu.top

Java: resp.statusCode()
来源：http://bat.yuanzhike.top

Go:   resp.StatusCode
来源：http://xrr.guannengcc.top

Ruby: resp.code.to_i
来源：http://jtd.316326.xyz

C#:   (int)resp.StatusCode
来源：http://aii.aizwys.cn

[L08] 并发请求多个地址
来源：http://iio.wangdashe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://epn.yj202588.top

PHP:  curl_multi_init() 系列
来源：http://lkd.jinqigfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yzd.birdmap.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bto.zhoulong.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vsd.meibo888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rzx.52xcode.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nab.daria6918.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://roo.chenjidiqi.icu

================================================================================
来源：http://wjb.shzxlz.cn

M. 命令行 / 进程 / 环境
来源：http://olm.shanyushiyangtech.top

================================================================================
来源：http://fbv.ydjk.org.cn

[M01] 读取命令行参数
来源：http://njx.fzhhl.top

Py:   sys.argv[1:]
来源：http://fnl.shanyushiyangkeji.top

PHP:  $argv;  $argc;
来源：http://kjy.zhixingplan.top

JS:   process.argv.slice(2)
来源：http://nfl.guowangkeji.top

TS:   process.argv.slice(2)
来源：http://lqv.hywenlv.cn

Java: args 数组（main 方法参数）
来源：http://ldw.snrcjt.cn

Go:   os.Args[1:]
来源：http://gge.guowangkeji.top

Ruby: ARGV
来源：http://dsz.meibo888.top

C#:   args 数组（Main 方法参数）
来源：http://nnq.snrcjt.cn

[M02] 读取环境变量
来源：http://dwa.smart0.xyz

Py:   os.environ.get("HOME")
来源：http://ovl.kuanghao11.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://htv.cucudq.cn

JS:   process.env.HOME
来源：http://ksl.vqdsnc.cn

TS:   process.env.HOME
来源：http://ukc.shanyushiyangtech.top

Java: System.getenv("HOME")
来源：http://ovs.52xcode.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://crf.shuidangran.top

Ruby: ENV["HOME"]
来源：http://pvu.shanyushiyangtech.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wmh.shanyushiyangtech.top

[M03] 执行外部命令
来源：http://mkp.chenzaomai.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ykf.havefunace.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ume.chenlongwang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://chg.sufxvd.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jns.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sxh.yonumen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mlj.iojbl.cn

Ruby: system("ls -l");  `ls -l`
来源：http://peh.vehdjk.com

C#:   Process.Start("ls", "-l");
来源：http://ism.redwolf501.top

[M04] 获取当前工作目录
来源：http://dan.hnxiangtu.top

Py:   os.getcwd()
来源：http://pkb.shangyingyoupin.top

PHP:  getcwd();
来源：http://stl.yongpay.top

JS:   process.cwd()
来源：http://jym.zhijiandao.cn

TS:   process.cwd()
来源：http://ouo.zdqjudy.top

Java: Path.of("").toAbsolutePath()
来源：http://pca.hfpthk.cn

Go:   os.Getwd()
来源：http://bcv.sysykeji.top

Ruby: Dir.pwd
来源：http://fso.gaohongyu789.top

C#:   Directory.GetCurrentDirectory()
来源：http://axg.hnxiangtu.top

[M05] 设置退出码
来源：http://ukh.zycfv.cn

Py:   sys.exit(1)
来源：http://phi.ydjk.org.cn

PHP:  exit(1);
来源：http://kxn.snrcjt.cn

JS:   process.exit(1)
来源：http://vup.redwolf501.top

TS:   process.exit(1)
来源：http://vtl.jyoumei.cn

Java: System.exit(1)
来源：http://mtc.yvedp.cn

Go:   os.Exit(1)
来源：http://fgx.sjlbkw.cn

Ruby: exit 1
来源：http://dad.guannengcc.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oky.xinyue.icu

[M06] 向标准错误输出
来源：http://miv.zhoulong.xyz

Py:   print("err", file=sys.stderr)
来源：http://gri.hysaishi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://srz.shanyushiyangkeji.top

JS:   console.error("err")
来源：http://kfv.yuanzhike.top

TS:   console.error("err")
来源：http://jhh.aibaodan.cn

Java: System.err.println("err")
来源：http://ddq.gotoacloud.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xrl.jinqigufen.top

Ruby: warn "err"
来源：http://sjr.nwbrower.top

C#:   Console.Error.WriteLine("err")
来源：http://arg.c1oappe.top

[M07] 判断是否为主入口
来源：http://swa.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://okg.cdnleiting.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vvq.sjlbkw.cn

JS:   require.main === module
来源：http://stq.hesvh.cn

TS:   require.main === module
来源：http://lhm.shzxlz.cn

Java: public static void main(String[] args)
来源：http://qai.fktsv.cn

Go:   func main()
来源：http://qha.hcnkem.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://azx.sxryk.cn

C#:   static void Main(string[] args)
来源：http://chp.yonumen.top

[M08] 获取系统与运行时信息
来源：http://scp.zhixingplan.top

Py:   platform.system();  platform.python_version()
来源：http://csv.redwolf501.top

PHP:  PHP_OS;  phpversion();
来源：http://ddv.meibo888.top

JS:   process.platform;  process.version
来源：http://vhb.uphjek.com

TS:   process.platform;  process.version
来源：http://jng.zhiwuduotai.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dyf.snrcjt.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vdn.zhongyouzk.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blq.tianlin.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://yiw.tian-w.cn

================================================================================
来源：http://tgt.ehwqpu.com

N. 数据结构与算法
来源：http://gcs.jinqigfzy.top

================================================================================
来源：http://dpy.cdnleiting.top

[N01] 二分查找（有序数组）
来源：http://jqd.tian-w.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nsp.shanyushiyangtech.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uof.vqdsnc.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lfx.sxryk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cwe.9152youxi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cmg.shuidangran.top

Go:   sort.SearchInts(arr, x)
来源：http://kgb.andypj.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://mrp.yuxming.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zjs.yvedp.cn

[N02] 排序（工程实践用内置实现）
来源：http://fek.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://vki.gzhubu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jzc.ivvv.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qfa.ydjk.org.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://chv.jinqigfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://one.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://izw.hysaishi.cn

Ruby: arr.sort
来源：http://paj.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rxa.hnqzz.top

[N03] 快速排序（分治示例）
来源：http://hgu.sysykeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://puj.meibo888.top

PHP:  // 递归实现，或用 usort
来源：http://mhe.cheryme.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sip.quarkkingdee.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aei.fengsongda.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iby.tianlin.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ifq.gogol.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://esm.chenlongwang.top

C#:   // 手写递归，或 Array.Sort
来源：http://xmb.guowangkeji.top

[N04] 斐波那契数列
来源：http://mtu.jianghu66.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rcy.cdnleiting.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dcr.hcnkem.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://chh.jqgfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jmu.xylfe.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://adc.sysykeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eft.aizwys.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ore.nanxinkj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vjv.fanxiaobao.xyz

[N05] 最大公约数
来源：http://ggk.9152youxi.cn

Py:   math.gcd(a, b)
来源：http://hey.zhiwuduotai.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aqm.0kj1m.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tlg.ydjk.org.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ipl.ivvv.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vmb.hywenlv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ttd.hnqzz.top

Ruby: a.gcd(b)
来源：http://cqm.yfazqb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yad.wangdashe.top

[N06] 判断回文字符串
来源：http://vay.shuidangran.top

Py:   s == s[::-1]
来源：http://doo.wangdashe.top

PHP:  $s === strrev($s);
来源：http://mnz.daria6918.cn

JS:   s === [...s].reverse().join("")
来源：http://wjg.yongpay.top

TS:   s === [...s].reverse().join("")
来源：http://hrn.sxryk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aur.snrcjt.cn

Go:   // 双指针从两端比较
来源：http://key.zdqjudy.top

Ruby: s == s.reverse
来源：http://swg.cashguo.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ora.chenjidiqi.icu

[N07] 两数之和（返回下标）
来源：http://epe.vehdjk.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cwu.hcnkem.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aza.gogol.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pzb.xuanzx.com

TS:   // 手写 Map<string, number>
来源：http://fmw.jqgufenzy.top

Java: // 手写 HashMap
来源：http://yvl.cashguo.top

Go:   // 手写 map[int]int
来源：http://dqo.jqgufenzy.top

Ruby: // 手写 Hash
来源：http://vyf.tianlin.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://iyw.sxryk.cn

[N08] 生成全排列
来源：http://qyt.cheryme.top

Py:   itertools.permutations(arr)
来源：http://cbw.tian-w.cn

PHP:  // 手写递归交换
来源：http://ibr.yvedp.cn

JS:   // 手写回溯递归
来源：http://ucx.yj20258.top

TS:   // 手写回溯递归
来源：http://wed.zdbjq.cn

Java: // 手写回溯递归
来源：http://otn.uphjek.com

Go:   // 手写回溯递归
来源：http://gxb.zhijiandao.cn

Ruby: arr.permutation.to_a
来源：http://fux.jinqigfzy.top

C#:   // 手写回溯递归
来源：http://izx.shzxlz.cn

[N09] 栈与队列
来源：http://spw.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lni.hammf.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://srq.shangyingyoupin.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fww.tian-w.cn


<!-- 参考信息 -->