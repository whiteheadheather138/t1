代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zui.hesvh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pay.fktsv.cn

[J05] 时间加减（加 7 天）
来源：http://ume.zhongyouzk.top

Py:   now + timedelta(days=7)
来源：http://rpu.zhiwuduotai.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://yks.hongshengwenyu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://auw.yuxming.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yrv.hnqzz.top

Java: LocalDate.now().plusDays(7)
来源：http://mvg.sweek.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://egf.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://bym.zdbjq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ecr.cqqwz.cn

[J06] 计算两时间之差
来源：http://kje.hammf.cn

Py:   (end - start).total_seconds()
来源：http://pxx.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://xdk.ehwqpu.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vji.nanxinkj.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hst.snrcjt.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dnu.ywan-chungtsiang.top

Go:   end.Sub(start).Hours()
来源：http://lsn.guannengcc.top

Ruby: end - start                 # 返回秒数
来源：http://iur.andypj.xyz

C#:   (end - start).TotalSeconds
来源：http://ixm.jiagoushi.top

[J07] 比较两个日期
来源：http://uqm.havefunace.top

Py:   d1 < d2;  d1 == d2
来源：http://ajj.uphjek.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yno.shanyushiyangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://nye.xziqi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://stt.sxryk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zvy.hysaishi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gsv.zhiwuduotai.top

Ruby: d1 < d2;  d1 == d2
来源：http://lhc.shanyushiyangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://fzn.gogol.net.cn

[J08] 提取年月日与星期
来源：http://fdl.gotoacloud.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gul.ywan-chungtsiang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kop.daria6918.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mgh.zhixingplan.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zry.vehdjk.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://otz.fktsv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rmo.birdmap.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ijy.xuanzx.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kvp.ctjpmb.com

[J09] 时区处理
来源：http://elb.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ncd.snrcjt.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zwq.9152youxi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oso.uphjek.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cre.ppjwa.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gsf.xuanzx.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cgh.zhixingplan.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ikf.0kj1m.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yig.dianchejie.cn

[J10] 取今天 / 本月第一天
来源：http://mxj.fzhhl.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ryt.wangshuangyany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nwy.haohaochexian.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jbe.gzhubu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kjg.hongshengwenyu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gec.dianchejie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hui.xuetiantiany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ifs.yueranfly.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bsr.tianlin.xyz

================================================================================
来源：http://ixa.jlsjyb.cn

K. JSON 与序列化
来源：http://bek.52xcode.cn

================================================================================
来源：http://nim.smart0.xyz

[K01] 对象转 JSON 字符串
来源：http://rom.sjlbkw.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vva.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rjv.dashuyun.cn

JS:   JSON.stringify(obj)
来源：http://njz.jlsjyb.cn

TS:   JSON.stringify(obj)
来源：http://yns.yj20258.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vwb.zhongyouzk.top

Go:   json.Marshal(obj)
来源：http://wfk.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://jny.yongpay.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lfu.bjfxy.top

[K02] JSON 字符串转对象
来源：http://mki.yj20258888.top

Py:   json.loads(s)
来源：http://vam.cqqwz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gkm.pycfn.com

JS:   JSON.parse(s)
来源：http://rjv.tarul.cn

TS:   JSON.parse(s)
来源：http://qcx.yfazqb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vfs.daxiang520.top

Go:   json.Unmarshal(data, &v)
来源：http://fkz.fengsongda.top

Ruby: JSON.parse(s)
来源：http://ebv.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cxn.gogol.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://tpz.zhaomingkeji.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fbq.vehdjk.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ayu.dashuyun.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ymq.ydjk.org.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tgc.ivvv.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cqu.xuanzx.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://glq.hcnkem.com

Ruby: JSON.pretty_generate(obj)
来源：http://mkx.316326.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wds.jinghuilouyu.cn

[K04] 读取 JSON 文件
来源：http://qhe.shanyushiyangtech.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qmx.quarkkingdee.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pbh.0kj1m.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://npy.zhongyouzk.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hrf.gotoacloud.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nvp.ctjpmb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://buv.hywenlv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://omr.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qzk.316326.xyz

[K05] 深拷贝对象
来源：http://sep.cdnleiting.top

Py:   copy.deepcopy(obj)
来源：http://cai.shangyingyoupin.top

PHP:  unserialize(serialize($obj));
来源：http://jek.jqgfzy.top

JS:   structuredClone(obj)
来源：http://num.zhijiandao.cn

TS:   structuredClone(obj)
来源：http://jxl.ybcxt.top

Java: // 手写拷贝构造，或序列化往返
来源：http://oce.yuanzhike.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qbk.fktsv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ohz.gzhubu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://okw.ctjpmb.com

[K06] 解析 URL 查询串
来源：http://dei.gogol.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://buj.chenlongwang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pwt.shzxlz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kid.hcnkem.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nor.yj20258.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ywb.0kj1m.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://aaw.sweek.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kmw.haohaochexian.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vkr.daria6918.cn

[K07] 进制转换
来源：http://vrm.zycfv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xtl.guowangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jpd.chenjidiqi.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gko.chenjidiqi.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vxg.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jyl.yvedp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://psq.zhengqikj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cyo.cdnleiting.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://buu.hcnkem.com

[K08] 二进制序列化（非 JSON）
来源：http://ncj.ivvv.top

Py:   pickle.dumps(obj)
来源：http://xdf.fanxiaobao.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://gdr.zhixingplan.top

JS:   v8.serialize(obj)        // Node
来源：http://hab.snrcjt.cn

TS:   v8.serialize(obj)        // Node
来源：http://xrc.shuidangran.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lmq.yueranfly.top

Go:   encoding/gob
来源：http://zon.aibaodan.cn

Ruby: Marshal.dump(obj)
来源：http://zst.redwolf501.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vly.nwbrower.top

================================================================================
来源：http://pct.yfazqb.com

L. 网络请求
来源：http://oqu.zhijiandao.cn

================================================================================
来源：http://uis.redwolf501.top

[L01] 发送 GET 请求
来源：http://rve.yanxiufei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fif.guannengcc.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xbk.hongshengwenyu.top

JS:   await fetch(url)
来源：http://tsu.wangshuangyany.cn

TS:   await fetch(url)
来源：http://mps.jinyuanbaomall.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ngf.redwolf501.top

Go:   resp, err := http.Get(url)
来源：http://alx.yfazqb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://abq.gzhubu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bmy.havefunace.top

[L02] 发送 POST JSON
来源：http://ktk.shzxlz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nhq.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jfc.52xcode.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qzc.tanke756.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rvz.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uia.pycfn.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dsq.fanxiaobao.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fry.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kxr.pycfn.com

[L03] 设置自定义请求头
来源：http://sig.xziqi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ngo.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mzo.ivvv.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wfy.nanxuanxn.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oxs.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eoz.zdbjq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uhj.sxryk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ohd.nwbrower.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vud.shzxlz.cn

[L04] 设置超时
来源：http://sbn.cdnleiting.top

Py:   requests.get(url, timeout=5)
来源：http://nms.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://njj.kuanghao11.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sdl.cucudq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yog.guannengcc.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mmj.haohaochexian.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://csy.jqgfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qlx.nwbrower.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tmo.quarkkingdee.top

[L05] 上传文件（multipart）
来源：http://law.zhiwuduotai.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ius.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://onv.aibaodan.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wji.zhijiandao.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://syk.9152youxi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rwe.hywenlv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fyl.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iab.gaohongyu789.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nmh.ivvv.top

[L06] 解析响应为 JSON
来源：http://cji.yvedp.cn

Py:   resp.json()
来源：http://nyv.hnxiangtu.top

PHP:  json_decode($body, true);
来源：http://mls.hesvh.cn

JS:   await resp.json()
来源：http://xjj.ywan-chungtsiang.top

TS:   await resp.json()
来源：http://rws.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xlg.svipenyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://twg.tianlin.xyz

Ruby: JSON.parse(resp.body)
来源：http://zfk.jyoumei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jci.bjfxy.top

[L07] 处理 HTTP 状态码
来源：http://yww.yj202588.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nob.hysaishi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://let.andypj.xyz

JS:   resp.ok;  resp.status
来源：http://kdj.dashuyun.cn

TS:   resp.ok;  resp.status
来源：http://eaw.zdqjudy.top

Java: resp.statusCode()
来源：http://ctl.zhaomingkeji.xyz

Go:   resp.StatusCode
来源：http://zzn.chenlongwang.top

Ruby: resp.code.to_i
来源：http://rrj.chenjidiqi.icu

C#:   (int)resp.StatusCode
来源：http://xuk.jqgfzy.top

[L08] 并发请求多个地址
来源：http://nnf.cucudq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://luz.cheryme.top

PHP:  curl_multi_init() 系列
来源：http://tmk.xuanzx.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xtt.316326.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vng.haohaochexian.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dut.xuanzx.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ers.meibo888.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dzv.tarul.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jfh.jqgufenzy.top

================================================================================
来源：http://ide.pengpengdd.cyou

M. 命令行 / 进程 / 环境
来源：http://isq.chenzaomai.com

================================================================================
来源：http://xky.chenzaomai.com

[M01] 读取命令行参数
来源：http://iiq.chenzaomai.com

Py:   sys.argv[1:]
来源：http://jkk.chenzaomai.com

PHP:  $argv;  $argc;
来源：http://afm.cheryme.top

JS:   process.argv.slice(2)
来源：http://tlt.dianchejie.cn

TS:   process.argv.slice(2)
来源：http://xro.snrcjt.cn

Java: args 数组（main 方法参数）
来源：http://fqz.jiagoushi.top

Go:   os.Args[1:]
来源：http://hte.birdmap.top

Ruby: ARGV
来源：http://mun.kuanghao11.cn

C#:   args 数组（Main 方法参数）
来源：http://iko.xinyue.icu

[M02] 读取环境变量
来源：http://dks.cdnleiting.top

Py:   os.environ.get("HOME")
来源：http://jgm.gotoacloud.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lok.feifeiyinyue.top

JS:   process.env.HOME
来源：http://ure.nanxuanxn.top

TS:   process.env.HOME
来源：http://pwp.shuidangran.top

Java: System.getenv("HOME")
来源：http://lxc.cucudq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wfy.ybcxt.top

Ruby: ENV["HOME"]
来源：http://qao.yfazqb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uce.aizwys.cn

[M03] 执行外部命令
来源：http://bxi.hnxiangtu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cyt.yj20258888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nkl.52xcode.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tfm.fzhhl.top

TS:   child_process.execSync("ls -l").toString()
来源：http://edo.yanxiufei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sob.jqgufenzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cfu.nanxuanxn.top

Ruby: system("ls -l");  `ls -l`
来源：http://xvq.smart0.xyz

C#:   Process.Start("ls", "-l");
来源：http://iur.shangyingyoupin.top

[M04] 获取当前工作目录
来源：http://whh.jyoumei.cn

Py:   os.getcwd()
来源：http://jvn.jinyuanbaomall.cn

PHP:  getcwd();
来源：http://kqt.nanxinkj.top

JS:   process.cwd()
来源：http://xtd.cashguo.top

TS:   process.cwd()
来源：http://ira.yj20258888.top

Java: Path.of("").toAbsolutePath()
来源：http://vwo.9152youxi.cn

Go:   os.Getwd()
来源：http://zva.52xcode.cn

Ruby: Dir.pwd
来源：http://hrk.shanyushiyangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://kai.c1oappe.top

[M05] 设置退出码
来源：http://dyj.zhengqikj.top

Py:   sys.exit(1)
来源：http://bej.jiagoushi.top

PHP:  exit(1);
来源：http://swp.yfazqb.com

JS:   process.exit(1)
来源：http://crz.9152youxi.cn

TS:   process.exit(1)
来源：http://ush.pycfn.com

Java: System.exit(1)
来源：http://edu.fengsongda.top

Go:   os.Exit(1)
来源：http://lwj.ppjwa.cn

Ruby: exit 1
来源：http://aci.ywan-chungtsiang.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zlj.pycfn.com

[M06] 向标准错误输出
来源：http://mab.uphjek.com

Py:   print("err", file=sys.stderr)
来源：http://sny.xingfuxueyuan.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://ttp.cashguo.top

JS:   console.error("err")
来源：http://lwt.hammf.cn

TS:   console.error("err")
来源：http://kxe.hammf.cn

Java: System.err.println("err")
来源：http://opx.jinghuilouyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rvp.dianchejie.cn

Ruby: warn "err"
来源：http://qlg.yonumen.top

C#:   Console.Error.WriteLine("err")
来源：http://gko.gogol.net.cn

[M07] 判断是否为主入口
来源：http://isk.gaohongyu789.top

Py:   if __name__ == "__main__":
来源：http://all.yangfankeji.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zxg.gzhubu.top

JS:   require.main === module
来源：http://num.nanxinkj.top

TS:   require.main === module
来源：http://mvh.kuanghao11.cn

Java: public static void main(String[] args)
来源：http://pkm.jinqigufen.top

Go:   func main()
来源：http://rym.zhengqikj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kii.redwolf501.top

C#:   static void Main(string[] args)
来源：http://bcu.quarkkingdee.top

[M08] 获取系统与运行时信息
来源：http://jih.hongshengwenyu.top

Py:   platform.system();  platform.python_version()
来源：http://bze.yangfankeji.com

PHP:  PHP_OS;  phpversion();
来源：http://dni.nanxuanxn.top

JS:   process.platform;  process.version
来源：http://das.sjlbkw.cn

TS:   process.platform;  process.version
来源：http://luz.nanxinkj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xoj.birdmap.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://all.wangshuangyany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cwv.iojbl.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wfl.zhongyouzk.top

================================================================================
来源：http://ahq.yonumen.top

N. 数据结构与算法
来源：http://ump.sxryk.cn

================================================================================
来源：http://kwq.smart0.xyz

[N01] 二分查找（有序数组）
来源：http://wgb.andypj.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://ssd.sufxvd.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tfo.yuanzhike.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ibt.nwbrower.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jdt.yuanzhike.top

Java: Arrays.binarySearch(arr, x)
来源：http://whj.tanke756.top

Go:   sort.SearchInts(arr, x)
来源：http://gxb.gogol.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://onz.chenzaomai.com

C#:   Array.BinarySearch(arr, x)
来源：http://rcm.yj202588.top

[N02] 排序（工程实践用内置实现）
来源：http://xwa.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://evc.gogol.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sjg.chenlongwang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://cha.birdmap.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yvg.zhixingplan.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kfj.uphjek.com

Go:   slices.Sort(arr)
来源：http://qrw.ywan-chungtsiang.top


<!-- 参考信息 -->