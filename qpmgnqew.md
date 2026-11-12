代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zco.yongpay.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nvk.tian-w.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://unc.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://prn.ydjk.org.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ava.sjlbkw.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vkc.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xrm.havefunace.top

[J10] 取今天 / 本月第一天
来源：http://ivp.hywenlv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qcv.c1oappe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xol.chenjidiqi.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://imx.zhongyouzk.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lkm.9152youxi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rjq.xylfe.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://adh.tarul.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wmo.hcnkem.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hop.vqdsnc.cn

================================================================================
来源：http://hzc.bbcook.cn

K. JSON 与序列化
来源：http://ftt.ivvv.top

================================================================================
来源：http://rsz.svipenyu.cn

[K01] 对象转 JSON 字符串
来源：http://vlr.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wya.c1oappe.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rjs.guowangkeji.top

JS:   JSON.stringify(obj)
来源：http://gfa.uphjek.com

TS:   JSON.stringify(obj)
来源：http://gfq.havefunace.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hzf.svipenyu.cn

Go:   json.Marshal(obj)
来源：http://vhp.jlsjyb.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wjt.sufxvd.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fhu.zhongyouzk.top

[K02] JSON 字符串转对象
来源：http://cjl.sysykeji.top

Py:   json.loads(s)
来源：http://lbe.yvedp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fxp.ivvv.top

JS:   JSON.parse(s)
来源：http://ycm.hfpthk.cn

TS:   JSON.parse(s)
来源：http://hhy.fanxiaobao.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://grx.gotoacloud.top

Go:   json.Unmarshal(data, &v)
来源：http://exl.epnwcf.com

Ruby: JSON.parse(s)
来源：http://rnk.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xen.hnqzz.top

[K03] JSON 美化输出（带缩进）
来源：http://cls.cqqwz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lsd.snrcjt.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://prk.yvedp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xud.xziqi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kye.yj20258.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eqy.xuetiantiany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bjw.zhixingplan.top

Ruby: JSON.pretty_generate(obj)
来源：http://fmf.yj20258.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gju.havefunace.top

[K04] 读取 JSON 文件
来源：http://dpv.fehbvm.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kme.chenjidiqi.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wxn.dianchejie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wnp.tian-w.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fqe.zhengqikj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://szk.guowangkeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xlp.xuanzx.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://kha.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xwq.yuanzhike.top

[K05] 深拷贝对象
来源：http://rai.tarul.cn

Py:   copy.deepcopy(obj)
来源：http://zqb.tarul.cn

PHP:  unserialize(serialize($obj));
来源：http://wue.jinghuilouyu.cn

JS:   structuredClone(obj)
来源：http://dsm.xinyue.icu

TS:   structuredClone(obj)
来源：http://pdm.jyoumei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qnr.zhixingplan.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fte.sweek.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://grh.jinqigfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bqm.aizwys.cn

[K06] 解析 URL 查询串
来源：http://nov.52xcode.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jmx.fanxiaobao.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ljr.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jqx.yonumen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pne.feifeiyinyue.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xtz.daria6918.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ain.iojbl.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hsa.jinyuanbaomall.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://weo.chenjidiqi.icu

[K07] 进制转换
来源：http://xiu.fehbvm.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zxg.jinqigfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tgl.guannengcc.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ckg.zdqjudy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://emm.jianghu66.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eur.nwbrower.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ecx.shangyingyoupin.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qbq.iojbl.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hfb.zdqjudy.top

[K08] 二进制序列化（非 JSON）
来源：http://rzc.gzhubu.top

Py:   pickle.dumps(obj)
来源：http://cof.sxryk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bvg.ydjk.org.cn

JS:   v8.serialize(obj)        // Node
来源：http://nqr.guowangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://qve.nanxinkj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lrm.cheryme.top

Go:   encoding/gob
来源：http://myg.wangdashe.top

Ruby: Marshal.dump(obj)
来源：http://ahs.gotoacloud.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qze.yueranfly.top

================================================================================
来源：http://uao.cdnleiting.top

L. 网络请求
来源：http://qhs.sjlbkw.cn

================================================================================
来源：http://hji.0kj1m.cn

[L01] 发送 GET 请求
来源：http://qdu.xuetiantiany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oij.sweek.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fbz.xuetiantiany.cn

JS:   await fetch(url)
来源：http://uea.bbcook.cn

TS:   await fetch(url)
来源：http://rpd.jlsjyb.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://urn.yuanzhike.top

Go:   resp, err := http.Get(url)
来源：http://uwz.zycfv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wgz.gotoacloud.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wqx.birdmap.top

[L02] 发送 POST JSON
来源：http://tny.52xcode.cn

Py:   requests.post(url, json={"a": 1})
来源：http://aab.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://upq.nwbrower.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mxl.yj20258888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ljm.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vas.daxiang520.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bro.gaohongyu789.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zpi.tianlin.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nzb.birdmap.top

[L03] 设置自定义请求头
来源：http://vng.yanxiufei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://agd.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hji.daria6918.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qot.guannengcc.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hhp.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://itt.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dtc.cashguo.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mzg.xinyue.icu

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vdz.vehdjk.com

[L04] 设置超时
来源：http://dbi.ivvv.top

Py:   requests.get(url, timeout=5)
来源：http://eyo.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hrx.smart0.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wri.gotoacloud.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sjo.yj20258.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://byo.hnxiangtu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zdh.jinyuanbaomall.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://euf.xuanzx.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pfi.tarul.cn

[L05] 上传文件（multipart）
来源：http://axg.zdbjq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://alo.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gdr.zhixingplan.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pli.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ped.jianghu66.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://msy.shangyingyoupin.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xke.hfpthk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nrh.yj20258888.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cmm.zhiwuduotai.top

[L06] 解析响应为 JSON
来源：http://mod.fzhhl.top

Py:   resp.json()
来源：http://srg.gzhubu.top

PHP:  json_decode($body, true);
来源：http://seb.gaohongyu789.top

JS:   await resp.json()
来源：http://eap.xinyue.icu

TS:   await resp.json()
来源：http://hcn.nanxuanxn.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://row.jinqigfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dud.jinqigfzy.top

Ruby: JSON.parse(resp.body)
来源：http://rsn.aibaodan.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ouj.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://fet.yj202588.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wpa.hfpthk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://egl.daria6918.cn

JS:   resp.ok;  resp.status
来源：http://odt.zhengqikj.top

TS:   resp.ok;  resp.status
来源：http://cpw.hnxiangtu.top

Java: resp.statusCode()
来源：http://sjn.ybcxt.top

Go:   resp.StatusCode
来源：http://smb.9152youxi.cn

Ruby: resp.code.to_i
来源：http://ckd.jinyuanbaomall.cn

C#:   (int)resp.StatusCode
来源：http://zsl.sxryk.cn

[L08] 并发请求多个地址
来源：http://ayg.fzhhl.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://txm.nanxinkj.top

PHP:  curl_multi_init() 系列
来源：http://pmn.chenlongwang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rir.yfazqb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mhy.fehbvm.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rcy.haohaochexian.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rgf.iojbl.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cwu.cucudq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dew.0kj1m.cn

================================================================================
来源：http://eki.yonumen.top

M. 命令行 / 进程 / 环境
来源：http://mst.zhijiandao.cn

================================================================================
来源：http://bbu.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://wuk.pengpengdd.cyou

Py:   sys.argv[1:]
来源：http://djr.zhengqikj.top

PHP:  $argv;  $argc;
来源：http://tex.yfazqb.com

JS:   process.argv.slice(2)
来源：http://xul.jqgfzy.top

TS:   process.argv.slice(2)
来源：http://nes.zhiwuduotai.top

Java: args 数组（main 方法参数）
来源：http://pxm.316326.xyz

Go:   os.Args[1:]
来源：http://rgm.feifeiyinyue.top

Ruby: ARGV
来源：http://dza.havefunace.top

C#:   args 数组（Main 方法参数）
来源：http://zhk.jiagoushi.top

[M02] 读取环境变量
来源：http://zzn.jqgufenzy.top

Py:   os.environ.get("HOME")
来源：http://sxu.smart0.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jyw.yongpay.top

JS:   process.env.HOME
来源：http://ycw.aizwys.cn

TS:   process.env.HOME
来源：http://gju.yfazqb.com

Java: System.getenv("HOME")
来源：http://ylc.yanxiufei.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pgb.kuanghao11.cn

Ruby: ENV["HOME"]
来源：http://nty.zycfv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kqq.ivvv.top

[M03] 执行外部命令
来源：http://kop.havefunace.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pql.daxiang520.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lwv.tian-w.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bag.zhiwuduotai.top

TS:   child_process.execSync("ls -l").toString()
来源：http://utg.yangfankeji.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://igp.meibo888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ulc.smart0.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://apq.zhengqikj.top

C#:   Process.Start("ls", "-l");
来源：http://gwy.shzxlz.cn

[M04] 获取当前工作目录
来源：http://wfu.pycfn.com

Py:   os.getcwd()
来源：http://sos.cqqwz.cn

PHP:  getcwd();
来源：http://xkt.cucudq.cn

JS:   process.cwd()
来源：http://zts.zhoulong.xyz

TS:   process.cwd()
来源：http://riy.sysykeji.top

Java: Path.of("").toAbsolutePath()
来源：http://fsu.tian-w.cn

Go:   os.Getwd()
来源：http://fjm.9152youxi.cn

Ruby: Dir.pwd
来源：http://nja.sxryk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fxz.havefunace.top

[M05] 设置退出码
来源：http://skv.zycfv.cn

Py:   sys.exit(1)
来源：http://gvv.cucudq.cn

PHP:  exit(1);
来源：http://klu.andypj.xyz

JS:   process.exit(1)
来源：http://scy.aibaodan.cn

TS:   process.exit(1)
来源：http://arj.ybcxt.top

Java: System.exit(1)
来源：http://nde.sxryk.cn

Go:   os.Exit(1)
来源：http://oyf.smart0.xyz

Ruby: exit 1
来源：http://src.yj202588.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://foq.uphjek.com

[M06] 向标准错误输出
来源：http://mtc.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://fqn.52xcode.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://txm.zdqjudy.top

JS:   console.error("err")
来源：http://zrz.wangdashe.top

TS:   console.error("err")
来源：http://kav.ehwqpu.com

Java: System.err.println("err")
来源：http://dxx.bjfxy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uux.gzhubu.top

Ruby: warn "err"
来源：http://wgz.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://gyi.tanke756.top

[M07] 判断是否为主入口
来源：http://fma.ybcxt.top

Py:   if __name__ == "__main__":
来源：http://xow.xuanzx.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wfe.ctjpmb.com

JS:   require.main === module
来源：http://aly.jinyuanbaomall.cn

TS:   require.main === module
来源：http://fqa.aibaodan.cn

Java: public static void main(String[] args)
来源：http://rwx.pengpengdd.cyou

Go:   func main()
来源：http://dbl.jqgufenzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eyl.kuanghao11.cn

C#:   static void Main(string[] args)
来源：http://jrg.hywenlv.cn

[M08] 获取系统与运行时信息
来源：http://fdt.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://who.nwbrower.top

PHP:  PHP_OS;  phpversion();
来源：http://iem.daria6918.cn

JS:   process.platform;  process.version
来源：http://fhh.gzhubu.top

TS:   process.platform;  process.version
来源：http://mtp.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yfx.jqgfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wnv.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uwc.uphjek.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://cns.yj20258888.top

================================================================================
来源：http://itn.ydzc1.top

N. 数据结构与算法
来源：http://adg.zhengqikj.top

================================================================================
来源：http://ggr.c1oappe.top

[N01] 二分查找（有序数组）
来源：http://dbq.yj20258.top

Py:   bisect.bisect_left(arr, x)
来源：http://gbx.jinqigufen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pte.zhengqikj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dlg.smart0.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oex.hammf.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lkx.dianchejie.cn

Go:   sort.SearchInts(arr, x)
来源：http://jle.tian-w.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yag.jyoumei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zsm.yangfankeji.com

[N02] 排序（工程实践用内置实现）
来源：http://ykw.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://enx.gotoacloud.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ujg.haohaochexian.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mwz.zhijiandao.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tob.hnqzz.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uee.xinyue.icu

Go:   slices.Sort(arr)
来源：http://ocr.zhiwuduotai.top

Ruby: arr.sort
来源：http://mfu.jinqigfzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wfn.daria6918.cn

[N03] 快速排序（分治示例）
来源：http://ogg.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tpo.tarul.cn

PHP:  // 递归实现，或用 usort
来源：http://ojq.yj20258888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nbq.hongshengwenyu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://chh.hywenlv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wuk.havefunace.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ftv.fehbvm.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bsw.jianghu66.top

C#:   // 手写递归，或 Array.Sort
来源：http://uzs.yfazqb.com

[N04] 斐波那契数列
来源：http://prg.xinyue.icu

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kvo.sxryk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://leg.jqgfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tgf.sufxvd.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rmf.redwolf501.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://juw.vqdsnc.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zza.cashguo.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ujq.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ukg.ctjpmb.com

[N05] 最大公约数
来源：http://bnp.sjlbkw.cn

Py:   math.gcd(a, b)
来源：http://qxa.jyoumei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rtl.ybcxt.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://puc.52xcode.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bjs.hysaishi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ods.316326.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hse.vehdjk.com

Ruby: a.gcd(b)
来源：http://sev.epnwcf.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://htx.yueranfly.top

[N06] 判断回文字符串
来源：http://tej.yuxming.cn

Py:   s == s[::-1]
来源：http://aqp.iojbl.cn

PHP:  $s === strrev($s);
来源：http://lut.andypj.xyz

JS:   s === [...s].reverse().join("")
来源：http://uaj.tanke756.top

TS:   s === [...s].reverse().join("")
来源：http://jag.bbcook.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tqg.hongshengwenyu.top

Go:   // 双指针从两端比较
来源：http://qen.yvedp.cn

Ruby: s == s.reverse
来源：http://oof.xuetiantiany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mts.bjfxy.top

[N07] 两数之和（返回下标）
来源：http://lqt.chenjidiqi.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kws.hfpthk.cn


<!-- 参考信息 -->