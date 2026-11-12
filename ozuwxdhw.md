代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://gqb.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://ysu.dashuyun.cn

Ruby: end - start                 # 返回秒数
来源：http://nnf.jianghu66.top

C#:   (end - start).TotalSeconds
来源：http://nes.tian-w.cn

[J07] 比较两个日期
来源：http://cxc.sweek.top

Py:   d1 < d2;  d1 == d2
来源：http://idi.cashguo.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gzm.andypj.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://ioq.daxiang520.top

TS:   d1.getTime() < d2.getTime()
来源：http://utn.yangfankeji.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hyt.nanxinkj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ztj.c1oappe.top

Ruby: d1 < d2;  d1 == d2
来源：http://let.cdnleiting.top

C#:   d1 < d2;  d1 == d2
来源：http://gir.dashuyun.cn

[J08] 提取年月日与星期
来源：http://vgk.fktsv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pje.hnqzz.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lvz.fengsongda.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bct.uphjek.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tns.wangdashe.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yqv.chenzaomai.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://evc.shzxlz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aso.yanxiufei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sve.gaohongyu789.top

[J09] 时区处理
来源：http://ydz.pycfn.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mxw.fehbvm.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ocg.jinghuilouyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dvy.cheryme.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zod.yvedp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://doz.nanxuanxn.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zfa.redwolf501.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hnw.ybcxt.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oys.mhx1999.top

[J10] 取今天 / 本月第一天
来源：http://fpg.sufxvd.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tsm.gaohongyu789.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mfb.gzhubu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qch.hnqzz.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bet.yuanzhike.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rto.cheryme.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kbb.zhiwuduotai.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tus.yangfankeji.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dwg.zhengqikj.top

================================================================================
来源：http://iiz.feifeiyinyue.top

K. JSON 与序列化
来源：http://exj.jinghuilouyu.cn

================================================================================
来源：http://ddu.yj20258888.top

[K01] 对象转 JSON 字符串
来源：http://ezg.yvedp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ukw.xinyue.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qcd.sjlbkw.cn

JS:   JSON.stringify(obj)
来源：http://kgm.52xcode.cn

TS:   JSON.stringify(obj)
来源：http://bwj.xingfuxueyuan.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ucw.hfpthk.cn

Go:   json.Marshal(obj)
来源：http://ztu.chenjidiqi.icu

Ruby: obj.to_json                                     // require "json"
来源：http://yls.wangdashe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xyj.feifeiyinyue.top

[K02] JSON 字符串转对象
来源：http://bgy.sjlbkw.cn

Py:   json.loads(s)
来源：http://xpr.jianghu66.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bcq.zhoulong.xyz

JS:   JSON.parse(s)
来源：http://scb.ydzc1.top

TS:   JSON.parse(s)
来源：http://osh.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vow.shanyushiyangtech.top

Go:   json.Unmarshal(data, &v)
来源：http://fqm.pengpengdd.cyou

Ruby: JSON.parse(s)
来源：http://nis.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lsp.sjlbkw.cn

[K03] JSON 美化输出（带缩进）
来源：http://cfa.chenjidiqi.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bzz.chenjidiqi.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hsv.hnxiangtu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dyo.yj20258888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jdu.daria6918.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jyb.wangshuangyany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pga.mhx1999.top

Ruby: JSON.pretty_generate(obj)
来源：http://ijp.ybcxt.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://roi.quarkkingdee.top

[K04] 读取 JSON 文件
来源：http://zos.xinyue.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mub.hcnkem.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xuv.hcnkem.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ouf.vqdsnc.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ayv.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eae.0kj1m.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jql.svipenyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qsw.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bgm.hysaishi.cn

[K05] 深拷贝对象
来源：http://jgk.chenlongwang.top

Py:   copy.deepcopy(obj)
来源：http://ewr.chenjidiqi.icu

PHP:  unserialize(serialize($obj));
来源：http://nhk.vqdsnc.cn

JS:   structuredClone(obj)
来源：http://gpq.nwbrower.top

TS:   structuredClone(obj)
来源：http://osd.yvedp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lhv.chenjidiqi.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wjw.aizwys.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zfp.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zeo.316326.xyz

[K06] 解析 URL 查询串
来源：http://wqt.hongshengwenyu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kld.aibaodan.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yun.iojbl.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lni.ydjk.org.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hio.zhaomingkeji.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pij.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mki.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aov.cucudq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dmy.andypj.xyz

[K07] 进制转换
来源：http://iuu.9152youxi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ils.quarkkingdee.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rix.hongshengwenyu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qus.aizwys.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xtw.svipenyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qis.jinghuilouyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oua.gzhubu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sdm.sufxvd.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dto.dashuyun.cn

[K08] 二进制序列化（非 JSON）
来源：http://qzx.feifeiyinyue.top

Py:   pickle.dumps(obj)
来源：http://tto.bjfxy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ght.chenzaomai.com

JS:   v8.serialize(obj)        // Node
来源：http://ebr.yueranfly.top

TS:   v8.serialize(obj)        // Node
来源：http://neq.hywenlv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lhj.nanxuanxn.top

Go:   encoding/gob
来源：http://qtj.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://iyk.wangdashe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zni.fktsv.cn

================================================================================
来源：http://chq.nanxuanxn.top

L. 网络请求
来源：http://oeo.cucudq.cn

================================================================================
来源：http://skp.yvedp.cn

[L01] 发送 GET 请求
来源：http://cnx.hnqzz.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vdc.zhoulong.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://okn.shanyushiyangtech.top

JS:   await fetch(url)
来源：http://erw.xziqi.cn

TS:   await fetch(url)
来源：http://bmf.xylfe.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kml.52xcode.cn

Go:   resp, err := http.Get(url)
来源：http://tqq.yj20258.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wtr.zhixingplan.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gql.sufxvd.cn

[L02] 发送 POST JSON
来源：http://kqf.wangshuangyany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ekr.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://enp.yongpay.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eou.jinqigufen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hds.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qcx.sweek.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dyl.mhx1999.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bzz.nanxinkj.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ulx.cqqwz.cn

[L03] 设置自定义请求头
来源：http://jci.xinyue.icu

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uaw.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nzv.quarkkingdee.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ojh.jiagoushi.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yrd.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eqo.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://snm.yanxiufei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ktr.jinghuilouyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://foh.hnxiangtu.top

[L04] 设置超时
来源：http://rod.guannengcc.top

Py:   requests.get(url, timeout=5)
来源：http://fkj.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ogq.smart0.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pkp.sufxvd.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nyt.xziqi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://egk.epnwcf.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ikx.shzxlz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bvr.yangfankeji.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jua.gzhubu.top

[L05] 上传文件（multipart）
来源：http://vxq.andypj.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fpo.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://skz.fehbvm.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://upc.xingfuxueyuan.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fzk.yj20258.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://shb.wangshuangyany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://etz.snrcjt.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kta.hywenlv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://akf.yuxming.cn

[L06] 解析响应为 JSON
来源：http://jsg.ydzc1.top

Py:   resp.json()
来源：http://xld.feifeiyinyue.top

PHP:  json_decode($body, true);
来源：http://gmc.jinyuanbaomall.cn

JS:   await resp.json()
来源：http://wqi.chenlongwang.top

TS:   await resp.json()
来源：http://aaz.yfazqb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://grh.aizwys.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uhi.52xcode.cn

Ruby: JSON.parse(resp.body)
来源：http://mef.zhaomingkeji.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dpw.ydzc1.top

[L07] 处理 HTTP 状态码
来源：http://jol.mhx1999.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ueu.cucudq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qgb.havefunace.top

JS:   resp.ok;  resp.status
来源：http://tba.cheryme.top

TS:   resp.ok;  resp.status
来源：http://lkz.zhoulong.xyz

Java: resp.statusCode()
来源：http://pqg.guannengcc.top

Go:   resp.StatusCode
来源：http://poj.shuidangran.top

Ruby: resp.code.to_i
来源：http://llk.mhx1999.top

C#:   (int)resp.StatusCode
来源：http://syn.zhaomingkeji.xyz

[L08] 并发请求多个地址
来源：http://gsf.guowangkeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rgw.nwbrower.top

PHP:  curl_multi_init() 系列
来源：http://kfh.sufxvd.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cqm.zhiwuduotai.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jmg.9152youxi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qpp.kuanghao11.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cud.ywan-chungtsiang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sgw.snrcjt.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eki.uphjek.com

================================================================================
来源：http://dch.xylfe.cn

M. 命令行 / 进程 / 环境
来源：http://cpj.yfazqb.com

================================================================================
来源：http://wro.iojbl.cn

[M01] 读取命令行参数
来源：http://mwt.cucudq.cn

Py:   sys.argv[1:]
来源：http://oza.quarkkingdee.top

PHP:  $argv;  $argc;
来源：http://fdr.aizwys.cn

JS:   process.argv.slice(2)
来源：http://obk.andypj.xyz

TS:   process.argv.slice(2)
来源：http://obe.zycfv.cn

Java: args 数组（main 方法参数）
来源：http://moi.ivvv.top

Go:   os.Args[1:]
来源：http://sac.nwbrower.top

Ruby: ARGV
来源：http://mxg.xuanzx.com

C#:   args 数组（Main 方法参数）
来源：http://xdz.9152youxi.cn

[M02] 读取环境变量
来源：http://sye.fehbvm.com

Py:   os.environ.get("HOME")
来源：http://xvh.gzhubu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yqf.ivvv.top

JS:   process.env.HOME
来源：http://zth.gogol.net.cn

TS:   process.env.HOME
来源：http://ife.wangshuangyany.cn

Java: System.getenv("HOME")
来源：http://cwk.yj20258.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zjs.nwbrower.top

Ruby: ENV["HOME"]
来源：http://pkh.fktsv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wlw.xingfuxueyuan.xyz

[M03] 执行外部命令
来源：http://yqm.wangdashe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://opn.tarul.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dnb.chenzaomai.com

JS:   child_process.execSync("ls -l").toString()
来源：http://vlu.gzhubu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://rvo.shuidangran.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dlb.zhaomingkeji.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://yzm.tianlin.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://njm.gotoacloud.top

C#:   Process.Start("ls", "-l");
来源：http://dxq.daxiang520.top

[M04] 获取当前工作目录
来源：http://rbj.c1oappe.top

Py:   os.getcwd()
来源：http://jrp.fzhhl.top

PHP:  getcwd();
来源：http://hwd.zdqjudy.top

JS:   process.cwd()
来源：http://otr.xingfuxueyuan.xyz

TS:   process.cwd()
来源：http://xsy.hnxiangtu.top

Java: Path.of("").toAbsolutePath()
来源：http://gfa.haohaochexian.top

Go:   os.Getwd()
来源：http://cmn.gaohongyu789.top

Ruby: Dir.pwd
来源：http://vmx.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://vwk.jqgufenzy.top

[M05] 设置退出码
来源：http://wck.shzxlz.cn

Py:   sys.exit(1)
来源：http://keu.cheryme.top

PHP:  exit(1);
来源：http://aob.sxryk.cn

JS:   process.exit(1)
来源：http://rso.chenjidiqi.icu

TS:   process.exit(1)
来源：http://ofn.yuanzhike.top

Java: System.exit(1)
来源：http://lls.hesvh.cn

Go:   os.Exit(1)
来源：http://iox.vqdsnc.cn

Ruby: exit 1
来源：http://buh.yuxming.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nir.hesvh.cn

[M06] 向标准错误输出
来源：http://snt.haohaochexian.top

Py:   print("err", file=sys.stderr)
来源：http://myj.gogol.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ckz.yvedp.cn

JS:   console.error("err")
来源：http://mfw.vqdsnc.cn

TS:   console.error("err")
来源：http://igv.smart0.xyz

Java: System.err.println("err")
来源：http://zow.bbcook.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://anh.sysykeji.top

Ruby: warn "err"
来源：http://bwc.zdqjudy.top

C#:   Console.Error.WriteLine("err")
来源：http://yad.sjlbkw.cn

[M07] 判断是否为主入口
来源：http://gja.yanxiufei.cn

Py:   if __name__ == "__main__":
来源：http://hto.hnxiangtu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cfh.316326.xyz

JS:   require.main === module
来源：http://zpz.jlsjyb.cn

TS:   require.main === module
来源：http://lmd.ctjpmb.com

Java: public static void main(String[] args)
来源：http://jgu.yuxming.cn

Go:   func main()
来源：http://pwf.nanxuanxn.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wke.feifeiyinyue.top

C#:   static void Main(string[] args)
来源：http://lka.hcnkem.com

[M08] 获取系统与运行时信息
来源：http://fpp.fehbvm.com

Py:   platform.system();  platform.python_version()
来源：http://ujq.zhengqikj.top

PHP:  PHP_OS;  phpversion();
来源：http://yvk.xziqi.cn

JS:   process.platform;  process.version
来源：http://jrs.gzhubu.top

TS:   process.platform;  process.version
来源：http://snz.dashuyun.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yrd.shangyingyoupin.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://cjk.yongpay.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lgs.gotoacloud.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://umi.cdnleiting.top

================================================================================
来源：http://seo.gotoacloud.top

N. 数据结构与算法
来源：http://rax.svipenyu.cn

================================================================================
来源：http://ppn.tanke756.top

[N01] 二分查找（有序数组）
来源：http://ati.mhx1999.top

Py:   bisect.bisect_left(arr, x)
来源：http://orb.zycfv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fdf.xingfuxueyuan.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hdz.shzxlz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vzo.daxiang520.top

Java: Arrays.binarySearch(arr, x)
来源：http://lkr.feifeiyinyue.top

Go:   sort.SearchInts(arr, x)
来源：http://bzt.zhoulong.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://zmz.yj20258.top

C#:   Array.BinarySearch(arr, x)
来源：http://zas.jinghuilouyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://wqj.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://vdm.jiagoushi.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qfc.sweek.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://thb.sysykeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://eyi.ywan-chungtsiang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fiq.tanke756.top

Go:   slices.Sort(arr)
来源：http://nxl.svipenyu.cn

Ruby: arr.sort
来源：http://ond.jqgfzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://idp.zhoulong.xyz

[N03] 快速排序（分治示例）
来源：http://uqy.shanyushiyangtech.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pne.chenlongwang.top

PHP:  // 递归实现，或用 usort
来源：http://ahx.ehwqpu.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oef.nwbrower.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://asb.vehdjk.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vpb.fehbvm.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://com.havefunace.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://erf.zhiwuduotai.top

C#:   // 手写递归，或 Array.Sort
来源：http://edc.jqgufenzy.top

[N04] 斐波那契数列
来源：http://eko.hnqzz.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pyp.xylfe.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kra.hnqzz.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ecm.vehdjk.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qsa.tarul.cn


<!-- 参考信息 -->