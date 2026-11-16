代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://htn.xuanzx.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xfx.316326.xyz

[J05] 时间加减（加 7 天）
来源：http://vdr.yuanzhike.top

Py:   now + timedelta(days=7)
来源：http://dri.52xcode.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kym.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xbs.mhx1999.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ekl.kuanghao11.cn

Java: LocalDate.now().plusDays(7)
来源：http://uff.cheryme.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jpn.uphjek.com

Ruby: Time.now + 7 * 86400
来源：http://zsp.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://wof.zhixingplan.top

[J06] 计算两时间之差
来源：http://kfo.tanke756.top

Py:   (end - start).total_seconds()
来源：http://dya.daria6918.cn

PHP:  $end->diff($start)->days;
来源：http://lws.iojbl.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gkl.epnwcf.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tjk.hysaishi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://quq.jinqigufen.top

Go:   end.Sub(start).Hours()
来源：http://tmf.ydzc1.top

Ruby: end - start                 # 返回秒数
来源：http://gfg.zhijiandao.cn

C#:   (end - start).TotalSeconds
来源：http://cla.tarul.cn

[J07] 比较两个日期
来源：http://geu.shanyushiyangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://hmc.hnqzz.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jug.zycfv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nlk.c1oappe.top

TS:   d1.getTime() < d2.getTime()
来源：http://xhs.yanxiufei.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cjn.mhx1999.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vkc.yj20258888.top

Ruby: d1 < d2;  d1 == d2
来源：http://wkc.jinyuanbaomall.cn

C#:   d1 < d2;  d1 == d2
来源：http://djc.sxryk.cn

[J08] 提取年月日与星期
来源：http://qlj.ivvv.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zkz.fanxiaobao.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sbb.yongpay.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pkj.wangshuangyany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kuv.xuetiantiany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xof.hnxiangtu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xdq.yuanzhike.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bwe.andypj.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uqb.shanyushiyangkeji.top

[J09] 时区处理
来源：http://bne.daxiang520.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dpv.shzxlz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://crz.gzhubu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ixk.zdbjq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cdg.xuetiantiany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cyb.gaohongyu789.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iha.iojbl.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rjx.yangfankeji.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fcx.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://egg.iojbl.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vpq.chenlongwang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ejk.yanxiufei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ejk.jinghuilouyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vtm.gotoacloud.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qew.zhaomingkeji.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mtr.redwolf501.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nap.hywenlv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://crg.wangshuangyany.cn

================================================================================
来源：http://gcr.andypj.xyz

K. JSON 与序列化
来源：http://ukm.xuetiantiany.cn

================================================================================
来源：http://zej.316326.xyz

[K01] 对象转 JSON 字符串
来源：http://xvu.redwolf501.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://onb.ivvv.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mjs.feifeiyinyue.top

JS:   JSON.stringify(obj)
来源：http://bul.yvedp.cn

TS:   JSON.stringify(obj)
来源：http://qjs.jinqigfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lkj.yvedp.cn

Go:   json.Marshal(obj)
来源：http://lqb.zhongyouzk.top

Ruby: obj.to_json                                     // require "json"
来源：http://etg.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj)
来源：http://njk.zhoulong.xyz

[K02] JSON 字符串转对象
来源：http://zua.kuanghao11.cn

Py:   json.loads(s)
来源：http://mxq.yonumen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lgx.quarkkingdee.top

JS:   JSON.parse(s)
来源：http://lyl.xylfe.cn

TS:   JSON.parse(s)
来源：http://gry.tianlin.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tlx.hnqzz.top

Go:   json.Unmarshal(data, &v)
来源：http://ghm.quarkkingdee.top

Ruby: JSON.parse(s)
来源：http://cjz.yuanzhike.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://twk.dashuyun.cn

[K03] JSON 美化输出（带缩进）
来源：http://ztg.bbcook.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wvt.gogol.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kgx.ydjk.org.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fwl.jqgfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zsv.pycfn.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://odl.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oqk.yonumen.top

Ruby: JSON.pretty_generate(obj)
来源：http://uyh.snrcjt.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qll.dashuyun.cn

[K04] 读取 JSON 文件
来源：http://ufw.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nnq.zdbjq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rft.redwolf501.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pmd.zhaomingkeji.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fwo.epnwcf.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://std.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gur.zdbjq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xpm.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zky.9152youxi.cn

[K05] 深拷贝对象
来源：http://cun.hywenlv.cn

Py:   copy.deepcopy(obj)
来源：http://cff.chenjidiqi.icu

PHP:  unserialize(serialize($obj));
来源：http://lxa.cqqwz.cn

JS:   structuredClone(obj)
来源：http://izb.ctjpmb.com

TS:   structuredClone(obj)
来源：http://bgo.iojbl.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nli.shangyingyoupin.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://die.chenlongwang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bpt.pengpengdd.cyou

C#:   // 序列化往返，或自定义 Clone
来源：http://svg.tianlin.xyz

[K06] 解析 URL 查询串
来源：http://frf.yj20258.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zkd.hongshengwenyu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://adj.chenlongwang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gdw.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pvp.xziqi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://byt.fanxiaobao.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://hho.xziqi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xep.yuxming.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cwc.zdqjudy.top

[K07] 进制转换
来源：http://suo.ehwqpu.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fmg.fktsv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mbg.ywan-chungtsiang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://drx.gotoacloud.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rwn.jinqigufen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ojj.smart0.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bkq.ywan-chungtsiang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xao.shuidangran.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bcc.quarkkingdee.top

[K08] 二进制序列化（非 JSON）
来源：http://ril.yj202588.top

Py:   pickle.dumps(obj)
来源：http://jxr.yuanzhike.top

PHP:  serialize($obj);  unserialize($s);
来源：http://eyv.andypj.xyz

JS:   v8.serialize(obj)        // Node
来源：http://vhi.bjfxy.top

TS:   v8.serialize(obj)        // Node
来源：http://wvw.smart0.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tah.vehdjk.com

Go:   encoding/gob
来源：http://efo.jinyuanbaomall.cn

Ruby: Marshal.dump(obj)
来源：http://knt.yfazqb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mqz.jqgfzy.top

================================================================================
来源：http://qxx.tianlin.xyz

L. 网络请求
来源：http://uwh.gogol.net.cn

================================================================================
来源：http://wdy.snrcjt.cn

[L01] 发送 GET 请求
来源：http://jrn.cashguo.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pmu.zhongyouzk.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cvq.jlsjyb.cn

JS:   await fetch(url)
来源：http://cxj.tian-w.cn

TS:   await fetch(url)
来源：http://uep.ehwqpu.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xes.cqqwz.cn

Go:   resp, err := http.Get(url)
来源：http://fup.ydzc1.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dyf.yonumen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bpz.jinqigufen.top

[L02] 发送 POST JSON
来源：http://nzn.ydzc1.top

Py:   requests.post(url, json={"a": 1})
来源：http://ypk.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gpm.iojbl.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nlq.ehwqpu.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://drl.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gva.shzxlz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hop.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fru.sufxvd.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zle.cucudq.cn

[L03] 设置自定义请求头
来源：http://ida.cheryme.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pct.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gxx.wangshuangyany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zqp.yj20258888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yqa.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blw.hfpthk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tkr.havefunace.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gdm.epnwcf.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uxk.xylfe.cn

[L04] 设置超时
来源：http://mxe.jinghuilouyu.cn

Py:   requests.get(url, timeout=5)
来源：http://bql.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dve.shzxlz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kxt.dashuyun.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zkc.xinyue.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gyb.hfpthk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wfc.ybcxt.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qpx.sufxvd.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ajq.sjlbkw.cn

[L05] 上传文件（multipart）
来源：http://jvk.pycfn.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xjr.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://evi.daxiang520.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qdf.cdnleiting.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fsn.shuidangran.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vat.fzhhl.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://skn.sjlbkw.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hvy.yuxming.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ovw.316326.xyz

[L06] 解析响应为 JSON
来源：http://gqp.yuxming.cn

Py:   resp.json()
来源：http://vri.uphjek.com

PHP:  json_decode($body, true);
来源：http://wnz.birdmap.top

JS:   await resp.json()
来源：http://mup.nwbrower.top

TS:   await resp.json()
来源：http://ksq.sjlbkw.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lnd.cqqwz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ccj.dashuyun.cn

Ruby: JSON.parse(resp.body)
来源：http://kao.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fqk.hfpthk.cn

[L07] 处理 HTTP 状态码
来源：http://lem.yfazqb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xrh.hcnkem.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qoy.fktsv.cn

JS:   resp.ok;  resp.status
来源：http://rqe.bbcook.cn

TS:   resp.ok;  resp.status
来源：http://vxq.yj20258888.top

Java: resp.statusCode()
来源：http://xnr.c1oappe.top

Go:   resp.StatusCode
来源：http://xwk.andypj.xyz

Ruby: resp.code.to_i
来源：http://tba.mhx1999.top

C#:   (int)resp.StatusCode
来源：http://klr.xuetiantiany.cn

[L08] 并发请求多个地址
来源：http://jnt.gzhubu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://asa.cheryme.top

PHP:  curl_multi_init() 系列
来源：http://loe.9152youxi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wsm.mhx1999.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rum.chenlongwang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oem.jinqigfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kgq.fengsongda.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vyq.ydjk.org.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ibr.fanxiaobao.xyz

================================================================================
来源：http://zgx.fengsongda.top

M. 命令行 / 进程 / 环境
来源：http://uay.sjlbkw.cn

================================================================================
来源：http://rsv.nanxinkj.top

[M01] 读取命令行参数
来源：http://ops.gogol.net.cn

Py:   sys.argv[1:]
来源：http://vbx.shuidangran.top

PHP:  $argv;  $argc;
来源：http://nxd.nwbrower.top

JS:   process.argv.slice(2)
来源：http://sgr.zhengqikj.top

TS:   process.argv.slice(2)
来源：http://ykw.yueranfly.top

Java: args 数组（main 方法参数）
来源：http://xgm.svipenyu.cn

Go:   os.Args[1:]
来源：http://kah.shuidangran.top

Ruby: ARGV
来源：http://yji.316326.xyz

C#:   args 数组（Main 方法参数）
来源：http://orv.yuanzhike.top

[M02] 读取环境变量
来源：http://gip.zhengqikj.top

Py:   os.environ.get("HOME")
来源：http://rjl.jinyuanbaomall.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vej.hywenlv.cn

JS:   process.env.HOME
来源：http://lku.shangyingyoupin.top

TS:   process.env.HOME
来源：http://zyc.yj202588.top

Java: System.getenv("HOME")
来源：http://cmo.shzxlz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dgx.ydzc1.top

Ruby: ENV["HOME"]
来源：http://bkv.xuetiantiany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jzc.uphjek.com

[M03] 执行外部命令
来源：http://gwh.xuanzx.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://orw.hysaishi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hcu.bjfxy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tiw.cdnleiting.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xfe.yangfankeji.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kuz.nanxuanxn.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ymd.ydzc1.top

Ruby: system("ls -l");  `ls -l`
来源：http://oqs.cashguo.top

C#:   Process.Start("ls", "-l");
来源：http://mdh.shzxlz.cn

[M04] 获取当前工作目录
来源：http://nuy.yvedp.cn

Py:   os.getcwd()
来源：http://aps.zhaomingkeji.xyz

PHP:  getcwd();
来源：http://wqz.zdbjq.cn

JS:   process.cwd()
来源：http://nrb.hnqzz.top

TS:   process.cwd()
来源：http://fqi.jqgfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://jyc.ydzc1.top

Go:   os.Getwd()
来源：http://tlr.ehwqpu.com

Ruby: Dir.pwd
来源：http://rfc.ybcxt.top

C#:   Directory.GetCurrentDirectory()
来源：http://dkh.yongpay.top

[M05] 设置退出码
来源：http://qth.fanxiaobao.xyz

Py:   sys.exit(1)
来源：http://cxh.uphjek.com

PHP:  exit(1);
来源：http://sfj.fehbvm.com

JS:   process.exit(1)
来源：http://sft.vqdsnc.cn

TS:   process.exit(1)
来源：http://err.hnxiangtu.top

Java: System.exit(1)
来源：http://jsb.jianghu66.top

Go:   os.Exit(1)
来源：http://hma.jinqigfzy.top

Ruby: exit 1
来源：http://inp.havefunace.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zfz.birdmap.top

[M06] 向标准错误输出
来源：http://hfe.kuanghao11.cn

Py:   print("err", file=sys.stderr)
来源：http://wmw.hnqzz.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ftg.hfpthk.cn

JS:   console.error("err")
来源：http://bom.cucudq.cn

TS:   console.error("err")
来源：http://apg.yangfankeji.com

Java: System.err.println("err")
来源：http://sjz.ywan-chungtsiang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://awp.cheryme.top

Ruby: warn "err"
来源：http://dwp.ctjpmb.com

C#:   Console.Error.WriteLine("err")
来源：http://tab.fengsongda.top

[M07] 判断是否为主入口
来源：http://zrv.shanyushiyangtech.top

Py:   if __name__ == "__main__":
来源：http://mcx.tanke756.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lia.sysykeji.top

JS:   require.main === module
来源：http://quh.havefunace.top

TS:   require.main === module
来源：http://knt.hammf.cn

Java: public static void main(String[] args)
来源：http://tdp.hfpthk.cn

Go:   func main()
来源：http://drq.yuxming.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://han.hywenlv.cn

C#:   static void Main(string[] args)
来源：http://mat.svipenyu.cn

[M08] 获取系统与运行时信息
来源：http://dga.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://ggn.cucudq.cn

PHP:  PHP_OS;  phpversion();
来源：http://uhi.ivvv.top

JS:   process.platform;  process.version
来源：http://tcw.wangdashe.top

TS:   process.platform;  process.version
来源：http://prn.snrcjt.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://but.daria6918.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://oyz.sjlbkw.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fpp.xziqi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mon.nwbrower.top

================================================================================
来源：http://qma.c1oappe.top

N. 数据结构与算法
来源：http://lsp.zhixingplan.top

================================================================================
来源：http://sxi.xziqi.cn

[N01] 二分查找（有序数组）
来源：http://dux.0kj1m.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ipv.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hpa.yuanzhike.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zyw.ctjpmb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hvv.bbcook.cn

Java: Arrays.binarySearch(arr, x)
来源：http://eej.fktsv.cn

Go:   sort.SearchInts(arr, x)
来源：http://uqh.tianlin.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://mmy.c1oappe.top

C#:   Array.BinarySearch(arr, x)
来源：http://ezg.xuanzx.com

[N02] 排序（工程实践用内置实现）
来源：http://cwq.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://kdo.yfazqb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lqa.yj20258.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://gbj.kuanghao11.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mzt.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pxb.kuanghao11.cn

Go:   slices.Sort(arr)
来源：http://bzp.vehdjk.com


<!-- 参考信息 -->