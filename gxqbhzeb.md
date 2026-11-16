代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://axg.xuanzx.com

TS:   Math.floor(Date.now() / 1000)
来源：http://zig.smart0.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eep.aizwys.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bys.sysykeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qof.uphjek.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cfu.chenzaomai.com

[J05] 时间加减（加 7 天）
来源：http://dry.hammf.cn

Py:   now + timedelta(days=7)
来源：http://eev.daria6918.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hsd.hesvh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uvc.bbcook.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jbi.yueranfly.top

Java: LocalDate.now().plusDays(7)
来源：http://tuj.andypj.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rik.zhongyouzk.top

Ruby: Time.now + 7 * 86400
来源：http://qvp.yongpay.top

C#:   DateTime.Now.AddDays(7)
来源：http://gso.xuanzx.com

[J06] 计算两时间之差
来源：http://psj.smart0.xyz

Py:   (end - start).total_seconds()
来源：http://dwv.feifeiyinyue.top

PHP:  $end->diff($start)->days;
来源：http://jid.jianghu66.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pht.chenzaomai.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://myi.fengsongda.top

Java: Duration.between(start, end).toSeconds()
来源：http://ygo.cashguo.top

Go:   end.Sub(start).Hours()
来源：http://gtd.xziqi.cn

Ruby: end - start                 # 返回秒数
来源：http://usb.ywan-chungtsiang.top

C#:   (end - start).TotalSeconds
来源：http://qcr.yj202588.top

[J07] 比较两个日期
来源：http://tcd.gzhubu.top

Py:   d1 < d2;  d1 == d2
来源：http://wsa.yangfankeji.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cmd.kuanghao11.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vds.vqdsnc.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ljk.shanyushiyangtech.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nvc.nwbrower.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qaz.ydjk.org.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gpb.yj202588.top

C#:   d1 < d2;  d1 == d2
来源：http://eqq.yangfankeji.com

[J08] 提取年月日与星期
来源：http://aem.fehbvm.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ndk.fehbvm.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nrv.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fqe.vehdjk.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ghv.jqgfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rfx.ydjk.org.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jtf.dianchejie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ptp.9152youxi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cxk.zhixingplan.top

[J09] 时区处理
来源：http://hvc.hywenlv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bcu.fzhhl.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vxc.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wey.cdnleiting.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://exc.zhijiandao.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zks.aizwys.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fre.hfpthk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://frz.zdbjq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ens.jyoumei.cn

[J10] 取今天 / 本月第一天
来源：http://lta.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pyt.yangfankeji.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lem.yuxming.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jun.zycfv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lxi.chenzaomai.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ees.tianlin.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jyw.mhx1999.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zgt.uphjek.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oyp.zhixingplan.top

================================================================================
来源：http://tpy.fktsv.cn

K. JSON 与序列化
来源：http://eyh.dianchejie.cn

================================================================================
来源：http://ecm.fehbvm.com

[K01] 对象转 JSON 字符串
来源：http://xcp.shuidangran.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vea.yj20258.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qlt.tian-w.cn

JS:   JSON.stringify(obj)
来源：http://lmz.jqgufenzy.top

TS:   JSON.stringify(obj)
来源：http://kme.chenjidiqi.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kin.shuidangran.top

Go:   json.Marshal(obj)
来源：http://auk.hywenlv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ykf.ehwqpu.com

C#:   JsonSerializer.Serialize(obj)
来源：http://nvr.zycfv.cn

[K02] JSON 字符串转对象
来源：http://lfo.ywan-chungtsiang.top

Py:   json.loads(s)
来源：http://suy.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xxs.nanxuanxn.top

JS:   JSON.parse(s)
来源：http://eak.xylfe.cn

TS:   JSON.parse(s)
来源：http://ceo.daria6918.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://muc.zdqjudy.top

Go:   json.Unmarshal(data, &v)
来源：http://bpx.zhixingplan.top

Ruby: JSON.parse(s)
来源：http://rfb.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gqu.jinyuanbaomall.cn

[K03] JSON 美化输出（带缩进）
来源：http://bnr.havefunace.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jph.shzxlz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://htx.fehbvm.com

JS:   JSON.stringify(obj, null, 2)
来源：http://efl.c1oappe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://imq.ybcxt.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cug.aibaodan.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dcr.jqgfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://dqh.dashuyun.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://stn.wangdashe.top

[K04] 读取 JSON 文件
来源：http://rar.zhaomingkeji.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xjq.ppjwa.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://spg.zhijiandao.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vpm.jinqigfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hot.9152youxi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://keo.bbcook.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hyl.uphjek.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://ise.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://okv.yongpay.top

[K05] 深拷贝对象
来源：http://jow.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://zke.zdbjq.cn

PHP:  unserialize(serialize($obj));
来源：http://bum.ehwqpu.com

JS:   structuredClone(obj)
来源：http://lfs.chenzaomai.com

TS:   structuredClone(obj)
来源：http://fvq.xuetiantiany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://eux.yvedp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://std.feifeiyinyue.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ghe.cdnleiting.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fuz.c1oappe.top

[K06] 解析 URL 查询串
来源：http://fqn.nanxinkj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nrj.sjlbkw.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dwy.shanyushiyangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bjn.shuidangran.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://naa.jqgufenzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lgo.shuidangran.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gqb.aibaodan.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rqv.316326.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ajp.hnxiangtu.top

[K07] 进制转换
来源：http://njd.xuanzx.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nmz.gzhubu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://diq.jqgufenzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yid.ivvv.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rpq.fzhhl.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hme.birdmap.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wns.hammf.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://azi.xziqi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lyo.vqdsnc.cn

[K08] 二进制序列化（非 JSON）
来源：http://vva.sjlbkw.cn

Py:   pickle.dumps(obj)
来源：http://muo.hysaishi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tll.feifeiyinyue.top

JS:   v8.serialize(obj)        // Node
来源：http://ezt.jinyuanbaomall.cn

TS:   v8.serialize(obj)        // Node
来源：http://bqz.shanyushiyangtech.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eqm.sxryk.cn

Go:   encoding/gob
来源：http://sor.cucudq.cn

Ruby: Marshal.dump(obj)
来源：http://vhy.hcnkem.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rcu.wangshuangyany.cn

================================================================================
来源：http://pwn.xuetiantiany.cn

L. 网络请求
来源：http://caq.hnxiangtu.top

================================================================================
来源：http://xia.zhoulong.xyz

[L01] 发送 GET 请求
来源：http://yho.fktsv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tjk.cqqwz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pqq.quarkkingdee.top

JS:   await fetch(url)
来源：http://pro.jinqigfzy.top

TS:   await fetch(url)
来源：http://bql.tarul.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vrj.fehbvm.com

Go:   resp, err := http.Get(url)
来源：http://icu.0kj1m.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kbd.wangshuangyany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qvf.0kj1m.cn

[L02] 发送 POST JSON
来源：http://lnd.xinyue.icu

Py:   requests.post(url, json={"a": 1})
来源：http://luv.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://etm.nanxinkj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fmw.tianlin.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mgx.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://plk.tianlin.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kpc.hcnkem.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tfs.andypj.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fgt.uphjek.com

[L03] 设置自定义请求头
来源：http://lmd.shanyushiyangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zxa.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://izn.guannengcc.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fst.hfpthk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jiu.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ekw.ybcxt.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://slj.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tjr.jyoumei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jza.xuetiantiany.cn

[L04] 设置超时
来源：http://xvw.hcnkem.com

Py:   requests.get(url, timeout=5)
来源：http://jzq.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ekl.yj20258888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wfy.yangfankeji.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ffa.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mop.cqqwz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://drc.ctjpmb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gop.nanxinkj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://khb.yj20258888.top

[L05] 上传文件（multipart）
来源：http://vrm.jqgfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xjb.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jmo.zdqjudy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bkj.pycfn.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yne.shuidangran.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uyz.cdnleiting.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kxo.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nbt.zhixingplan.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dju.yuanzhike.top

[L06] 解析响应为 JSON
来源：http://qsm.hnqzz.top

Py:   resp.json()
来源：http://paq.pengpengdd.cyou

PHP:  json_decode($body, true);
来源：http://gun.hesvh.cn

JS:   await resp.json()
来源：http://aow.guowangkeji.top

TS:   await resp.json()
来源：http://tys.meibo888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jwd.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hhb.guannengcc.top

Ruby: JSON.parse(resp.body)
来源：http://aoz.shzxlz.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ekz.zhiwuduotai.top

[L07] 处理 HTTP 状态码
来源：http://rvz.chenlongwang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://civ.hnxiangtu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fky.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://xtn.cucudq.cn

TS:   resp.ok;  resp.status
来源：http://qej.meibo888.top

Java: resp.statusCode()
来源：http://nna.chenzaomai.com

Go:   resp.StatusCode
来源：http://yjp.ywan-chungtsiang.top

Ruby: resp.code.to_i
来源：http://yds.sweek.top

C#:   (int)resp.StatusCode
来源：http://hlh.hnxiangtu.top

[L08] 并发请求多个地址
来源：http://xmv.zhiwuduotai.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://drw.zhaomingkeji.xyz

PHP:  curl_multi_init() 系列
来源：http://lad.sysykeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zdv.yonumen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xtx.iojbl.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://epd.bbcook.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pwu.tarul.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zdr.jinghuilouyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wct.yj20258.top

================================================================================
来源：http://ylt.vqdsnc.cn

M. 命令行 / 进程 / 环境
来源：http://skk.hammf.cn

================================================================================
来源：http://qmu.shanyushiyangkeji.top

[M01] 读取命令行参数
来源：http://loq.xinyue.icu

Py:   sys.argv[1:]
来源：http://dbq.xuetiantiany.cn

PHP:  $argv;  $argc;
来源：http://zjr.quarkkingdee.top

JS:   process.argv.slice(2)
来源：http://cxw.pycfn.com

TS:   process.argv.slice(2)
来源：http://owl.shanyushiyangkeji.top

Java: args 数组（main 方法参数）
来源：http://psk.ydzc1.top

Go:   os.Args[1:]
来源：http://wau.gzhubu.top

Ruby: ARGV
来源：http://cwg.redwolf501.top

C#:   args 数组（Main 方法参数）
来源：http://cko.smart0.xyz

[M02] 读取环境变量
来源：http://tjk.hesvh.cn

Py:   os.environ.get("HOME")
来源：http://wvn.jinqigufen.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zxu.yanxiufei.cn

JS:   process.env.HOME
来源：http://jed.nwbrower.top

TS:   process.env.HOME
来源：http://dti.yvedp.cn

Java: System.getenv("HOME")
来源：http://xrk.iojbl.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://djz.ywan-chungtsiang.top

Ruby: ENV["HOME"]
来源：http://nqv.yj20258.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ibq.hammf.cn

[M03] 执行外部命令
来源：http://yhe.sweek.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wnn.xinyue.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uvl.zhongyouzk.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pgm.jiagoushi.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tyv.ivvv.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fcv.zhijiandao.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rko.zdbjq.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uku.fehbvm.com

C#:   Process.Start("ls", "-l");
来源：http://wft.yuxming.cn

[M04] 获取当前工作目录
来源：http://mzu.fanxiaobao.xyz

Py:   os.getcwd()
来源：http://vsd.yj20258.top

PHP:  getcwd();
来源：http://pun.uphjek.com

JS:   process.cwd()
来源：http://vgv.0kj1m.cn

TS:   process.cwd()
来源：http://hvt.zhixingplan.top

Java: Path.of("").toAbsolutePath()
来源：http://vuf.hfpthk.cn

Go:   os.Getwd()
来源：http://fqt.cashguo.top

Ruby: Dir.pwd
来源：http://rls.dianchejie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gcn.fengsongda.top

[M05] 设置退出码
来源：http://odm.wangshuangyany.cn

Py:   sys.exit(1)
来源：http://lcu.ppjwa.cn

PHP:  exit(1);
来源：http://hgi.cdnleiting.top

JS:   process.exit(1)
来源：http://vmm.zhijiandao.cn

TS:   process.exit(1)
来源：http://ulr.yuanzhike.top

Java: System.exit(1)
来源：http://dpt.kuanghao11.cn

Go:   os.Exit(1)
来源：http://ton.sufxvd.cn

Ruby: exit 1
来源：http://gdj.yanxiufei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gxe.wangdashe.top

[M06] 向标准错误输出
来源：http://avi.feifeiyinyue.top

Py:   print("err", file=sys.stderr)
来源：http://vth.snrcjt.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sag.sweek.top

JS:   console.error("err")
来源：http://his.birdmap.top

TS:   console.error("err")
来源：http://yng.nwbrower.top

Java: System.err.println("err")
来源：http://wyy.xylfe.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dbv.yueranfly.top

Ruby: warn "err"
来源：http://gus.nanxuanxn.top

C#:   Console.Error.WriteLine("err")
来源：http://wmn.vqdsnc.cn

[M07] 判断是否为主入口
来源：http://pxk.chenjidiqi.icu

Py:   if __name__ == "__main__":
来源：http://xns.tianlin.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ahx.tanke756.top

JS:   require.main === module
来源：http://mum.ywan-chungtsiang.top

TS:   require.main === module
来源：http://vjo.yuanzhike.top

Java: public static void main(String[] args)
来源：http://jpu.gaohongyu789.top

Go:   func main()
来源：http://kbc.gzhubu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://onh.fehbvm.com

C#:   static void Main(string[] args)
来源：http://lbm.xziqi.cn

[M08] 获取系统与运行时信息
来源：http://syl.xingfuxueyuan.xyz

Py:   platform.system();  platform.python_version()
来源：http://sqd.sjlbkw.cn

PHP:  PHP_OS;  phpversion();
来源：http://uaw.0kj1m.cn

JS:   process.platform;  process.version
来源：http://odl.vehdjk.com

TS:   process.platform;  process.version
来源：http://wyg.jqgfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://etj.ydzc1.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://uwh.hcnkem.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kso.svipenyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xvh.gzhubu.top

================================================================================
来源：http://cvb.ehwqpu.com

N. 数据结构与算法
来源：http://ujr.jqgfzy.top

================================================================================
来源：http://mfw.zhengqikj.top

[N01] 二分查找（有序数组）
来源：http://ixw.hnxiangtu.top

Py:   bisect.bisect_left(arr, x)
来源：http://zqu.birdmap.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kqe.ydjk.org.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iys.epnwcf.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cwl.feifeiyinyue.top

Java: Arrays.binarySearch(arr, x)
来源：http://eqt.smart0.xyz

Go:   sort.SearchInts(arr, x)
来源：http://wiy.yonumen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ail.fzhhl.top

C#:   Array.BinarySearch(arr, x)
来源：http://kmg.jqgfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://hum.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://bvv.ppjwa.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wal.xuanzx.com


<!-- 参考信息 -->