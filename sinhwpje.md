代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ect.zhoulong.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cch.tianlin.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wec.fzhhl.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://chg.zhaomingkeji.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sqq.yvedp.cn

[J05] 时间加减（加 7 天）
来源：http://mgt.zhixingplan.top

Py:   now + timedelta(days=7)
来源：http://ycx.jianghu66.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://glt.xziqi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://emn.cucudq.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vbj.hnqzz.top

Java: LocalDate.now().plusDays(7)
来源：http://orm.iojbl.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://awc.sweek.top

Ruby: Time.now + 7 * 86400
来源：http://mhq.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://qdm.cashguo.top

[J06] 计算两时间之差
来源：http://hpn.nanxuanxn.top

Py:   (end - start).total_seconds()
来源：http://iwh.cucudq.cn

PHP:  $end->diff($start)->days;
来源：http://yiy.yonumen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cpb.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://brj.cashguo.top

Java: Duration.between(start, end).toSeconds()
来源：http://imk.birdmap.top

Go:   end.Sub(start).Hours()
来源：http://ktp.0kj1m.cn

Ruby: end - start                 # 返回秒数
来源：http://ruz.sjlbkw.cn

C#:   (end - start).TotalSeconds
来源：http://jss.zhoulong.xyz

[J07] 比较两个日期
来源：http://fvb.zdbjq.cn

Py:   d1 < d2;  d1 == d2
来源：http://ces.jiagoushi.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://deh.hnxiangtu.top

JS:   d1.getTime() < d2.getTime()
来源：http://fcj.jyoumei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ydc.pengpengdd.cyou

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tdk.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://afn.xuetiantiany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://moi.xylfe.cn

C#:   d1 < d2;  d1 == d2
来源：http://uzn.hongshengwenyu.top

[J08] 提取年月日与星期
来源：http://nsf.mhx1999.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://flb.gogol.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rvf.9152youxi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xxb.zdqjudy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yxx.jyoumei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://saf.ydjk.org.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vtl.hammf.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://asu.sysykeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zpf.jinqigfzy.top

[J09] 时区处理
来源：http://aej.sweek.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xcx.shangyingyoupin.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qfb.gzhubu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aep.chenzaomai.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yai.cdnleiting.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://czp.0kj1m.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kkp.shzxlz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yos.yangfankeji.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nca.feifeiyinyue.top

[J10] 取今天 / 本月第一天
来源：http://ser.0kj1m.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://deh.meibo888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mfn.sjlbkw.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nrr.chenzaomai.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mob.sjlbkw.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nwl.ctjpmb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rqx.cdnleiting.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nty.yueranfly.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rrw.nanxuanxn.top

================================================================================
来源：http://ohr.xuetiantiany.cn

K. JSON 与序列化
来源：http://rdk.yanxiufei.cn

================================================================================
来源：http://asj.quarkkingdee.top

[K01] 对象转 JSON 字符串
来源：http://xni.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wgj.hnxiangtu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kms.mhx1999.top

JS:   JSON.stringify(obj)
来源：http://ely.gotoacloud.top

TS:   JSON.stringify(obj)
来源：http://wzl.birdmap.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ral.nanxinkj.top

Go:   json.Marshal(obj)
来源：http://doe.birdmap.top

Ruby: obj.to_json                                     // require "json"
来源：http://dix.epnwcf.com

C#:   JsonSerializer.Serialize(obj)
来源：http://kwl.jqgfzy.top

[K02] JSON 字符串转对象
来源：http://bjw.daxiang520.top

Py:   json.loads(s)
来源：http://upa.shanyushiyangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yir.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://yxh.dianchejie.cn

TS:   JSON.parse(s)
来源：http://vnf.epnwcf.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ubr.hysaishi.cn

Go:   json.Unmarshal(data, &v)
来源：http://adc.fehbvm.com

Ruby: JSON.parse(s)
来源：http://kef.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tjy.tianlin.xyz

[K03] JSON 美化输出（带缩进）
来源：http://waq.ybcxt.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://prt.ydjk.org.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wrt.dashuyun.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://phv.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nai.vehdjk.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://not.sysykeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kzm.tanke756.top

Ruby: JSON.pretty_generate(obj)
来源：http://tdk.chenlongwang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uze.hnxiangtu.top

[K04] 读取 JSON 文件
来源：http://udh.xuetiantiany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dyn.c1oappe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://egu.pycfn.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jtn.nanxinkj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jdv.daxiang520.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ysm.hesvh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ipw.tianlin.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://utx.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dgl.jiagoushi.top

[K05] 深拷贝对象
来源：http://ozi.fzhhl.top

Py:   copy.deepcopy(obj)
来源：http://jtz.chenjidiqi.icu

PHP:  unserialize(serialize($obj));
来源：http://osi.zhoulong.xyz

JS:   structuredClone(obj)
来源：http://tjs.zhongyouzk.top

TS:   structuredClone(obj)
来源：http://zfm.aibaodan.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jpa.guowangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bwo.jyoumei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bzu.yuxming.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rjm.zhongyouzk.top

[K06] 解析 URL 查询串
来源：http://dor.yangfankeji.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sxd.birdmap.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://osv.tarul.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rsw.vehdjk.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dld.ehwqpu.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gdk.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mkl.hongshengwenyu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hqh.ydzc1.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jgw.xylfe.cn

[K07] 进制转换
来源：http://ojd.aizwys.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tds.yuxming.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ean.cdnleiting.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ipq.dianchejie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xjt.sjlbkw.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uqn.jinqigufen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dpl.jiagoushi.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uie.xinyue.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://itv.tianlin.xyz

[K08] 二进制序列化（非 JSON）
来源：http://qgh.hysaishi.cn

Py:   pickle.dumps(obj)
来源：http://zjs.yuanzhike.top

PHP:  serialize($obj);  unserialize($s);
来源：http://khy.hnqzz.top

JS:   v8.serialize(obj)        // Node
来源：http://sne.yanxiufei.cn

TS:   v8.serialize(obj)        // Node
来源：http://xrc.cqqwz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qip.fktsv.cn

Go:   encoding/gob
来源：http://rqw.yvedp.cn

Ruby: Marshal.dump(obj)
来源：http://fce.nwbrower.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tqs.andypj.xyz

================================================================================
来源：http://tij.zhaomingkeji.xyz

L. 网络请求
来源：http://tez.aibaodan.cn

================================================================================
来源：http://ful.yanxiufei.cn

[L01] 发送 GET 请求
来源：http://oqr.316326.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kfi.yj20258.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ctj.daria6918.cn

JS:   await fetch(url)
来源：http://jsp.ydjk.org.cn

TS:   await fetch(url)
来源：http://cpj.shuidangran.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pij.sysykeji.top

Go:   resp, err := http.Get(url)
来源：http://eqh.cucudq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dmj.yangfankeji.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yma.ywan-chungtsiang.top

[L02] 发送 POST JSON
来源：http://dym.zhaomingkeji.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://xgo.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://imp.meibo888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gdn.hysaishi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jie.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://phh.shzxlz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://axl.chenjidiqi.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vps.yuanzhike.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xwk.gotoacloud.top

[L03] 设置自定义请求头
来源：http://vny.iojbl.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://akq.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hof.haohaochexian.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bbk.xylfe.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://twc.yj20258.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nah.gotoacloud.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kab.ydjk.org.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ozw.yueranfly.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bai.jlsjyb.cn

[L04] 设置超时
来源：http://rnd.0kj1m.cn

Py:   requests.get(url, timeout=5)
来源：http://ckr.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://iqd.shanyushiyangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nnj.yj20258.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ukk.tarul.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dcg.ywan-chungtsiang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dsd.yanxiufei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ihd.cashguo.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vsv.dashuyun.cn

[L05] 上传文件（multipart）
来源：http://adr.guowangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://suf.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://veu.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pwl.sufxvd.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vra.zhoulong.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ljs.yfazqb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mkq.hnqzz.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oef.hnqzz.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xje.yvedp.cn

[L06] 解析响应为 JSON
来源：http://eno.quarkkingdee.top

Py:   resp.json()
来源：http://qin.jinqigufen.top

PHP:  json_decode($body, true);
来源：http://cfq.shanyushiyangkeji.top

JS:   await resp.json()
来源：http://lol.daria6918.cn

TS:   await resp.json()
来源：http://btl.quarkkingdee.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pgw.ppjwa.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wjk.gogol.net.cn

Ruby: JSON.parse(resp.body)
来源：http://azo.gogol.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zwl.sysykeji.top

[L07] 处理 HTTP 状态码
来源：http://qax.chenzaomai.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mgy.cheryme.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ybn.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://fur.zdqjudy.top

TS:   resp.ok;  resp.status
来源：http://cwk.redwolf501.top

Java: resp.statusCode()
来源：http://rsz.zdqjudy.top

Go:   resp.StatusCode
来源：http://mlx.andypj.xyz

Ruby: resp.code.to_i
来源：http://bbh.daxiang520.top

C#:   (int)resp.StatusCode
来源：http://mun.zhengqikj.top

[L08] 并发请求多个地址
来源：http://frg.hysaishi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mnh.tian-w.cn

PHP:  curl_multi_init() 系列
来源：http://iug.smart0.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fnp.hcnkem.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ozi.hongshengwenyu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mrr.aibaodan.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hdp.tianlin.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qdu.yuxming.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://npu.cqqwz.cn

================================================================================
来源：http://bjk.cheryme.top

M. 命令行 / 进程 / 环境
来源：http://jkx.pengpengdd.cyou

================================================================================
来源：http://vmj.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://twy.shanyushiyangkeji.top

Py:   sys.argv[1:]
来源：http://rgs.zhoulong.xyz

PHP:  $argv;  $argc;
来源：http://odr.vehdjk.com

JS:   process.argv.slice(2)
来源：http://zqc.havefunace.top

TS:   process.argv.slice(2)
来源：http://nrq.xuanzx.com

Java: args 数组（main 方法参数）
来源：http://mlo.snrcjt.cn

Go:   os.Args[1:]
来源：http://hkw.aibaodan.cn

Ruby: ARGV
来源：http://nlg.ctjpmb.com

C#:   args 数组（Main 方法参数）
来源：http://jfe.ybcxt.top

[M02] 读取环境变量
来源：http://fem.ehwqpu.com

Py:   os.environ.get("HOME")
来源：http://aoy.kuanghao11.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xkg.chenzaomai.com

JS:   process.env.HOME
来源：http://bzw.zhaomingkeji.xyz

TS:   process.env.HOME
来源：http://qxg.ywan-chungtsiang.top

Java: System.getenv("HOME")
来源：http://mnh.jlsjyb.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rrt.jianghu66.top

Ruby: ENV["HOME"]
来源：http://qpt.fzhhl.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ulx.iojbl.cn

[M03] 执行外部命令
来源：http://wiv.aibaodan.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fld.hongshengwenyu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lvv.jinqigfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rnt.zdqjudy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bdc.yuxming.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rzl.jinghuilouyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://eqi.gogol.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mth.xingfuxueyuan.xyz

C#:   Process.Start("ls", "-l");
来源：http://hey.yj20258888.top

[M04] 获取当前工作目录
来源：http://fuo.zhiwuduotai.top

Py:   os.getcwd()
来源：http://lcw.hammf.cn

PHP:  getcwd();
来源：http://sii.jianghu66.top

JS:   process.cwd()
来源：http://buu.xinyue.icu

TS:   process.cwd()
来源：http://utj.tianlin.xyz

Java: Path.of("").toAbsolutePath()
来源：http://huk.gaohongyu789.top

Go:   os.Getwd()
来源：http://nty.guowangkeji.top

Ruby: Dir.pwd
来源：http://bvx.tianlin.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://ltr.andypj.xyz

[M05] 设置退出码
来源：http://ywe.jinqigufen.top

Py:   sys.exit(1)
来源：http://fuh.jqgfzy.top

PHP:  exit(1);
来源：http://qkg.0kj1m.cn

JS:   process.exit(1)
来源：http://fwq.tian-w.cn

TS:   process.exit(1)
来源：http://dek.zhixingplan.top

Java: System.exit(1)
来源：http://wlw.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://sqk.jqgfzy.top

Ruby: exit 1
来源：http://kom.yuanzhike.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eqz.jlsjyb.cn

[M06] 向标准错误输出
来源：http://ykx.tian-w.cn

Py:   print("err", file=sys.stderr)
来源：http://xrs.jlsjyb.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://znj.zhoulong.xyz

JS:   console.error("err")
来源：http://gkt.kuanghao11.cn

TS:   console.error("err")
来源：http://fuo.havefunace.top

Java: System.err.println("err")
来源：http://lvj.xziqi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xkr.ivvv.top

Ruby: warn "err"
来源：http://xru.zdbjq.cn

C#:   Console.Error.WriteLine("err")
来源：http://zlk.quarkkingdee.top

[M07] 判断是否为主入口
来源：http://shh.shzxlz.cn

Py:   if __name__ == "__main__":
来源：http://vln.jinqigufen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rrl.guannengcc.top

JS:   require.main === module
来源：http://fky.shangyingyoupin.top

TS:   require.main === module
来源：http://llo.andypj.xyz

Java: public static void main(String[] args)
来源：http://vtb.xinyue.icu

Go:   func main()
来源：http://aoy.yonumen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qln.gotoacloud.top

C#:   static void Main(string[] args)
来源：http://jmk.hnxiangtu.top

[M08] 获取系统与运行时信息
来源：http://zks.chenjidiqi.icu

Py:   platform.system();  platform.python_version()
来源：http://oqw.yonumen.top

PHP:  PHP_OS;  phpversion();
来源：http://nyc.tanke756.top

JS:   process.platform;  process.version
来源：http://eda.aibaodan.cn

TS:   process.platform;  process.version
来源：http://qbz.jinqigufen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ytu.wangshuangyany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://aga.vehdjk.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sij.bjfxy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://zuv.hywenlv.cn

================================================================================
来源：http://kep.quarkkingdee.top

N. 数据结构与算法
来源：http://gow.yvedp.cn

================================================================================
来源：http://cjh.jqgufenzy.top

[N01] 二分查找（有序数组）
来源：http://wnk.shzxlz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://itc.yueranfly.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://plf.yuxming.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cqw.ywan-chungtsiang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tws.nanxinkj.top

Java: Arrays.binarySearch(arr, x)
来源：http://qck.jyoumei.cn

Go:   sort.SearchInts(arr, x)
来源：http://dlo.hnxiangtu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qiu.zhoulong.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://vtv.yanxiufei.cn

[N02] 排序（工程实践用内置实现）
来源：http://icm.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://wff.dianchejie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dvm.daria6918.cn


<!-- 参考信息 -->