代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://kxw.zhengqikj.top

Go:   end.Sub(start).Hours()
来源：http://szo.daxiang520.top

Ruby: end - start                 # 返回秒数
来源：http://bad.tanke756.top

C#:   (end - start).TotalSeconds
来源：http://aya.cucudq.cn

[J07] 比较两个日期
来源：http://qad.chenzaomai.com

Py:   d1 < d2;  d1 == d2
来源：http://nym.9152youxi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zna.gogol.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pus.shanyushiyangtech.top

TS:   d1.getTime() < d2.getTime()
来源：http://cgk.shanyushiyangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rxm.nanxinkj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rkr.jqgufenzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://qkj.hammf.cn

C#:   d1 < d2;  d1 == d2
来源：http://hcx.jiagoushi.top

[J08] 提取年月日与星期
来源：http://ilp.sufxvd.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cjm.hammf.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cdc.guowangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wnx.quarkkingdee.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gjt.ybcxt.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ort.zhoulong.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xui.jlsjyb.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://glf.gotoacloud.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yvi.shangyingyoupin.top

[J09] 时区处理
来源：http://leu.yanxiufei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vxl.shanyushiyangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://drq.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ete.316326.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zge.tanke756.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://erh.yj20258888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://msc.svipenyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qmu.cdnleiting.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://anz.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://oxt.aizwys.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://eck.sufxvd.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wtk.shuidangran.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dpm.nanxinkj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sdz.jianghu66.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://leb.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dyw.jiagoushi.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rya.bjfxy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bcd.cucudq.cn

================================================================================
来源：http://sbh.shangyingyoupin.top

K. JSON 与序列化
来源：http://fyh.andypj.xyz

================================================================================
来源：http://duk.zhoulong.xyz

[K01] 对象转 JSON 字符串
来源：http://tsf.pengpengdd.cyou

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sek.xziqi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://izd.kuanghao11.cn

JS:   JSON.stringify(obj)
来源：http://ecx.yuxming.cn

TS:   JSON.stringify(obj)
来源：http://qoy.shangyingyoupin.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sid.jianghu66.top

Go:   json.Marshal(obj)
来源：http://prk.52xcode.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jzj.havefunace.top

C#:   JsonSerializer.Serialize(obj)
来源：http://sad.cdnleiting.top

[K02] JSON 字符串转对象
来源：http://pck.havefunace.top

Py:   json.loads(s)
来源：http://iff.jinqigfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://whh.cashguo.top

JS:   JSON.parse(s)
来源：http://vgt.fzhhl.top

TS:   JSON.parse(s)
来源：http://amh.zdbjq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ccf.xingfuxueyuan.xyz

Go:   json.Unmarshal(data, &v)
来源：http://iwq.xuetiantiany.cn

Ruby: JSON.parse(s)
来源：http://vfj.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ywo.zycfv.cn

[K03] JSON 美化输出（带缩进）
来源：http://ltf.redwolf501.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rke.xylfe.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ymj.cdnleiting.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jtf.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tkt.aizwys.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kkk.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ext.zdbjq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://aje.fktsv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://npu.tianlin.xyz

[K04] 读取 JSON 文件
来源：http://ceb.hnxiangtu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mjz.xuanzx.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pbg.daria6918.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://che.pycfn.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sjs.cashguo.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qmx.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xrf.zhixingplan.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xps.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pez.cqqwz.cn

[K05] 深拷贝对象
来源：http://gmt.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://cqa.xuetiantiany.cn

PHP:  unserialize(serialize($obj));
来源：http://bkb.dashuyun.cn

JS:   structuredClone(obj)
来源：http://wwo.birdmap.top

TS:   structuredClone(obj)
来源：http://mzj.svipenyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fvk.sufxvd.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://npd.yuxming.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pso.hammf.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mcr.hesvh.cn

[K06] 解析 URL 查询串
来源：http://sxu.jyoumei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jhd.nwbrower.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fnz.yueranfly.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://two.ywan-chungtsiang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tmn.yangfankeji.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bro.chenjidiqi.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://bvg.cucudq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vtv.c1oappe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ooe.pengpengdd.cyou

[K07] 进制转换
来源：http://klj.gaohongyu789.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wtq.hesvh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tzo.chenzaomai.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sif.ctjpmb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vbj.ywan-chungtsiang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kfl.9152youxi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vbs.yongpay.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ysl.zhijiandao.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://thq.nwbrower.top

[K08] 二进制序列化（非 JSON）
来源：http://kby.gotoacloud.top

Py:   pickle.dumps(obj)
来源：http://jrc.cdnleiting.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lfa.jianghu66.top

JS:   v8.serialize(obj)        // Node
来源：http://hbn.yvedp.cn

TS:   v8.serialize(obj)        // Node
来源：http://iri.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://emh.sysykeji.top

Go:   encoding/gob
来源：http://psw.vqdsnc.cn

Ruby: Marshal.dump(obj)
来源：http://brx.xingfuxueyuan.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dnl.tanke756.top

================================================================================
来源：http://ntv.yongpay.top

L. 网络请求
来源：http://toj.zhoulong.xyz

================================================================================
来源：http://ydg.hesvh.cn

[L01] 发送 GET 请求
来源：http://gqq.sjlbkw.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vmd.jinqigufen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vat.zhaomingkeji.xyz

JS:   await fetch(url)
来源：http://esb.tanke756.top

TS:   await fetch(url)
来源：http://mrq.zdqjudy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wmp.mhx1999.top

Go:   resp, err := http.Get(url)
来源：http://zgk.nwbrower.top

Ruby: Net::HTTP.get(URI(url))
来源：http://uxc.zhoulong.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://euy.xuetiantiany.cn

[L02] 发送 POST JSON
来源：http://lxe.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://cpx.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eir.cheryme.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://poy.gzhubu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vkm.316326.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zbk.yj20258.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://njo.hcnkem.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tnq.9152youxi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vnc.wangdashe.top

[L03] 设置自定义请求头
来源：http://lts.tianlin.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rqm.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mxd.hammf.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ges.yuanzhike.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dry.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qsj.tian-w.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fyd.fktsv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hni.zhengqikj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ffl.dianchejie.cn

[L04] 设置超时
来源：http://ims.hywenlv.cn

Py:   requests.get(url, timeout=5)
来源：http://nco.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ohm.ehwqpu.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ikk.jinqigfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://znq.fengsongda.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zok.jiagoushi.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bdc.ydjk.org.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dqs.cdnleiting.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://aro.cashguo.top

[L05] 上传文件（multipart）
来源：http://guw.zhijiandao.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zgw.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lah.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tga.fehbvm.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://urz.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oza.cashguo.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ubb.shzxlz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wsf.yanxiufei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rwn.yfazqb.com

[L06] 解析响应为 JSON
来源：http://zss.sufxvd.cn

Py:   resp.json()
来源：http://hoy.wangdashe.top

PHP:  json_decode($body, true);
来源：http://hhc.quarkkingdee.top

JS:   await resp.json()
来源：http://sjw.hysaishi.cn

TS:   await resp.json()
来源：http://hls.vehdjk.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ngi.vehdjk.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pgj.ehwqpu.com

Ruby: JSON.parse(resp.body)
来源：http://pfr.hnxiangtu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lqi.feifeiyinyue.top

[L07] 处理 HTTP 状态码
来源：http://ncb.hysaishi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sqz.wangdashe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://efd.ivvv.top

JS:   resp.ok;  resp.status
来源：http://had.tarul.cn

TS:   resp.ok;  resp.status
来源：http://vef.jiagoushi.top

Java: resp.statusCode()
来源：http://cnc.ybcxt.top

Go:   resp.StatusCode
来源：http://ehv.jinqigufen.top

Ruby: resp.code.to_i
来源：http://kpq.yj202588.top

C#:   (int)resp.StatusCode
来源：http://adi.hfpthk.cn

[L08] 并发请求多个地址
来源：http://xlb.gogol.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://omx.pengpengdd.cyou

PHP:  curl_multi_init() 系列
来源：http://mae.sweek.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mdz.zhoulong.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://thr.hesvh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://phf.svipenyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jdq.hongshengwenyu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sza.yangfankeji.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rtt.ybcxt.top

================================================================================
来源：http://hzi.fehbvm.com

M. 命令行 / 进程 / 环境
来源：http://rts.gogol.net.cn

================================================================================
来源：http://eip.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://myp.iojbl.cn

Py:   sys.argv[1:]
来源：http://yar.snrcjt.cn

PHP:  $argv;  $argc;
来源：http://pyu.yangfankeji.com

JS:   process.argv.slice(2)
来源：http://cos.jianghu66.top

TS:   process.argv.slice(2)
来源：http://oef.9152youxi.cn

Java: args 数组（main 方法参数）
来源：http://cam.yonumen.top

Go:   os.Args[1:]
来源：http://vkc.tian-w.cn

Ruby: ARGV
来源：http://njz.feifeiyinyue.top

C#:   args 数组（Main 方法参数）
来源：http://laq.jinqigufen.top

[M02] 读取环境变量
来源：http://acz.fzhhl.top

Py:   os.environ.get("HOME")
来源：http://mzc.yongpay.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://woy.hongshengwenyu.top

JS:   process.env.HOME
来源：http://xoh.fengsongda.top

TS:   process.env.HOME
来源：http://cjz.nwbrower.top

Java: System.getenv("HOME")
来源：http://aex.ivvv.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nhr.chenzaomai.com

Ruby: ENV["HOME"]
来源：http://wor.316326.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bll.nanxinkj.top

[M03] 执行外部命令
来源：http://lvh.quarkkingdee.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kcn.yj202588.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fzw.hfpthk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://acn.xuetiantiany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://boq.jlsjyb.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ocr.yvedp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mag.wangshuangyany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bis.cheryme.top

C#:   Process.Start("ls", "-l");
来源：http://bqa.svipenyu.cn

[M04] 获取当前工作目录
来源：http://qlc.yfazqb.com

Py:   os.getcwd()
来源：http://xfp.shuidangran.top

PHP:  getcwd();
来源：http://ykq.smart0.xyz

JS:   process.cwd()
来源：http://nwn.gzhubu.top

TS:   process.cwd()
来源：http://rdt.jianghu66.top

Java: Path.of("").toAbsolutePath()
来源：http://ipd.yanxiufei.cn

Go:   os.Getwd()
来源：http://fuo.xylfe.cn

Ruby: Dir.pwd
来源：http://ekd.nanxuanxn.top

C#:   Directory.GetCurrentDirectory()
来源：http://dhz.ybcxt.top

[M05] 设置退出码
来源：http://sly.daxiang520.top

Py:   sys.exit(1)
来源：http://mxn.zhiwuduotai.top

PHP:  exit(1);
来源：http://rus.xinyue.icu

JS:   process.exit(1)
来源：http://onq.tarul.cn

TS:   process.exit(1)
来源：http://lix.feifeiyinyue.top

Java: System.exit(1)
来源：http://ltn.zhixingplan.top

Go:   os.Exit(1)
来源：http://pxy.52xcode.cn

Ruby: exit 1
来源：http://ref.hfpthk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zls.chenlongwang.top

[M06] 向标准错误输出
来源：http://xrs.yonumen.top

Py:   print("err", file=sys.stderr)
来源：http://pgc.c1oappe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lhm.redwolf501.top

JS:   console.error("err")
来源：http://eut.daria6918.cn

TS:   console.error("err")
来源：http://bou.wangshuangyany.cn

Java: System.err.println("err")
来源：http://ups.haohaochexian.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ucz.zhixingplan.top

Ruby: warn "err"
来源：http://hja.svipenyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://xqy.gzhubu.top

[M07] 判断是否为主入口
来源：http://oiq.shangyingyoupin.top

Py:   if __name__ == "__main__":
来源：http://qgv.aizwys.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xcq.tianlin.xyz

JS:   require.main === module
来源：http://udx.hfpthk.cn

TS:   require.main === module
来源：http://ifz.dashuyun.cn

Java: public static void main(String[] args)
来源：http://byx.cucudq.cn

Go:   func main()
来源：http://pvn.bjfxy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xug.yj20258.top

C#:   static void Main(string[] args)
来源：http://wdm.jqgufenzy.top

[M08] 获取系统与运行时信息
来源：http://bvj.jianghu66.top

Py:   platform.system();  platform.python_version()
来源：http://sya.snrcjt.cn

PHP:  PHP_OS;  phpversion();
来源：http://mlr.nwbrower.top

JS:   process.platform;  process.version
来源：http://pod.iojbl.cn

TS:   process.platform;  process.version
来源：http://oij.kuanghao11.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dvi.zhijiandao.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yvp.ywan-chungtsiang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ngp.feifeiyinyue.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lfs.meibo888.top

================================================================================
来源：http://buk.quarkkingdee.top

N. 数据结构与算法
来源：http://sou.xziqi.cn

================================================================================
来源：http://kdj.gaohongyu789.top

[N01] 二分查找（有序数组）
来源：http://ada.quarkkingdee.top

Py:   bisect.bisect_left(arr, x)
来源：http://vby.ivvv.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://abq.cheryme.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jeb.nanxinkj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eep.sxryk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jth.ehwqpu.com

Go:   sort.SearchInts(arr, x)
来源：http://urt.hammf.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://syf.tarul.cn

C#:   Array.BinarySearch(arr, x)
来源：http://spw.zdbjq.cn

[N02] 排序（工程实践用内置实现）
来源：http://nfs.wangdashe.top

Py:   sorted(arr);  arr.sort()
来源：http://ace.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aml.guannengcc.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://sje.hcnkem.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://zsw.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://run.uphjek.com

Go:   slices.Sort(arr)
来源：http://nnz.xinyue.icu

Ruby: arr.sort
来源：http://gwf.316326.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://mbw.hammf.cn

[N03] 快速排序（分治示例）
来源：http://rbr.zdqjudy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zar.bbcook.cn

PHP:  // 递归实现，或用 usort
来源：http://jhj.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lnf.ppjwa.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ipc.ywan-chungtsiang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gqd.316326.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kqt.hcnkem.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://shj.jinqigfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://gmr.xuetiantiany.cn

[N04] 斐波那契数列
来源：http://wri.kuanghao11.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gki.cashguo.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tlf.hywenlv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wzw.vqdsnc.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aew.xziqi.cn


<!-- 参考信息 -->