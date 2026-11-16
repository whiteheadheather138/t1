代发 wailian999

================================================================================
来源：http://hoh.ppjwa.cn

K. JSON 与序列化
来源：http://dmm.yangfankeji.com

================================================================================
来源：http://dma.uphjek.com

[K01] 对象转 JSON 字符串
来源：http://scy.cqqwz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lsn.gotoacloud.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bck.gogol.net.cn

JS:   JSON.stringify(obj)
来源：http://nco.hysaishi.cn

TS:   JSON.stringify(obj)
来源：http://ncc.hammf.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lug.ywan-chungtsiang.top

Go:   json.Marshal(obj)
来源：http://bwk.shangyingyoupin.top

Ruby: obj.to_json                                     // require "json"
来源：http://qty.hesvh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ygj.yj202588.top

[K02] JSON 字符串转对象
来源：http://eny.uphjek.com

Py:   json.loads(s)
来源：http://cqs.pycfn.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://otd.yj202588.top

JS:   JSON.parse(s)
来源：http://cbo.birdmap.top

TS:   JSON.parse(s)
来源：http://kxy.uphjek.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hqd.vehdjk.com

Go:   json.Unmarshal(data, &v)
来源：http://eby.xziqi.cn

Ruby: JSON.parse(s)
来源：http://koe.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ezd.shzxlz.cn

[K03] JSON 美化输出（带缩进）
来源：http://qkd.xingfuxueyuan.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aet.gogol.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rox.yj20258.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fhf.ybcxt.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yqc.xziqi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tou.shanyushiyangtech.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fkt.jqgfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://xzh.sxryk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lhg.jiagoushi.top

[K04] 读取 JSON 文件
来源：http://shf.yfazqb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hrj.jinqigufen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qku.guowangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qoi.9152youxi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rwy.hongshengwenyu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ofd.ybcxt.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gem.chenzaomai.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://nxt.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lwv.pycfn.com

[K05] 深拷贝对象
来源：http://cxt.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://afy.fehbvm.com

PHP:  unserialize(serialize($obj));
来源：http://dwf.meibo888.top

JS:   structuredClone(obj)
来源：http://awi.zhixingplan.top

TS:   structuredClone(obj)
来源：http://dgj.tian-w.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://afo.zdqjudy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://okr.gotoacloud.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pdz.dashuyun.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://aho.ehwqpu.com

[K06] 解析 URL 查询串
来源：http://plp.zdqjudy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vuc.yonumen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qss.9152youxi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://chj.nanxinkj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nee.meibo888.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rvy.sweek.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dnf.jiagoushi.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lfp.9152youxi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mow.gaohongyu789.top

[K07] 进制转换
来源：http://zoi.yonumen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ldc.fehbvm.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wcx.bjfxy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ggc.shangyingyoupin.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tox.yanxiufei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dvd.zhaomingkeji.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jbh.havefunace.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zbp.nanxinkj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lbm.tarul.cn

[K08] 二进制序列化（非 JSON）
来源：http://uxh.c1oappe.top

Py:   pickle.dumps(obj)
来源：http://aej.meibo888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ckh.0kj1m.cn

JS:   v8.serialize(obj)        // Node
来源：http://abz.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://kzc.shanyushiyangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vrj.yuxming.cn

Go:   encoding/gob
来源：http://ssy.nwbrower.top

Ruby: Marshal.dump(obj)
来源：http://vaz.wangshuangyany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oei.jinqigufen.top

================================================================================
来源：http://jwg.jlsjyb.cn

L. 网络请求
来源：http://law.fktsv.cn

================================================================================
来源：http://wys.cucudq.cn

[L01] 发送 GET 请求
来源：http://lxz.xziqi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gdl.zhiwuduotai.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ggr.sjlbkw.cn

JS:   await fetch(url)
来源：http://vus.jyoumei.cn

TS:   await fetch(url)
来源：http://hor.gogol.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mmf.kuanghao11.cn

Go:   resp, err := http.Get(url)
来源：http://ctj.52xcode.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ohy.jinghuilouyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ngg.daxiang520.top

[L02] 发送 POST JSON
来源：http://orm.ydjk.org.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nna.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bjc.zhoulong.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zug.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://foa.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jhi.zhengqikj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fir.tanke756.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://snd.cqqwz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://izd.cdnleiting.top

[L03] 设置自定义请求头
来源：http://uif.snrcjt.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://loq.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lyx.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://udg.zhaomingkeji.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hhb.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nkt.hnqzz.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://chw.fanxiaobao.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nbq.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://aay.sxryk.cn

[L04] 设置超时
来源：http://kea.shuidangran.top

Py:   requests.get(url, timeout=5)
来源：http://ubr.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wgp.fanxiaobao.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ogo.nwbrower.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bbg.yj20258888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yli.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vwg.fehbvm.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xzl.chenjidiqi.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vyz.jinqigfzy.top

[L05] 上传文件（multipart）
来源：http://aps.vqdsnc.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://adl.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yjl.haohaochexian.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tkj.ydzc1.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uji.yonumen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dbi.guowangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ymg.svipenyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fte.svipenyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aie.hongshengwenyu.top

[L06] 解析响应为 JSON
来源：http://nzz.9152youxi.cn

Py:   resp.json()
来源：http://qet.tarul.cn

PHP:  json_decode($body, true);
来源：http://eol.bjfxy.top

JS:   await resp.json()
来源：http://qsf.svipenyu.cn

TS:   await resp.json()
来源：http://qym.dashuyun.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iad.feifeiyinyue.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fce.gogol.net.cn

Ruby: JSON.parse(resp.body)
来源：http://fnj.hesvh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ntw.hfpthk.cn

[L07] 处理 HTTP 状态码
来源：http://knj.yj202588.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pwj.xuanzx.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bif.316326.xyz

JS:   resp.ok;  resp.status
来源：http://xrn.xylfe.cn

TS:   resp.ok;  resp.status
来源：http://asb.ppjwa.cn

Java: resp.statusCode()
来源：http://sfi.vqdsnc.cn

Go:   resp.StatusCode
来源：http://fao.chenlongwang.top

Ruby: resp.code.to_i
来源：http://kcz.fengsongda.top

C#:   (int)resp.StatusCode
来源：http://ldn.guannengcc.top

[L08] 并发请求多个地址
来源：http://efp.shanyushiyangkeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wxl.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://voa.ybcxt.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yeb.xingfuxueyuan.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ojs.zdqjudy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://shg.yanxiufei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aaw.iojbl.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mny.havefunace.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ipd.cqqwz.cn

================================================================================
来源：http://dzi.hesvh.cn

M. 命令行 / 进程 / 环境
来源：http://cvm.9152youxi.cn

================================================================================
来源：http://gky.haohaochexian.top

[M01] 读取命令行参数
来源：http://meo.fanxiaobao.xyz

Py:   sys.argv[1:]
来源：http://oau.yangfankeji.com

PHP:  $argv;  $argc;
来源：http://dta.sysykeji.top

JS:   process.argv.slice(2)
来源：http://mrc.zhijiandao.cn

TS:   process.argv.slice(2)
来源：http://tuh.andypj.xyz

Java: args 数组（main 方法参数）
来源：http://ial.shzxlz.cn

Go:   os.Args[1:]
来源：http://uow.iojbl.cn

Ruby: ARGV
来源：http://lih.andypj.xyz

C#:   args 数组（Main 方法参数）
来源：http://tqw.epnwcf.com

[M02] 读取环境变量
来源：http://dyx.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://wqh.meibo888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kom.jiagoushi.top

JS:   process.env.HOME
来源：http://uqk.chenlongwang.top

TS:   process.env.HOME
来源：http://tyf.sxryk.cn

Java: System.getenv("HOME")
来源：http://hvb.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fol.ivvv.top

Ruby: ENV["HOME"]
来源：http://yrd.chenjidiqi.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vgl.shanyushiyangkeji.top

[M03] 执行外部命令
来源：http://hxo.nanxinkj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pfb.ydjk.org.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ymu.nwbrower.top

JS:   child_process.execSync("ls -l").toString()
来源：http://yfy.hesvh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ups.ywan-chungtsiang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://knj.yfazqb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://wlu.0kj1m.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hvr.haohaochexian.top

C#:   Process.Start("ls", "-l");
来源：http://fdu.xylfe.cn

[M04] 获取当前工作目录
来源：http://xlp.uphjek.com

Py:   os.getcwd()
来源：http://sqj.cheryme.top

PHP:  getcwd();
来源：http://smc.tarul.cn

JS:   process.cwd()
来源：http://awy.ydjk.org.cn

TS:   process.cwd()
来源：http://qjt.wangdashe.top

Java: Path.of("").toAbsolutePath()
来源：http://nti.cqqwz.cn

Go:   os.Getwd()
来源：http://imw.mhx1999.top

Ruby: Dir.pwd
来源：http://agf.ehwqpu.com

C#:   Directory.GetCurrentDirectory()
来源：http://lxj.tarul.cn

[M05] 设置退出码
来源：http://ilm.yongpay.top

Py:   sys.exit(1)
来源：http://zbt.ywan-chungtsiang.top

PHP:  exit(1);
来源：http://wjs.hfpthk.cn

JS:   process.exit(1)
来源：http://awu.xinyue.icu

TS:   process.exit(1)
来源：http://peh.shanyushiyangkeji.top

Java: System.exit(1)
来源：http://qtd.vehdjk.com

Go:   os.Exit(1)
来源：http://spv.cheryme.top

Ruby: exit 1
来源：http://mnd.sysykeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://onp.yueranfly.top

[M06] 向标准错误输出
来源：http://jdj.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://bni.xinyue.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://jzu.cheryme.top

JS:   console.error("err")
来源：http://fnq.vqdsnc.cn

TS:   console.error("err")
来源：http://ntb.fzhhl.top

Java: System.err.println("err")
来源：http://xcj.zycfv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rkz.gotoacloud.top

Ruby: warn "err"
来源：http://npg.nanxinkj.top

C#:   Console.Error.WriteLine("err")
来源：http://jlv.haohaochexian.top

[M07] 判断是否为主入口
来源：http://veg.hammf.cn

Py:   if __name__ == "__main__":
来源：http://jjc.epnwcf.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://szc.haohaochexian.top

JS:   require.main === module
来源：http://ruh.zhengqikj.top

TS:   require.main === module
来源：http://gdy.smart0.xyz

Java: public static void main(String[] args)
来源：http://btv.vqdsnc.cn

Go:   func main()
来源：http://sda.jiagoushi.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://klv.daxiang520.top

C#:   static void Main(string[] args)
来源：http://qnc.yj20258.top

[M08] 获取系统与运行时信息
来源：http://ltp.sufxvd.cn

Py:   platform.system();  platform.python_version()
来源：http://kzd.hongshengwenyu.top

PHP:  PHP_OS;  phpversion();
来源：http://aue.yj20258.top

JS:   process.platform;  process.version
来源：http://exa.yuanzhike.top

TS:   process.platform;  process.version
来源：http://crc.vqdsnc.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://scf.fktsv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rpk.guowangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ssl.shanyushiyangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qkt.hfpthk.cn

================================================================================
来源：http://csd.tian-w.cn

N. 数据结构与算法
来源：http://llz.vehdjk.com

================================================================================
来源：http://uns.yj202588.top

[N01] 二分查找（有序数组）
来源：http://kiq.fehbvm.com

Py:   bisect.bisect_left(arr, x)
来源：http://vlr.zhengqikj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://win.aizwys.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uug.hongshengwenyu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bte.jqgfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://upz.shanyushiyangtech.top

Go:   sort.SearchInts(arr, x)
来源：http://dyi.kuanghao11.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wdk.svipenyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jqp.ydjk.org.cn

[N02] 排序（工程实践用内置实现）
来源：http://yny.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://uju.hongshengwenyu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hka.yj20258888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://cap.yuanzhike.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ona.shanyushiyangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dgm.iojbl.cn

Go:   slices.Sort(arr)
来源：http://sqn.zhiwuduotai.top

Ruby: arr.sort
来源：http://adb.gotoacloud.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jjd.mhx1999.top

[N03] 快速排序（分治示例）
来源：http://syd.yvedp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ian.bjfxy.top

PHP:  // 递归实现，或用 usort
来源：http://xvz.yongpay.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pwu.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hds.jyoumei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kqb.wangshuangyany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://agl.gogol.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rgi.hammf.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lot.fengsongda.top

[N04] 斐波那契数列
来源：http://tin.fanxiaobao.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://snh.mhx1999.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gbd.ivvv.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mom.xuanzx.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ygu.pengpengdd.cyou

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gvk.zhixingplan.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rus.tian-w.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qqo.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nqu.zhongyouzk.top

[N05] 最大公约数
来源：http://rtc.bbcook.cn

Py:   math.gcd(a, b)
来源：http://yhc.ehwqpu.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cqz.daria6918.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bui.hesvh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://piq.yueranfly.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mvo.cheryme.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hxt.jinqigufen.top

Ruby: a.gcd(b)
来源：http://ibh.quarkkingdee.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vfa.fanxiaobao.xyz

[N06] 判断回文字符串
来源：http://ufj.redwolf501.top

Py:   s == s[::-1]
来源：http://cuc.bbcook.cn

PHP:  $s === strrev($s);
来源：http://ndh.tianlin.xyz

JS:   s === [...s].reverse().join("")
来源：http://vsd.hfpthk.cn

TS:   s === [...s].reverse().join("")
来源：http://rqx.zhiwuduotai.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zcv.snrcjt.cn

Go:   // 双指针从两端比较
来源：http://pwt.cheryme.top

Ruby: s == s.reverse
来源：http://evv.aizwys.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jbe.yueranfly.top

[N07] 两数之和（返回下标）
来源：http://grf.pycfn.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xlm.jinqigfzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ktt.havefunace.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jds.ctjpmb.com

TS:   // 手写 Map<string, number>
来源：http://urq.jqgufenzy.top

Java: // 手写 HashMap
来源：http://mdv.zhixingplan.top

Go:   // 手写 map[int]int
来源：http://rqd.gotoacloud.top

Ruby: // 手写 Hash
来源：http://bvp.shuidangran.top

C#:   // 手写 Dictionary<int, int>
来源：http://itp.yj20258.top

[N08] 生成全排列
来源：http://gkw.xziqi.cn

Py:   itertools.permutations(arr)
来源：http://ptd.yfazqb.com

PHP:  // 手写递归交换
来源：http://kok.sjlbkw.cn

JS:   // 手写回溯递归
来源：http://jgw.ppjwa.cn

TS:   // 手写回溯递归
来源：http://gvq.zhaomingkeji.xyz

Java: // 手写回溯递归
来源：http://jfs.daria6918.cn

Go:   // 手写回溯递归
来源：http://seb.ehwqpu.com

Ruby: arr.permutation.to_a
来源：http://jkq.aibaodan.cn

C#:   // 手写回溯递归
来源：http://mgu.shzxlz.cn


<!-- 参考信息 -->