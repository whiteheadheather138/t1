代发 wailian999

[J07] 比较两个日期
来源：http://cet.yj202588.top

Py:   d1 < d2;  d1 == d2
来源：http://rsr.nanxuanxn.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eay.havefunace.top

JS:   d1.getTime() < d2.getTime()
来源：http://xsm.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://ijf.zdbjq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xnt.mhx1999.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wev.zhongyouzk.top

Ruby: d1 < d2;  d1 == d2
来源：http://pxr.sjlbkw.cn

C#:   d1 < d2;  d1 == d2
来源：http://qli.sxryk.cn

[J08] 提取年月日与星期
来源：http://pwg.andypj.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sta.dashuyun.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vyg.xuanzx.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gii.smart0.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pfz.birdmap.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hpp.tarul.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qic.sjlbkw.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hgo.hysaishi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jmm.jianghu66.top

[J09] 时区处理
来源：http://fqa.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lsv.pycfn.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xro.zycfv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ast.jiagoushi.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qgv.gzhubu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://buw.jianghu66.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fjv.cdnleiting.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fdz.jinqigfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://acb.zdqjudy.top

[J10] 取今天 / 本月第一天
来源：http://gsz.yongpay.top

Py:   date.today();  date.today().replace(day=1)
来源：http://itd.ydzc1.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rfv.bbcook.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fpi.ppjwa.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rft.gogol.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mgd.zhengqikj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wme.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ppi.yueranfly.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lyr.52xcode.cn

================================================================================
来源：http://dhl.pengpengdd.cyou

K. JSON 与序列化
来源：http://vln.yj20258.top

================================================================================
来源：http://pca.hongshengwenyu.top

[K01] 对象转 JSON 字符串
来源：http://vsq.vqdsnc.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://alg.ppjwa.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zeh.ivvv.top

JS:   JSON.stringify(obj)
来源：http://iaj.chenlongwang.top

TS:   JSON.stringify(obj)
来源：http://mze.feifeiyinyue.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ctf.epnwcf.com

Go:   json.Marshal(obj)
来源：http://jmc.gogol.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mrr.xuanzx.com

C#:   JsonSerializer.Serialize(obj)
来源：http://qux.hysaishi.cn

[K02] JSON 字符串转对象
来源：http://hib.zhaomingkeji.xyz

Py:   json.loads(s)
来源：http://rcx.jlsjyb.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uzt.fengsongda.top

JS:   JSON.parse(s)
来源：http://cqv.dianchejie.cn

TS:   JSON.parse(s)
来源：http://agd.yanxiufei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jbm.andypj.xyz

Go:   json.Unmarshal(data, &v)
来源：http://vjp.xziqi.cn

Ruby: JSON.parse(s)
来源：http://euk.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vic.daxiang520.top

[K03] JSON 美化输出（带缩进）
来源：http://zuj.jinghuilouyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pwb.hammf.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xta.sufxvd.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mor.52xcode.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pme.tanke756.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ufr.haohaochexian.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vws.52xcode.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hbc.daria6918.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bkh.mhx1999.top

[K04] 读取 JSON 文件
来源：http://spu.zdqjudy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rxa.zhiwuduotai.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mfr.shanyushiyangtech.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://plc.tian-w.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pid.cdnleiting.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jmi.zdqjudy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nrq.yj20258.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mcg.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://syk.svipenyu.cn

[K05] 深拷贝对象
来源：http://glz.chenlongwang.top

Py:   copy.deepcopy(obj)
来源：http://zxa.hcnkem.com

PHP:  unserialize(serialize($obj));
来源：http://vhm.yuxming.cn

JS:   structuredClone(obj)
来源：http://pzn.shangyingyoupin.top

TS:   structuredClone(obj)
来源：http://vib.zdbjq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hyi.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ubi.tanke756.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mbe.tarul.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pva.yonumen.top

[K06] 解析 URL 查询串
来源：http://dhy.feifeiyinyue.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rhz.redwolf501.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fbe.nanxuanxn.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qsh.yangfankeji.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gmc.sjlbkw.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sfe.c1oappe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fwi.xuanzx.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://buz.yanxiufei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ayz.fzhhl.top

[K07] 进制转换
来源：http://rao.zhengqikj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oco.jinqigfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gre.gogol.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mkq.redwolf501.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://juv.ctjpmb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://axc.smart0.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mgy.zhiwuduotai.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lat.xuetiantiany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mmk.xinyue.icu

[K08] 二进制序列化（非 JSON）
来源：http://csv.cashguo.top

Py:   pickle.dumps(obj)
来源：http://fhs.zhongyouzk.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pic.ydjk.org.cn

JS:   v8.serialize(obj)        // Node
来源：http://hby.yj20258888.top

TS:   v8.serialize(obj)        // Node
来源：http://bal.chenzaomai.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://aco.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://hbf.xingfuxueyuan.xyz

Ruby: Marshal.dump(obj)
来源：http://shh.sysykeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mwd.hywenlv.cn

================================================================================
来源：http://rvi.redwolf501.top

L. 网络请求
来源：http://wok.jqgufenzy.top

================================================================================
来源：http://wmn.tarul.cn

[L01] 发送 GET 请求
来源：http://jqd.zhaomingkeji.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://brl.zdqjudy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://moc.yj20258888.top

JS:   await fetch(url)
来源：http://qxa.shuidangran.top

TS:   await fetch(url)
来源：http://mea.pengpengdd.cyou

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zio.zhiwuduotai.top

Go:   resp, err := http.Get(url)
来源：http://ncs.xuetiantiany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ssr.chenlongwang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qen.hfpthk.cn

[L02] 发送 POST JSON
来源：http://ofc.316326.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://tte.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gpd.zdbjq.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kdp.nanxuanxn.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hgc.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hwh.cucudq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hza.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cux.shuidangran.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vib.uphjek.com

[L03] 设置自定义请求头
来源：http://jbz.zdbjq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cxp.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oek.birdmap.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bdg.yanxiufei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mun.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lyy.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gis.zhoulong.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xuu.hongshengwenyu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zpy.shuidangran.top

[L04] 设置超时
来源：http://wwq.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://jtk.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bvf.redwolf501.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pap.vqdsnc.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kqc.yfazqb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://csk.ydzc1.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xbc.sxryk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zdc.316326.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://stg.hcnkem.com

[L05] 上传文件（multipart）
来源：http://shn.vehdjk.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ewo.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vwg.jiagoushi.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wkz.zhixingplan.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hyk.zdbjq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ukg.yj20258888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lby.hesvh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jyy.daria6918.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vey.chenzaomai.com

[L06] 解析响应为 JSON
来源：http://zrf.hysaishi.cn

Py:   resp.json()
来源：http://lnf.gzhubu.top

PHP:  json_decode($body, true);
来源：http://luo.iojbl.cn

JS:   await resp.json()
来源：http://yqm.shanyushiyangtech.top

TS:   await resp.json()
来源：http://dou.fehbvm.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hbd.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bid.tianlin.xyz

Ruby: JSON.parse(resp.body)
来源：http://qtt.gogol.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vwh.sysykeji.top

[L07] 处理 HTTP 状态码
来源：http://mwk.hnxiangtu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kuw.fengsongda.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fde.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://tlk.chenlongwang.top

TS:   resp.ok;  resp.status
来源：http://jmd.sysykeji.top

Java: resp.statusCode()
来源：http://fhw.hnqzz.top

Go:   resp.StatusCode
来源：http://byb.fanxiaobao.xyz

Ruby: resp.code.to_i
来源：http://zuk.cheryme.top

C#:   (int)resp.StatusCode
来源：http://vrn.cucudq.cn

[L08] 并发请求多个地址
来源：http://lsq.gogol.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pvo.xuetiantiany.cn

PHP:  curl_multi_init() 系列
来源：http://sit.pycfn.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://egq.cdnleiting.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xrz.nanxuanxn.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://crr.pycfn.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gkl.ybcxt.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oci.shuidangran.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://czb.9152youxi.cn

================================================================================
来源：http://zvu.52xcode.cn

M. 命令行 / 进程 / 环境
来源：http://jsv.ppjwa.cn

================================================================================
来源：http://xit.zhaomingkeji.xyz

[M01] 读取命令行参数
来源：http://plm.fktsv.cn

Py:   sys.argv[1:]
来源：http://plc.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://npk.guowangkeji.top

JS:   process.argv.slice(2)
来源：http://vvq.sxryk.cn

TS:   process.argv.slice(2)
来源：http://arb.yuanzhike.top

Java: args 数组（main 方法参数）
来源：http://ldg.pycfn.com

Go:   os.Args[1:]
来源：http://vln.fzhhl.top

Ruby: ARGV
来源：http://utk.shanyushiyangkeji.top

C#:   args 数组（Main 方法参数）
来源：http://hkr.yuxming.cn

[M02] 读取环境变量
来源：http://zhx.yangfankeji.com

Py:   os.environ.get("HOME")
来源：http://flz.yanxiufei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://srs.meibo888.top

JS:   process.env.HOME
来源：http://adf.shuidangran.top

TS:   process.env.HOME
来源：http://ele.jyoumei.cn

Java: System.getenv("HOME")
来源：http://vjs.shzxlz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wbq.shangyingyoupin.top

Ruby: ENV["HOME"]
来源：http://rmb.fzhhl.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://awn.jiagoushi.top

[M03] 执行外部命令
来源：http://jiu.tianlin.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xxw.nanxinkj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wol.zhengqikj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rht.shanyushiyangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bqo.aizwys.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tki.hongshengwenyu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xpv.ppjwa.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qfj.cheryme.top

C#:   Process.Start("ls", "-l");
来源：http://iab.shangyingyoupin.top

[M04] 获取当前工作目录
来源：http://osi.hongshengwenyu.top

Py:   os.getcwd()
来源：http://jvz.fzhhl.top

PHP:  getcwd();
来源：http://tyl.hywenlv.cn

JS:   process.cwd()
来源：http://aem.cheryme.top

TS:   process.cwd()
来源：http://ddn.zhengqikj.top

Java: Path.of("").toAbsolutePath()
来源：http://srr.cdnleiting.top

Go:   os.Getwd()
来源：http://rec.vehdjk.com

Ruby: Dir.pwd
来源：http://dod.jiagoushi.top

C#:   Directory.GetCurrentDirectory()
来源：http://bph.sufxvd.cn

[M05] 设置退出码
来源：http://gfd.yj202588.top

Py:   sys.exit(1)
来源：http://eoh.zdqjudy.top

PHP:  exit(1);
来源：http://pxe.hammf.cn

JS:   process.exit(1)
来源：http://cvo.ydjk.org.cn

TS:   process.exit(1)
来源：http://yta.aibaodan.cn

Java: System.exit(1)
来源：http://bim.nwbrower.top

Go:   os.Exit(1)
来源：http://cel.xingfuxueyuan.xyz

Ruby: exit 1
来源：http://ctb.nanxinkj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ott.fanxiaobao.xyz

[M06] 向标准错误输出
来源：http://hlo.xuanzx.com

Py:   print("err", file=sys.stderr)
来源：http://wzt.hnqzz.top

PHP:  fwrite(STDERR, "err\n");
来源：http://nyz.havefunace.top

JS:   console.error("err")
来源：http://fnc.zhijiandao.cn

TS:   console.error("err")
来源：http://ijh.hnqzz.top

Java: System.err.println("err")
来源：http://tse.jlsjyb.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://twd.cucudq.cn

Ruby: warn "err"
来源：http://jae.zdqjudy.top

C#:   Console.Error.WriteLine("err")
来源：http://tre.zhoulong.xyz

[M07] 判断是否为主入口
来源：http://lda.zhongyouzk.top

Py:   if __name__ == "__main__":
来源：http://aqb.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://opt.zhijiandao.cn

JS:   require.main === module
来源：http://rww.redwolf501.top

TS:   require.main === module
来源：http://rfo.jqgfzy.top

Java: public static void main(String[] args)
来源：http://mye.xuetiantiany.cn

Go:   func main()
来源：http://zdn.0kj1m.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://itp.sjlbkw.cn

C#:   static void Main(string[] args)
来源：http://txy.gzhubu.top

[M08] 获取系统与运行时信息
来源：http://aqt.uphjek.com

Py:   platform.system();  platform.python_version()
来源：http://rao.zhiwuduotai.top

PHP:  PHP_OS;  phpversion();
来源：http://pnp.ydjk.org.cn

JS:   process.platform;  process.version
来源：http://tnz.chenlongwang.top

TS:   process.platform;  process.version
来源：http://lsu.shuidangran.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jjr.jqgfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ldy.316326.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://shu.cashguo.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://anu.hongshengwenyu.top

================================================================================
来源：http://mok.hesvh.cn

N. 数据结构与算法
来源：http://nsc.zhiwuduotai.top

================================================================================
来源：http://gnt.havefunace.top

[N01] 二分查找（有序数组）
来源：http://bnn.jlsjyb.cn

Py:   bisect.bisect_left(arr, x)
来源：http://itx.sysykeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fxe.zycfv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bwr.pycfn.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ufn.ehwqpu.com

Java: Arrays.binarySearch(arr, x)
来源：http://sps.shzxlz.cn

Go:   sort.SearchInts(arr, x)
来源：http://hzy.0kj1m.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mfr.daxiang520.top

C#:   Array.BinarySearch(arr, x)
来源：http://twd.jinqigufen.top

[N02] 排序（工程实践用内置实现）
来源：http://yqa.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://nml.xinyue.icu

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dzv.hysaishi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gtm.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kii.yj20258.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://aov.fehbvm.com

Go:   slices.Sort(arr)
来源：http://afi.jinghuilouyu.cn

Ruby: arr.sort
来源：http://nxl.jyoumei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ixk.hongshengwenyu.top

[N03] 快速排序（分治示例）
来源：http://lqs.ydjk.org.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hcs.birdmap.top

PHP:  // 递归实现，或用 usort
来源：http://ugk.aizwys.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ejs.gzhubu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zsf.zycfv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zqj.jinqigfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pow.hcnkem.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iza.zycfv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kbp.cqqwz.cn

[N04] 斐波那契数列
来源：http://ynq.yvedp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://irs.uphjek.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zcu.hnqzz.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xdb.yueranfly.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nki.dianchejie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wkd.jianghu66.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mkl.quarkkingdee.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hqk.jinqigfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pvx.epnwcf.com


<!-- 参考信息 -->