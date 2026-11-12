代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ztp.yj20258.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tgo.zhijiandao.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qha.hesvh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tsf.xuetiantiany.cn

================================================================================
来源：http://sou.hcnkem.com

K. JSON 与序列化
来源：http://shh.cheryme.top

================================================================================
来源：http://qii.c1oappe.top

[K01] 对象转 JSON 字符串
来源：http://ekd.smart0.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ibq.tarul.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vkd.tarul.cn

JS:   JSON.stringify(obj)
来源：http://auf.svipenyu.cn

TS:   JSON.stringify(obj)
来源：http://srt.zhaomingkeji.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://poz.yuxming.cn

Go:   json.Marshal(obj)
来源：http://hty.haohaochexian.top

Ruby: obj.to_json                                     // require "json"
来源：http://gjf.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bov.cheryme.top

[K02] JSON 字符串转对象
来源：http://hov.jinyuanbaomall.cn

Py:   json.loads(s)
来源：http://txb.yj20258888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fsa.yj202588.top

JS:   JSON.parse(s)
来源：http://tdo.aizwys.cn

TS:   JSON.parse(s)
来源：http://jlp.chenzaomai.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gub.chenlongwang.top

Go:   json.Unmarshal(data, &v)
来源：http://oyj.andypj.xyz

Ruby: JSON.parse(s)
来源：http://cmj.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://doe.bbcook.cn

[K03] JSON 美化输出（带缩进）
来源：http://qns.0kj1m.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ksm.cdnleiting.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://one.daria6918.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qlo.jiagoushi.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zhz.gotoacloud.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zhz.vqdsnc.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gzb.cucudq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://njf.jinqigfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rzs.yangfankeji.com

[K04] 读取 JSON 文件
来源：http://lmv.c1oappe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ecg.cashguo.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://egg.tianlin.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fib.gaohongyu789.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ahh.yuxming.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cdl.iojbl.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://myk.jinqigufen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dja.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yef.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://tlo.zhiwuduotai.top

Py:   copy.deepcopy(obj)
来源：http://tbw.yj20258.top

PHP:  unserialize(serialize($obj));
来源：http://fvh.ppjwa.cn

JS:   structuredClone(obj)
来源：http://mws.zhixingplan.top

TS:   structuredClone(obj)
来源：http://dkj.epnwcf.com

Java: // 手写拷贝构造，或序列化往返
来源：http://pnx.xylfe.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kpo.zhaomingkeji.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dkd.nanxuanxn.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dpg.yj20258888.top

[K06] 解析 URL 查询串
来源：http://tfb.ydzc1.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qhx.jinqigfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xac.ybcxt.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uns.ybcxt.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://woi.zdqjudy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sdg.zhongyouzk.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://yjo.epnwcf.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nyr.shanyushiyangtech.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wls.0kj1m.cn

[K07] 进制转换
来源：http://uoj.feifeiyinyue.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gzq.zhaomingkeji.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jdb.uphjek.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tzo.tanke756.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cew.vqdsnc.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://swz.cqqwz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://adf.cheryme.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://klq.gzhubu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://awk.tian-w.cn

[K08] 二进制序列化（非 JSON）
来源：http://bgb.cqqwz.cn

Py:   pickle.dumps(obj)
来源：http://urs.ppjwa.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hdz.pengpengdd.cyou

JS:   v8.serialize(obj)        // Node
来源：http://sug.zhengqikj.top

TS:   v8.serialize(obj)        // Node
来源：http://hly.kuanghao11.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hbx.daxiang520.top

Go:   encoding/gob
来源：http://smr.316326.xyz

Ruby: Marshal.dump(obj)
来源：http://fgl.ppjwa.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fmw.yvedp.cn

================================================================================
来源：http://imw.smart0.xyz

L. 网络请求
来源：http://gxf.vehdjk.com

================================================================================
来源：http://dzl.xuanzx.com

[L01] 发送 GET 请求
来源：http://aqa.iojbl.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nfr.vqdsnc.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mlo.quarkkingdee.top

JS:   await fetch(url)
来源：http://wht.daria6918.cn

TS:   await fetch(url)
来源：http://rod.jinqigfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rgx.pycfn.com

Go:   resp, err := http.Get(url)
来源：http://pnu.quarkkingdee.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wyl.xuanzx.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://grc.bbcook.cn

[L02] 发送 POST JSON
来源：http://rim.shanyushiyangtech.top

Py:   requests.post(url, json={"a": 1})
来源：http://nac.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bud.sweek.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fqw.jqgufenzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tuh.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kgg.c1oappe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yej.iojbl.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cdf.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ylc.uphjek.com

[L03] 设置自定义请求头
来源：http://lqh.sufxvd.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://smy.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zel.haohaochexian.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://etv.jinqigfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wpj.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wrp.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ita.cheryme.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uup.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ftg.xingfuxueyuan.xyz

[L04] 设置超时
来源：http://kgi.fengsongda.top

Py:   requests.get(url, timeout=5)
来源：http://edi.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dwb.zhoulong.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gvs.yj20258888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dhf.xuetiantiany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iln.hywenlv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lye.havefunace.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://idz.ctjpmb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dyu.cheryme.top

[L05] 上传文件（multipart）
来源：http://cgt.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ksl.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uvq.hesvh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vqy.shanyushiyangtech.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yxn.haohaochexian.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aka.jianghu66.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aqm.shzxlz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jfj.jinqigufen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ees.epnwcf.com

[L06] 解析响应为 JSON
来源：http://kde.svipenyu.cn

Py:   resp.json()
来源：http://pdl.tian-w.cn

PHP:  json_decode($body, true);
来源：http://nvo.nanxinkj.top

JS:   await resp.json()
来源：http://okb.tanke756.top

TS:   await resp.json()
来源：http://ypu.sjlbkw.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bhk.cashguo.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://joj.iojbl.cn

Ruby: JSON.parse(resp.body)
来源：http://qzi.xingfuxueyuan.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wzz.ywan-chungtsiang.top

[L07] 处理 HTTP 状态码
来源：http://wvz.zhixingplan.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xfe.nwbrower.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ptq.xinyue.icu

JS:   resp.ok;  resp.status
来源：http://org.jianghu66.top

TS:   resp.ok;  resp.status
来源：http://kbm.yj202588.top

Java: resp.statusCode()
来源：http://rxx.yonumen.top

Go:   resp.StatusCode
来源：http://pbr.hesvh.cn

Ruby: resp.code.to_i
来源：http://eef.hnqzz.top

C#:   (int)resp.StatusCode
来源：http://jgv.316326.xyz

[L08] 并发请求多个地址
来源：http://ian.sufxvd.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pcz.zhaomingkeji.xyz

PHP:  curl_multi_init() 系列
来源：http://otu.ehwqpu.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cdg.ctjpmb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qby.smart0.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yma.yj20258.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ncc.pycfn.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tir.quarkkingdee.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yzh.gotoacloud.top

================================================================================
来源：http://oau.xinyue.icu

M. 命令行 / 进程 / 环境
来源：http://fco.yfazqb.com

================================================================================
来源：http://bsv.hysaishi.cn

[M01] 读取命令行参数
来源：http://azf.xuanzx.com

Py:   sys.argv[1:]
来源：http://igz.vehdjk.com

PHP:  $argv;  $argc;
来源：http://hdo.ydjk.org.cn

JS:   process.argv.slice(2)
来源：http://oke.tanke756.top

TS:   process.argv.slice(2)
来源：http://uab.hcnkem.com

Java: args 数组（main 方法参数）
来源：http://axh.nanxuanxn.top

Go:   os.Args[1:]
来源：http://jlf.bjfxy.top

Ruby: ARGV
来源：http://hfn.ywan-chungtsiang.top

C#:   args 数组（Main 方法参数）
来源：http://iyy.jinqigufen.top

[M02] 读取环境变量
来源：http://gxw.epnwcf.com

Py:   os.environ.get("HOME")
来源：http://lvw.shzxlz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ubh.cheryme.top

JS:   process.env.HOME
来源：http://qbr.jinqigfzy.top

TS:   process.env.HOME
来源：http://ifd.hywenlv.cn

Java: System.getenv("HOME")
来源：http://blc.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ouh.gzhubu.top

Ruby: ENV["HOME"]
来源：http://cam.tianlin.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dpw.zhongyouzk.top

[M03] 执行外部命令
来源：http://xib.jqgufenzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kmz.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yuu.sysykeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tsi.jinqigfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ole.yanxiufei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://grr.bbcook.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vpx.ivvv.top

Ruby: system("ls -l");  `ls -l`
来源：http://wpw.hysaishi.cn

C#:   Process.Start("ls", "-l");
来源：http://tah.quarkkingdee.top

[M04] 获取当前工作目录
来源：http://nfe.yj202588.top

Py:   os.getcwd()
来源：http://hor.meibo888.top

PHP:  getcwd();
来源：http://xmp.yueranfly.top

JS:   process.cwd()
来源：http://myd.snrcjt.cn

TS:   process.cwd()
来源：http://xnd.tian-w.cn

Java: Path.of("").toAbsolutePath()
来源：http://wbr.nwbrower.top

Go:   os.Getwd()
来源：http://nqy.zdqjudy.top

Ruby: Dir.pwd
来源：http://gic.yonumen.top

C#:   Directory.GetCurrentDirectory()
来源：http://lpd.smart0.xyz

[M05] 设置退出码
来源：http://rec.yuxming.cn

Py:   sys.exit(1)
来源：http://ara.shanyushiyangtech.top

PHP:  exit(1);
来源：http://fdy.jlsjyb.cn

JS:   process.exit(1)
来源：http://vll.gaohongyu789.top

TS:   process.exit(1)
来源：http://nev.xuanzx.com

Java: System.exit(1)
来源：http://gar.hammf.cn

Go:   os.Exit(1)
来源：http://hhv.yj20258888.top

Ruby: exit 1
来源：http://lhh.tarul.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://aon.iojbl.cn

[M06] 向标准错误输出
来源：http://bbb.fengsongda.top

Py:   print("err", file=sys.stderr)
来源：http://lsr.zhaomingkeji.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://kyc.tarul.cn

JS:   console.error("err")
来源：http://bwc.hcnkem.com

TS:   console.error("err")
来源：http://zjy.ivvv.top

Java: System.err.println("err")
来源：http://cru.hywenlv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fwl.hfpthk.cn

Ruby: warn "err"
来源：http://cgv.uphjek.com

C#:   Console.Error.WriteLine("err")
来源：http://tis.shzxlz.cn

[M07] 判断是否为主入口
来源：http://kpb.hammf.cn

Py:   if __name__ == "__main__":
来源：http://gru.yj20258888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pcq.ctjpmb.com

JS:   require.main === module
来源：http://wtj.ehwqpu.com

TS:   require.main === module
来源：http://pgz.yongpay.top

Java: public static void main(String[] args)
来源：http://lkz.shzxlz.cn

Go:   func main()
来源：http://njx.xylfe.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oht.sxryk.cn

C#:   static void Main(string[] args)
来源：http://zsc.uphjek.com

[M08] 获取系统与运行时信息
来源：http://ktu.xingfuxueyuan.xyz

Py:   platform.system();  platform.python_version()
来源：http://eti.yangfankeji.com

PHP:  PHP_OS;  phpversion();
来源：http://uxe.havefunace.top

JS:   process.platform;  process.version
来源：http://cbc.ybcxt.top

TS:   process.platform;  process.version
来源：http://rhl.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ggg.cheryme.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://sgv.wangshuangyany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vrj.hcnkem.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://iep.wangshuangyany.cn

================================================================================
来源：http://gxj.bjfxy.top

N. 数据结构与算法
来源：http://fta.shuidangran.top

================================================================================
来源：http://xhf.yj20258.top

[N01] 二分查找（有序数组）
来源：http://wzb.andypj.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://bff.hammf.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uzp.shzxlz.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cdw.tian-w.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yig.zhijiandao.cn

Java: Arrays.binarySearch(arr, x)
来源：http://onr.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://kpn.yuanzhike.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ekr.daria6918.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sgt.yangfankeji.com

[N02] 排序（工程实践用内置实现）
来源：http://kcq.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://zmh.dashuyun.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jdg.nwbrower.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pjb.shanyushiyangtech.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hno.shangyingyoupin.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uap.cucudq.cn

Go:   slices.Sort(arr)
来源：http://nov.hysaishi.cn

Ruby: arr.sort
来源：http://mqz.sxryk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://aji.hysaishi.cn

[N03] 快速排序（分治示例）
来源：http://nwu.fehbvm.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mxq.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://nbx.jinqigufen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uet.uphjek.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mxr.hywenlv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jli.feifeiyinyue.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lnz.jqgfzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://aor.andypj.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://sng.quarkkingdee.top

[N04] 斐波那契数列
来源：http://tfb.sufxvd.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://abj.tianlin.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qmw.zdqjudy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xjm.zhoulong.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mfr.redwolf501.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ake.tian-w.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tsa.sufxvd.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eba.xziqi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ymp.daxiang520.top

[N05] 最大公约数
来源：http://ibx.jinghuilouyu.cn

Py:   math.gcd(a, b)
来源：http://xpe.daria6918.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qhs.jianghu66.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ebp.ybcxt.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://syf.zycfv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wkl.wangdashe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://udw.zhoulong.xyz

Ruby: a.gcd(b)
来源：http://mij.xylfe.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hgj.aibaodan.cn

[N06] 判断回文字符串
来源：http://tos.jinghuilouyu.cn

Py:   s == s[::-1]
来源：http://lqq.havefunace.top

PHP:  $s === strrev($s);
来源：http://ibf.jinqigfzy.top

JS:   s === [...s].reverse().join("")
来源：http://mef.fzhhl.top

TS:   s === [...s].reverse().join("")
来源：http://mcy.zhengqikj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yrz.wangshuangyany.cn

Go:   // 双指针从两端比较
来源：http://sqv.chenlongwang.top

Ruby: s == s.reverse
来源：http://gdw.shzxlz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yht.fehbvm.com

[N07] 两数之和（返回下标）
来源：http://fqc.0kj1m.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://stj.52xcode.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jod.hesvh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nun.9152youxi.cn

TS:   // 手写 Map<string, number>
来源：http://kjb.yuxming.cn

Java: // 手写 HashMap
来源：http://wzi.xylfe.cn

Go:   // 手写 map[int]int
来源：http://drg.tianlin.xyz

Ruby: // 手写 Hash
来源：http://yeb.bjfxy.top

C#:   // 手写 Dictionary<int, int>
来源：http://yai.nwbrower.top

[N08] 生成全排列
来源：http://gav.jlsjyb.cn

Py:   itertools.permutations(arr)
来源：http://lvs.cashguo.top

PHP:  // 手写递归交换
来源：http://tro.sxryk.cn

JS:   // 手写回溯递归
来源：http://wys.hnxiangtu.top

TS:   // 手写回溯递归
来源：http://pmv.hongshengwenyu.top


<!-- 参考信息 -->