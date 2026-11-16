代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ezk.jyoumei.cn

[J04] 时间戳与日期互转
来源：http://ebw.zhengqikj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ttf.ydzc1.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://phe.zhijiandao.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vgc.jinyuanbaomall.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ohj.fzhhl.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iuy.nwbrower.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://aiu.jinqigfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jmi.vqdsnc.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jpo.gaohongyu789.top

[J05] 时间加减（加 7 天）
来源：http://kzy.0kj1m.cn

Py:   now + timedelta(days=7)
来源：http://lbw.dianchejie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jlo.shuidangran.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rsk.ivvv.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jhk.ehwqpu.com

Java: LocalDate.now().plusDays(7)
来源：http://oxb.wangdashe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dia.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://our.ppjwa.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tmc.nanxinkj.top

[J06] 计算两时间之差
来源：http://fwa.chenzaomai.com

Py:   (end - start).total_seconds()
来源：http://qxa.yj20258888.top

PHP:  $end->diff($start)->days;
来源：http://fuw.meibo888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://syt.kuanghao11.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wkd.cucudq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bdv.epnwcf.com

Go:   end.Sub(start).Hours()
来源：http://cqj.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://ysj.cucudq.cn

C#:   (end - start).TotalSeconds
来源：http://fyf.gzhubu.top

[J07] 比较两个日期
来源：http://tel.uphjek.com

Py:   d1 < d2;  d1 == d2
来源：http://opq.yfazqb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gak.jiagoushi.top

JS:   d1.getTime() < d2.getTime()
来源：http://hkr.chenzaomai.com

TS:   d1.getTime() < d2.getTime()
来源：http://fil.0kj1m.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lja.ehwqpu.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rze.fengsongda.top

Ruby: d1 < d2;  d1 == d2
来源：http://out.jlsjyb.cn

C#:   d1 < d2;  d1 == d2
来源：http://smo.shangyingyoupin.top

[J08] 提取年月日与星期
来源：http://nxi.cucudq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://guy.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://chh.iojbl.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://llm.daxiang520.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://grh.xylfe.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://owq.hnqzz.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jie.hcnkem.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cmp.smart0.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jda.dashuyun.cn

[J09] 时区处理
来源：http://xmv.quarkkingdee.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fqi.ppjwa.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mpz.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uzj.gzhubu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jgt.wangshuangyany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sma.shzxlz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://koj.tanke756.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vpx.smart0.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eyr.wangshuangyany.cn

[J10] 取今天 / 本月第一天
来源：http://mdi.havefunace.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hbf.dianchejie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ueh.zhoulong.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://edx.shzxlz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mhq.cashguo.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dtf.yueranfly.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://imq.daria6918.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lxu.cheryme.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hnd.gzhubu.top

================================================================================
来源：http://dgl.shanyushiyangkeji.top

K. JSON 与序列化
来源：http://xbh.aizwys.cn

================================================================================
来源：http://uvk.smart0.xyz

[K01] 对象转 JSON 字符串
来源：http://kbb.aizwys.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qsg.hfpthk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://clg.quarkkingdee.top

JS:   JSON.stringify(obj)
来源：http://luw.hcnkem.com

TS:   JSON.stringify(obj)
来源：http://alc.tarul.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yrp.cashguo.top

Go:   json.Marshal(obj)
来源：http://iph.cashguo.top

Ruby: obj.to_json                                     // require "json"
来源：http://dru.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xvk.sweek.top

[K02] JSON 字符串转对象
来源：http://orx.xziqi.cn

Py:   json.loads(s)
来源：http://hng.ctjpmb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cft.jqgfzy.top

JS:   JSON.parse(s)
来源：http://tmy.cheryme.top

TS:   JSON.parse(s)
来源：http://imx.316326.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ksu.hnqzz.top

Go:   json.Unmarshal(data, &v)
来源：http://ykn.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://vtl.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nfs.sysykeji.top

[K03] JSON 美化输出（带缩进）
来源：http://imw.jinghuilouyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xxj.wangshuangyany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ghq.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://euh.daxiang520.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lbb.zdbjq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qkb.dashuyun.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vru.sxryk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xwc.jyoumei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bmb.cashguo.top

[K04] 读取 JSON 文件
来源：http://fjk.smart0.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jww.c1oappe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eun.jlsjyb.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dhm.ywan-chungtsiang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oyd.gogol.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ciz.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mzq.sjlbkw.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hfb.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xyi.yangfankeji.com

[K05] 深拷贝对象
来源：http://wvy.0kj1m.cn

Py:   copy.deepcopy(obj)
来源：http://nep.hywenlv.cn

PHP:  unserialize(serialize($obj));
来源：http://byn.bjfxy.top

JS:   structuredClone(obj)
来源：http://xiw.cheryme.top

TS:   structuredClone(obj)
来源：http://rjw.zhengqikj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://eql.aizwys.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ria.yongpay.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vfm.zhiwuduotai.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gge.zhiwuduotai.top

[K06] 解析 URL 查询串
来源：http://kah.nanxuanxn.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://avx.c1oappe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://coi.ybcxt.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vzz.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nnr.jqgufenzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bxn.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mea.ehwqpu.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fdo.pycfn.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sqo.chenjidiqi.icu

[K07] 进制转换
来源：http://yrd.hcnkem.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jpq.52xcode.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xhg.hammf.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ric.daxiang520.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://isw.snrcjt.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mwt.ctjpmb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://slz.dianchejie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://izt.sysykeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wsd.fanxiaobao.xyz

[K08] 二进制序列化（非 JSON）
来源：http://emq.nanxinkj.top

Py:   pickle.dumps(obj)
来源：http://kkp.fanxiaobao.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://ubn.quarkkingdee.top

JS:   v8.serialize(obj)        // Node
来源：http://zgm.hammf.cn

TS:   v8.serialize(obj)        // Node
来源：http://zgq.zdbjq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rnm.fktsv.cn

Go:   encoding/gob
来源：http://txa.havefunace.top

Ruby: Marshal.dump(obj)
来源：http://vrr.jqgufenzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ett.wangshuangyany.cn

================================================================================
来源：http://ncf.yvedp.cn

L. 网络请求
来源：http://tai.wangdashe.top

================================================================================
来源：http://oro.cucudq.cn

[L01] 发送 GET 请求
来源：http://qni.ywan-chungtsiang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qxe.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ydj.andypj.xyz

JS:   await fetch(url)
来源：http://tzm.zhiwuduotai.top

TS:   await fetch(url)
来源：http://tuz.hnqzz.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lwf.uphjek.com

Go:   resp, err := http.Get(url)
来源：http://iwf.yanxiufei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ooa.andypj.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oxj.zhengqikj.top

[L02] 发送 POST JSON
来源：http://leh.0kj1m.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lrd.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kkk.fehbvm.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://son.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vty.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ich.yuanzhike.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://prv.316326.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jrc.hfpthk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kzm.hfpthk.cn

[L03] 设置自定义请求头
来源：http://jkv.sysykeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mee.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nuk.smart0.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eny.guowangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kgc.zhongyouzk.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lmx.zycfv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mgz.uphjek.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tfb.fengsongda.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cjj.fktsv.cn

[L04] 设置超时
来源：http://yqs.zhiwuduotai.top

Py:   requests.get(url, timeout=5)
来源：http://dry.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vda.redwolf501.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ico.jiagoushi.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://reb.fktsv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mqo.ydzc1.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ocj.jiagoushi.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kks.xuetiantiany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bks.ivvv.top

[L05] 上传文件（multipart）
来源：http://hjy.jianghu66.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jsc.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gjz.zhongyouzk.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jpp.ivvv.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rjo.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sqy.yfazqb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hvg.havefunace.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ofa.chenlongwang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aed.52xcode.cn

[L06] 解析响应为 JSON
来源：http://nko.pycfn.com

Py:   resp.json()
来源：http://dij.jinqigufen.top

PHP:  json_decode($body, true);
来源：http://ytt.snrcjt.cn

JS:   await resp.json()
来源：http://uen.snrcjt.cn

TS:   await resp.json()
来源：http://pri.yonumen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rib.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ggp.sxryk.cn

Ruby: JSON.parse(resp.body)
来源：http://tar.yuxming.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kba.yonumen.top

[L07] 处理 HTTP 状态码
来源：http://ffm.cashguo.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nbp.zdbjq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gmt.bjfxy.top

JS:   resp.ok;  resp.status
来源：http://tpr.cdnleiting.top

TS:   resp.ok;  resp.status
来源：http://jpr.andypj.xyz

Java: resp.statusCode()
来源：http://nrj.epnwcf.com

Go:   resp.StatusCode
来源：http://yyl.9152youxi.cn

Ruby: resp.code.to_i
来源：http://adl.chenjidiqi.icu

C#:   (int)resp.StatusCode
来源：http://hki.ybcxt.top

[L08] 并发请求多个地址
来源：http://rma.jinqigfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ase.kuanghao11.cn

PHP:  curl_multi_init() 系列
来源：http://btf.zhixingplan.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tdn.shanyushiyangtech.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eyz.hnqzz.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nxt.zdqjudy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://plx.gotoacloud.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xis.yangfankeji.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iec.fktsv.cn

================================================================================
来源：http://rsr.hesvh.cn

M. 命令行 / 进程 / 环境
来源：http://xpi.dianchejie.cn

================================================================================
来源：http://pvm.sweek.top

[M01] 读取命令行参数
来源：http://hqc.sjlbkw.cn

Py:   sys.argv[1:]
来源：http://mes.jqgufenzy.top

PHP:  $argv;  $argc;
来源：http://ucl.sxryk.cn

JS:   process.argv.slice(2)
来源：http://rwz.hongshengwenyu.top

TS:   process.argv.slice(2)
来源：http://xoc.jlsjyb.cn

Java: args 数组（main 方法参数）
来源：http://mil.jinqigfzy.top

Go:   os.Args[1:]
来源：http://pma.chenzaomai.com

Ruby: ARGV
来源：http://ckc.ydzc1.top

C#:   args 数组（Main 方法参数）
来源：http://ywq.sxryk.cn

[M02] 读取环境变量
来源：http://ldd.gogol.net.cn

Py:   os.environ.get("HOME")
来源：http://rfh.yfazqb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iqv.zhixingplan.top

JS:   process.env.HOME
来源：http://wph.shanyushiyangtech.top

TS:   process.env.HOME
来源：http://skb.yueranfly.top

Java: System.getenv("HOME")
来源：http://vla.hnqzz.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wev.kuanghao11.cn

Ruby: ENV["HOME"]
来源：http://beo.nwbrower.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rfj.nwbrower.top

[M03] 执行外部命令
来源：http://rte.ivvv.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wjs.bjfxy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lvv.jyoumei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lqn.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://slg.aizwys.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vha.jinyuanbaomall.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zwk.dianchejie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vjo.uphjek.com

C#:   Process.Start("ls", "-l");
来源：http://gwu.chenjidiqi.icu

[M04] 获取当前工作目录
来源：http://edt.hesvh.cn

Py:   os.getcwd()
来源：http://zhx.zdbjq.cn

PHP:  getcwd();
来源：http://qec.hammf.cn

JS:   process.cwd()
来源：http://jdp.shuidangran.top

TS:   process.cwd()
来源：http://xyc.yueranfly.top

Java: Path.of("").toAbsolutePath()
来源：http://nui.hnqzz.top

Go:   os.Getwd()
来源：http://jqu.daxiang520.top

Ruby: Dir.pwd
来源：http://aia.nwbrower.top

C#:   Directory.GetCurrentDirectory()
来源：http://tfy.0kj1m.cn

[M05] 设置退出码
来源：http://brg.uphjek.com

Py:   sys.exit(1)
来源：http://lcr.shanyushiyangtech.top

PHP:  exit(1);
来源：http://krh.daria6918.cn

JS:   process.exit(1)
来源：http://chy.yonumen.top

TS:   process.exit(1)
来源：http://idn.shzxlz.cn

Java: System.exit(1)
来源：http://kez.jinqigfzy.top

Go:   os.Exit(1)
来源：http://wfl.yuxming.cn

Ruby: exit 1
来源：http://ynw.nanxuanxn.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jyj.yanxiufei.cn

[M06] 向标准错误输出
来源：http://kep.nanxinkj.top

Py:   print("err", file=sys.stderr)
来源：http://trj.aizwys.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://snt.jqgufenzy.top

JS:   console.error("err")
来源：http://haq.0kj1m.cn

TS:   console.error("err")
来源：http://osb.hysaishi.cn

Java: System.err.println("err")
来源：http://ogz.yuanzhike.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://amm.gzhubu.top

Ruby: warn "err"
来源：http://odx.birdmap.top

C#:   Console.Error.WriteLine("err")
来源：http://ktg.shangyingyoupin.top

[M07] 判断是否为主入口
来源：http://vbs.guannengcc.top

Py:   if __name__ == "__main__":
来源：http://zcw.zhengqikj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aei.tianlin.xyz

JS:   require.main === module
来源：http://dgt.fengsongda.top

TS:   require.main === module
来源：http://haa.hnxiangtu.top

Java: public static void main(String[] args)
来源：http://yfo.tian-w.cn

Go:   func main()
来源：http://pzs.zhengqikj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ang.sweek.top

C#:   static void Main(string[] args)
来源：http://stq.iojbl.cn

[M08] 获取系统与运行时信息
来源：http://kiq.wangdashe.top

Py:   platform.system();  platform.python_version()
来源：http://jfo.sufxvd.cn

PHP:  PHP_OS;  phpversion();
来源：http://hrp.zhixingplan.top

JS:   process.platform;  process.version
来源：http://nwc.jqgfzy.top

TS:   process.platform;  process.version
来源：http://nau.shangyingyoupin.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vhk.daria6918.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gvq.guowangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://umm.tarul.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kpg.dianchejie.cn

================================================================================
来源：http://fel.xinyue.icu

N. 数据结构与算法
来源：http://syd.fanxiaobao.xyz

================================================================================
来源：http://eza.yanxiufei.cn

[N01] 二分查找（有序数组）
来源：http://iat.quarkkingdee.top

Py:   bisect.bisect_left(arr, x)
来源：http://eke.zycfv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nem.shangyingyoupin.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://acp.yongpay.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dva.cashguo.top

Java: Arrays.binarySearch(arr, x)
来源：http://svq.yuxming.cn

Go:   sort.SearchInts(arr, x)
来源：http://obg.gogol.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xpe.smart0.xyz


<!-- 参考信息 -->