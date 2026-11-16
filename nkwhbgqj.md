代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mmh.hongshengwenyu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tdj.zhaomingkeji.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://izn.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cyd.jlsjyb.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://din.ywan-chungtsiang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gep.bjfxy.top

[J05] 时间加减（加 7 天）
来源：http://vtl.snrcjt.cn

Py:   now + timedelta(days=7)
来源：http://exj.zhengqikj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hyr.hammf.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://occ.cashguo.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ugi.shangyingyoupin.top

Java: LocalDate.now().plusDays(7)
来源：http://uip.jyoumei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://enl.daxiang520.top

Ruby: Time.now + 7 * 86400
来源：http://eoi.xuanzx.com

C#:   DateTime.Now.AddDays(7)
来源：http://gpb.kuanghao11.cn

[J06] 计算两时间之差
来源：http://jmx.xylfe.cn

Py:   (end - start).total_seconds()
来源：http://bnd.ydjk.org.cn

PHP:  $end->diff($start)->days;
来源：http://bqi.kuanghao11.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nba.yonumen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dii.quarkkingdee.top

Java: Duration.between(start, end).toSeconds()
来源：http://gnh.aizwys.cn

Go:   end.Sub(start).Hours()
来源：http://zkb.cucudq.cn

Ruby: end - start                 # 返回秒数
来源：http://ebt.aizwys.cn

C#:   (end - start).TotalSeconds
来源：http://bqo.wangdashe.top

[J07] 比较两个日期
来源：http://mqt.shzxlz.cn

Py:   d1 < d2;  d1 == d2
来源：http://bry.yj20258.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tvg.chenjidiqi.icu

JS:   d1.getTime() < d2.getTime()
来源：http://znh.tarul.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ogm.shzxlz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xae.chenjidiqi.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://apg.shuidangran.top

Ruby: d1 < d2;  d1 == d2
来源：http://oqw.hysaishi.cn

C#:   d1 < d2;  d1 == d2
来源：http://jsh.zdqjudy.top

[J08] 提取年月日与星期
来源：http://okb.cashguo.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vvh.zdqjudy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xvq.vqdsnc.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://asm.52xcode.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hun.jqgufenzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dmq.yanxiufei.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dft.shuidangran.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://soa.cheryme.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qtv.dashuyun.cn

[J09] 时区处理
来源：http://hdp.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nyz.zhixingplan.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cmq.zdqjudy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hps.xziqi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hvx.tianlin.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gcs.hammf.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bss.dianchejie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://aua.zhengqikj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hon.zhengqikj.top

[J10] 取今天 / 本月第一天
来源：http://cbu.xinyue.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://yxv.bjfxy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cui.meibo888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qev.chenzaomai.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://peo.gzhubu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ouq.wangdashe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://akv.jianghu66.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qzs.hcnkem.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://piq.gzhubu.top

================================================================================
来源：http://ykp.yanxiufei.cn

K. JSON 与序列化
来源：http://vjx.52xcode.cn

================================================================================
来源：http://rvk.yonumen.top

[K01] 对象转 JSON 字符串
来源：http://fbo.tarul.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tcf.havefunace.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oot.jinqigfzy.top

JS:   JSON.stringify(obj)
来源：http://vnt.vehdjk.com

TS:   JSON.stringify(obj)
来源：http://uvw.fanxiaobao.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://asr.vehdjk.com

Go:   json.Marshal(obj)
来源：http://ddt.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ilv.zhiwuduotai.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jjz.chenlongwang.top

[K02] JSON 字符串转对象
来源：http://kjx.hnxiangtu.top

Py:   json.loads(s)
来源：http://vfe.zhijiandao.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gkg.sufxvd.cn

JS:   JSON.parse(s)
来源：http://crp.yonumen.top

TS:   JSON.parse(s)
来源：http://ghg.chenzaomai.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vmw.zhaomingkeji.xyz

Go:   json.Unmarshal(data, &v)
来源：http://aby.jinyuanbaomall.cn

Ruby: JSON.parse(s)
来源：http://ujd.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ffm.jqgfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://uso.aizwys.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mcb.birdmap.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yhd.mhx1999.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jpu.jyoumei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ash.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tyo.zhaomingkeji.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uio.snrcjt.cn

Ruby: JSON.pretty_generate(obj)
来源：http://smx.hfpthk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xql.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://ymk.yvedp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://roy.jiagoushi.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rcr.guannengcc.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ebc.sjlbkw.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ljx.yfazqb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kgj.epnwcf.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ndk.smart0.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://iju.ivvv.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wjn.ppjwa.cn

[K05] 深拷贝对象
来源：http://guk.yuanzhike.top

Py:   copy.deepcopy(obj)
来源：http://fec.birdmap.top

PHP:  unserialize(serialize($obj));
来源：http://waq.yj20258888.top

JS:   structuredClone(obj)
来源：http://uww.chenlongwang.top

TS:   structuredClone(obj)
来源：http://hel.guowangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jqp.tian-w.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fbn.feifeiyinyue.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://orc.ybcxt.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ncz.snrcjt.cn

[K06] 解析 URL 查询串
来源：http://rek.feifeiyinyue.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jyr.gzhubu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ezj.zdbjq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mzo.tarul.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oyc.gotoacloud.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aso.zhongyouzk.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mfa.aizwys.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gwn.hysaishi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ntj.gogol.net.cn

[K07] 进制转换
来源：http://tqz.gzhubu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://txs.jyoumei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jji.chenzaomai.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yoi.ydzc1.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://utc.zhongyouzk.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jls.chenzaomai.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gli.yueranfly.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nyi.pengpengdd.cyou

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fwg.jlsjyb.cn

[K08] 二进制序列化（非 JSON）
来源：http://hch.meibo888.top

Py:   pickle.dumps(obj)
来源：http://oju.xylfe.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gvq.nwbrower.top

JS:   v8.serialize(obj)        // Node
来源：http://jhy.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://ica.zhijiandao.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wkm.pengpengdd.cyou

Go:   encoding/gob
来源：http://gpi.jinghuilouyu.cn

Ruby: Marshal.dump(obj)
来源：http://sqh.jyoumei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ufh.jiagoushi.top

================================================================================
来源：http://vnh.hcnkem.com

L. 网络请求
来源：http://zmu.hnqzz.top

================================================================================
来源：http://aws.zycfv.cn

[L01] 发送 GET 请求
来源：http://ihx.jinyuanbaomall.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cmb.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ceq.ybcxt.top

JS:   await fetch(url)
来源：http://pyy.hongshengwenyu.top

TS:   await fetch(url)
来源：http://acb.yongpay.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aci.gogol.net.cn

Go:   resp, err := http.Get(url)
来源：http://kct.chenlongwang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hzs.zhixingplan.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://whn.jianghu66.top

[L02] 发送 POST JSON
来源：http://mls.hesvh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://krw.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mze.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fmi.hnqzz.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://koe.jiagoushi.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lts.ybcxt.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ktq.gaohongyu789.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qzh.zhongyouzk.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vlq.jinyuanbaomall.cn

[L03] 设置自定义请求头
来源：http://cny.hywenlv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lye.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mla.zhiwuduotai.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wyj.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wjq.yangfankeji.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ygt.yj202588.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lij.snrcjt.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xrs.zhiwuduotai.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://puj.birdmap.top

[L04] 设置超时
来源：http://lqd.guowangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://swp.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tht.nanxinkj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sry.zhaomingkeji.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kjm.jqgfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nlo.hfpthk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jkq.dianchejie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xkg.havefunace.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dgo.nwbrower.top

[L05] 上传文件（multipart）
来源：http://fue.snrcjt.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dmt.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ifk.guannengcc.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pgl.yonumen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cvm.jinqigufen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xzk.zdqjudy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://urg.zhiwuduotai.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jwi.9152youxi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hba.shanyushiyangtech.top

[L06] 解析响应为 JSON
来源：http://kbd.feifeiyinyue.top

Py:   resp.json()
来源：http://cms.yj20258.top

PHP:  json_decode($body, true);
来源：http://xcq.guannengcc.top

JS:   await resp.json()
来源：http://zhb.hesvh.cn

TS:   await resp.json()
来源：http://zxp.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nun.wangshuangyany.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vvz.ydjk.org.cn

Ruby: JSON.parse(resp.body)
来源：http://pfo.ivvv.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bts.aibaodan.cn

[L07] 处理 HTTP 状态码
来源：http://hvv.chenzaomai.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sjy.sxryk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nmc.fanxiaobao.xyz

JS:   resp.ok;  resp.status
来源：http://gxm.aibaodan.cn

TS:   resp.ok;  resp.status
来源：http://fha.tian-w.cn

Java: resp.statusCode()
来源：http://wzv.smart0.xyz

Go:   resp.StatusCode
来源：http://cva.ehwqpu.com

Ruby: resp.code.to_i
来源：http://qek.xylfe.cn

C#:   (int)resp.StatusCode
来源：http://ngf.smart0.xyz

[L08] 并发请求多个地址
来源：http://qni.jqgufenzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sgi.ctjpmb.com

PHP:  curl_multi_init() 系列
来源：http://slu.havefunace.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vtu.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://acg.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yfa.daria6918.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://esw.chenzaomai.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://khp.svipenyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mfx.yuxming.cn

================================================================================
来源：http://zsq.jinqigufen.top

M. 命令行 / 进程 / 环境
来源：http://grn.xuetiantiany.cn

================================================================================
来源：http://mvf.snrcjt.cn

[M01] 读取命令行参数
来源：http://lom.xinyue.icu

Py:   sys.argv[1:]
来源：http://tui.shzxlz.cn

PHP:  $argv;  $argc;
来源：http://ewl.shuidangran.top

JS:   process.argv.slice(2)
来源：http://dll.hysaishi.cn

TS:   process.argv.slice(2)
来源：http://pvp.yj20258.top

Java: args 数组（main 方法参数）
来源：http://ovd.yj202588.top

Go:   os.Args[1:]
来源：http://vgu.zhaomingkeji.xyz

Ruby: ARGV
来源：http://oej.tarul.cn

C#:   args 数组（Main 方法参数）
来源：http://jys.quarkkingdee.top

[M02] 读取环境变量
来源：http://dkz.nanxuanxn.top

Py:   os.environ.get("HOME")
来源：http://nos.xylfe.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ise.xylfe.cn

JS:   process.env.HOME
来源：http://xfx.fehbvm.com

TS:   process.env.HOME
来源：http://ond.hfpthk.cn

Java: System.getenv("HOME")
来源：http://btc.dianchejie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fuf.ehwqpu.com

Ruby: ENV["HOME"]
来源：http://xiy.hysaishi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qis.wangshuangyany.cn

[M03] 执行外部命令
来源：http://pke.0kj1m.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gng.fanxiaobao.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xzp.hammf.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dbm.shanyushiyangtech.top

TS:   child_process.execSync("ls -l").toString()
来源：http://eca.zycfv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jlp.hammf.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dzj.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pvm.wangdashe.top

C#:   Process.Start("ls", "-l");
来源：http://bqy.vqdsnc.cn

[M04] 获取当前工作目录
来源：http://vsj.xziqi.cn

Py:   os.getcwd()
来源：http://ymq.yanxiufei.cn

PHP:  getcwd();
来源：http://ojc.sxryk.cn

JS:   process.cwd()
来源：http://egb.0kj1m.cn

TS:   process.cwd()
来源：http://azc.guannengcc.top

Java: Path.of("").toAbsolutePath()
来源：http://ama.daxiang520.top

Go:   os.Getwd()
来源：http://jxl.andypj.xyz

Ruby: Dir.pwd
来源：http://npz.shangyingyoupin.top

C#:   Directory.GetCurrentDirectory()
来源：http://ryv.vqdsnc.cn

[M05] 设置退出码
来源：http://hjk.guowangkeji.top

Py:   sys.exit(1)
来源：http://rgo.tian-w.cn

PHP:  exit(1);
来源：http://kdd.zhiwuduotai.top

JS:   process.exit(1)
来源：http://lrr.fehbvm.com

TS:   process.exit(1)
来源：http://rwg.bbcook.cn

Java: System.exit(1)
来源：http://iun.guowangkeji.top

Go:   os.Exit(1)
来源：http://rls.zhaomingkeji.xyz

Ruby: exit 1
来源：http://jly.yuxming.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jxv.redwolf501.top

[M06] 向标准错误输出
来源：http://hay.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://bhv.yanxiufei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tak.zhoulong.xyz

JS:   console.error("err")
来源：http://hhh.epnwcf.com

TS:   console.error("err")
来源：http://mnn.ivvv.top

Java: System.err.println("err")
来源：http://xwk.smart0.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pyf.andypj.xyz

Ruby: warn "err"
来源：http://qrp.zhixingplan.top

C#:   Console.Error.WriteLine("err")
来源：http://bnm.hammf.cn

[M07] 判断是否为主入口
来源：http://zdv.hesvh.cn

Py:   if __name__ == "__main__":
来源：http://vuo.zhijiandao.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nxi.jinyuanbaomall.cn

JS:   require.main === module
来源：http://bpz.yuanzhike.top

TS:   require.main === module
来源：http://dzk.hywenlv.cn

Java: public static void main(String[] args)
来源：http://fco.cqqwz.cn

Go:   func main()
来源：http://akp.ehwqpu.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qth.nanxuanxn.top

C#:   static void Main(string[] args)
来源：http://uta.zdbjq.cn

[M08] 获取系统与运行时信息
来源：http://vcl.316326.xyz

Py:   platform.system();  platform.python_version()
来源：http://wzm.hysaishi.cn

PHP:  PHP_OS;  phpversion();
来源：http://wyo.yonumen.top

JS:   process.platform;  process.version
来源：http://skc.yj20258888.top

TS:   process.platform;  process.version
来源：http://pfz.9152youxi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rlc.bbcook.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jha.zhengqikj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://adi.zhiwuduotai.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nsx.zhoulong.xyz

================================================================================
来源：http://cfs.hnqzz.top

N. 数据结构与算法
来源：http://uqb.fehbvm.com

================================================================================
来源：http://rmp.quarkkingdee.top

[N01] 二分查找（有序数组）
来源：http://qkh.aibaodan.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ygt.hnqzz.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hvc.snrcjt.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tzq.birdmap.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vxx.pycfn.com

Java: Arrays.binarySearch(arr, x)
来源：http://dyv.sufxvd.cn

Go:   sort.SearchInts(arr, x)
来源：http://zzb.tarul.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ndl.hnqzz.top

C#:   Array.BinarySearch(arr, x)
来源：http://byw.gogol.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://bxg.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://thv.zycfv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hmj.jqgufenzy.top


<!-- 参考信息 -->