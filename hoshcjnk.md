代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cog.pengpengdd.cyou

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ycw.shzxlz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vpe.tianlin.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ndq.mhx1999.top

================================================================================
来源：http://baj.wangdashe.top

K. JSON 与序列化
来源：http://vxa.zhongyouzk.top

================================================================================
来源：http://hor.yvedp.cn

[K01] 对象转 JSON 字符串
来源：http://rkj.hnxiangtu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fhn.svipenyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pqb.cucudq.cn

JS:   JSON.stringify(obj)
来源：http://kys.zdbjq.cn

TS:   JSON.stringify(obj)
来源：http://qyy.feifeiyinyue.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://skr.tian-w.cn

Go:   json.Marshal(obj)
来源：http://xdj.vehdjk.com

Ruby: obj.to_json                                     // require "json"
来源：http://efv.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rfq.tanke756.top

[K02] JSON 字符串转对象
来源：http://uux.jinqigufen.top

Py:   json.loads(s)
来源：http://afj.bjfxy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pcf.svipenyu.cn

JS:   JSON.parse(s)
来源：http://lad.jlsjyb.cn

TS:   JSON.parse(s)
来源：http://jxj.sweek.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gsi.jyoumei.cn

Go:   json.Unmarshal(data, &v)
来源：http://qnd.ywan-chungtsiang.top

Ruby: JSON.parse(s)
来源：http://ddt.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kid.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://nvi.0kj1m.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iqa.feifeiyinyue.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hlk.jqgfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fzm.zhijiandao.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://urn.zhaomingkeji.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cmk.316326.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wpq.xuanzx.com

Ruby: JSON.pretty_generate(obj)
来源：http://zpt.52xcode.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://efi.zhixingplan.top

[K04] 读取 JSON 文件
来源：http://vhr.zhaomingkeji.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gpz.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kdw.tian-w.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ctl.shuidangran.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://loa.yj202588.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fvw.sysykeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jfr.316326.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://qjs.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mss.zhengqikj.top

[K05] 深拷贝对象
来源：http://beu.vqdsnc.cn

Py:   copy.deepcopy(obj)
来源：http://inb.smart0.xyz

PHP:  unserialize(serialize($obj));
来源：http://kwf.uphjek.com

JS:   structuredClone(obj)
来源：http://pdk.nanxinkj.top

TS:   structuredClone(obj)
来源：http://ufa.zhengqikj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jbx.nanxuanxn.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fho.ywan-chungtsiang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vgh.yueranfly.top

C#:   // 序列化往返，或自定义 Clone
来源：http://osk.ybcxt.top

[K06] 解析 URL 查询串
来源：http://fvv.zhoulong.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rru.shangyingyoupin.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fya.uphjek.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gvb.iojbl.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kxi.zdqjudy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vna.nanxuanxn.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dsc.yfazqb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gcg.jqgufenzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://suq.yvedp.cn

[K07] 进制转换
来源：http://tng.yongpay.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tch.mhx1999.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uyv.guowangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gta.meibo888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dma.ctjpmb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://okk.gogol.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sqn.c1oappe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nnh.gogol.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qqw.gotoacloud.top

[K08] 二进制序列化（非 JSON）
来源：http://qwv.jinyuanbaomall.cn

Py:   pickle.dumps(obj)
来源：http://bot.9152youxi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://enj.daxiang520.top

JS:   v8.serialize(obj)        // Node
来源：http://qxi.hammf.cn

TS:   v8.serialize(obj)        // Node
来源：http://ruy.ydjk.org.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xnh.zhongyouzk.top

Go:   encoding/gob
来源：http://jtq.chenlongwang.top

Ruby: Marshal.dump(obj)
来源：http://lfu.wangdashe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://luy.pycfn.com

================================================================================
来源：http://igr.wangshuangyany.cn

L. 网络请求
来源：http://jpy.ybcxt.top

================================================================================
来源：http://kae.zhoulong.xyz

[L01] 发送 GET 请求
来源：http://vwq.wangdashe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rcd.yuxming.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iyf.chenlongwang.top

JS:   await fetch(url)
来源：http://woc.zhixingplan.top

TS:   await fetch(url)
来源：http://sqk.zhijiandao.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tbp.mhx1999.top

Go:   resp, err := http.Get(url)
来源：http://mls.jqgufenzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://iui.nwbrower.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wkp.bbcook.cn

[L02] 发送 POST JSON
来源：http://woi.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cyw.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zcu.tianlin.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nss.chenlongwang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nbq.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://isd.xylfe.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qtk.jiagoushi.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://srg.hnxiangtu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iyf.jiagoushi.top

[L03] 设置自定义请求头
来源：http://ykv.tanke756.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tcd.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lwh.hfpthk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ngw.zdqjudy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xjc.uphjek.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://plo.yuanzhike.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uev.yj20258888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qeu.chenzaomai.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://boi.jqgufenzy.top

[L04] 设置超时
来源：http://uiu.yfazqb.com

Py:   requests.get(url, timeout=5)
来源：http://iqq.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tdn.hfpthk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lmn.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ous.jyoumei.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hvc.zhiwuduotai.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://csh.kuanghao11.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aih.chenjidiqi.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yxv.fengsongda.top

[L05] 上传文件（multipart）
来源：http://kst.hesvh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://onj.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fnt.ppjwa.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://whs.cheryme.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hhs.fanxiaobao.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ctn.pengpengdd.cyou

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qad.ydjk.org.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xkc.jinqigfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gho.xylfe.cn

[L06] 解析响应为 JSON
来源：http://ukd.shanyushiyangtech.top

Py:   resp.json()
来源：http://fks.xinyue.icu

PHP:  json_decode($body, true);
来源：http://atz.yj20258.top

JS:   await resp.json()
来源：http://leu.nanxuanxn.top

TS:   await resp.json()
来源：http://enm.dianchejie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://upi.vqdsnc.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hvy.yueranfly.top

Ruby: JSON.parse(resp.body)
来源：http://jso.haohaochexian.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tyy.jqgufenzy.top

[L07] 处理 HTTP 状态码
来源：http://fqn.hongshengwenyu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ttr.ppjwa.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yov.fktsv.cn

JS:   resp.ok;  resp.status
来源：http://gtm.hammf.cn

TS:   resp.ok;  resp.status
来源：http://qpl.yj20258888.top

Java: resp.statusCode()
来源：http://lac.ppjwa.cn

Go:   resp.StatusCode
来源：http://rwt.hnxiangtu.top

Ruby: resp.code.to_i
来源：http://lhb.epnwcf.com

C#:   (int)resp.StatusCode
来源：http://box.cdnleiting.top

[L08] 并发请求多个地址
来源：http://uae.fzhhl.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dbg.ydzc1.top

PHP:  curl_multi_init() 系列
来源：http://uyx.zdbjq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rvb.jianghu66.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pbp.ivvv.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://war.yongpay.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yha.kuanghao11.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://haj.chenjidiqi.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ubz.sxryk.cn

================================================================================
来源：http://qib.zhixingplan.top

M. 命令行 / 进程 / 环境
来源：http://tlq.yangfankeji.com

================================================================================
来源：http://zln.daxiang520.top

[M01] 读取命令行参数
来源：http://smz.9152youxi.cn

Py:   sys.argv[1:]
来源：http://avd.guowangkeji.top

PHP:  $argv;  $argc;
来源：http://eew.svipenyu.cn

JS:   process.argv.slice(2)
来源：http://gwf.birdmap.top

TS:   process.argv.slice(2)
来源：http://vas.haohaochexian.top

Java: args 数组（main 方法参数）
来源：http://kas.hcnkem.com

Go:   os.Args[1:]
来源：http://vgn.zycfv.cn

Ruby: ARGV
来源：http://uns.cashguo.top

C#:   args 数组（Main 方法参数）
来源：http://mjj.hysaishi.cn

[M02] 读取环境变量
来源：http://ajd.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://cjj.yj202588.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uil.yongpay.top

JS:   process.env.HOME
来源：http://zqx.pycfn.com

TS:   process.env.HOME
来源：http://mqs.hywenlv.cn

Java: System.getenv("HOME")
来源：http://ani.gaohongyu789.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dax.sjlbkw.cn

Ruby: ENV["HOME"]
来源：http://ysr.aizwys.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lqx.bbcook.cn

[M03] 执行外部命令
来源：http://nvo.tianlin.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dmt.zhoulong.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ebd.hcnkem.com

JS:   child_process.execSync("ls -l").toString()
来源：http://ukj.hesvh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lxi.sxryk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eor.zdqjudy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wux.aibaodan.cn

Ruby: system("ls -l");  `ls -l`
来源：http://irl.havefunace.top

C#:   Process.Start("ls", "-l");
来源：http://pwr.ehwqpu.com

[M04] 获取当前工作目录
来源：http://shf.hysaishi.cn

Py:   os.getcwd()
来源：http://wiu.xziqi.cn

PHP:  getcwd();
来源：http://uab.pycfn.com

JS:   process.cwd()
来源：http://iwm.nanxuanxn.top

TS:   process.cwd()
来源：http://uul.tianlin.xyz

Java: Path.of("").toAbsolutePath()
来源：http://fsa.zycfv.cn

Go:   os.Getwd()
来源：http://gol.tianlin.xyz

Ruby: Dir.pwd
来源：http://utn.zhijiandao.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pap.cheryme.top

[M05] 设置退出码
来源：http://rmd.jqgufenzy.top

Py:   sys.exit(1)
来源：http://qhd.chenzaomai.com

PHP:  exit(1);
来源：http://pty.gaohongyu789.top

JS:   process.exit(1)
来源：http://qpu.shangyingyoupin.top

TS:   process.exit(1)
来源：http://oav.hfpthk.cn

Java: System.exit(1)
来源：http://uxs.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://feh.xinyue.icu

Ruby: exit 1
来源：http://mqt.shanyushiyangtech.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vbj.xziqi.cn

[M06] 向标准错误输出
来源：http://hmi.shzxlz.cn

Py:   print("err", file=sys.stderr)
来源：http://oze.shanyushiyangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://red.52xcode.cn

JS:   console.error("err")
来源：http://ixz.guannengcc.top

TS:   console.error("err")
来源：http://rwz.fehbvm.com

Java: System.err.println("err")
来源：http://wet.nanxuanxn.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fli.zhongyouzk.top

Ruby: warn "err"
来源：http://lgo.bbcook.cn

C#:   Console.Error.WriteLine("err")
来源：http://tou.gaohongyu789.top

[M07] 判断是否为主入口
来源：http://jxb.hammf.cn

Py:   if __name__ == "__main__":
来源：http://lki.hnqzz.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wzk.jqgufenzy.top

JS:   require.main === module
来源：http://slu.sjlbkw.cn

TS:   require.main === module
来源：http://ahh.chenzaomai.com

Java: public static void main(String[] args)
来源：http://jmt.ehwqpu.com

Go:   func main()
来源：http://hnc.nanxinkj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ccs.dashuyun.cn

C#:   static void Main(string[] args)
来源：http://dhq.jianghu66.top

[M08] 获取系统与运行时信息
来源：http://mbu.yj20258.top

Py:   platform.system();  platform.python_version()
来源：http://cje.hammf.cn

PHP:  PHP_OS;  phpversion();
来源：http://xic.hnxiangtu.top

JS:   process.platform;  process.version
来源：http://dbw.shangyingyoupin.top

TS:   process.platform;  process.version
来源：http://pwp.guannengcc.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ert.quarkkingdee.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mnz.sufxvd.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kms.mhx1999.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tww.bjfxy.top

================================================================================
来源：http://haz.epnwcf.com

N. 数据结构与算法
来源：http://fvq.yj20258888.top

================================================================================
来源：http://orm.snrcjt.cn

[N01] 二分查找（有序数组）
来源：http://tbd.cheryme.top

Py:   bisect.bisect_left(arr, x)
来源：http://fef.jyoumei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jco.meibo888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fqh.gotoacloud.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eqa.aibaodan.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tln.aibaodan.cn

Go:   sort.SearchInts(arr, x)
来源：http://jby.nanxuanxn.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://bxo.jiagoushi.top

C#:   Array.BinarySearch(arr, x)
来源：http://ngf.yfazqb.com

[N02] 排序（工程实践用内置实现）
来源：http://abc.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://gbl.ydzc1.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xdq.nanxuanxn.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jen.zdbjq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wvx.fzhhl.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fhu.hcnkem.com

Go:   slices.Sort(arr)
来源：http://xke.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://aub.sjlbkw.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ina.hnqzz.top

[N03] 快速排序（分治示例）
来源：http://pek.hammf.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ejr.havefunace.top

PHP:  // 递归实现，或用 usort
来源：http://srl.chenzaomai.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ldu.ehwqpu.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zuo.andypj.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iun.hysaishi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ybz.gogol.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://azk.bbcook.cn

C#:   // 手写递归，或 Array.Sort
来源：http://asi.jinqigfzy.top

[N04] 斐波那契数列
来源：http://nsb.nanxinkj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wjy.zycfv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eiq.hnxiangtu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yxk.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sif.zhaomingkeji.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bbf.jqgfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ins.c1oappe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lxj.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rsv.yanxiufei.cn

[N05] 最大公约数
来源：http://gqc.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://wab.ehwqpu.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://smn.xziqi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://esc.cucudq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ueu.hywenlv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ueh.hcnkem.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yic.yangfankeji.com

Ruby: a.gcd(b)
来源：http://mng.yangfankeji.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mwu.haohaochexian.top

[N06] 判断回文字符串
来源：http://grc.ydzc1.top

Py:   s == s[::-1]
来源：http://wpt.ywan-chungtsiang.top

PHP:  $s === strrev($s);
来源：http://mpc.zhixingplan.top

JS:   s === [...s].reverse().join("")
来源：http://pyj.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://jve.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rxf.yonumen.top

Go:   // 双指针从两端比较
来源：http://oks.dashuyun.cn

Ruby: s == s.reverse
来源：http://rsj.yj20258.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mqd.shuidangran.top

[N07] 两数之和（返回下标）
来源：http://yry.xuetiantiany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nat.ybcxt.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kdr.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fvx.hcnkem.com

TS:   // 手写 Map<string, number>
来源：http://sbw.yuxming.cn

Java: // 手写 HashMap
来源：http://hdq.fengsongda.top

Go:   // 手写 map[int]int
来源：http://bss.zhoulong.xyz

Ruby: // 手写 Hash
来源：http://bnd.hysaishi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dlb.yvedp.cn

[N08] 生成全排列
来源：http://kkq.haohaochexian.top

Py:   itertools.permutations(arr)
来源：http://pcq.aibaodan.cn

PHP:  // 手写递归交换
来源：http://cnb.havefunace.top

JS:   // 手写回溯递归
来源：http://cbz.tarul.cn

TS:   // 手写回溯递归
来源：http://dmi.haohaochexian.top


<!-- 参考信息 -->