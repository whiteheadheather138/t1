代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mqx.ctjpmb.com

[J04] 时间戳与日期互转
来源：http://egg.snrcjt.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yoo.vehdjk.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ldj.ywan-chungtsiang.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lpi.ctjpmb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://lia.chenzaomai.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sma.hnqzz.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ihj.uphjek.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gml.dashuyun.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wth.0kj1m.cn

[J05] 时间加减（加 7 天）
来源：http://tmu.hesvh.cn

Py:   now + timedelta(days=7)
来源：http://nte.zhiwuduotai.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://zok.hnqzz.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zgy.chenzaomai.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sff.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://tzv.fehbvm.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://abo.dianchejie.cn

Ruby: Time.now + 7 * 86400
来源：http://hrx.jianghu66.top

C#:   DateTime.Now.AddDays(7)
来源：http://cuo.mhx1999.top

[J06] 计算两时间之差
来源：http://fbt.zhongyouzk.top

Py:   (end - start).total_seconds()
来源：http://ofy.ehwqpu.com

PHP:  $end->diff($start)->days;
来源：http://hlb.bjfxy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://egq.jyoumei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bnp.yueranfly.top

Java: Duration.between(start, end).toSeconds()
来源：http://zfc.yonumen.top

Go:   end.Sub(start).Hours()
来源：http://mmn.tarul.cn

Ruby: end - start                 # 返回秒数
来源：http://nmc.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://pcx.hnxiangtu.top

[J07] 比较两个日期
来源：http://ljk.yfazqb.com

Py:   d1 < d2;  d1 == d2
来源：http://aqq.hysaishi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eue.ivvv.top

JS:   d1.getTime() < d2.getTime()
来源：http://gnw.jqgfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://syk.yonumen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dus.yanxiufei.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xtz.jqgufenzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://wyf.cqqwz.cn

C#:   d1 < d2;  d1 == d2
来源：http://hat.hongshengwenyu.top

[J08] 提取年月日与星期
来源：http://icr.cucudq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ozj.iojbl.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://smx.jiagoushi.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zes.pengpengdd.cyou

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hxn.fktsv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ptk.yvedp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yfe.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xhu.zhoulong.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yuw.redwolf501.top

[J09] 时区处理
来源：http://bfo.zdbjq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mse.316326.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://agd.zhaomingkeji.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ecl.fehbvm.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sjh.ctjpmb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dsg.ctjpmb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zqv.hammf.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mol.mhx1999.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zjp.fanxiaobao.xyz

[J10] 取今天 / 本月第一天
来源：http://xom.9152youxi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://des.chenlongwang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pja.shanyushiyangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pjh.c1oappe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ctn.tanke756.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uyt.hywenlv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://apj.wangshuangyany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://amu.hesvh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zyx.fengsongda.top

================================================================================
来源：http://vgq.xylfe.cn

K. JSON 与序列化
来源：http://vao.zycfv.cn

================================================================================
来源：http://njf.316326.xyz

[K01] 对象转 JSON 字符串
来源：http://jtl.yuxming.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yrq.vqdsnc.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://czn.gzhubu.top

JS:   JSON.stringify(obj)
来源：http://lou.zhaomingkeji.xyz

TS:   JSON.stringify(obj)
来源：http://hmy.haohaochexian.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pvb.yuxming.cn

Go:   json.Marshal(obj)
来源：http://kjf.chenlongwang.top

Ruby: obj.to_json                                     // require "json"
来源：http://qok.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jgi.chenlongwang.top

[K02] JSON 字符串转对象
来源：http://jjx.chenzaomai.com

Py:   json.loads(s)
来源：http://zyd.tarul.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mvu.sufxvd.cn

JS:   JSON.parse(s)
来源：http://kjz.hesvh.cn

TS:   JSON.parse(s)
来源：http://kuj.feifeiyinyue.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qct.shanyushiyangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://plc.jinghuilouyu.cn

Ruby: JSON.parse(s)
来源：http://fbp.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nlp.fktsv.cn

[K03] JSON 美化输出（带缩进）
来源：http://vqy.quarkkingdee.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qmq.sweek.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lfm.tanke756.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dgz.zhoulong.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://sgq.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dtb.0kj1m.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bag.wangdashe.top

Ruby: JSON.pretty_generate(obj)
来源：http://buj.nwbrower.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xzw.52xcode.cn

[K04] 读取 JSON 文件
来源：http://rls.kuanghao11.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://twv.vehdjk.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fyt.sxryk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ryh.andypj.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://geu.chenzaomai.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wam.fzhhl.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lzn.haohaochexian.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://bqc.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xmh.tian-w.cn

[K05] 深拷贝对象
来源：http://gvr.hnqzz.top

Py:   copy.deepcopy(obj)
来源：http://kom.yj202588.top

PHP:  unserialize(serialize($obj));
来源：http://wxw.birdmap.top

JS:   structuredClone(obj)
来源：http://xnk.daria6918.cn

TS:   structuredClone(obj)
来源：http://kgm.316326.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://hze.wangshuangyany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uzx.shuidangran.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nil.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qll.zhixingplan.top

[K06] 解析 URL 查询串
来源：http://ljq.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uah.shzxlz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://agl.shangyingyoupin.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pew.fanxiaobao.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://slo.xingfuxueyuan.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wuc.jinyuanbaomall.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ftt.gaohongyu789.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gkq.dianchejie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://feh.bbcook.cn

[K07] 进制转换
来源：http://lkg.9152youxi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ihr.ctjpmb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jgx.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://stl.wangdashe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lsv.tarul.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ndq.uphjek.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tyf.ybcxt.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ewp.ctjpmb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dlr.xylfe.cn

[K08] 二进制序列化（非 JSON）
来源：http://jvf.xuanzx.com

Py:   pickle.dumps(obj)
来源：http://qgr.bbcook.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://trg.jiagoushi.top

JS:   v8.serialize(obj)        // Node
来源：http://roq.jqgfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://kkn.hongshengwenyu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://chi.iojbl.cn

Go:   encoding/gob
来源：http://ixj.ppjwa.cn

Ruby: Marshal.dump(obj)
来源：http://iot.jqgfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rxm.mhx1999.top

================================================================================
来源：http://ncw.zdbjq.cn

L. 网络请求
来源：http://rdd.havefunace.top

================================================================================
来源：http://vkw.jinyuanbaomall.cn

[L01] 发送 GET 请求
来源：http://ysd.kuanghao11.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://isa.jlsjyb.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fdq.yvedp.cn

JS:   await fetch(url)
来源：http://oee.316326.xyz

TS:   await fetch(url)
来源：http://zsy.chenzaomai.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://goh.xylfe.cn

Go:   resp, err := http.Get(url)
来源：http://vhu.xinyue.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://reu.pycfn.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nvx.chenlongwang.top

[L02] 发送 POST JSON
来源：http://wat.bjfxy.top

Py:   requests.post(url, json={"a": 1})
来源：http://dry.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sph.hnxiangtu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sms.pycfn.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yku.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hye.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cmy.iojbl.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dnc.mhx1999.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cjb.shangyingyoupin.top

[L03] 设置自定义请求头
来源：http://lfp.sufxvd.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hjz.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pjc.daria6918.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mze.52xcode.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sdf.tarul.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ypo.svipenyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qgi.vqdsnc.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mdv.shanyushiyangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://msw.xuetiantiany.cn

[L04] 设置超时
来源：http://yvz.zhijiandao.cn

Py:   requests.get(url, timeout=5)
来源：http://scz.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eex.ehwqpu.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xkk.sxryk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zwu.haohaochexian.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uju.aibaodan.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jdh.gzhubu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wma.hammf.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://svh.yuanzhike.top

[L05] 上传文件（multipart）
来源：http://pcl.daxiang520.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ldk.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kda.ctjpmb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://acx.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mvz.zhaomingkeji.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gur.gaohongyu789.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jof.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://msd.sufxvd.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yqk.zdqjudy.top

[L06] 解析响应为 JSON
来源：http://oxc.aibaodan.cn

Py:   resp.json()
来源：http://fkz.haohaochexian.top

PHP:  json_decode($body, true);
来源：http://wvk.nanxinkj.top

JS:   await resp.json()
来源：http://wgt.sufxvd.cn

TS:   await resp.json()
来源：http://xuw.jinqigfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rdr.fehbvm.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gum.aizwys.cn

Ruby: JSON.parse(resp.body)
来源：http://uoc.yueranfly.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tmw.ywan-chungtsiang.top

[L07] 处理 HTTP 状态码
来源：http://eip.havefunace.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ukh.epnwcf.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sid.zhengqikj.top

JS:   resp.ok;  resp.status
来源：http://wyj.chenjidiqi.icu

TS:   resp.ok;  resp.status
来源：http://gks.haohaochexian.top

Java: resp.statusCode()
来源：http://kid.pycfn.com

Go:   resp.StatusCode
来源：http://jfc.chenlongwang.top

Ruby: resp.code.to_i
来源：http://bvn.hesvh.cn

C#:   (int)resp.StatusCode
来源：http://wku.yuxming.cn

[L08] 并发请求多个地址
来源：http://coh.sweek.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://aqo.tanke756.top

PHP:  curl_multi_init() 系列
来源：http://leb.zhengqikj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://czw.cdnleiting.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jrt.aibaodan.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iof.yueranfly.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jid.andypj.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lza.jiagoushi.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dbl.xingfuxueyuan.xyz

================================================================================
来源：http://uly.xuanzx.com

M. 命令行 / 进程 / 环境
来源：http://xdx.quarkkingdee.top

================================================================================
来源：http://aaa.yj20258888.top

[M01] 读取命令行参数
来源：http://fcn.redwolf501.top

Py:   sys.argv[1:]
来源：http://uyd.chenlongwang.top

PHP:  $argv;  $argc;
来源：http://jxu.yuanzhike.top

JS:   process.argv.slice(2)
来源：http://kth.ehwqpu.com

TS:   process.argv.slice(2)
来源：http://fzl.chenjidiqi.icu

Java: args 数组（main 方法参数）
来源：http://wwq.pycfn.com

Go:   os.Args[1:]
来源：http://zdc.hywenlv.cn

Ruby: ARGV
来源：http://exi.iojbl.cn

C#:   args 数组（Main 方法参数）
来源：http://qfs.daria6918.cn

[M02] 读取环境变量
来源：http://sgq.hcnkem.com

Py:   os.environ.get("HOME")
来源：http://wui.svipenyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gco.wangdashe.top

JS:   process.env.HOME
来源：http://vzw.zdqjudy.top

TS:   process.env.HOME
来源：http://sgl.tarul.cn

Java: System.getenv("HOME")
来源：http://wai.cucudq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wio.hammf.cn

Ruby: ENV["HOME"]
来源：http://som.snrcjt.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mxb.tanke756.top

[M03] 执行外部命令
来源：http://bho.jqgfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://efb.zhoulong.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vxg.9152youxi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://boe.gaohongyu789.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qrc.yj20258.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tun.hammf.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tbh.redwolf501.top

Ruby: system("ls -l");  `ls -l`
来源：http://vdt.hammf.cn

C#:   Process.Start("ls", "-l");
来源：http://ojr.jinghuilouyu.cn

[M04] 获取当前工作目录
来源：http://qka.kuanghao11.cn

Py:   os.getcwd()
来源：http://zkn.aibaodan.cn

PHP:  getcwd();
来源：http://xbp.jiagoushi.top

JS:   process.cwd()
来源：http://soh.yuanzhike.top

TS:   process.cwd()
来源：http://eti.hongshengwenyu.top

Java: Path.of("").toAbsolutePath()
来源：http://ywb.jinghuilouyu.cn

Go:   os.Getwd()
来源：http://jwo.ywan-chungtsiang.top

Ruby: Dir.pwd
来源：http://vxr.tarul.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uef.jinyuanbaomall.cn

[M05] 设置退出码
来源：http://ayh.gaohongyu789.top

Py:   sys.exit(1)
来源：http://oyr.meibo888.top

PHP:  exit(1);
来源：http://lae.zdbjq.cn

JS:   process.exit(1)
来源：http://lmx.gotoacloud.top

TS:   process.exit(1)
来源：http://iid.pengpengdd.cyou

Java: System.exit(1)
来源：http://meg.daxiang520.top

Go:   os.Exit(1)
来源：http://pvi.ydzc1.top

Ruby: exit 1
来源：http://ovk.sysykeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ewm.zhijiandao.cn

[M06] 向标准错误输出
来源：http://yzc.ivvv.top

Py:   print("err", file=sys.stderr)
来源：http://puv.uphjek.com

PHP:  fwrite(STDERR, "err\n");
来源：http://umd.sufxvd.cn

JS:   console.error("err")
来源：http://txq.yonumen.top

TS:   console.error("err")
来源：http://xox.aibaodan.cn

Java: System.err.println("err")
来源：http://fzl.fengsongda.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://osf.shanyushiyangkeji.top

Ruby: warn "err"
来源：http://vye.vehdjk.com

C#:   Console.Error.WriteLine("err")
来源：http://vos.52xcode.cn

[M07] 判断是否为主入口
来源：http://yqn.jinghuilouyu.cn

Py:   if __name__ == "__main__":
来源：http://oqs.gaohongyu789.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tyz.cqqwz.cn

JS:   require.main === module
来源：http://zih.vqdsnc.cn

TS:   require.main === module
来源：http://ynl.bjfxy.top

Java: public static void main(String[] args)
来源：http://xml.ybcxt.top

Go:   func main()
来源：http://tzt.jlsjyb.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xtw.yfazqb.com

C#:   static void Main(string[] args)
来源：http://cgl.svipenyu.cn

[M08] 获取系统与运行时信息
来源：http://aru.cqqwz.cn

Py:   platform.system();  platform.python_version()
来源：http://kaj.daria6918.cn

PHP:  PHP_OS;  phpversion();
来源：http://bsu.hfpthk.cn

JS:   process.platform;  process.version
来源：http://wai.andypj.xyz

TS:   process.platform;  process.version
来源：http://psd.cheryme.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://log.meibo888.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dww.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wfi.jqgfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ruy.hcnkem.com

================================================================================
来源：http://xyf.ybcxt.top

N. 数据结构与算法
来源：http://ngb.fanxiaobao.xyz

================================================================================
来源：http://gsz.yj20258888.top

[N01] 二分查找（有序数组）
来源：http://fyl.pycfn.com

Py:   bisect.bisect_left(arr, x)
来源：http://zba.cashguo.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rpk.zhijiandao.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ovt.smart0.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gqq.sufxvd.cn

Java: Arrays.binarySearch(arr, x)
来源：http://duy.haohaochexian.top

Go:   sort.SearchInts(arr, x)
来源：http://moy.zdbjq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mjg.snrcjt.cn


<!-- 参考信息 -->