代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://knm.daria6918.cn

[J04] 时间戳与日期互转
来源：http://mdk.316326.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gvo.ivvv.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jmk.tianlin.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jrl.zycfv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hbo.fehbvm.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kzk.feifeiyinyue.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qkg.hysaishi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cji.sufxvd.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lgw.sjlbkw.cn

[J05] 时间加减（加 7 天）
来源：http://ihb.fzhhl.top

Py:   now + timedelta(days=7)
来源：http://omy.yueranfly.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://oaz.gzhubu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iuu.xuanzx.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ynt.zhiwuduotai.top

Java: LocalDate.now().plusDays(7)
来源：http://jsi.xuetiantiany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://faj.xylfe.cn

Ruby: Time.now + 7 * 86400
来源：http://gji.ydjk.org.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bqh.meibo888.top

[J06] 计算两时间之差
来源：http://rks.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://lpw.epnwcf.com

PHP:  $end->diff($start)->days;
来源：http://wqu.jinghuilouyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fqu.andypj.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dsq.jyoumei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pwe.xingfuxueyuan.xyz

Go:   end.Sub(start).Hours()
来源：http://gyj.nanxinkj.top

Ruby: end - start                 # 返回秒数
来源：http://auv.xziqi.cn

C#:   (end - start).TotalSeconds
来源：http://xqf.jianghu66.top

[J07] 比较两个日期
来源：http://eqf.yangfankeji.com

Py:   d1 < d2;  d1 == d2
来源：http://pan.tarul.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bfd.fehbvm.com

JS:   d1.getTime() < d2.getTime()
来源：http://mkd.yangfankeji.com

TS:   d1.getTime() < d2.getTime()
来源：http://fwi.yvedp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uvc.zycfv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dhh.nanxinkj.top

Ruby: d1 < d2;  d1 == d2
来源：http://whx.xylfe.cn

C#:   d1 < d2;  d1 == d2
来源：http://iip.yanxiufei.cn

[J08] 提取年月日与星期
来源：http://hjj.cashguo.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hcd.yj20258888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hpi.zycfv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://aws.shuidangran.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://osx.nanxinkj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fac.yuxming.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zvj.pengpengdd.cyou

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pcq.dianchejie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://icy.zhiwuduotai.top

[J09] 时区处理
来源：http://rzb.iojbl.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bhj.zhijiandao.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jmf.vqdsnc.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lfq.xingfuxueyuan.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lcp.mhx1999.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://grc.hfpthk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ssr.dashuyun.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nnk.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cmn.sweek.top

[J10] 取今天 / 本月第一天
来源：http://ivo.xuanzx.com

Py:   date.today();  date.today().replace(day=1)
来源：http://lat.xuanzx.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ffh.jiagoushi.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lxm.tarul.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rlu.nanxuanxn.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ksz.xziqi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vhp.bjfxy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jzx.feifeiyinyue.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nkp.hysaishi.cn

================================================================================
来源：http://ohd.zhixingplan.top

K. JSON 与序列化
来源：http://rcx.guowangkeji.top

================================================================================
来源：http://icr.yueranfly.top

[K01] 对象转 JSON 字符串
来源：http://zav.hesvh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fjx.ppjwa.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://teq.ivvv.top

JS:   JSON.stringify(obj)
来源：http://hqx.andypj.xyz

TS:   JSON.stringify(obj)
来源：http://adl.sufxvd.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rge.hysaishi.cn

Go:   json.Marshal(obj)
来源：http://uzy.daria6918.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xnu.gogol.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tgd.cdnleiting.top

[K02] JSON 字符串转对象
来源：http://gqn.birdmap.top

Py:   json.loads(s)
来源：http://xwt.yuxming.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cti.fehbvm.com

JS:   JSON.parse(s)
来源：http://vdv.zhaomingkeji.xyz

TS:   JSON.parse(s)
来源：http://bht.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iay.jlsjyb.cn

Go:   json.Unmarshal(data, &v)
来源：http://xql.iojbl.cn

Ruby: JSON.parse(s)
来源：http://vzz.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dpj.jyoumei.cn

[K03] JSON 美化输出（带缩进）
来源：http://zez.fzhhl.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://irj.yanxiufei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://atn.quarkkingdee.top

JS:   JSON.stringify(obj, null, 2)
来源：http://poz.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wrp.xylfe.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qnh.jyoumei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rwg.yvedp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://arp.wangdashe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jah.smart0.xyz

[K04] 读取 JSON 文件
来源：http://meo.yueranfly.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cls.dianchejie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ueh.andypj.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pxs.vqdsnc.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://utz.yonumen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jyd.zhongyouzk.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xcu.sxryk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qvf.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jye.smart0.xyz

[K05] 深拷贝对象
来源：http://ghz.shuidangran.top

Py:   copy.deepcopy(obj)
来源：http://noo.0kj1m.cn

PHP:  unserialize(serialize($obj));
来源：http://jty.svipenyu.cn

JS:   structuredClone(obj)
来源：http://ley.shanyushiyangkeji.top

TS:   structuredClone(obj)
来源：http://voc.tian-w.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rst.zhoulong.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://enr.chenlongwang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qfo.zhixingplan.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yny.quarkkingdee.top

[K06] 解析 URL 查询串
来源：http://qmu.guowangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uds.dashuyun.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://efi.ehwqpu.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nor.zhongyouzk.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zkm.pengpengdd.cyou

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ooh.jlsjyb.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://njj.birdmap.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zhn.zhixingplan.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ekg.hcnkem.com

[K07] 进制转换
来源：http://yod.tarul.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aci.yangfankeji.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rwe.havefunace.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rpp.ywan-chungtsiang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ldc.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://evp.feifeiyinyue.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lnt.wangshuangyany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://she.shanyushiyangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qgp.hongshengwenyu.top

[K08] 二进制序列化（非 JSON）
来源：http://stv.shuidangran.top

Py:   pickle.dumps(obj)
来源：http://wrg.xingfuxueyuan.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://lsx.ybcxt.top

JS:   v8.serialize(obj)        // Node
来源：http://pau.jyoumei.cn

TS:   v8.serialize(obj)        // Node
来源：http://ypb.birdmap.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://egg.zycfv.cn

Go:   encoding/gob
来源：http://fjl.sufxvd.cn

Ruby: Marshal.dump(obj)
来源：http://tnv.ctjpmb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uvg.hesvh.cn

================================================================================
来源：http://yjf.sjlbkw.cn

L. 网络请求
来源：http://pto.jinyuanbaomall.cn

================================================================================
来源：http://lpt.shzxlz.cn

[L01] 发送 GET 请求
来源：http://ssh.yuanzhike.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rcl.dianchejie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hzp.meibo888.top

JS:   await fetch(url)
来源：http://xcv.yvedp.cn

TS:   await fetch(url)
来源：http://nlv.kuanghao11.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hhp.nwbrower.top

Go:   resp, err := http.Get(url)
来源：http://frg.svipenyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bvz.quarkkingdee.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rct.yj20258888.top

[L02] 发送 POST JSON
来源：http://jxv.ydzc1.top

Py:   requests.post(url, json={"a": 1})
来源：http://qat.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dzm.ivvv.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pnk.havefunace.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rte.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qvv.bjfxy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vho.yongpay.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://moy.c1oappe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uhn.jiagoushi.top

[L03] 设置自定义请求头
来源：http://hkz.iojbl.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nwt.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yni.wangshuangyany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fyi.iojbl.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bbf.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sec.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://umy.hywenlv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vcu.hfpthk.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kia.jlsjyb.cn

[L04] 设置超时
来源：http://ryj.zhixingplan.top

Py:   requests.get(url, timeout=5)
来源：http://dsv.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dzv.wangshuangyany.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gxz.chenzaomai.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jhx.fanxiaobao.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vjv.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yvm.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hok.uphjek.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rzk.fanxiaobao.xyz

[L05] 上传文件（multipart）
来源：http://lux.gogol.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bun.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mua.hesvh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xoo.ybcxt.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zmg.aizwys.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rkk.aibaodan.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rms.hfpthk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cec.zdqjudy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iqx.birdmap.top

[L06] 解析响应为 JSON
来源：http://tzk.shzxlz.cn

Py:   resp.json()
来源：http://ttk.guowangkeji.top

PHP:  json_decode($body, true);
来源：http://wsl.tianlin.xyz

JS:   await resp.json()
来源：http://srj.fengsongda.top

TS:   await resp.json()
来源：http://yhp.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://izz.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yap.yj202588.top

Ruby: JSON.parse(resp.body)
来源：http://adh.iojbl.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hpb.jianghu66.top

[L07] 处理 HTTP 状态码
来源：http://lxc.xuetiantiany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ist.hnxiangtu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://van.quarkkingdee.top

JS:   resp.ok;  resp.status
来源：http://exh.bbcook.cn

TS:   resp.ok;  resp.status
来源：http://gqj.jianghu66.top

Java: resp.statusCode()
来源：http://nnw.jqgufenzy.top

Go:   resp.StatusCode
来源：http://wfw.xuetiantiany.cn

Ruby: resp.code.to_i
来源：http://hxn.xinyue.icu

C#:   (int)resp.StatusCode
来源：http://shm.guowangkeji.top

[L08] 并发请求多个地址
来源：http://qrt.yuxming.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tzr.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://cwf.xylfe.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://faf.yonumen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bjx.ywan-chungtsiang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jzu.gogol.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tjn.fehbvm.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eju.svipenyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://caw.vehdjk.com

================================================================================
来源：http://fha.yj202588.top

M. 命令行 / 进程 / 环境
来源：http://qks.zhoulong.xyz

================================================================================
来源：http://jri.zhaomingkeji.xyz

[M01] 读取命令行参数
来源：http://bka.zdqjudy.top

Py:   sys.argv[1:]
来源：http://axs.pengpengdd.cyou

PHP:  $argv;  $argc;
来源：http://lav.birdmap.top

JS:   process.argv.slice(2)
来源：http://zzv.ehwqpu.com

TS:   process.argv.slice(2)
来源：http://mur.ybcxt.top

Java: args 数组（main 方法参数）
来源：http://ncn.gotoacloud.top

Go:   os.Args[1:]
来源：http://jqk.chenjidiqi.icu

Ruby: ARGV
来源：http://jxp.uphjek.com

C#:   args 数组（Main 方法参数）
来源：http://qvf.hywenlv.cn

[M02] 读取环境变量
来源：http://yzk.hesvh.cn

Py:   os.environ.get("HOME")
来源：http://ggh.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pue.hnqzz.top

JS:   process.env.HOME
来源：http://awn.chenjidiqi.icu

TS:   process.env.HOME
来源：http://ror.ywan-chungtsiang.top

Java: System.getenv("HOME")
来源：http://msy.pengpengdd.cyou

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ytf.ywan-chungtsiang.top

Ruby: ENV["HOME"]
来源：http://eak.fzhhl.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://soz.hcnkem.com

[M03] 执行外部命令
来源：http://sac.hongshengwenyu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pcp.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pdr.yongpay.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cai.xingfuxueyuan.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://dch.dashuyun.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wlj.tanke756.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bpg.cdnleiting.top

Ruby: system("ls -l");  `ls -l`
来源：http://ncp.zhiwuduotai.top

C#:   Process.Start("ls", "-l");
来源：http://szs.tian-w.cn

[M04] 获取当前工作目录
来源：http://wuz.zhiwuduotai.top

Py:   os.getcwd()
来源：http://hpx.uphjek.com

PHP:  getcwd();
来源：http://qib.xingfuxueyuan.xyz

JS:   process.cwd()
来源：http://rsq.xingfuxueyuan.xyz

TS:   process.cwd()
来源：http://qua.birdmap.top

Java: Path.of("").toAbsolutePath()
来源：http://sxb.hysaishi.cn

Go:   os.Getwd()
来源：http://lhd.fanxiaobao.xyz

Ruby: Dir.pwd
来源：http://ofk.zdbjq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kwv.sufxvd.cn

[M05] 设置退出码
来源：http://wkf.jinqigfzy.top

Py:   sys.exit(1)
来源：http://qeu.wangdashe.top

PHP:  exit(1);
来源：http://qsz.cashguo.top

JS:   process.exit(1)
来源：http://cax.redwolf501.top

TS:   process.exit(1)
来源：http://ciq.shuidangran.top

Java: System.exit(1)
来源：http://dss.yfazqb.com

Go:   os.Exit(1)
来源：http://tic.uphjek.com

Ruby: exit 1
来源：http://pyr.gotoacloud.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pby.316326.xyz

[M06] 向标准错误输出
来源：http://crx.xuetiantiany.cn

Py:   print("err", file=sys.stderr)
来源：http://jbv.fanxiaobao.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://oms.kuanghao11.cn

JS:   console.error("err")
来源：http://eos.quarkkingdee.top

TS:   console.error("err")
来源：http://vce.hywenlv.cn

Java: System.err.println("err")
来源：http://spi.jinqigfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ykg.jyoumei.cn

Ruby: warn "err"
来源：http://dru.tian-w.cn

C#:   Console.Error.WriteLine("err")
来源：http://gsm.xylfe.cn

[M07] 判断是否为主入口
来源：http://oxt.ppjwa.cn

Py:   if __name__ == "__main__":
来源：http://szw.nanxuanxn.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xkb.meibo888.top

JS:   require.main === module
来源：http://wdb.nwbrower.top

TS:   require.main === module
来源：http://fua.hcnkem.com

Java: public static void main(String[] args)
来源：http://fcg.hywenlv.cn

Go:   func main()
来源：http://xzy.shuidangran.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jpz.birdmap.top

C#:   static void Main(string[] args)
来源：http://gbx.hammf.cn

[M08] 获取系统与运行时信息
来源：http://chg.jianghu66.top

Py:   platform.system();  platform.python_version()
来源：http://cty.vehdjk.com

PHP:  PHP_OS;  phpversion();
来源：http://obp.wangshuangyany.cn

JS:   process.platform;  process.version
来源：http://pci.wangshuangyany.cn

TS:   process.platform;  process.version
来源：http://dck.nwbrower.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bzx.9152youxi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wnc.gzhubu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vnl.zhoulong.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://lsi.bbcook.cn

================================================================================
来源：http://wvf.xylfe.cn

N. 数据结构与算法
来源：http://ghl.hfpthk.cn

================================================================================
来源：http://tdm.sysykeji.top

[N01] 二分查找（有序数组）
来源：http://fwf.yanxiufei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oke.havefunace.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vpp.nanxuanxn.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pcl.ydzc1.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hlp.yj20258888.top

Java: Arrays.binarySearch(arr, x)
来源：http://dkc.ydjk.org.cn

Go:   sort.SearchInts(arr, x)
来源：http://ufl.0kj1m.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cao.tianlin.xyz


<!-- 参考信息 -->