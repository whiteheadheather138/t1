代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qzm.ctjpmb.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xsz.gogol.net.cn

[J05] 时间加减（加 7 天）
来源：http://ngn.zdbjq.cn

Py:   now + timedelta(days=7)
来源：http://mqo.sweek.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://zkh.jqgufenzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pqb.c1oappe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fli.fehbvm.com

Java: LocalDate.now().plusDays(7)
来源：http://hvs.yueranfly.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ysv.vqdsnc.cn

Ruby: Time.now + 7 * 86400
来源：http://zjo.zhaomingkeji.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://jcc.wangshuangyany.cn

[J06] 计算两时间之差
来源：http://tpm.hcnkem.com

Py:   (end - start).total_seconds()
来源：http://vmk.316326.xyz

PHP:  $end->diff($start)->days;
来源：http://ubi.tanke756.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://khf.uphjek.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bja.redwolf501.top

Java: Duration.between(start, end).toSeconds()
来源：http://dji.iojbl.cn

Go:   end.Sub(start).Hours()
来源：http://psx.quarkkingdee.top

Ruby: end - start                 # 返回秒数
来源：http://lgj.cucudq.cn

C#:   (end - start).TotalSeconds
来源：http://mgr.sweek.top

[J07] 比较两个日期
来源：http://vhc.yfazqb.com

Py:   d1 < d2;  d1 == d2
来源：http://iwm.zhiwuduotai.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ipt.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vfs.jlsjyb.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yai.zhoulong.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ykz.shangyingyoupin.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blm.316326.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://tio.jiagoushi.top

C#:   d1 < d2;  d1 == d2
来源：http://xjk.gzhubu.top

[J08] 提取年月日与星期
来源：http://arn.shzxlz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://upw.fehbvm.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ciz.tanke756.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jfa.shangyingyoupin.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uia.zhixingplan.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mdk.nwbrower.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ghh.jyoumei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ech.yuxming.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ish.fzhhl.top

[J09] 时区处理
来源：http://mxy.guowangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fvm.bjfxy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eyh.fzhhl.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kpm.jyoumei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wii.vehdjk.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tpd.smart0.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aqp.havefunace.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ldf.jinqigufen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nbm.9152youxi.cn

[J10] 取今天 / 本月第一天
来源：http://jlx.sxryk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ogz.jinqigfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uru.hcnkem.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gya.andypj.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fjb.xziqi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://coo.wangdashe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://twn.jyoumei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://prb.sysykeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://szv.zhoulong.xyz

================================================================================
来源：http://hcb.nanxuanxn.top

K. JSON 与序列化
来源：http://hbu.yangfankeji.com

================================================================================
来源：http://fml.zhongyouzk.top

[K01] 对象转 JSON 字符串
来源：http://vag.yonumen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pub.yangfankeji.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fnt.fanxiaobao.xyz

JS:   JSON.stringify(obj)
来源：http://vij.gotoacloud.top

TS:   JSON.stringify(obj)
来源：http://xow.quarkkingdee.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ovn.fktsv.cn

Go:   json.Marshal(obj)
来源：http://dkt.smart0.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://yrq.yonumen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lqb.aibaodan.cn

[K02] JSON 字符串转对象
来源：http://gyd.xuanzx.com

Py:   json.loads(s)
来源：http://tlg.yvedp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pmx.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://ltf.chenzaomai.com

TS:   JSON.parse(s)
来源：http://zak.9152youxi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ahh.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://ilj.zycfv.cn

Ruby: JSON.parse(s)
来源：http://gzd.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zlq.jqgufenzy.top

[K03] JSON 美化输出（带缩进）
来源：http://fuh.xuanzx.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ltr.jyoumei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yip.gaohongyu789.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bgg.ydjk.org.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://luz.hysaishi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sal.vqdsnc.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://osi.jlsjyb.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sgm.bjfxy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zbx.aibaodan.cn

[K04] 读取 JSON 文件
来源：http://elg.sufxvd.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tdz.hnqzz.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://glw.pengpengdd.cyou

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pwt.nanxinkj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mks.birdmap.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fpb.andypj.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://plv.zhiwuduotai.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pkr.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vjz.fzhhl.top

[K05] 深拷贝对象
来源：http://dko.gzhubu.top

Py:   copy.deepcopy(obj)
来源：http://xhk.zhengqikj.top

PHP:  unserialize(serialize($obj));
来源：http://xfv.hnqzz.top

JS:   structuredClone(obj)
来源：http://dbt.meibo888.top

TS:   structuredClone(obj)
来源：http://gav.svipenyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tdu.fehbvm.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eev.ivvv.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rmj.shzxlz.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://eme.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://mnp.snrcjt.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qwk.xylfe.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ldq.meibo888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sie.andypj.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zmm.daria6918.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cih.yueranfly.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kuc.jianghu66.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kkd.yanxiufei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fqp.vehdjk.com

[K07] 进制转换
来源：http://ohd.tanke756.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vcj.meibo888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tzr.xuanzx.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kbn.fengsongda.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://emf.xziqi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mtk.nanxinkj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bln.ybcxt.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pmr.jianghu66.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kfv.316326.xyz

[K08] 二进制序列化（非 JSON）
来源：http://fzm.sjlbkw.cn

Py:   pickle.dumps(obj)
来源：http://ljs.andypj.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://frc.daria6918.cn

JS:   v8.serialize(obj)        // Node
来源：http://akv.ppjwa.cn

TS:   v8.serialize(obj)        // Node
来源：http://aqq.birdmap.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gjb.ydjk.org.cn

Go:   encoding/gob
来源：http://otd.snrcjt.cn

Ruby: Marshal.dump(obj)
来源：http://ung.yuxming.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://phy.dianchejie.cn

================================================================================
来源：http://kqb.ctjpmb.com

L. 网络请求
来源：http://nof.xuanzx.com

================================================================================
来源：http://csu.yfazqb.com

[L01] 发送 GET 请求
来源：http://hfh.fzhhl.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://caj.bjfxy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://crg.chenzaomai.com

JS:   await fetch(url)
来源：http://iaq.jinqigfzy.top

TS:   await fetch(url)
来源：http://hyk.hfpthk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cic.cheryme.top

Go:   resp, err := http.Get(url)
来源：http://bpt.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lfk.ctjpmb.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xrz.xylfe.cn

[L02] 发送 POST JSON
来源：http://pof.zhixingplan.top

Py:   requests.post(url, json={"a": 1})
来源：http://ayp.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eyc.aibaodan.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://brw.aizwys.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rtf.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cgj.fengsongda.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dgf.zhiwuduotai.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ffl.hfpthk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zfy.cheryme.top

[L03] 设置自定义请求头
来源：http://dkn.9152youxi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://drb.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xed.yangfankeji.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xpg.cheryme.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oui.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ubm.gogol.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://czu.zdqjudy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hxq.gotoacloud.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gqh.tian-w.cn

[L04] 设置超时
来源：http://fwk.shanyushiyangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://qwi.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wmk.fanxiaobao.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lzs.dashuyun.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jix.jqgufenzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kmu.xuetiantiany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tgj.52xcode.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dct.yj20258.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dsc.cqqwz.cn

[L05] 上传文件（multipart）
来源：http://oqz.guannengcc.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eiv.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rwf.shzxlz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gas.hfpthk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xda.shzxlz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wun.yfazqb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://onm.andypj.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tbb.yanxiufei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wtb.gaohongyu789.top

[L06] 解析响应为 JSON
来源：http://lae.yuanzhike.top

Py:   resp.json()
来源：http://usz.svipenyu.cn

PHP:  json_decode($body, true);
来源：http://dio.uphjek.com

JS:   await resp.json()
来源：http://uho.nwbrower.top

TS:   await resp.json()
来源：http://zfb.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ieb.jlsjyb.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ywb.xylfe.cn

Ruby: JSON.parse(resp.body)
来源：http://pzy.shuidangran.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zkw.ydzc1.top

[L07] 处理 HTTP 状态码
来源：http://bxe.birdmap.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://avz.yanxiufei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://otm.xinyue.icu

JS:   resp.ok;  resp.status
来源：http://cig.mhx1999.top

TS:   resp.ok;  resp.status
来源：http://wdy.yongpay.top

Java: resp.statusCode()
来源：http://xew.ivvv.top

Go:   resp.StatusCode
来源：http://phi.yueranfly.top

Ruby: resp.code.to_i
来源：http://vag.uphjek.com

C#:   (int)resp.StatusCode
来源：http://ddf.hnxiangtu.top

[L08] 并发请求多个地址
来源：http://wjd.jinqigufen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yok.xziqi.cn

PHP:  curl_multi_init() 系列
来源：http://mug.pengpengdd.cyou

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fiu.quarkkingdee.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qgl.tian-w.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kuv.52xcode.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lkf.kuanghao11.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ths.gogol.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tgf.jqgfzy.top

================================================================================
来源：http://rtw.zdqjudy.top

M. 命令行 / 进程 / 环境
来源：http://gpz.hnxiangtu.top

================================================================================
来源：http://moa.wangdashe.top

[M01] 读取命令行参数
来源：http://art.iojbl.cn

Py:   sys.argv[1:]
来源：http://mhp.chenlongwang.top

PHP:  $argv;  $argc;
来源：http://nqg.guowangkeji.top

JS:   process.argv.slice(2)
来源：http://sjb.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://xat.cqqwz.cn

Java: args 数组（main 方法参数）
来源：http://apr.nwbrower.top

Go:   os.Args[1:]
来源：http://ppn.havefunace.top

Ruby: ARGV
来源：http://fho.guowangkeji.top

C#:   args 数组（Main 方法参数）
来源：http://ohl.tian-w.cn

[M02] 读取环境变量
来源：http://cec.epnwcf.com

Py:   os.environ.get("HOME")
来源：http://kip.gogol.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kuz.ivvv.top

JS:   process.env.HOME
来源：http://dra.xinyue.icu

TS:   process.env.HOME
来源：http://iju.yj202588.top

Java: System.getenv("HOME")
来源：http://bgi.yuxming.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pss.ydjk.org.cn

Ruby: ENV["HOME"]
来源：http://plr.ctjpmb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oct.cucudq.cn

[M03] 执行外部命令
来源：http://qip.shanyushiyangkeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nei.yuanzhike.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ama.yj20258.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hoi.fktsv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mbp.cashguo.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hic.xziqi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ldg.yongpay.top

Ruby: system("ls -l");  `ls -l`
来源：http://ywj.xinyue.icu

C#:   Process.Start("ls", "-l");
来源：http://zjh.zhijiandao.cn

[M04] 获取当前工作目录
来源：http://bvo.ybcxt.top

Py:   os.getcwd()
来源：http://vpp.sxryk.cn

PHP:  getcwd();
来源：http://lnk.zhijiandao.cn

JS:   process.cwd()
来源：http://knm.haohaochexian.top

TS:   process.cwd()
来源：http://aux.sjlbkw.cn

Java: Path.of("").toAbsolutePath()
来源：http://kaa.vehdjk.com

Go:   os.Getwd()
来源：http://tcw.andypj.xyz

Ruby: Dir.pwd
来源：http://onb.xylfe.cn

C#:   Directory.GetCurrentDirectory()
来源：http://chi.bjfxy.top

[M05] 设置退出码
来源：http://nhd.iojbl.cn

Py:   sys.exit(1)
来源：http://sei.hnqzz.top

PHP:  exit(1);
来源：http://ekr.shanyushiyangkeji.top

JS:   process.exit(1)
来源：http://gxe.ivvv.top

TS:   process.exit(1)
来源：http://wqe.jinqigfzy.top

Java: System.exit(1)
来源：http://vvc.uphjek.com

Go:   os.Exit(1)
来源：http://dyw.smart0.xyz

Ruby: exit 1
来源：http://qra.52xcode.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xgi.jqgfzy.top

[M06] 向标准错误输出
来源：http://iwa.cucudq.cn

Py:   print("err", file=sys.stderr)
来源：http://apy.fktsv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://axd.aizwys.cn

JS:   console.error("err")
来源：http://jwb.gzhubu.top

TS:   console.error("err")
来源：http://slq.jinyuanbaomall.cn

Java: System.err.println("err")
来源：http://qwe.daxiang520.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://amz.hesvh.cn

Ruby: warn "err"
来源：http://zrn.vehdjk.com

C#:   Console.Error.WriteLine("err")
来源：http://rjg.havefunace.top

[M07] 判断是否为主入口
来源：http://oba.zhaomingkeji.xyz

Py:   if __name__ == "__main__":
来源：http://djo.fehbvm.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rpv.yangfankeji.com

JS:   require.main === module
来源：http://yst.shangyingyoupin.top

TS:   require.main === module
来源：http://dgn.316326.xyz

Java: public static void main(String[] args)
来源：http://brx.yanxiufei.cn

Go:   func main()
来源：http://lrx.guannengcc.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rtc.c1oappe.top

C#:   static void Main(string[] args)
来源：http://dan.fktsv.cn

[M08] 获取系统与运行时信息
来源：http://nvo.zycfv.cn

Py:   platform.system();  platform.python_version()
来源：http://mlt.zhixingplan.top

PHP:  PHP_OS;  phpversion();
来源：http://hcx.cdnleiting.top

JS:   process.platform;  process.version
来源：http://dll.aibaodan.cn

TS:   process.platform;  process.version
来源：http://tcs.yfazqb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tna.ydjk.org.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lvi.tianlin.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mpf.yuxming.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://itz.snrcjt.cn

================================================================================
来源：http://rhj.dianchejie.cn

N. 数据结构与算法
来源：http://osj.bjfxy.top

================================================================================
来源：http://fml.yuanzhike.top

[N01] 二分查找（有序数组）
来源：http://egf.hesvh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jav.sjlbkw.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://psz.kuanghao11.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yia.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://daz.hysaishi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pew.jqgufenzy.top

Go:   sort.SearchInts(arr, x)
来源：http://skb.yueranfly.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://svd.shanyushiyangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://jix.meibo888.top

[N02] 排序（工程实践用内置实现）
来源：http://crv.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://wtr.wangshuangyany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sio.hammf.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://spu.zdqjudy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://nql.gogol.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qhs.havefunace.top

Go:   slices.Sort(arr)
来源：http://rvg.svipenyu.cn


<!-- 参考信息 -->