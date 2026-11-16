代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qfu.yanxiufei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://myt.kuanghao11.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iyr.jqgufenzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://brx.mhx1999.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hzr.dianchejie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ejp.cashguo.top

[J05] 时间加减（加 7 天）
来源：http://gst.tian-w.cn

Py:   now + timedelta(days=7)
来源：http://qpd.zhaomingkeji.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://upd.zycfv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wcc.fehbvm.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://prz.aizwys.cn

Java: LocalDate.now().plusDays(7)
来源：http://dyc.yangfankeji.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://adu.smart0.xyz

Ruby: Time.now + 7 * 86400
来源：http://qhl.guowangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://yhx.andypj.xyz

[J06] 计算两时间之差
来源：http://hyt.kuanghao11.cn

Py:   (end - start).total_seconds()
来源：http://wzf.vqdsnc.cn

PHP:  $end->diff($start)->days;
来源：http://kkb.zhiwuduotai.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dqo.tian-w.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hqj.hnxiangtu.top

Java: Duration.between(start, end).toSeconds()
来源：http://zyp.chenjidiqi.icu

Go:   end.Sub(start).Hours()
来源：http://dfu.c1oappe.top

Ruby: end - start                 # 返回秒数
来源：http://blm.hysaishi.cn

C#:   (end - start).TotalSeconds
来源：http://otl.jinqigufen.top

[J07] 比较两个日期
来源：http://ynj.zhongyouzk.top

Py:   d1 < d2;  d1 == d2
来源：http://xih.quarkkingdee.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nfm.yj20258.top

JS:   d1.getTime() < d2.getTime()
来源：http://jki.dianchejie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ujh.dianchejie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://doc.chenjidiqi.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://afi.fzhhl.top

Ruby: d1 < d2;  d1 == d2
来源：http://myw.xziqi.cn

C#:   d1 < d2;  d1 == d2
来源：http://gsh.chenzaomai.com

[J08] 提取年月日与星期
来源：http://guz.jianghu66.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pre.shanyushiyangtech.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lth.cheryme.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ndb.shangyingyoupin.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yfd.xinyue.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eso.cucudq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rmi.dianchejie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jxe.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wzv.fengsongda.top

[J09] 时区处理
来源：http://zbx.ybcxt.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tzw.quarkkingdee.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wpp.pycfn.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iix.jqgfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ldx.nanxuanxn.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mok.kuanghao11.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dxm.cdnleiting.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qco.sweek.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://agj.hnxiangtu.top

[J10] 取今天 / 本月第一天
来源：http://pwm.dianchejie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://aye.0kj1m.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tmq.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jcl.cqqwz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jjz.zhongyouzk.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vja.ctjpmb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oaq.jiagoushi.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cog.aibaodan.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://myo.ydjk.org.cn

================================================================================
来源：http://jgr.yfazqb.com

K. JSON 与序列化
来源：http://rsq.sufxvd.cn

================================================================================
来源：http://eaz.yj202588.top

[K01] 对象转 JSON 字符串
来源：http://qtv.vehdjk.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wpa.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jyj.jiagoushi.top

JS:   JSON.stringify(obj)
来源：http://kyo.hongshengwenyu.top

TS:   JSON.stringify(obj)
来源：http://fgs.jqgufenzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gle.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://cyb.tanke756.top

Ruby: obj.to_json                                     // require "json"
来源：http://mtf.xingfuxueyuan.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://pos.gaohongyu789.top

[K02] JSON 字符串转对象
来源：http://ylr.wangdashe.top

Py:   json.loads(s)
来源：http://ori.guannengcc.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bhk.zhixingplan.top

JS:   JSON.parse(s)
来源：http://eid.nanxuanxn.top

TS:   JSON.parse(s)
来源：http://xra.9152youxi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mwh.redwolf501.top

Go:   json.Unmarshal(data, &v)
来源：http://eov.gaohongyu789.top

Ruby: JSON.parse(s)
来源：http://sbq.cheryme.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uci.xziqi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ekp.yfazqb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ivq.hnxiangtu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mto.hongshengwenyu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xlk.ehwqpu.com

TS:   JSON.stringify(obj, null, 2)
来源：http://xah.jqgufenzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sin.zdqjudy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fzo.pengpengdd.cyou

Ruby: JSON.pretty_generate(obj)
来源：http://zbl.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lsn.yvedp.cn

[K04] 读取 JSON 文件
来源：http://eoh.hywenlv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kzo.zhoulong.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://asm.haohaochexian.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://emi.zhaomingkeji.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tsc.birdmap.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ynn.birdmap.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kbf.yj20258.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://uei.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dlm.xuanzx.com

[K05] 深拷贝对象
来源：http://pwl.yfazqb.com

Py:   copy.deepcopy(obj)
来源：http://xwa.jianghu66.top

PHP:  unserialize(serialize($obj));
来源：http://chh.nanxinkj.top

JS:   structuredClone(obj)
来源：http://afm.yongpay.top

TS:   structuredClone(obj)
来源：http://dpn.jlsjyb.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ehn.tianlin.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lfw.yj20258.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lsh.yj20258888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vcs.yangfankeji.com

[K06] 解析 URL 查询串
来源：http://vdb.zhaomingkeji.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kgx.tanke756.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ktc.xuanzx.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yjz.wangshuangyany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kzr.0kj1m.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kag.bjfxy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://opx.xuetiantiany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://shj.meibo888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sdh.9152youxi.cn

[K07] 进制转换
来源：http://etp.zhiwuduotai.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iny.hesvh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pnq.yj20258888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eyh.jqgufenzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hvq.yonumen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jpr.shzxlz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cwd.aibaodan.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dev.shzxlz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tun.chenlongwang.top

[K08] 二进制序列化（非 JSON）
来源：http://vru.aizwys.cn

Py:   pickle.dumps(obj)
来源：http://elj.yj20258888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hvi.ydzc1.top

JS:   v8.serialize(obj)        // Node
来源：http://qjs.jinyuanbaomall.cn

TS:   v8.serialize(obj)        // Node
来源：http://vcw.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bgr.mhx1999.top

Go:   encoding/gob
来源：http://gqj.meibo888.top

Ruby: Marshal.dump(obj)
来源：http://ruf.birdmap.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vog.316326.xyz

================================================================================
来源：http://vdx.xylfe.cn

L. 网络请求
来源：http://rtx.yanxiufei.cn

================================================================================
来源：http://wde.guannengcc.top

[L01] 发送 GET 请求
来源：http://tku.nanxuanxn.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lei.cheryme.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aht.yongpay.top

JS:   await fetch(url)
来源：http://mhy.andypj.xyz

TS:   await fetch(url)
来源：http://gey.jlsjyb.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gwa.nanxinkj.top

Go:   resp, err := http.Get(url)
来源：http://usl.tanke756.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vuc.sjlbkw.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zga.shzxlz.cn

[L02] 发送 POST JSON
来源：http://nyc.yvedp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mwn.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wgm.fanxiaobao.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uvn.daxiang520.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gvf.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://etx.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bzw.chenzaomai.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nsr.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eni.cucudq.cn

[L03] 设置自定义请求头
来源：http://odj.daria6918.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tqk.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://paa.vqdsnc.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ayq.316326.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ahp.vqdsnc.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rkz.yj20258888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qkj.xziqi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ucn.yuxming.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gxn.yj20258888.top

[L04] 设置超时
来源：http://fau.jqgfzy.top

Py:   requests.get(url, timeout=5)
来源：http://bhr.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dcs.yj20258.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jaf.wangdashe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aaa.jqgfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zwo.shzxlz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pox.fengsongda.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kru.nanxinkj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gll.fktsv.cn

[L05] 上传文件（multipart）
来源：http://uph.meibo888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tvj.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mbh.zhaomingkeji.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cyh.shangyingyoupin.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iiu.redwolf501.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bzj.hcnkem.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qxt.jlsjyb.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://elh.gogol.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ckx.gaohongyu789.top

[L06] 解析响应为 JSON
来源：http://mbu.uphjek.com

Py:   resp.json()
来源：http://ihj.mhx1999.top

PHP:  json_decode($body, true);
来源：http://uvk.dianchejie.cn

JS:   await resp.json()
来源：http://qxk.smart0.xyz

TS:   await resp.json()
来源：http://huz.ybcxt.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yyk.yonumen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pkj.tian-w.cn

Ruby: JSON.parse(resp.body)
来源：http://mbq.hysaishi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://awn.smart0.xyz

[L07] 处理 HTTP 状态码
来源：http://tpj.pengpengdd.cyou

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gdo.xziqi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wdh.xinyue.icu

JS:   resp.ok;  resp.status
来源：http://sig.52xcode.cn

TS:   resp.ok;  resp.status
来源：http://wsk.sweek.top

Java: resp.statusCode()
来源：http://ubi.0kj1m.cn

Go:   resp.StatusCode
来源：http://gts.jianghu66.top

Ruby: resp.code.to_i
来源：http://bas.chenlongwang.top

C#:   (int)resp.StatusCode
来源：http://oii.gogol.net.cn

[L08] 并发请求多个地址
来源：http://ckx.cucudq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zrz.ydzc1.top

PHP:  curl_multi_init() 系列
来源：http://gus.feifeiyinyue.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ihk.haohaochexian.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sqv.cqqwz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://onf.bjfxy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://onf.uphjek.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iuo.yvedp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zfm.svipenyu.cn

================================================================================
来源：http://qvl.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境
来源：http://yiw.zhaomingkeji.xyz

================================================================================
来源：http://ths.0kj1m.cn

[M01] 读取命令行参数
来源：http://upu.zhoulong.xyz

Py:   sys.argv[1:]
来源：http://vje.52xcode.cn

PHP:  $argv;  $argc;
来源：http://law.wangdashe.top

JS:   process.argv.slice(2)
来源：http://wav.shangyingyoupin.top

TS:   process.argv.slice(2)
来源：http://ebq.jinyuanbaomall.cn

Java: args 数组（main 方法参数）
来源：http://fks.sysykeji.top

Go:   os.Args[1:]
来源：http://mbj.cucudq.cn

Ruby: ARGV
来源：http://zmh.xinyue.icu

C#:   args 数组（Main 方法参数）
来源：http://tre.zhijiandao.cn

[M02] 读取环境变量
来源：http://eyf.jiagoushi.top

Py:   os.environ.get("HOME")
来源：http://ucn.ehwqpu.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cyr.zhaomingkeji.xyz

JS:   process.env.HOME
来源：http://qts.tarul.cn

TS:   process.env.HOME
来源：http://uxr.andypj.xyz

Java: System.getenv("HOME")
来源：http://sbz.fzhhl.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yef.hfpthk.cn

Ruby: ENV["HOME"]
来源：http://uwo.aizwys.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ude.yj20258888.top

[M03] 执行外部命令
来源：http://cqg.quarkkingdee.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mlt.jinyuanbaomall.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ruu.shzxlz.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ygx.jiagoushi.top

TS:   child_process.execSync("ls -l").toString()
来源：http://azp.fehbvm.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://swb.gotoacloud.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gvg.cashguo.top

Ruby: system("ls -l");  `ls -l`
来源：http://mya.jinghuilouyu.cn

C#:   Process.Start("ls", "-l");
来源：http://rlu.smart0.xyz

[M04] 获取当前工作目录
来源：http://lsg.fzhhl.top

Py:   os.getcwd()
来源：http://mza.gaohongyu789.top

PHP:  getcwd();
来源：http://ttj.epnwcf.com

JS:   process.cwd()
来源：http://xxt.yangfankeji.com

TS:   process.cwd()
来源：http://jqj.wangshuangyany.cn

Java: Path.of("").toAbsolutePath()
来源：http://lnz.tanke756.top

Go:   os.Getwd()
来源：http://mme.feifeiyinyue.top

Ruby: Dir.pwd
来源：http://ygd.tian-w.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ltw.kuanghao11.cn

[M05] 设置退出码
来源：http://jtw.nwbrower.top

Py:   sys.exit(1)
来源：http://apa.yuanzhike.top

PHP:  exit(1);
来源：http://por.chenlongwang.top

JS:   process.exit(1)
来源：http://uuj.andypj.xyz

TS:   process.exit(1)
来源：http://rdu.cqqwz.cn

Java: System.exit(1)
来源：http://yqs.xuanzx.com

Go:   os.Exit(1)
来源：http://qae.iojbl.cn

Ruby: exit 1
来源：http://ftl.52xcode.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cgi.wangdashe.top

[M06] 向标准错误输出
来源：http://xtt.yj20258888.top

Py:   print("err", file=sys.stderr)
来源：http://kzx.yongpay.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ccj.birdmap.top

JS:   console.error("err")
来源：http://hdo.zhixingplan.top

TS:   console.error("err")
来源：http://cpu.hammf.cn

Java: System.err.println("err")
来源：http://jir.cheryme.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qsv.zhixingplan.top

Ruby: warn "err"
来源：http://gpe.ydjk.org.cn

C#:   Console.Error.WriteLine("err")
来源：http://rur.xinyue.icu

[M07] 判断是否为主入口
来源：http://vgt.gzhubu.top

Py:   if __name__ == "__main__":
来源：http://qnu.zhixingplan.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aof.0kj1m.cn

JS:   require.main === module
来源：http://mni.cucudq.cn

TS:   require.main === module
来源：http://ovr.nanxuanxn.top

Java: public static void main(String[] args)
来源：http://jie.daxiang520.top

Go:   func main()
来源：http://uop.xylfe.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vid.0kj1m.cn

C#:   static void Main(string[] args)
来源：http://wwx.gzhubu.top

[M08] 获取系统与运行时信息
来源：http://plk.fzhhl.top

Py:   platform.system();  platform.python_version()
来源：http://wyy.meibo888.top

PHP:  PHP_OS;  phpversion();
来源：http://mnt.hesvh.cn

JS:   process.platform;  process.version
来源：http://uty.xziqi.cn

TS:   process.platform;  process.version
来源：http://hjr.jiagoushi.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vmt.sysykeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hkt.0kj1m.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qvv.yanxiufei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lzq.tianlin.xyz

================================================================================
来源：http://osy.xziqi.cn

N. 数据结构与算法
来源：http://xgd.zhiwuduotai.top

================================================================================
来源：http://rzt.redwolf501.top

[N01] 二分查找（有序数组）
来源：http://syn.feifeiyinyue.top

Py:   bisect.bisect_left(arr, x)
来源：http://jkq.vqdsnc.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wvj.fktsv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://szf.nwbrower.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pbh.zhijiandao.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wjl.tarul.cn

Go:   sort.SearchInts(arr, x)
来源：http://cof.zycfv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tus.yj202588.top

C#:   Array.BinarySearch(arr, x)
来源：http://xsh.sysykeji.top

[N02] 排序（工程实践用内置实现）
来源：http://gii.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://kha.fengsongda.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ihd.cqqwz.cn


<!-- 参考信息 -->