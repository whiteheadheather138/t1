代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ykr.svipenyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://utz.andypj.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gjn.gotoacloud.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pxt.svipenyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://win.yj202588.top

Ruby: Time.now.getlocal("+08:00")
来源：http://yho.quarkkingdee.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hxs.zhoulong.xyz

[J10] 取今天 / 本月第一天
来源：http://zlq.uphjek.com

Py:   date.today();  date.today().replace(day=1)
来源：http://jbn.quarkkingdee.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hto.nanxuanxn.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bxm.ehwqpu.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gst.hnxiangtu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://knk.nanxuanxn.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kak.yanxiufei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lsi.feifeiyinyue.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ree.chenzaomai.com

================================================================================
来源：http://uij.ydjk.org.cn

K. JSON 与序列化
来源：http://fwo.hfpthk.cn

================================================================================
来源：http://abu.jiagoushi.top

[K01] 对象转 JSON 字符串
来源：http://nbc.52xcode.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ata.vqdsnc.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://chx.sxryk.cn

JS:   JSON.stringify(obj)
来源：http://nkh.aibaodan.cn

TS:   JSON.stringify(obj)
来源：http://pan.pycfn.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mla.kuanghao11.cn

Go:   json.Marshal(obj)
来源：http://tkm.shzxlz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kxs.yj202588.top

C#:   JsonSerializer.Serialize(obj)
来源：http://iok.daria6918.cn

[K02] JSON 字符串转对象
来源：http://sto.fktsv.cn

Py:   json.loads(s)
来源：http://hpn.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ljg.tian-w.cn

JS:   JSON.parse(s)
来源：http://ika.quarkkingdee.top

TS:   JSON.parse(s)
来源：http://ayx.9152youxi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dsn.xziqi.cn

Go:   json.Unmarshal(data, &v)
来源：http://mpf.zhixingplan.top

Ruby: JSON.parse(s)
来源：http://nak.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gwl.hysaishi.cn

[K03] JSON 美化输出（带缩进）
来源：http://hzz.meibo888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://izh.xuanzx.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cqu.ywan-chungtsiang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tfj.shangyingyoupin.top

TS:   JSON.stringify(obj, null, 2)
来源：http://pot.tanke756.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vdz.yj202588.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wjw.zycfv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gzj.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mcc.yueranfly.top

[K04] 读取 JSON 文件
来源：http://crz.zhijiandao.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hul.hnqzz.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://grx.xylfe.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://who.ywan-chungtsiang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hnt.aibaodan.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ttp.cqqwz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cmn.yvedp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zyl.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dej.ydzc1.top

[K05] 深拷贝对象
来源：http://yeb.tianlin.xyz

Py:   copy.deepcopy(obj)
来源：http://qho.fktsv.cn

PHP:  unserialize(serialize($obj));
来源：http://exg.hfpthk.cn

JS:   structuredClone(obj)
来源：http://sqx.vqdsnc.cn

TS:   structuredClone(obj)
来源：http://svs.zycfv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yzg.guowangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gsj.cashguo.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ush.chenlongwang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rcz.guowangkeji.top

[K06] 解析 URL 查询串
来源：http://lnd.andypj.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wux.hammf.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ryh.xylfe.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lgn.gaohongyu789.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://efi.zhoulong.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://btl.daxiang520.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zfm.hammf.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yhk.yfazqb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yop.shangyingyoupin.top

[K07] 进制转换
来源：http://jsj.hysaishi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fhf.jinqigufen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sta.fzhhl.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mpf.zhongyouzk.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wvu.xziqi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hbt.ivvv.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nxc.cheryme.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dyw.pengpengdd.cyou

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xxd.uphjek.com

[K08] 二进制序列化（非 JSON）
来源：http://sjn.feifeiyinyue.top

Py:   pickle.dumps(obj)
来源：http://twq.ydzc1.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hms.yonumen.top

JS:   v8.serialize(obj)        // Node
来源：http://rzr.zhoulong.xyz

TS:   v8.serialize(obj)        // Node
来源：http://ekx.daxiang520.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jve.hesvh.cn

Go:   encoding/gob
来源：http://xol.yanxiufei.cn

Ruby: Marshal.dump(obj)
来源：http://gku.tian-w.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zky.chenlongwang.top

================================================================================
来源：http://dcs.jyoumei.cn

L. 网络请求
来源：http://cwl.uphjek.com

================================================================================
来源：http://ppb.yvedp.cn

[L01] 发送 GET 请求
来源：http://dki.gzhubu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oen.hammf.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oli.jinghuilouyu.cn

JS:   await fetch(url)
来源：http://ocl.kuanghao11.cn

TS:   await fetch(url)
来源：http://djl.jinyuanbaomall.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://agr.ybcxt.top

Go:   resp, err := http.Get(url)
来源：http://uek.tarul.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://swo.vqdsnc.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ruu.shzxlz.cn

[L02] 发送 POST JSON
来源：http://ycu.yvedp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xkf.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eqx.yanxiufei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://idr.gotoacloud.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fmr.hammf.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fzx.xylfe.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://osd.snrcjt.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://klz.bbcook.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ygk.smart0.xyz

[L03] 设置自定义请求头
来源：http://hrd.ydzc1.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kao.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nxz.sweek.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qci.316326.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aje.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rfz.bbcook.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zob.yuanzhike.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xti.0kj1m.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ahg.xingfuxueyuan.xyz

[L04] 设置超时
来源：http://gzd.nanxinkj.top

Py:   requests.get(url, timeout=5)
来源：http://spg.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wmk.birdmap.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://noz.jlsjyb.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qeb.fktsv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xwf.gogol.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://elz.jlsjyb.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mon.tanke756.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://asv.shuidangran.top

[L05] 上传文件（multipart）
来源：http://mod.nanxinkj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://orb.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zbj.andypj.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cja.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lnv.vehdjk.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://whk.aibaodan.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tbu.shuidangran.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fdf.c1oappe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wqy.tian-w.cn

[L06] 解析响应为 JSON
来源：http://qto.hnxiangtu.top

Py:   resp.json()
来源：http://nqx.zdqjudy.top

PHP:  json_decode($body, true);
来源：http://mvc.xuetiantiany.cn

JS:   await resp.json()
来源：http://cuj.bbcook.cn

TS:   await resp.json()
来源：http://nwp.yj20258888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gpn.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://srz.smart0.xyz

Ruby: JSON.parse(resp.body)
来源：http://nqk.sxryk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://aqp.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://srw.guowangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ses.ivvv.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pyt.c1oappe.top

JS:   resp.ok;  resp.status
来源：http://ble.ydzc1.top

TS:   resp.ok;  resp.status
来源：http://fxb.sysykeji.top

Java: resp.statusCode()
来源：http://ort.meibo888.top

Go:   resp.StatusCode
来源：http://dpk.redwolf501.top

Ruby: resp.code.to_i
来源：http://goj.guowangkeji.top

C#:   (int)resp.StatusCode
来源：http://jhj.jinqigfzy.top

[L08] 并发请求多个地址
来源：http://ijb.smart0.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ney.xziqi.cn

PHP:  curl_multi_init() 系列
来源：http://rwv.bbcook.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bbv.uphjek.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jtp.nanxuanxn.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://riq.cqqwz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fjw.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qug.c1oappe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oxr.yfazqb.com

================================================================================
来源：http://bob.wangdashe.top

M. 命令行 / 进程 / 环境
来源：http://zvg.cdnleiting.top

================================================================================
来源：http://wzu.yuxming.cn

[M01] 读取命令行参数
来源：http://ala.yj202588.top

Py:   sys.argv[1:]
来源：http://wwt.zhaomingkeji.xyz

PHP:  $argv;  $argc;
来源：http://bql.guannengcc.top

JS:   process.argv.slice(2)
来源：http://jen.9152youxi.cn

TS:   process.argv.slice(2)
来源：http://tzx.yanxiufei.cn

Java: args 数组（main 方法参数）
来源：http://ieb.bbcook.cn

Go:   os.Args[1:]
来源：http://hve.sufxvd.cn

Ruby: ARGV
来源：http://zcs.nwbrower.top

C#:   args 数组（Main 方法参数）
来源：http://nxs.yangfankeji.com

[M02] 读取环境变量
来源：http://ykb.chenzaomai.com

Py:   os.environ.get("HOME")
来源：http://sxv.zhijiandao.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mzm.yvedp.cn

JS:   process.env.HOME
来源：http://ztb.kuanghao11.cn

TS:   process.env.HOME
来源：http://uhf.jqgufenzy.top

Java: System.getenv("HOME")
来源：http://tby.hongshengwenyu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://frj.cqqwz.cn

Ruby: ENV["HOME"]
来源：http://vld.zdbjq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mut.gotoacloud.top

[M03] 执行外部命令
来源：http://vyg.zhixingplan.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://btx.yongpay.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mys.yj202588.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zrw.mhx1999.top

TS:   child_process.execSync("ls -l").toString()
来源：http://htw.iojbl.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bed.hfpthk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zsu.jianghu66.top

Ruby: system("ls -l");  `ls -l`
来源：http://fql.sweek.top

C#:   Process.Start("ls", "-l");
来源：http://vim.daria6918.cn

[M04] 获取当前工作目录
来源：http://ozb.jinghuilouyu.cn

Py:   os.getcwd()
来源：http://vzk.fzhhl.top

PHP:  getcwd();
来源：http://jyq.haohaochexian.top

JS:   process.cwd()
来源：http://jlc.tarul.cn

TS:   process.cwd()
来源：http://hcs.bjfxy.top

Java: Path.of("").toAbsolutePath()
来源：http://vwz.shanyushiyangkeji.top

Go:   os.Getwd()
来源：http://cqg.yonumen.top

Ruby: Dir.pwd
来源：http://csa.cucudq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dci.nwbrower.top

[M05] 设置退出码
来源：http://vsq.xinyue.icu

Py:   sys.exit(1)
来源：http://osz.chenzaomai.com

PHP:  exit(1);
来源：http://upg.chenzaomai.com

JS:   process.exit(1)
来源：http://kod.dashuyun.cn

TS:   process.exit(1)
来源：http://fht.ehwqpu.com

Java: System.exit(1)
来源：http://erp.feifeiyinyue.top

Go:   os.Exit(1)
来源：http://shq.andypj.xyz

Ruby: exit 1
来源：http://ole.tian-w.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ldj.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://lrr.uphjek.com

Py:   print("err", file=sys.stderr)
来源：http://qlg.fktsv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zxd.fehbvm.com

JS:   console.error("err")
来源：http://mvv.nanxuanxn.top

TS:   console.error("err")
来源：http://gpf.52xcode.cn

Java: System.err.println("err")
来源：http://blt.0kj1m.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uts.aibaodan.cn

Ruby: warn "err"
来源：http://xqh.gaohongyu789.top

C#:   Console.Error.WriteLine("err")
来源：http://tjp.tianlin.xyz

[M07] 判断是否为主入口
来源：http://wby.yj202588.top

Py:   if __name__ == "__main__":
来源：http://ama.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fld.xuanzx.com

JS:   require.main === module
来源：http://zhm.xuanzx.com

TS:   require.main === module
来源：http://elu.aibaodan.cn

Java: public static void main(String[] args)
来源：http://mtb.yuanzhike.top

Go:   func main()
来源：http://fye.yuanzhike.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://afw.nwbrower.top

C#:   static void Main(string[] args)
来源：http://feq.yonumen.top

[M08] 获取系统与运行时信息
来源：http://ylc.zhixingplan.top

Py:   platform.system();  platform.python_version()
来源：http://ahs.yj20258.top

PHP:  PHP_OS;  phpversion();
来源：http://urr.hysaishi.cn

JS:   process.platform;  process.version
来源：http://uby.vqdsnc.cn

TS:   process.platform;  process.version
来源：http://ibi.nanxinkj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ukn.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wkm.daria6918.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mfg.hammf.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ucp.fzhhl.top

================================================================================
来源：http://lkr.ydjk.org.cn

N. 数据结构与算法
来源：http://kzp.gaohongyu789.top

================================================================================
来源：http://ytu.jlsjyb.cn

[N01] 二分查找（有序数组）
来源：http://vot.iojbl.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ebb.aibaodan.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fay.snrcjt.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oyb.kuanghao11.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ujz.hysaishi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://idm.zdbjq.cn

Go:   sort.SearchInts(arr, x)
来源：http://vpk.jinqigufen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://bed.52xcode.cn

C#:   Array.BinarySearch(arr, x)
来源：http://njf.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://pib.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://iiq.0kj1m.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bxv.chenlongwang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://det.gotoacloud.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://duj.shuidangran.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jbq.cheryme.top

Go:   slices.Sort(arr)
来源：http://dov.xuanzx.com

Ruby: arr.sort
来源：http://dvc.gogol.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dzy.cashguo.top

[N03] 快速排序（分治示例）
来源：http://aby.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yri.cdnleiting.top

PHP:  // 递归实现，或用 usort
来源：http://izw.jqgfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hqh.yj20258888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fwn.jianghu66.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://div.yj20258.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wng.shanyushiyangtech.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jeh.iojbl.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jdo.cheryme.top

[N04] 斐波那契数列
来源：http://vrg.jlsjyb.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tsf.jinqigfzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tuy.yanxiufei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ple.vehdjk.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hjz.bbcook.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rzq.9152youxi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://slo.hongshengwenyu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eto.shangyingyoupin.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jem.meibo888.top

[N05] 最大公约数
来源：http://zmq.gogol.net.cn

Py:   math.gcd(a, b)
来源：http://qed.gaohongyu789.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qpq.jinghuilouyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pyc.316326.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lvj.nwbrower.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lqu.ybcxt.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://elf.jianghu66.top

Ruby: a.gcd(b)
来源：http://cap.nanxuanxn.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mvk.xylfe.cn

[N06] 判断回文字符串
来源：http://bfe.chenlongwang.top

Py:   s == s[::-1]
来源：http://ikg.tanke756.top

PHP:  $s === strrev($s);
来源：http://lnu.tian-w.cn

JS:   s === [...s].reverse().join("")
来源：http://dta.yj20258.top

TS:   s === [...s].reverse().join("")
来源：http://fsq.mhx1999.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mwc.sysykeji.top

Go:   // 双指针从两端比较
来源：http://ggm.yuxming.cn

Ruby: s == s.reverse
来源：http://zzk.316326.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://fax.316326.xyz

[N07] 两数之和（返回下标）
来源：http://gla.52xcode.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gwm.vqdsnc.cn


<!-- 参考信息 -->