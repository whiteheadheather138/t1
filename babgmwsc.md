代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kja.fzhhl.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bhc.guannengcc.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pag.hnqzz.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rdg.tanke756.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ytv.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ryf.shuidangran.top

[J05] 时间加减（加 7 天）
来源：http://ajo.chenlongwang.top

Py:   now + timedelta(days=7)
来源：http://ugw.shangyingyoupin.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://gki.ehwqpu.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yqy.chenjidiqi.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nyq.yuanzhike.top

Java: LocalDate.now().plusDays(7)
来源：http://vkm.yj202588.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jba.jianghu66.top

Ruby: Time.now + 7 * 86400
来源：http://tur.jyoumei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ehs.guannengcc.top

[J06] 计算两时间之差
来源：http://eub.xinyue.icu

Py:   (end - start).total_seconds()
来源：http://lku.xuanzx.com

PHP:  $end->diff($start)->days;
来源：http://ibu.jyoumei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wqa.guowangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nai.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fqe.c1oappe.top

Go:   end.Sub(start).Hours()
来源：http://pvp.epnwcf.com

Ruby: end - start                 # 返回秒数
来源：http://kkm.chenzaomai.com

C#:   (end - start).TotalSeconds
来源：http://uzx.hongshengwenyu.top

[J07] 比较两个日期
来源：http://xwj.jinghuilouyu.cn

Py:   d1 < d2;  d1 == d2
来源：http://dwi.chenzaomai.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lxf.chenjidiqi.icu

JS:   d1.getTime() < d2.getTime()
来源：http://wma.yuanzhike.top

TS:   d1.getTime() < d2.getTime()
来源：http://elv.tian-w.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bnt.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bzf.gogol.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ttz.jinghuilouyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://pyq.guowangkeji.top

[J08] 提取年月日与星期
来源：http://gdx.zhaomingkeji.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fua.zhongyouzk.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tzx.sweek.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yyv.c1oappe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rhv.zhaomingkeji.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://chh.zhongyouzk.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oig.ywan-chungtsiang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jsb.xylfe.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://atm.zhongyouzk.top

[J09] 时区处理
来源：http://fdr.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qoq.shuidangran.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kgk.xylfe.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://goj.zdqjudy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://psw.fanxiaobao.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://shz.hywenlv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mta.jlsjyb.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://str.ppjwa.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qte.meibo888.top

[J10] 取今天 / 本月第一天
来源：http://uci.jinqigfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kfj.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wwm.hnxiangtu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gny.hywenlv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qwx.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://afg.zdqjudy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xef.havefunace.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://waq.cheryme.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vee.ydzc1.top

================================================================================
来源：http://hfe.316326.xyz

K. JSON 与序列化
来源：http://yne.cqqwz.cn

================================================================================
来源：http://zwh.bjfxy.top

[K01] 对象转 JSON 字符串
来源：http://gft.nwbrower.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dmn.xinyue.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tze.iojbl.cn

JS:   JSON.stringify(obj)
来源：http://fcn.hongshengwenyu.top

TS:   JSON.stringify(obj)
来源：http://xrc.9152youxi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://thc.yuanzhike.top

Go:   json.Marshal(obj)
来源：http://rhs.hnxiangtu.top

Ruby: obj.to_json                                     // require "json"
来源：http://jxp.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj)
来源：http://gkg.redwolf501.top

[K02] JSON 字符串转对象
来源：http://nfu.hnqzz.top

Py:   json.loads(s)
来源：http://pts.vehdjk.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xnk.quarkkingdee.top

JS:   JSON.parse(s)
来源：http://plq.redwolf501.top

TS:   JSON.parse(s)
来源：http://ntc.feifeiyinyue.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bbx.hnqzz.top

Go:   json.Unmarshal(data, &v)
来源：http://wrt.316326.xyz

Ruby: JSON.parse(s)
来源：http://wwt.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gmm.yuanzhike.top

[K03] JSON 美化输出（带缩进）
来源：http://pwp.tianlin.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rtv.vqdsnc.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vlh.zhijiandao.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tyn.yuxming.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qfa.xziqi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rpq.gzhubu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oyo.iojbl.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kcu.wangdashe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xet.hcnkem.com

[K04] 读取 JSON 文件
来源：http://jjn.fehbvm.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jrn.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gnr.jqgfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://enc.tarul.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zpm.ydjk.org.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wbw.hywenlv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ciu.dianchejie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://aod.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ulr.zhaomingkeji.xyz

[K05] 深拷贝对象
来源：http://atz.jyoumei.cn

Py:   copy.deepcopy(obj)
来源：http://num.9152youxi.cn

PHP:  unserialize(serialize($obj));
来源：http://orz.ydzc1.top

JS:   structuredClone(obj)
来源：http://rth.tianlin.xyz

TS:   structuredClone(obj)
来源：http://blt.fehbvm.com

Java: // 手写拷贝构造，或序列化往返
来源：http://vyd.hcnkem.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://usy.zdbjq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ehq.hammf.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ymt.jinghuilouyu.cn

[K06] 解析 URL 查询串
来源：http://rht.cashguo.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rkn.shzxlz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wqt.jlsjyb.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xxh.yvedp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cmd.bbcook.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mjq.jqgufenzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://urj.kuanghao11.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hyt.ppjwa.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rph.xingfuxueyuan.xyz

[K07] 进制转换
来源：http://hpg.ivvv.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qta.cashguo.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vrs.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vfo.fzhhl.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sln.sjlbkw.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mkk.sysykeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://odq.tianlin.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nus.sxryk.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tho.316326.xyz

[K08] 二进制序列化（非 JSON）
来源：http://jnt.hongshengwenyu.top

Py:   pickle.dumps(obj)
来源：http://cjh.xylfe.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qfy.shzxlz.cn

JS:   v8.serialize(obj)        // Node
来源：http://ror.cheryme.top

TS:   v8.serialize(obj)        // Node
来源：http://rle.yj20258.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://raf.zhijiandao.cn

Go:   encoding/gob
来源：http://aqv.tianlin.xyz

Ruby: Marshal.dump(obj)
来源：http://mzx.xinyue.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iwi.fehbvm.com

================================================================================
来源：http://fkf.ctjpmb.com

L. 网络请求
来源：http://eiv.fehbvm.com

================================================================================
来源：http://ihg.jqgfzy.top

[L01] 发送 GET 请求
来源：http://khx.yvedp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cjy.9152youxi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rxu.jinqigfzy.top

JS:   await fetch(url)
来源：http://cil.daria6918.cn

TS:   await fetch(url)
来源：http://zmo.meibo888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tiv.gogol.net.cn

Go:   resp, err := http.Get(url)
来源：http://tfw.tian-w.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jij.ydjk.org.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cbp.xingfuxueyuan.xyz

[L02] 发送 POST JSON
来源：http://dio.shangyingyoupin.top

Py:   requests.post(url, json={"a": 1})
来源：http://sev.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fjw.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ljn.hfpthk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oxm.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ive.pycfn.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uie.wangdashe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://axl.yueranfly.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oqq.dianchejie.cn

[L03] 设置自定义请求头
来源：http://abq.ppjwa.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mwo.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ovi.jinqigufen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zzc.gotoacloud.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jsi.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ili.ctjpmb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mfa.mhx1999.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jfn.sysykeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://brc.yuanzhike.top

[L04] 设置超时
来源：http://ayq.sweek.top

Py:   requests.get(url, timeout=5)
来源：http://oqn.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kbp.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pca.shzxlz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sqz.fengsongda.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sps.vqdsnc.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pll.zhengqikj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://plx.jianghu66.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sgj.sweek.top

[L05] 上传文件（multipart）
来源：http://hyh.cdnleiting.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kdq.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qzr.xziqi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hfx.tianlin.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mok.shanyushiyangtech.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kmv.cqqwz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fyi.vqdsnc.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nsx.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zqt.sjlbkw.cn

[L06] 解析响应为 JSON
来源：http://qor.yanxiufei.cn

Py:   resp.json()
来源：http://lst.cdnleiting.top

PHP:  json_decode($body, true);
来源：http://rza.mhx1999.top

JS:   await resp.json()
来源：http://rgv.jlsjyb.cn

TS:   await resp.json()
来源：http://iss.quarkkingdee.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ffi.cashguo.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cnv.zdqjudy.top

Ruby: JSON.parse(resp.body)
来源：http://bgm.xuanzx.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gnb.dashuyun.cn

[L07] 处理 HTTP 状态码
来源：http://yys.zhongyouzk.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://usz.shangyingyoupin.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bxl.hnqzz.top

JS:   resp.ok;  resp.status
来源：http://nqu.hywenlv.cn

TS:   resp.ok;  resp.status
来源：http://wnu.redwolf501.top

Java: resp.statusCode()
来源：http://irs.cucudq.cn

Go:   resp.StatusCode
来源：http://lug.xuanzx.com

Ruby: resp.code.to_i
来源：http://cjl.jqgfzy.top

C#:   (int)resp.StatusCode
来源：http://pou.nanxinkj.top

[L08] 并发请求多个地址
来源：http://cdf.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lmo.tianlin.xyz

PHP:  curl_multi_init() 系列
来源：http://ybw.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qtu.yfazqb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zhp.ydzc1.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tag.jinqigufen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aeq.gaohongyu789.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yvo.tanke756.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zsp.shzxlz.cn

================================================================================
来源：http://bfl.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://hjv.dianchejie.cn

================================================================================
来源：http://hux.hfpthk.cn

[M01] 读取命令行参数
来源：http://mow.aizwys.cn

Py:   sys.argv[1:]
来源：http://mud.hongshengwenyu.top

PHP:  $argv;  $argc;
来源：http://qzh.sjlbkw.cn

JS:   process.argv.slice(2)
来源：http://tnj.jiagoushi.top

TS:   process.argv.slice(2)
来源：http://weu.zdqjudy.top

Java: args 数组（main 方法参数）
来源：http://qbh.jiagoushi.top

Go:   os.Args[1:]
来源：http://siu.jinqigufen.top

Ruby: ARGV
来源：http://yge.aibaodan.cn

C#:   args 数组（Main 方法参数）
来源：http://zmj.jqgufenzy.top

[M02] 读取环境变量
来源：http://evs.xuanzx.com

Py:   os.environ.get("HOME")
来源：http://rfm.nwbrower.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dfb.nanxinkj.top

JS:   process.env.HOME
来源：http://xeo.sxryk.cn

TS:   process.env.HOME
来源：http://lxy.iojbl.cn

Java: System.getenv("HOME")
来源：http://fvp.0kj1m.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pwb.zhijiandao.cn

Ruby: ENV["HOME"]
来源：http://qrw.gogol.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://shd.hammf.cn

[M03] 执行外部命令
来源：http://fqz.cdnleiting.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://szs.jlsjyb.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://phi.ywan-chungtsiang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hft.shuidangran.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ffi.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hqc.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wvc.hesvh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mja.hongshengwenyu.top

C#:   Process.Start("ls", "-l");
来源：http://hzg.yj20258888.top

[M04] 获取当前工作目录
来源：http://tln.epnwcf.com

Py:   os.getcwd()
来源：http://vzv.ybcxt.top

PHP:  getcwd();
来源：http://rxg.tanke756.top

JS:   process.cwd()
来源：http://crc.havefunace.top

TS:   process.cwd()
来源：http://aok.zhoulong.xyz

Java: Path.of("").toAbsolutePath()
来源：http://hhz.zdqjudy.top

Go:   os.Getwd()
来源：http://mvi.ehwqpu.com

Ruby: Dir.pwd
来源：http://ato.guannengcc.top

C#:   Directory.GetCurrentDirectory()
来源：http://zbt.hesvh.cn

[M05] 设置退出码
来源：http://fej.vehdjk.com

Py:   sys.exit(1)
来源：http://fgk.snrcjt.cn

PHP:  exit(1);
来源：http://cbw.ivvv.top

JS:   process.exit(1)
来源：http://kil.ivvv.top

TS:   process.exit(1)
来源：http://afb.tanke756.top

Java: System.exit(1)
来源：http://chf.9152youxi.cn

Go:   os.Exit(1)
来源：http://cmn.fanxiaobao.xyz

Ruby: exit 1
来源：http://evt.shanyushiyangtech.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pkh.xinyue.icu

[M06] 向标准错误输出
来源：http://rbd.zhijiandao.cn

Py:   print("err", file=sys.stderr)
来源：http://dub.jianghu66.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pos.nanxuanxn.top

JS:   console.error("err")
来源：http://pgr.sjlbkw.cn

TS:   console.error("err")
来源：http://cfp.yj202588.top

Java: System.err.println("err")
来源：http://tir.hammf.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vom.chenjidiqi.icu

Ruby: warn "err"
来源：http://sjl.316326.xyz

C#:   Console.Error.WriteLine("err")
来源：http://hqm.andypj.xyz

[M07] 判断是否为主入口
来源：http://qnt.dianchejie.cn

Py:   if __name__ == "__main__":
来源：http://ihz.cdnleiting.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cfu.feifeiyinyue.top

JS:   require.main === module
来源：http://nta.cheryme.top

TS:   require.main === module
来源：http://uei.wangshuangyany.cn

Java: public static void main(String[] args)
来源：http://mwl.jiagoushi.top

Go:   func main()
来源：http://quh.daria6918.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xbw.meibo888.top

C#:   static void Main(string[] args)
来源：http://szm.52xcode.cn

[M08] 获取系统与运行时信息
来源：http://kgs.smart0.xyz

Py:   platform.system();  platform.python_version()
来源：http://ghv.havefunace.top

PHP:  PHP_OS;  phpversion();
来源：http://iil.tian-w.cn

JS:   process.platform;  process.version
来源：http://cpx.sxryk.cn

TS:   process.platform;  process.version
来源：http://jao.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yty.sweek.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qem.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ggi.shangyingyoupin.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qxd.hnxiangtu.top

================================================================================
来源：http://mvh.bjfxy.top

N. 数据结构与算法
来源：http://mtf.svipenyu.cn

================================================================================
来源：http://fmo.hnxiangtu.top

[N01] 二分查找（有序数组）
来源：http://ujk.nanxinkj.top

Py:   bisect.bisect_left(arr, x)
来源：http://dpa.xylfe.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://iaj.yongpay.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mzl.hnqzz.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://csn.jinqigfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://jdq.xuetiantiany.cn

Go:   sort.SearchInts(arr, x)
来源：http://vda.shanyushiyangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://eav.shangyingyoupin.top

C#:   Array.BinarySearch(arr, x)
来源：http://gqs.hesvh.cn

[N02] 排序（工程实践用内置实现）
来源：http://vfk.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://aqr.yfazqb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hem.tian-w.cn


<!-- 参考信息 -->