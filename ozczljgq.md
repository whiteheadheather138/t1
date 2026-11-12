代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fpe.aibaodan.cn

[J04] 时间戳与日期互转
来源：http://qno.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mii.cucudq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bqi.pengpengdd.cyou

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lfq.gzhubu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://gkc.aizwys.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://krq.xingfuxueyuan.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://szx.hcnkem.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://teq.jianghu66.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lbs.iojbl.cn

[J05] 时间加减（加 7 天）
来源：http://kxo.kuanghao11.cn

Py:   now + timedelta(days=7)
来源：http://phi.haohaochexian.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jkf.cqqwz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://svv.bbcook.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://icd.cqqwz.cn

Java: LocalDate.now().plusDays(7)
来源：http://lws.fengsongda.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vdu.havefunace.top

Ruby: Time.now + 7 * 86400
来源：http://vqn.sjlbkw.cn

C#:   DateTime.Now.AddDays(7)
来源：http://upi.hcnkem.com

[J06] 计算两时间之差
来源：http://god.wangshuangyany.cn

Py:   (end - start).total_seconds()
来源：http://shj.tian-w.cn

PHP:  $end->diff($start)->days;
来源：http://yep.zdqjudy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vnn.dashuyun.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sjv.tianlin.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://gim.tian-w.cn

Go:   end.Sub(start).Hours()
来源：http://lxk.shzxlz.cn

Ruby: end - start                 # 返回秒数
来源：http://cmw.vehdjk.com

C#:   (end - start).TotalSeconds
来源：http://xzi.shzxlz.cn

[J07] 比较两个日期
来源：http://giu.meibo888.top

Py:   d1 < d2;  d1 == d2
来源：http://rxz.yfazqb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mjx.xuetiantiany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wsa.smart0.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://gqz.wangdashe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sam.yj20258888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jzk.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://oqi.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://ysg.xuanzx.com

[J08] 提取年月日与星期
来源：http://vei.zhoulong.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eno.yueranfly.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hep.hnqzz.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jgc.nanxinkj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rzo.yj20258888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fgt.birdmap.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nkb.ivvv.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ihn.yfazqb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zzu.gotoacloud.top

[J09] 时区处理
来源：http://vnw.0kj1m.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lgm.mhx1999.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ygb.jiagoushi.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rjy.redwolf501.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pfw.pycfn.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ofq.xziqi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nef.daria6918.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jth.xuanzx.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lyn.c1oappe.top

[J10] 取今天 / 本月第一天
来源：http://dbs.aibaodan.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wzr.uphjek.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ibo.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qpy.fanxiaobao.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xab.nwbrower.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cqd.yueranfly.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://scb.hammf.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xqi.zdqjudy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jvz.daxiang520.top

================================================================================
来源：http://uvo.52xcode.cn

K. JSON 与序列化
来源：http://uaz.cashguo.top

================================================================================
来源：http://fwa.tianlin.xyz

[K01] 对象转 JSON 字符串
来源：http://uht.zhongyouzk.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xxb.zhixingplan.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ccv.hnqzz.top

JS:   JSON.stringify(obj)
来源：http://nzt.xylfe.cn

TS:   JSON.stringify(obj)
来源：http://mlv.sufxvd.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vwn.hfpthk.cn

Go:   json.Marshal(obj)
来源：http://mlx.hnxiangtu.top

Ruby: obj.to_json                                     // require "json"
来源：http://zet.yonumen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bst.ybcxt.top

[K02] JSON 字符串转对象
来源：http://bmr.snrcjt.cn

Py:   json.loads(s)
来源：http://jij.sjlbkw.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ddn.ybcxt.top

JS:   JSON.parse(s)
来源：http://mzh.xinyue.icu

TS:   JSON.parse(s)
来源：http://cud.ydjk.org.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://znc.gogol.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://sbg.uphjek.com

Ruby: JSON.parse(s)
来源：http://pgk.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nlw.ydjk.org.cn

[K03] JSON 美化输出（带缩进）
来源：http://puw.shangyingyoupin.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://enq.pycfn.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cho.shanyushiyangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nqk.xuetiantiany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kxc.jinqigfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ilc.kuanghao11.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jen.fzhhl.top

Ruby: JSON.pretty_generate(obj)
来源：http://txy.yueranfly.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pfc.hnqzz.top

[K04] 读取 JSON 文件
来源：http://rwj.shuidangran.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hsq.fengsongda.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eru.zhongyouzk.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://udf.guowangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cow.sxryk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gza.aibaodan.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pho.fanxiaobao.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://xcj.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lle.dashuyun.cn

[K05] 深拷贝对象
来源：http://awm.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://wdv.zdqjudy.top

PHP:  unserialize(serialize($obj));
来源：http://zwf.chenzaomai.com

JS:   structuredClone(obj)
来源：http://zqk.ybcxt.top

TS:   structuredClone(obj)
来源：http://zix.zdbjq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://awd.jianghu66.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zro.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ywj.cqqwz.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lwn.pycfn.com

[K06] 解析 URL 查询串
来源：http://vpl.gotoacloud.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tdv.wangshuangyany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fde.hesvh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vrj.cqqwz.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://emv.tarul.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xro.zhaomingkeji.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://adq.svipenyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ajn.guannengcc.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gbu.yonumen.top

[K07] 进制转换
来源：http://hls.quarkkingdee.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gpc.zdbjq.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uvr.zdqjudy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lwl.xingfuxueyuan.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mof.vqdsnc.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bke.tianlin.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pwo.zhengqikj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ojq.jianghu66.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mlz.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://uts.vehdjk.com

Py:   pickle.dumps(obj)
来源：http://xpk.shanyushiyangtech.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mce.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://nnd.sxryk.cn

TS:   v8.serialize(obj)        // Node
来源：http://env.dianchejie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hsm.hysaishi.cn

Go:   encoding/gob
来源：http://dbx.hywenlv.cn

Ruby: Marshal.dump(obj)
来源：http://tvf.jinqigfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://alj.wangshuangyany.cn

================================================================================
来源：http://vfq.ivvv.top

L. 网络请求
来源：http://svt.fzhhl.top

================================================================================
来源：http://jyw.tianlin.xyz

[L01] 发送 GET 请求
来源：http://zuw.xuetiantiany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nuh.gaohongyu789.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lld.wangshuangyany.cn

JS:   await fetch(url)
来源：http://xit.hysaishi.cn

TS:   await fetch(url)
来源：http://hzt.jinghuilouyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://iio.fengsongda.top

Go:   resp, err := http.Get(url)
来源：http://kaz.daxiang520.top

Ruby: Net::HTTP.get(URI(url))
来源：http://msh.daxiang520.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wki.pengpengdd.cyou

[L02] 发送 POST JSON
来源：http://qgd.zhengqikj.top

Py:   requests.post(url, json={"a": 1})
来源：http://yio.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hqg.yanxiufei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iwe.zdqjudy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://okb.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ytn.ehwqpu.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gfd.aibaodan.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tcn.quarkkingdee.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://onm.nwbrower.top

[L03] 设置自定义请求头
来源：http://paj.fanxiaobao.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tpj.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rud.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kso.chenlongwang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yst.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tuz.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://owa.fehbvm.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bgt.ybcxt.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cax.guowangkeji.top

[L04] 设置超时
来源：http://pbp.zhiwuduotai.top

Py:   requests.get(url, timeout=5)
来源：http://cnf.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pyv.sysykeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xpk.sufxvd.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hzo.jlsjyb.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lsy.shuidangran.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://czq.fzhhl.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wki.yongpay.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lsu.guannengcc.top

[L05] 上传文件（multipart）
来源：http://qxp.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rzu.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://akb.pycfn.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zcv.jinqigfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jtq.ppjwa.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yfj.quarkkingdee.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://trm.tian-w.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pxe.cheryme.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gku.jinqigufen.top

[L06] 解析响应为 JSON
来源：http://grw.hongshengwenyu.top

Py:   resp.json()
来源：http://mmu.yfazqb.com

PHP:  json_decode($body, true);
来源：http://abf.ctjpmb.com

JS:   await resp.json()
来源：http://wuf.ivvv.top

TS:   await resp.json()
来源：http://mnj.snrcjt.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://shh.hnxiangtu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xrs.yangfankeji.com

Ruby: JSON.parse(resp.body)
来源：http://ihs.chenzaomai.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xjt.aibaodan.cn

[L07] 处理 HTTP 状态码
来源：http://hly.yj202588.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ptd.shanyushiyangtech.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pdl.ywan-chungtsiang.top

JS:   resp.ok;  resp.status
来源：http://xzs.yangfankeji.com

TS:   resp.ok;  resp.status
来源：http://nep.fengsongda.top

Java: resp.statusCode()
来源：http://neh.gogol.net.cn

Go:   resp.StatusCode
来源：http://nby.jyoumei.cn

Ruby: resp.code.to_i
来源：http://miy.chenjidiqi.icu

C#:   (int)resp.StatusCode
来源：http://ytv.zycfv.cn

[L08] 并发请求多个地址
来源：http://tak.fengsongda.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xkb.tanke756.top

PHP:  curl_multi_init() 系列
来源：http://nli.cqqwz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rno.wangdashe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tlm.tian-w.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kzn.zhijiandao.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oac.ctjpmb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qfh.nwbrower.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://emj.yangfankeji.com

================================================================================
来源：http://tvb.hysaishi.cn

M. 命令行 / 进程 / 环境
来源：http://zub.feifeiyinyue.top

================================================================================
来源：http://jwi.fzhhl.top

[M01] 读取命令行参数
来源：http://ywn.ivvv.top

Py:   sys.argv[1:]
来源：http://nxg.nanxinkj.top

PHP:  $argv;  $argc;
来源：http://kwz.fzhhl.top

JS:   process.argv.slice(2)
来源：http://wlu.hesvh.cn

TS:   process.argv.slice(2)
来源：http://ahu.quarkkingdee.top

Java: args 数组（main 方法参数）
来源：http://fqf.sweek.top

Go:   os.Args[1:]
来源：http://qij.zycfv.cn

Ruby: ARGV
来源：http://nay.kuanghao11.cn

C#:   args 数组（Main 方法参数）
来源：http://ynr.vehdjk.com

[M02] 读取环境变量
来源：http://zrv.uphjek.com

Py:   os.environ.get("HOME")
来源：http://tnl.shangyingyoupin.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tyx.vehdjk.com

JS:   process.env.HOME
来源：http://kwy.pengpengdd.cyou

TS:   process.env.HOME
来源：http://cvi.zhixingplan.top

Java: System.getenv("HOME")
来源：http://wao.yj20258888.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hsp.zhongyouzk.top

Ruby: ENV["HOME"]
来源：http://ium.wangshuangyany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ufe.jyoumei.cn

[M03] 执行外部命令
来源：http://bmq.jyoumei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qht.jinqigfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://plj.nanxinkj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tbd.wangshuangyany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qfa.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://weg.gaohongyu789.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pts.nanxinkj.top

Ruby: system("ls -l");  `ls -l`
来源：http://cnu.fanxiaobao.xyz

C#:   Process.Start("ls", "-l");
来源：http://fcf.shanyushiyangkeji.top

[M04] 获取当前工作目录
来源：http://izn.gotoacloud.top

Py:   os.getcwd()
来源：http://kpr.jinqigufen.top

PHP:  getcwd();
来源：http://svx.c1oappe.top

JS:   process.cwd()
来源：http://gtx.yangfankeji.com

TS:   process.cwd()
来源：http://sje.jinqigfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://lfc.daria6918.cn

Go:   os.Getwd()
来源：http://kuv.zdqjudy.top

Ruby: Dir.pwd
来源：http://mpq.hfpthk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kxl.gzhubu.top

[M05] 设置退出码
来源：http://waz.shanyushiyangtech.top

Py:   sys.exit(1)
来源：http://oxv.shanyushiyangkeji.top

PHP:  exit(1);
来源：http://vll.hfpthk.cn

JS:   process.exit(1)
来源：http://pav.jqgfzy.top

TS:   process.exit(1)
来源：http://pef.gotoacloud.top

Java: System.exit(1)
来源：http://kcz.ivvv.top

Go:   os.Exit(1)
来源：http://ass.bbcook.cn

Ruby: exit 1
来源：http://aai.zhijiandao.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wbt.tian-w.cn

[M06] 向标准错误输出
来源：http://eht.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://dqk.daxiang520.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vim.fengsongda.top

JS:   console.error("err")
来源：http://ddq.jqgfzy.top

TS:   console.error("err")
来源：http://yrb.sxryk.cn

Java: System.err.println("err")
来源：http://bfh.zhengqikj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jod.hysaishi.cn

Ruby: warn "err"
来源：http://fbk.wangshuangyany.cn

C#:   Console.Error.WriteLine("err")
来源：http://rxh.yj202588.top

[M07] 判断是否为主入口
来源：http://iny.kuanghao11.cn

Py:   if __name__ == "__main__":
来源：http://jhr.snrcjt.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uye.hnqzz.top

JS:   require.main === module
来源：http://vex.cucudq.cn

TS:   require.main === module
来源：http://cvg.tarul.cn

Java: public static void main(String[] args)
来源：http://sla.tian-w.cn

Go:   func main()
来源：http://ltn.cashguo.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vtz.nanxinkj.top

C#:   static void Main(string[] args)
来源：http://ssi.xuanzx.com

[M08] 获取系统与运行时信息
来源：http://emq.redwolf501.top

Py:   platform.system();  platform.python_version()
来源：http://jxe.52xcode.cn

PHP:  PHP_OS;  phpversion();
来源：http://kdr.pycfn.com

JS:   process.platform;  process.version
来源：http://vwh.kuanghao11.cn

TS:   process.platform;  process.version
来源：http://hcw.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wew.fanxiaobao.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://fxz.xuanzx.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lbx.shanyushiyangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ifd.jianghu66.top

================================================================================
来源：http://mvu.jinqigufen.top

N. 数据结构与算法
来源：http://mbo.sxryk.cn

================================================================================
来源：http://lnd.aizwys.cn

[N01] 二分查找（有序数组）
来源：http://ysh.hywenlv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wfz.shzxlz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vkq.mhx1999.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rzn.hnqzz.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://doq.jinghuilouyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qpi.pycfn.com

Go:   sort.SearchInts(arr, x)
来源：http://jbx.xinyue.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://rdn.aibaodan.cn


<!-- 参考信息 -->