代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ejo.nanxinkj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ioi.jinghuilouyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://djf.hcnkem.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gbk.xylfe.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kyf.xingfuxueyuan.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://mzl.nwbrower.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://unk.jqgufenzy.top

[J10] 取今天 / 本月第一天
来源：http://muz.havefunace.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bto.shzxlz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bsh.cucudq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wim.wangdashe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nyg.mhx1999.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uff.52xcode.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qab.sufxvd.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://adw.nwbrower.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rwp.epnwcf.com

================================================================================
来源：http://bdi.haohaochexian.top

K. JSON 与序列化
来源：http://poz.zhaomingkeji.xyz

================================================================================
来源：http://mxp.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://egr.meibo888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://emg.svipenyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xue.jiagoushi.top

JS:   JSON.stringify(obj)
来源：http://uyi.jinghuilouyu.cn

TS:   JSON.stringify(obj)
来源：http://kfm.hesvh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fwe.sxryk.cn

Go:   json.Marshal(obj)
来源：http://hqo.yj202588.top

Ruby: obj.to_json                                     // require "json"
来源：http://itp.cucudq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nrb.jlsjyb.cn

[K02] JSON 字符串转对象
来源：http://dya.tian-w.cn

Py:   json.loads(s)
来源：http://jgl.zhaomingkeji.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dky.c1oappe.top

JS:   JSON.parse(s)
来源：http://gny.zhiwuduotai.top

TS:   JSON.parse(s)
来源：http://qup.shangyingyoupin.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fys.fehbvm.com

Go:   json.Unmarshal(data, &v)
来源：http://kue.jinqigfzy.top

Ruby: JSON.parse(s)
来源：http://iul.jqgufenzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kvl.ctjpmb.com

[K03] JSON 美化输出（带缩进）
来源：http://nvb.chenjidiqi.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vyu.mhx1999.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tvp.chenzaomai.com

JS:   JSON.stringify(obj, null, 2)
来源：http://wkb.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bio.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ifh.ywan-chungtsiang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oin.ydjk.org.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ngu.haohaochexian.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yij.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://tbw.guowangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xex.sweek.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wbc.fanxiaobao.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yjt.guowangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xsj.yonumen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hie.316326.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oiz.cheryme.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wnp.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qpc.ydjk.org.cn

[K05] 深拷贝对象
来源：http://jry.andypj.xyz

Py:   copy.deepcopy(obj)
来源：http://ton.xuetiantiany.cn

PHP:  unserialize(serialize($obj));
来源：http://prq.9152youxi.cn

JS:   structuredClone(obj)
来源：http://jbj.yj20258888.top

TS:   structuredClone(obj)
来源：http://nvd.gzhubu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dlk.ybcxt.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hws.guowangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ogg.fehbvm.com

C#:   // 序列化往返，或自定义 Clone
来源：http://iil.zhaomingkeji.xyz

[K06] 解析 URL 查询串
来源：http://bxg.yuanzhike.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ewy.jinyuanbaomall.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vjd.daria6918.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ani.fanxiaobao.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tzk.chenlongwang.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ixf.cashguo.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wiw.hesvh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://frc.vqdsnc.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fam.birdmap.top

[K07] 进制转换
来源：http://gga.shanyushiyangtech.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://chm.cucudq.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hqk.feifeiyinyue.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wxz.quarkkingdee.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://caa.ybcxt.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tky.zdqjudy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://luw.yuanzhike.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cbi.0kj1m.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vjz.hongshengwenyu.top

[K08] 二进制序列化（非 JSON）
来源：http://bqt.ehwqpu.com

Py:   pickle.dumps(obj)
来源：http://foy.daria6918.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://igu.hnxiangtu.top

JS:   v8.serialize(obj)        // Node
来源：http://gil.redwolf501.top

TS:   v8.serialize(obj)        // Node
来源：http://koz.vehdjk.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gfv.smart0.xyz

Go:   encoding/gob
来源：http://xwj.9152youxi.cn

Ruby: Marshal.dump(obj)
来源：http://pdf.shzxlz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mzs.pengpengdd.cyou

================================================================================
来源：http://qtu.gogol.net.cn

L. 网络请求
来源：http://yum.tianlin.xyz

================================================================================
来源：http://mgd.nanxuanxn.top

[L01] 发送 GET 请求
来源：http://ybz.shangyingyoupin.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ghp.ybcxt.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ncu.zhijiandao.cn

JS:   await fetch(url)
来源：http://ftw.hnqzz.top

TS:   await fetch(url)
来源：http://bat.yj20258888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hxh.zdbjq.cn

Go:   resp, err := http.Get(url)
来源：http://ttf.yanxiufei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bpm.birdmap.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ujj.bbcook.cn

[L02] 发送 POST JSON
来源：http://ykv.hesvh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hqr.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cwo.yanxiufei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rsl.jqgfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uwa.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yib.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://obo.9152youxi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://upp.quarkkingdee.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fbj.iojbl.cn

[L03] 设置自定义请求头
来源：http://ihb.gogol.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://keu.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dno.zhijiandao.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mne.yj20258888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cem.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kzr.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bkb.gzhubu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://acl.dashuyun.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://txc.tanke756.top

[L04] 设置超时
来源：http://fpf.ehwqpu.com

Py:   requests.get(url, timeout=5)
来源：http://tku.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ouh.pengpengdd.cyou

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wom.andypj.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qxt.ppjwa.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bus.vqdsnc.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zfj.bjfxy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tvn.zhaomingkeji.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nkf.jlsjyb.cn

[L05] 上传文件（multipart）
来源：http://nva.cucudq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bgk.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pwk.shanyushiyangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ofj.tian-w.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tru.smart0.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qtr.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gna.nanxinkj.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://djy.gogol.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cfx.yvedp.cn

[L06] 解析响应为 JSON
来源：http://mde.pycfn.com

Py:   resp.json()
来源：http://kno.snrcjt.cn

PHP:  json_decode($body, true);
来源：http://lrz.snrcjt.cn

JS:   await resp.json()
来源：http://tzz.zhongyouzk.top

TS:   await resp.json()
来源：http://gqp.jinghuilouyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kng.316326.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lpr.cdnleiting.top

Ruby: JSON.parse(resp.body)
来源：http://fff.kuanghao11.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wpf.snrcjt.cn

[L07] 处理 HTTP 状态码
来源：http://vpv.cqqwz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fwy.hcnkem.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aad.ywan-chungtsiang.top

JS:   resp.ok;  resp.status
来源：http://dhu.zhoulong.xyz

TS:   resp.ok;  resp.status
来源：http://mso.zhongyouzk.top

Java: resp.statusCode()
来源：http://twg.zhengqikj.top

Go:   resp.StatusCode
来源：http://fmv.daxiang520.top

Ruby: resp.code.to_i
来源：http://cmy.316326.xyz

C#:   (int)resp.StatusCode
来源：http://wmu.yangfankeji.com

[L08] 并发请求多个地址
来源：http://gne.shanyushiyangtech.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sfx.sweek.top

PHP:  curl_multi_init() 系列
来源：http://fmf.shzxlz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pon.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://but.ivvv.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://duh.ivvv.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zoi.shzxlz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gky.sysykeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lct.gzhubu.top

================================================================================
来源：http://xsa.guowangkeji.top

M. 命令行 / 进程 / 环境
来源：http://nav.shanyushiyangtech.top

================================================================================
来源：http://ula.shanyushiyangkeji.top

[M01] 读取命令行参数
来源：http://rpy.iojbl.cn

Py:   sys.argv[1:]
来源：http://neu.iojbl.cn

PHP:  $argv;  $argc;
来源：http://quw.yanxiufei.cn

JS:   process.argv.slice(2)
来源：http://xxi.zhijiandao.cn

TS:   process.argv.slice(2)
来源：http://nud.fengsongda.top

Java: args 数组（main 方法参数）
来源：http://bdv.shzxlz.cn

Go:   os.Args[1:]
来源：http://rkx.yfazqb.com

Ruby: ARGV
来源：http://kvt.hcnkem.com

C#:   args 数组（Main 方法参数）
来源：http://vwp.shanyushiyangkeji.top

[M02] 读取环境变量
来源：http://hsj.xingfuxueyuan.xyz

Py:   os.environ.get("HOME")
来源：http://tko.xziqi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dqi.ybcxt.top

JS:   process.env.HOME
来源：http://lvd.c1oappe.top

TS:   process.env.HOME
来源：http://hrn.zdbjq.cn

Java: System.getenv("HOME")
来源：http://src.jinghuilouyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sdq.tianlin.xyz

Ruby: ENV["HOME"]
来源：http://cpi.fktsv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oiu.fktsv.cn

[M03] 执行外部命令
来源：http://pnb.sweek.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vrb.pengpengdd.cyou

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://snb.wangshuangyany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jkv.hfpthk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dnr.hywenlv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wkg.andypj.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://wag.ppjwa.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dhc.pengpengdd.cyou

C#:   Process.Start("ls", "-l");
来源：http://rpj.tianlin.xyz

[M04] 获取当前工作目录
来源：http://fqp.quarkkingdee.top

Py:   os.getcwd()
来源：http://myk.chenlongwang.top

PHP:  getcwd();
来源：http://hvq.zhijiandao.cn

JS:   process.cwd()
来源：http://yxc.yvedp.cn

TS:   process.cwd()
来源：http://dce.chenjidiqi.icu

Java: Path.of("").toAbsolutePath()
来源：http://wdr.yj20258888.top

Go:   os.Getwd()
来源：http://ges.xziqi.cn

Ruby: Dir.pwd
来源：http://kia.ydjk.org.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jcs.hfpthk.cn

[M05] 设置退出码
来源：http://nnu.hcnkem.com

Py:   sys.exit(1)
来源：http://cii.yueranfly.top

PHP:  exit(1);
来源：http://nbn.fzhhl.top

JS:   process.exit(1)
来源：http://aew.yonumen.top

TS:   process.exit(1)
来源：http://lkg.ctjpmb.com

Java: System.exit(1)
来源：http://ffd.sysykeji.top

Go:   os.Exit(1)
来源：http://hff.snrcjt.cn

Ruby: exit 1
来源：http://aym.aibaodan.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wlr.wangdashe.top

[M06] 向标准错误输出
来源：http://dpr.dashuyun.cn

Py:   print("err", file=sys.stderr)
来源：http://wzi.hnxiangtu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://jcv.ybcxt.top

JS:   console.error("err")
来源：http://fix.haohaochexian.top

TS:   console.error("err")
来源：http://vlf.yuxming.cn

Java: System.err.println("err")
来源：http://xsx.hnxiangtu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kju.9152youxi.cn

Ruby: warn "err"
来源：http://xpe.cucudq.cn

C#:   Console.Error.WriteLine("err")
来源：http://axi.yvedp.cn

[M07] 判断是否为主入口
来源：http://ryb.sjlbkw.cn

Py:   if __name__ == "__main__":
来源：http://spl.jqgfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wfn.chenzaomai.com

JS:   require.main === module
来源：http://iwd.pengpengdd.cyou

TS:   require.main === module
来源：http://gjz.chenjidiqi.icu

Java: public static void main(String[] args)
来源：http://kls.epnwcf.com

Go:   func main()
来源：http://yhm.ctjpmb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hln.xuanzx.com

C#:   static void Main(string[] args)
来源：http://ztu.c1oappe.top

[M08] 获取系统与运行时信息
来源：http://ywl.tarul.cn

Py:   platform.system();  platform.python_version()
来源：http://qlu.havefunace.top

PHP:  PHP_OS;  phpversion();
来源：http://coc.jinyuanbaomall.cn

JS:   process.platform;  process.version
来源：http://dzf.tarul.cn

TS:   process.platform;  process.version
来源：http://xmb.xziqi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cuj.wangshuangyany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kdg.mhx1999.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://auq.jianghu66.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tha.guowangkeji.top

================================================================================
来源：http://dxn.jianghu66.top

N. 数据结构与算法
来源：http://hrf.birdmap.top

================================================================================
来源：http://fwg.yanxiufei.cn

[N01] 二分查找（有序数组）
来源：http://oil.dianchejie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://brc.jinqigfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ebn.hfpthk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nmh.vqdsnc.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nds.kuanghao11.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fyl.birdmap.top

Go:   sort.SearchInts(arr, x)
来源：http://zsn.chenlongwang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vai.fanxiaobao.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://npq.zycfv.cn

[N02] 排序（工程实践用内置实现）
来源：http://vyb.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://lkm.tarul.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ctq.sysykeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://slw.xziqi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bjf.zhijiandao.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yye.smart0.xyz

Go:   slices.Sort(arr)
来源：http://zug.xinyue.icu

Ruby: arr.sort
来源：http://bwt.vehdjk.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://zpw.vehdjk.com

[N03] 快速排序（分治示例）
来源：http://olz.fanxiaobao.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bpp.zdqjudy.top

PHP:  // 递归实现，或用 usort
来源：http://uuw.pengpengdd.cyou

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://var.haohaochexian.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pmz.yonumen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://agj.zhengqikj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hfq.jqgufenzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xpi.yj20258.top

C#:   // 手写递归，或 Array.Sort
来源：http://pqw.nanxinkj.top

[N04] 斐波那契数列
来源：http://xou.svipenyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tmr.bbcook.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fvy.hongshengwenyu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wql.ydzc1.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tvi.zdbjq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zmw.ybcxt.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tvo.52xcode.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rqw.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dds.hongshengwenyu.top

[N05] 最大公约数
来源：http://aul.chenzaomai.com

Py:   math.gcd(a, b)
来源：http://brl.wangshuangyany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://iap.ywan-chungtsiang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aaw.fengsongda.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uss.yuanzhike.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gju.yj20258888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ntd.zhoulong.xyz

Ruby: a.gcd(b)
来源：http://uxg.nanxuanxn.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zrg.fengsongda.top

[N06] 判断回文字符串
来源：http://tfo.zhengqikj.top

Py:   s == s[::-1]
来源：http://hyr.hcnkem.com

PHP:  $s === strrev($s);
来源：http://zcy.quarkkingdee.top

JS:   s === [...s].reverse().join("")
来源：http://gkc.fehbvm.com

TS:   s === [...s].reverse().join("")
来源：http://vok.xuanzx.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dog.jinqigfzy.top

Go:   // 双指针从两端比较
来源：http://atb.fengsongda.top

Ruby: s == s.reverse
来源：http://pwg.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://mjj.jiagoushi.top

[N07] 两数之和（返回下标）
来源：http://jam.uphjek.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qdx.xinyue.icu


<!-- 参考信息 -->