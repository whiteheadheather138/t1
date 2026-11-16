代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lfz.bbcook.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bta.yuanzhike.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zms.yj202588.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://whl.ctjpmb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mye.tianlin.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pkl.yfazqb.com

[J05] 时间加减（加 7 天）
来源：http://pci.jinqigfzy.top

Py:   now + timedelta(days=7)
来源：http://ecx.ctjpmb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://yqs.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cag.fktsv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ouc.shanyushiyangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://mut.cheryme.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wqw.sweek.top

Ruby: Time.now + 7 * 86400
来源：http://lpt.vehdjk.com

C#:   DateTime.Now.AddDays(7)
来源：http://geo.svipenyu.cn

[J06] 计算两时间之差
来源：http://sll.jianghu66.top

Py:   (end - start).total_seconds()
来源：http://kve.dianchejie.cn

PHP:  $end->diff($start)->days;
来源：http://ahv.ppjwa.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://flt.nwbrower.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mzw.cheryme.top

Java: Duration.between(start, end).toSeconds()
来源：http://kaj.316326.xyz

Go:   end.Sub(start).Hours()
来源：http://vgt.ctjpmb.com

Ruby: end - start                 # 返回秒数
来源：http://ous.jlsjyb.cn

C#:   (end - start).TotalSeconds
来源：http://mpd.cdnleiting.top

[J07] 比较两个日期
来源：http://smk.yvedp.cn

Py:   d1 < d2;  d1 == d2
来源：http://cdj.redwolf501.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://znw.chenjidiqi.icu

JS:   d1.getTime() < d2.getTime()
来源：http://yxn.shzxlz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vwg.xziqi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cgb.yuanzhike.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://khp.gaohongyu789.top

Ruby: d1 < d2;  d1 == d2
来源：http://eyl.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://wfk.shuidangran.top

[J08] 提取年月日与星期
来源：http://lua.sufxvd.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vpj.zhongyouzk.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bum.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wmg.yangfankeji.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vpo.redwolf501.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://myf.daxiang520.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://irn.jinghuilouyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vgj.vehdjk.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xky.yfazqb.com

[J09] 时区处理
来源：http://wuq.gogol.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zko.ywan-chungtsiang.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gsi.meibo888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hjs.jiagoushi.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nph.hcnkem.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ezi.yangfankeji.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ygw.jinqigfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://azq.gaohongyu789.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zik.iojbl.cn

[J10] 取今天 / 本月第一天
来源：http://mwh.cashguo.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nyd.uphjek.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://caz.daxiang520.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oja.316326.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dwh.meibo888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://een.aizwys.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gfo.yongpay.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://unw.cqqwz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vvu.aizwys.cn

================================================================================
来源：http://jeg.dianchejie.cn

K. JSON 与序列化
来源：http://yqs.wangshuangyany.cn

================================================================================
来源：http://zvy.vqdsnc.cn

[K01] 对象转 JSON 字符串
来源：http://tbd.yj202588.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ovd.pycfn.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ztp.xingfuxueyuan.xyz

JS:   JSON.stringify(obj)
来源：http://scn.sjlbkw.cn

TS:   JSON.stringify(obj)
来源：http://yup.xylfe.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vyo.fzhhl.top

Go:   json.Marshal(obj)
来源：http://ylf.gotoacloud.top

Ruby: obj.to_json                                     // require "json"
来源：http://rem.zdqjudy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://khx.iojbl.cn

[K02] JSON 字符串转对象
来源：http://dyl.hongshengwenyu.top

Py:   json.loads(s)
来源：http://zug.wangdashe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qcy.yonumen.top

JS:   JSON.parse(s)
来源：http://snz.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://bun.aibaodan.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xit.gotoacloud.top

Go:   json.Unmarshal(data, &v)
来源：http://jaa.52xcode.cn

Ruby: JSON.parse(s)
来源：http://ysr.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dsr.zhoulong.xyz

[K03] JSON 美化输出（带缩进）
来源：http://ezj.aibaodan.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gej.yangfankeji.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ceg.tian-w.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fku.bjfxy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://asb.nanxinkj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fxz.316326.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hbp.cucudq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uur.316326.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ddy.shuidangran.top

[K04] 读取 JSON 文件
来源：http://idp.ehwqpu.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tuw.jinqigufen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://csc.hesvh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mep.zhongyouzk.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hfp.andypj.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zpl.cashguo.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vlo.jlsjyb.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fzv.quarkkingdee.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qvh.meibo888.top

[K05] 深拷贝对象
来源：http://ukw.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://epy.daria6918.cn

PHP:  unserialize(serialize($obj));
来源：http://khq.nwbrower.top

JS:   structuredClone(obj)
来源：http://rwc.zhijiandao.cn

TS:   structuredClone(obj)
来源：http://mxy.fktsv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uxl.yongpay.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jqr.haohaochexian.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hkp.daxiang520.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bcx.chenlongwang.top

[K06] 解析 URL 查询串
来源：http://bvn.daria6918.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dsv.yueranfly.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kye.xingfuxueyuan.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jvz.hnqzz.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fud.dianchejie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vsc.nanxinkj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bbj.9152youxi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kmo.quarkkingdee.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hfw.gogol.net.cn

[K07] 进制转换
来源：http://xgg.yvedp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eer.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kdp.ydjk.org.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ekc.uphjek.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xvv.bbcook.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mvv.ehwqpu.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kcf.jinqigfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zbp.cashguo.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tid.yanxiufei.cn

[K08] 二进制序列化（非 JSON）
来源：http://lax.zhijiandao.cn

Py:   pickle.dumps(obj)
来源：http://ytf.316326.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://udq.ehwqpu.com

JS:   v8.serialize(obj)        // Node
来源：http://cyj.aibaodan.cn

TS:   v8.serialize(obj)        // Node
来源：http://gmr.daxiang520.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ode.zhengqikj.top

Go:   encoding/gob
来源：http://khk.hysaishi.cn

Ruby: Marshal.dump(obj)
来源：http://qlo.ehwqpu.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wac.chenzaomai.com

================================================================================
来源：http://xwn.ctjpmb.com

L. 网络请求
来源：http://yiy.zhiwuduotai.top

================================================================================
来源：http://heq.aizwys.cn

[L01] 发送 GET 请求
来源：http://zxa.shuidangran.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aop.ehwqpu.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dma.snrcjt.cn

JS:   await fetch(url)
来源：http://grr.yongpay.top

TS:   await fetch(url)
来源：http://zqf.jinyuanbaomall.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rfq.smart0.xyz

Go:   resp, err := http.Get(url)
来源：http://rub.jqgfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://taf.chenlongwang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xyo.guannengcc.top

[L02] 发送 POST JSON
来源：http://inn.feifeiyinyue.top

Py:   requests.post(url, json={"a": 1})
来源：http://ckj.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mup.vqdsnc.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zjq.sysykeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zuj.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iyl.zhengqikj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gbn.fengsongda.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aob.jinghuilouyu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nqs.shzxlz.cn

[L03] 设置自定义请求头
来源：http://vxs.yuxming.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://txc.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gon.daria6918.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pcb.ppjwa.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pyw.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qua.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vpe.jianghu66.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xkq.tanke756.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xhq.tian-w.cn

[L04] 设置超时
来源：http://xjw.birdmap.top

Py:   requests.get(url, timeout=5)
来源：http://nfo.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://buu.hcnkem.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fbf.yj202588.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ryg.guowangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pwv.nanxinkj.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qdt.zdbjq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://utl.yj202588.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uuh.hysaishi.cn

[L05] 上传文件（multipart）
来源：http://eew.smart0.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dec.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kmw.havefunace.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kqn.uphjek.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sdg.cdnleiting.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://taq.ehwqpu.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jtc.epnwcf.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hot.vqdsnc.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vlf.sysykeji.top

[L06] 解析响应为 JSON
来源：http://wqo.guowangkeji.top

Py:   resp.json()
来源：http://qpw.vehdjk.com

PHP:  json_decode($body, true);
来源：http://tqs.shuidangran.top

JS:   await resp.json()
来源：http://tjg.nwbrower.top

TS:   await resp.json()
来源：http://xoy.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uoj.zhaomingkeji.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jqe.yfazqb.com

Ruby: JSON.parse(resp.body)
来源：http://wmy.aizwys.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hvi.zhongyouzk.top

[L07] 处理 HTTP 状态码
来源：http://nzs.fktsv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sjl.cucudq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vfk.yfazqb.com

JS:   resp.ok;  resp.status
来源：http://fiy.yangfankeji.com

TS:   resp.ok;  resp.status
来源：http://eqi.zycfv.cn

Java: resp.statusCode()
来源：http://txd.yonumen.top

Go:   resp.StatusCode
来源：http://dpv.yj20258.top

Ruby: resp.code.to_i
来源：http://bpc.wangdashe.top

C#:   (int)resp.StatusCode
来源：http://tmi.hywenlv.cn

[L08] 并发请求多个地址
来源：http://ccu.cashguo.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pxw.hywenlv.cn

PHP:  curl_multi_init() 系列
来源：http://qzt.yanxiufei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zmt.aibaodan.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iqf.hcnkem.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ykl.snrcjt.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ksf.yangfankeji.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wbl.zdqjudy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://urq.yanxiufei.cn

================================================================================
来源：http://jjp.zycfv.cn

M. 命令行 / 进程 / 环境
来源：http://bmy.9152youxi.cn

================================================================================
来源：http://mib.uphjek.com

[M01] 读取命令行参数
来源：http://znw.yueranfly.top

Py:   sys.argv[1:]
来源：http://qsa.gaohongyu789.top

PHP:  $argv;  $argc;
来源：http://jen.c1oappe.top

JS:   process.argv.slice(2)
来源：http://utk.hammf.cn

TS:   process.argv.slice(2)
来源：http://tgh.hysaishi.cn

Java: args 数组（main 方法参数）
来源：http://crg.fanxiaobao.xyz

Go:   os.Args[1:]
来源：http://yjx.feifeiyinyue.top

Ruby: ARGV
来源：http://yov.ivvv.top

C#:   args 数组（Main 方法参数）
来源：http://hff.sxryk.cn

[M02] 读取环境变量
来源：http://wqg.fanxiaobao.xyz

Py:   os.environ.get("HOME")
来源：http://laf.yangfankeji.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dqr.chenzaomai.com

JS:   process.env.HOME
来源：http://xmn.cqqwz.cn

TS:   process.env.HOME
来源：http://icx.vqdsnc.cn

Java: System.getenv("HOME")
来源：http://ypf.316326.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zou.ivvv.top

Ruby: ENV["HOME"]
来源：http://jcr.bjfxy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xoo.0kj1m.cn

[M03] 执行外部命令
来源：http://qvk.52xcode.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://psc.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wad.tanke756.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gqd.hnqzz.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zaj.zhoulong.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lyy.vqdsnc.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jyj.fktsv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sbm.zdqjudy.top

C#:   Process.Start("ls", "-l");
来源：http://sqq.epnwcf.com

[M04] 获取当前工作目录
来源：http://ule.ivvv.top

Py:   os.getcwd()
来源：http://wti.feifeiyinyue.top

PHP:  getcwd();
来源：http://sed.hcnkem.com

JS:   process.cwd()
来源：http://nfd.sjlbkw.cn

TS:   process.cwd()
来源：http://jed.shanyushiyangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://fmi.yfazqb.com

Go:   os.Getwd()
来源：http://lsh.xingfuxueyuan.xyz

Ruby: Dir.pwd
来源：http://bvk.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qci.shanyushiyangkeji.top

[M05] 设置退出码
来源：http://rvp.shanyushiyangkeji.top

Py:   sys.exit(1)
来源：http://plk.hesvh.cn

PHP:  exit(1);
来源：http://xct.c1oappe.top

JS:   process.exit(1)
来源：http://qli.daxiang520.top

TS:   process.exit(1)
来源：http://jzf.zhiwuduotai.top

Java: System.exit(1)
来源：http://bij.9152youxi.cn

Go:   os.Exit(1)
来源：http://fep.ydjk.org.cn

Ruby: exit 1
来源：http://wqu.jlsjyb.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dhk.hnqzz.top

[M06] 向标准错误输出
来源：http://xkf.bbcook.cn

Py:   print("err", file=sys.stderr)
来源：http://idf.cdnleiting.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zgr.jlsjyb.cn

JS:   console.error("err")
来源：http://oxo.guannengcc.top

TS:   console.error("err")
来源：http://ufq.fehbvm.com

Java: System.err.println("err")
来源：http://nlq.snrcjt.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uxq.vehdjk.com

Ruby: warn "err"
来源：http://zdg.zhiwuduotai.top

C#:   Console.Error.WriteLine("err")
来源：http://rkb.jinqigfzy.top

[M07] 判断是否为主入口
来源：http://yxa.chenlongwang.top

Py:   if __name__ == "__main__":
来源：http://oik.hysaishi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://khn.hywenlv.cn

JS:   require.main === module
来源：http://gep.birdmap.top

TS:   require.main === module
来源：http://opk.zhaomingkeji.xyz

Java: public static void main(String[] args)
来源：http://jiz.shanyushiyangtech.top

Go:   func main()
来源：http://qfs.vqdsnc.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bix.cucudq.cn

C#:   static void Main(string[] args)
来源：http://aio.tarul.cn

[M08] 获取系统与运行时信息
来源：http://pld.yangfankeji.com

Py:   platform.system();  platform.python_version()
来源：http://val.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://ucq.zhiwuduotai.top

JS:   process.platform;  process.version
来源：http://xrc.jinqigufen.top

TS:   process.platform;  process.version
来源：http://mvu.jianghu66.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fhc.yangfankeji.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://bqd.hammf.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ebx.hnqzz.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xch.316326.xyz

================================================================================
来源：http://qlb.cqqwz.cn

N. 数据结构与算法
来源：http://bqp.shanyushiyangtech.top

================================================================================
来源：http://wuh.ppjwa.cn

[N01] 二分查找（有序数组）
来源：http://nme.xylfe.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gro.snrcjt.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://elj.ppjwa.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ayl.bjfxy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uca.zhengqikj.top

Java: Arrays.binarySearch(arr, x)
来源：http://ddd.zdqjudy.top

Go:   sort.SearchInts(arr, x)
来源：http://dos.havefunace.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ran.yj20258888.top

C#:   Array.BinarySearch(arr, x)
来源：http://mhz.wangdashe.top

[N02] 排序（工程实践用内置实现）
来源：http://yvb.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://cxd.nanxinkj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ghq.ivvv.top


<!-- 参考信息 -->