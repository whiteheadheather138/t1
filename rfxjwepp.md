代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vgk.cucudq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://muh.jiagoushi.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://twa.yuxming.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dum.yvedp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mhw.aizwys.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kov.jinyuanbaomall.cn

[J05] 时间加减（加 7 天）
来源：http://dgh.cqqwz.cn

Py:   now + timedelta(days=7)
来源：http://izp.zhongyouzk.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://csg.zhijiandao.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://myi.pengpengdd.cyou

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nih.jianghu66.top

Java: LocalDate.now().plusDays(7)
来源：http://lxh.kuanghao11.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vox.havefunace.top

Ruby: Time.now + 7 * 86400
来源：http://xfb.fanxiaobao.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://lbx.nanxuanxn.top

[J06] 计算两时间之差
来源：http://mfd.zhijiandao.cn

Py:   (end - start).total_seconds()
来源：http://rzf.dianchejie.cn

PHP:  $end->diff($start)->days;
来源：http://jjv.yj202588.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vtu.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nox.epnwcf.com

Java: Duration.between(start, end).toSeconds()
来源：http://qgg.xinyue.icu

Go:   end.Sub(start).Hours()
来源：http://jbl.jlsjyb.cn

Ruby: end - start                 # 返回秒数
来源：http://gup.sweek.top

C#:   (end - start).TotalSeconds
来源：http://fsf.xuanzx.com

[J07] 比较两个日期
来源：http://xpk.ehwqpu.com

Py:   d1 < d2;  d1 == d2
来源：http://eab.jqgufenzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ssa.jiagoushi.top

JS:   d1.getTime() < d2.getTime()
来源：http://uoo.daxiang520.top

TS:   d1.getTime() < d2.getTime()
来源：http://ncb.fzhhl.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pfy.wangshuangyany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ufj.gzhubu.top

Ruby: d1 < d2;  d1 == d2
来源：http://low.fanxiaobao.xyz

C#:   d1 < d2;  d1 == d2
来源：http://adp.redwolf501.top

[J08] 提取年月日与星期
来源：http://bcm.c1oappe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mhn.tian-w.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wam.zhixingplan.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://war.nwbrower.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eur.ydzc1.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xuj.jinyuanbaomall.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rxh.vehdjk.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zmr.yonumen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lrv.quarkkingdee.top

[J09] 时区处理
来源：http://obt.zdbjq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://voq.fengsongda.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://efs.jqgfzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lfm.tanke756.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ppo.zhongyouzk.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pdm.guannengcc.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iqb.pycfn.com

Ruby: Time.now.getlocal("+08:00")
来源：http://guw.quarkkingdee.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://awq.shzxlz.cn

[J10] 取今天 / 本月第一天
来源：http://mdo.yfazqb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://fqe.zhoulong.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mko.ppjwa.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jof.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://noa.wangdashe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jle.yongpay.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rwt.xuanzx.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tdp.yj202588.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nnc.iojbl.cn

================================================================================
来源：http://ntk.bjfxy.top

K. JSON 与序列化
来源：http://tgp.nanxuanxn.top

================================================================================
来源：http://trn.jinghuilouyu.cn

[K01] 对象转 JSON 字符串
来源：http://ypw.sysykeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tvk.nwbrower.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dig.jinqigfzy.top

JS:   JSON.stringify(obj)
来源：http://yfs.ppjwa.cn

TS:   JSON.stringify(obj)
来源：http://wal.smart0.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mtp.tian-w.cn

Go:   json.Marshal(obj)
来源：http://uze.yuxming.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zys.gogol.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://iud.jinqigufen.top

[K02] JSON 字符串转对象
来源：http://tdv.uphjek.com

Py:   json.loads(s)
来源：http://snu.yongpay.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mvj.gogol.net.cn

JS:   JSON.parse(s)
来源：http://qfv.hnxiangtu.top

TS:   JSON.parse(s)
来源：http://kju.ppjwa.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://izj.havefunace.top

Go:   json.Unmarshal(data, &v)
来源：http://mzd.shanyushiyangtech.top

Ruby: JSON.parse(s)
来源：http://xfu.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qty.snrcjt.cn

[K03] JSON 美化输出（带缩进）
来源：http://gbu.ehwqpu.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ouo.pengpengdd.cyou

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bay.birdmap.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lka.yueranfly.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vqg.hongshengwenyu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ufc.yfazqb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fhu.uphjek.com

Ruby: JSON.pretty_generate(obj)
来源：http://lmr.gzhubu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://the.yj20258.top

[K04] 读取 JSON 文件
来源：http://ajp.meibo888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eqi.0kj1m.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wrv.zhijiandao.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xjy.hywenlv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zds.feifeiyinyue.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tud.shzxlz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cfl.yueranfly.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://moq.tanke756.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jqx.yongpay.top

[K05] 深拷贝对象
来源：http://fqz.fehbvm.com

Py:   copy.deepcopy(obj)
来源：http://ieh.zhongyouzk.top

PHP:  unserialize(serialize($obj));
来源：http://xgo.sufxvd.cn

JS:   structuredClone(obj)
来源：http://oda.gzhubu.top

TS:   structuredClone(obj)
来源：http://iog.52xcode.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qyl.hnxiangtu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bom.tian-w.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sfp.birdmap.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cxy.316326.xyz

[K06] 解析 URL 查询串
来源：http://dbu.yongpay.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ank.bbcook.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dkd.shanyushiyangtech.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://srk.redwolf501.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mnj.ydzc1.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xsf.zdqjudy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://aso.zdqjudy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tbo.xingfuxueyuan.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://aye.xingfuxueyuan.xyz

[K07] 进制转换
来源：http://vgg.316326.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ldk.yuanzhike.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zli.0kj1m.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cvl.zhaomingkeji.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kcc.fanxiaobao.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rms.jinghuilouyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ptf.dashuyun.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wah.yuxming.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tdt.0kj1m.cn

[K08] 二进制序列化（非 JSON）
来源：http://eru.birdmap.top

Py:   pickle.dumps(obj)
来源：http://vkv.jlsjyb.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fys.cheryme.top

JS:   v8.serialize(obj)        // Node
来源：http://ycn.havefunace.top

TS:   v8.serialize(obj)        // Node
来源：http://scb.cheryme.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ozz.mhx1999.top

Go:   encoding/gob
来源：http://llt.dianchejie.cn

Ruby: Marshal.dump(obj)
来源：http://gue.nanxinkj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xay.zhengqikj.top

================================================================================
来源：http://zhh.nwbrower.top

L. 网络请求
来源：http://etl.xingfuxueyuan.xyz

================================================================================
来源：http://ikl.meibo888.top

[L01] 发送 GET 请求
来源：http://exa.hnqzz.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wne.jinghuilouyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vfy.yongpay.top

JS:   await fetch(url)
来源：http://qcu.yj20258888.top

TS:   await fetch(url)
来源：http://lhi.cqqwz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://brk.bjfxy.top

Go:   resp, err := http.Get(url)
来源：http://dxe.sjlbkw.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://iyq.xingfuxueyuan.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ltz.hesvh.cn

[L02] 发送 POST JSON
来源：http://cuz.yanxiufei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vcy.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yfp.316326.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kdm.aizwys.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yin.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://six.shangyingyoupin.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ywx.c1oappe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wyp.yueranfly.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://car.ydzc1.top

[L03] 设置自定义请求头
来源：http://tyq.xuetiantiany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qip.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qpm.redwolf501.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wox.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ncz.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hlg.316326.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jxc.shanyushiyangtech.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qri.hywenlv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bqd.yangfankeji.com

[L04] 设置超时
来源：http://cjp.ivvv.top

Py:   requests.get(url, timeout=5)
来源：http://vmv.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tvk.quarkkingdee.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://swe.zhoulong.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://laf.sxryk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jba.jlsjyb.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aqm.zhengqikj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cbp.cdnleiting.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rti.daxiang520.top

[L05] 上传文件（multipart）
来源：http://ctm.zhaomingkeji.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wvw.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ruv.gaohongyu789.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fmh.hnxiangtu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zpq.yangfankeji.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rco.jiagoushi.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://scp.xylfe.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ybe.shzxlz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wso.hywenlv.cn

[L06] 解析响应为 JSON
来源：http://huf.aizwys.cn

Py:   resp.json()
来源：http://ihp.shangyingyoupin.top

PHP:  json_decode($body, true);
来源：http://vag.fktsv.cn

JS:   await resp.json()
来源：http://hwg.316326.xyz

TS:   await resp.json()
来源：http://imb.quarkkingdee.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pcj.bjfxy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ipp.yj20258.top

Ruby: JSON.parse(resp.body)
来源：http://bla.tarul.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cqq.gogol.net.cn

[L07] 处理 HTTP 状态码
来源：http://cuf.jiagoushi.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fql.bjfxy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zlw.xziqi.cn

JS:   resp.ok;  resp.status
来源：http://fko.havefunace.top

TS:   resp.ok;  resp.status
来源：http://luk.ppjwa.cn

Java: resp.statusCode()
来源：http://qeg.hywenlv.cn

Go:   resp.StatusCode
来源：http://vsf.aizwys.cn

Ruby: resp.code.to_i
来源：http://ldw.hywenlv.cn

C#:   (int)resp.StatusCode
来源：http://dgb.yj202588.top

[L08] 并发请求多个地址
来源：http://ztc.zhoulong.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yga.redwolf501.top

PHP:  curl_multi_init() 系列
来源：http://ymr.jqgfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://att.daria6918.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yig.yj20258888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sbr.0kj1m.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sqq.xingfuxueyuan.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xdt.dashuyun.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zsr.jiagoushi.top

================================================================================
来源：http://kiy.iojbl.cn

M. 命令行 / 进程 / 环境
来源：http://nmt.jqgfzy.top

================================================================================
来源：http://qlr.haohaochexian.top

[M01] 读取命令行参数
来源：http://ryw.ppjwa.cn

Py:   sys.argv[1:]
来源：http://khv.hesvh.cn

PHP:  $argv;  $argc;
来源：http://mtm.kuanghao11.cn

JS:   process.argv.slice(2)
来源：http://mry.vqdsnc.cn

TS:   process.argv.slice(2)
来源：http://qyu.wangdashe.top

Java: args 数组（main 方法参数）
来源：http://ihg.dianchejie.cn

Go:   os.Args[1:]
来源：http://tjf.birdmap.top

Ruby: ARGV
来源：http://trz.zdqjudy.top

C#:   args 数组（Main 方法参数）
来源：http://mat.havefunace.top

[M02] 读取环境变量
来源：http://bwd.shangyingyoupin.top

Py:   os.environ.get("HOME")
来源：http://ete.smart0.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pgs.yonumen.top

JS:   process.env.HOME
来源：http://zmd.hcnkem.com

TS:   process.env.HOME
来源：http://sac.xuetiantiany.cn

Java: System.getenv("HOME")
来源：http://zys.haohaochexian.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jhg.zhongyouzk.top

Ruby: ENV["HOME"]
来源：http://opr.meibo888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cmb.cheryme.top

[M03] 执行外部命令
来源：http://xic.c1oappe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xpl.hammf.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fpl.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kfg.yongpay.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nao.yonumen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rxn.cashguo.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cnf.zdqjudy.top

Ruby: system("ls -l");  `ls -l`
来源：http://axu.chenlongwang.top

C#:   Process.Start("ls", "-l");
来源：http://nit.yonumen.top

[M04] 获取当前工作目录
来源：http://vzd.ywan-chungtsiang.top

Py:   os.getcwd()
来源：http://kao.svipenyu.cn

PHP:  getcwd();
来源：http://dya.ehwqpu.com

JS:   process.cwd()
来源：http://pye.zycfv.cn

TS:   process.cwd()
来源：http://raj.yuxming.cn

Java: Path.of("").toAbsolutePath()
来源：http://paq.wangdashe.top

Go:   os.Getwd()
来源：http://utc.zhiwuduotai.top

Ruby: Dir.pwd
来源：http://kuy.gogol.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bwt.yangfankeji.com

[M05] 设置退出码
来源：http://evg.jianghu66.top

Py:   sys.exit(1)
来源：http://mri.yanxiufei.cn

PHP:  exit(1);
来源：http://vtv.gogol.net.cn

JS:   process.exit(1)
来源：http://hjy.sweek.top

TS:   process.exit(1)
来源：http://msx.cqqwz.cn

Java: System.exit(1)
来源：http://mcp.316326.xyz

Go:   os.Exit(1)
来源：http://jgk.sjlbkw.cn

Ruby: exit 1
来源：http://wob.c1oappe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://twb.sjlbkw.cn

[M06] 向标准错误输出
来源：http://jrr.cdnleiting.top

Py:   print("err", file=sys.stderr)
来源：http://gwb.cheryme.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mcd.yj20258888.top

JS:   console.error("err")
来源：http://xvy.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://iqn.redwolf501.top

Java: System.err.println("err")
来源：http://ncz.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://erl.bbcook.cn

Ruby: warn "err"
来源：http://xiw.shzxlz.cn

C#:   Console.Error.WriteLine("err")
来源：http://lpp.haohaochexian.top

[M07] 判断是否为主入口
来源：http://dgp.ehwqpu.com

Py:   if __name__ == "__main__":
来源：http://dzv.sweek.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oyy.aizwys.cn

JS:   require.main === module
来源：http://vxn.zhengqikj.top

TS:   require.main === module
来源：http://rgn.epnwcf.com

Java: public static void main(String[] args)
来源：http://oqs.yueranfly.top

Go:   func main()
来源：http://sxg.jinqigfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://srj.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://kpt.zhaomingkeji.xyz

[M08] 获取系统与运行时信息
来源：http://ytk.ppjwa.cn

Py:   platform.system();  platform.python_version()
来源：http://fdo.hesvh.cn

PHP:  PHP_OS;  phpversion();
来源：http://dnk.wangshuangyany.cn

JS:   process.platform;  process.version
来源：http://nvl.ydjk.org.cn

TS:   process.platform;  process.version
来源：http://rrr.havefunace.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nnn.wangdashe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dbn.xuetiantiany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://drm.nanxinkj.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://iyu.sweek.top

================================================================================
来源：http://fae.haohaochexian.top

N. 数据结构与算法
来源：http://ujs.shangyingyoupin.top

================================================================================
来源：http://ynl.dianchejie.cn

[N01] 二分查找（有序数组）
来源：http://yia.tian-w.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rsw.pycfn.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://olc.9152youxi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nur.hammf.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lrv.dianchejie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oay.yfazqb.com

Go:   sort.SearchInts(arr, x)
来源：http://qra.hywenlv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xby.birdmap.top

C#:   Array.BinarySearch(arr, x)
来源：http://szn.hcnkem.com

[N02] 排序（工程实践用内置实现）
来源：http://qtk.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://etf.redwolf501.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tiq.yj202588.top


<!-- 参考信息 -->