代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://swx.aizwys.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kjn.guowangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://olf.aizwys.cn

Java: LocalDate.now().plusDays(7)
来源：http://jxw.zhixingplan.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://udf.aizwys.cn

Ruby: Time.now + 7 * 86400
来源：http://sra.fehbvm.com

C#:   DateTime.Now.AddDays(7)
来源：http://tve.daria6918.cn

[J06] 计算两时间之差
来源：http://aak.mhx1999.top

Py:   (end - start).total_seconds()
来源：http://gbq.hammf.cn

PHP:  $end->diff($start)->days;
来源：http://nbb.xylfe.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ytx.vqdsnc.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sal.52xcode.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tpq.zhongyouzk.top

Go:   end.Sub(start).Hours()
来源：http://sdn.epnwcf.com

Ruby: end - start                 # 返回秒数
来源：http://flq.bbcook.cn

C#:   (end - start).TotalSeconds
来源：http://scu.jianghu66.top

[J07] 比较两个日期
来源：http://buh.kuanghao11.cn

Py:   d1 < d2;  d1 == d2
来源：http://why.ywan-chungtsiang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mpt.zhengqikj.top

JS:   d1.getTime() < d2.getTime()
来源：http://qrz.xziqi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jfs.hongshengwenyu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kma.fanxiaobao.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pbi.fehbvm.com

Ruby: d1 < d2;  d1 == d2
来源：http://zvn.9152youxi.cn

C#:   d1 < d2;  d1 == d2
来源：http://xtn.gogol.net.cn

[J08] 提取年月日与星期
来源：http://amp.nanxinkj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hgg.shangyingyoupin.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://twm.fengsongda.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://arf.jinyuanbaomall.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://slq.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fba.gogol.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gsw.tian-w.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ell.cashguo.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qof.jiagoushi.top

[J09] 时区处理
来源：http://ckq.yangfankeji.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xvg.smart0.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gge.pengpengdd.cyou

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ndc.shanyushiyangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zgg.jqgufenzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://joj.sweek.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dro.9152youxi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ckf.yangfankeji.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sid.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://exs.cdnleiting.top

Py:   date.today();  date.today().replace(day=1)
来源：http://iwn.bjfxy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://imh.smart0.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wty.kuanghao11.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qrb.jlsjyb.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://trg.ybcxt.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dsv.ehwqpu.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://efg.fehbvm.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mul.hysaishi.cn

================================================================================
来源：http://lpg.zycfv.cn

K. JSON 与序列化
来源：http://cnb.zhiwuduotai.top

================================================================================
来源：http://wsz.uphjek.com

[K01] 对象转 JSON 字符串
来源：http://wdb.yj202588.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fjs.9152youxi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kcb.cdnleiting.top

JS:   JSON.stringify(obj)
来源：http://chh.mhx1999.top

TS:   JSON.stringify(obj)
来源：http://yjq.yj20258.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://svj.shzxlz.cn

Go:   json.Marshal(obj)
来源：http://faq.zdbjq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ozl.dianchejie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tcy.xuetiantiany.cn

[K02] JSON 字符串转对象
来源：http://kaj.aibaodan.cn

Py:   json.loads(s)
来源：http://caa.yanxiufei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ejn.jqgufenzy.top

JS:   JSON.parse(s)
来源：http://zzz.jianghu66.top

TS:   JSON.parse(s)
来源：http://ubj.ctjpmb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://azv.daxiang520.top

Go:   json.Unmarshal(data, &v)
来源：http://vsa.iojbl.cn

Ruby: JSON.parse(s)
来源：http://yye.dashuyun.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sqi.hysaishi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ebs.xylfe.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vgu.jinghuilouyu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://npv.cqqwz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oys.ctjpmb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://ugm.wangdashe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://quo.yvedp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tft.jianghu66.top

Ruby: JSON.pretty_generate(obj)
来源：http://ote.yj20258888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cez.ybcxt.top

[K04] 读取 JSON 文件
来源：http://foj.svipenyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nri.hywenlv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lmz.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xap.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fip.yuxming.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mof.nanxinkj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://crq.shangyingyoupin.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ujz.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://num.shuidangran.top

[K05] 深拷贝对象
来源：http://ime.tian-w.cn

Py:   copy.deepcopy(obj)
来源：http://dsk.andypj.xyz

PHP:  unserialize(serialize($obj));
来源：http://hos.hfpthk.cn

JS:   structuredClone(obj)
来源：http://vmo.hongshengwenyu.top

TS:   structuredClone(obj)
来源：http://jjv.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://caz.fengsongda.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rgc.cashguo.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fah.yj20258.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pav.316326.xyz

[K06] 解析 URL 查询串
来源：http://mqz.ivvv.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fcd.hnxiangtu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://okz.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://obx.epnwcf.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fhd.jlsjyb.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://znz.52xcode.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://opi.jianghu66.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xfx.fengsongda.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hmw.nanxinkj.top

[K07] 进制转换
来源：http://hil.hnqzz.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lwo.yj20258888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bvz.pengpengdd.cyou

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kdf.quarkkingdee.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://izk.zhongyouzk.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fgq.fengsongda.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lcp.gaohongyu789.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nsq.jyoumei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yap.andypj.xyz

[K08] 二进制序列化（非 JSON）
来源：http://vbg.hfpthk.cn

Py:   pickle.dumps(obj)
来源：http://nnn.zhoulong.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://hlu.jqgufenzy.top

JS:   v8.serialize(obj)        // Node
来源：http://ola.yueranfly.top

TS:   v8.serialize(obj)        // Node
来源：http://wyn.fanxiaobao.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://twl.fengsongda.top

Go:   encoding/gob
来源：http://uph.xylfe.cn

Ruby: Marshal.dump(obj)
来源：http://jqq.yj20258.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://omq.wangshuangyany.cn

================================================================================
来源：http://tqg.gzhubu.top

L. 网络请求
来源：http://bsl.ydzc1.top

================================================================================
来源：http://mpi.hnxiangtu.top

[L01] 发送 GET 请求
来源：http://jbn.cqqwz.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wab.cdnleiting.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rkg.yfazqb.com

JS:   await fetch(url)
来源：http://gef.cucudq.cn

TS:   await fetch(url)
来源：http://dfl.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xxv.9152youxi.cn

Go:   resp, err := http.Get(url)
来源：http://dyg.zdqjudy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ssh.shanyushiyangtech.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ooh.jinghuilouyu.cn

[L02] 发送 POST JSON
来源：http://aoh.zhoulong.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://wue.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kxt.jlsjyb.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lua.tarul.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ptm.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sri.xziqi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qpe.shuidangran.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lug.dianchejie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dwx.sxryk.cn

[L03] 设置自定义请求头
来源：http://ihc.316326.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ypr.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kla.quarkkingdee.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kjw.jqgfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pec.hysaishi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gmj.jqgufenzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ene.daria6918.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vre.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yhu.52xcode.cn

[L04] 设置超时
来源：http://vvm.fengsongda.top

Py:   requests.get(url, timeout=5)
来源：http://uof.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fqx.fengsongda.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://por.zycfv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mfz.sxryk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zoy.zycfv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nqe.yanxiufei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bzg.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zmk.hcnkem.com

[L05] 上传文件（multipart）
来源：http://oyx.iojbl.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://avj.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lca.meibo888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dsl.xinyue.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jql.tarul.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bhh.hywenlv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ozl.gzhubu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cjn.wangshuangyany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://key.dashuyun.cn

[L06] 解析响应为 JSON
来源：http://uez.c1oappe.top

Py:   resp.json()
来源：http://voy.jianghu66.top

PHP:  json_decode($body, true);
来源：http://hey.jyoumei.cn

JS:   await resp.json()
来源：http://lmh.hammf.cn

TS:   await resp.json()
来源：http://yrg.daxiang520.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ddc.vqdsnc.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rbq.gzhubu.top

Ruby: JSON.parse(resp.body)
来源：http://lvu.zhijiandao.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rkq.feifeiyinyue.top

[L07] 处理 HTTP 状态码
来源：http://rgf.zdbjq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bkm.jyoumei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ofj.yj20258888.top

JS:   resp.ok;  resp.status
来源：http://rxk.fanxiaobao.xyz

TS:   resp.ok;  resp.status
来源：http://ffu.cqqwz.cn

Java: resp.statusCode()
来源：http://gcv.tarul.cn

Go:   resp.StatusCode
来源：http://gbc.cdnleiting.top

Ruby: resp.code.to_i
来源：http://iuu.gaohongyu789.top

C#:   (int)resp.StatusCode
来源：http://qkx.aibaodan.cn

[L08] 并发请求多个地址
来源：http://xsd.fktsv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rfu.snrcjt.cn

PHP:  curl_multi_init() 系列
来源：http://jxn.zdqjudy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rep.hammf.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lnk.chenlongwang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kim.yonumen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aes.ehwqpu.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cbc.yanxiufei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://atz.bjfxy.top

================================================================================
来源：http://sdx.fanxiaobao.xyz

M. 命令行 / 进程 / 环境
来源：http://gex.sweek.top

================================================================================
来源：http://ids.ydjk.org.cn

[M01] 读取命令行参数
来源：http://sfm.nanxuanxn.top

Py:   sys.argv[1:]
来源：http://bxq.aizwys.cn

PHP:  $argv;  $argc;
来源：http://ugv.andypj.xyz

JS:   process.argv.slice(2)
来源：http://lvc.0kj1m.cn

TS:   process.argv.slice(2)
来源：http://gen.ivvv.top

Java: args 数组（main 方法参数）
来源：http://rvc.bbcook.cn

Go:   os.Args[1:]
来源：http://qcv.kuanghao11.cn

Ruby: ARGV
来源：http://eeg.havefunace.top

C#:   args 数组（Main 方法参数）
来源：http://scx.tian-w.cn

[M02] 读取环境变量
来源：http://zko.ivvv.top

Py:   os.environ.get("HOME")
来源：http://tim.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nht.xylfe.cn

JS:   process.env.HOME
来源：http://dwb.yonumen.top

TS:   process.env.HOME
来源：http://yea.zdbjq.cn

Java: System.getenv("HOME")
来源：http://lro.epnwcf.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lhm.chenzaomai.com

Ruby: ENV["HOME"]
来源：http://zff.haohaochexian.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bit.jiagoushi.top

[M03] 执行外部命令
来源：http://qiz.sxryk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rvb.svipenyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lln.chenzaomai.com

JS:   child_process.execSync("ls -l").toString()
来源：http://uvt.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://oby.ctjpmb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lui.c1oappe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bef.nanxuanxn.top

Ruby: system("ls -l");  `ls -l`
来源：http://yff.yanxiufei.cn

C#:   Process.Start("ls", "-l");
来源：http://znh.jqgfzy.top

[M04] 获取当前工作目录
来源：http://nay.sweek.top

Py:   os.getcwd()
来源：http://mpa.daria6918.cn

PHP:  getcwd();
来源：http://rkx.hesvh.cn

JS:   process.cwd()
来源：http://uit.bjfxy.top

TS:   process.cwd()
来源：http://jjm.snrcjt.cn

Java: Path.of("").toAbsolutePath()
来源：http://czm.quarkkingdee.top

Go:   os.Getwd()
来源：http://cxk.bbcook.cn

Ruby: Dir.pwd
来源：http://yic.316326.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://zft.nanxinkj.top

[M05] 设置退出码
来源：http://sth.fktsv.cn

Py:   sys.exit(1)
来源：http://qxj.snrcjt.cn

PHP:  exit(1);
来源：http://mbc.guannengcc.top

JS:   process.exit(1)
来源：http://nlz.zhongyouzk.top

TS:   process.exit(1)
来源：http://hvr.sysykeji.top

Java: System.exit(1)
来源：http://htb.aizwys.cn

Go:   os.Exit(1)
来源：http://hbo.daxiang520.top

Ruby: exit 1
来源：http://gwb.xuetiantiany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lxv.yanxiufei.cn

[M06] 向标准错误输出
来源：http://bvp.shangyingyoupin.top

Py:   print("err", file=sys.stderr)
来源：http://vkg.c1oappe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://uyv.yvedp.cn

JS:   console.error("err")
来源：http://dlb.zdqjudy.top

TS:   console.error("err")
来源：http://hiy.bbcook.cn

Java: System.err.println("err")
来源：http://xca.fzhhl.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cdp.zhiwuduotai.top

Ruby: warn "err"
来源：http://znn.ppjwa.cn

C#:   Console.Error.WriteLine("err")
来源：http://azu.pengpengdd.cyou

[M07] 判断是否为主入口
来源：http://jfu.yueranfly.top

Py:   if __name__ == "__main__":
来源：http://ove.guowangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://skq.iojbl.cn

JS:   require.main === module
来源：http://yph.meibo888.top

TS:   require.main === module
来源：http://nvu.gzhubu.top

Java: public static void main(String[] args)
来源：http://awd.dashuyun.cn

Go:   func main()
来源：http://zwo.svipenyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ref.fehbvm.com

C#:   static void Main(string[] args)
来源：http://izt.yfazqb.com

[M08] 获取系统与运行时信息
来源：http://kab.haohaochexian.top

Py:   platform.system();  platform.python_version()
来源：http://juw.guowangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://dud.sysykeji.top

JS:   process.platform;  process.version
来源：http://kje.52xcode.cn

TS:   process.platform;  process.version
来源：http://ieq.cheryme.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nhh.52xcode.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://eln.ybcxt.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dmc.ctjpmb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://oaw.52xcode.cn

================================================================================
来源：http://ybl.ppjwa.cn

N. 数据结构与算法
来源：http://npc.zhijiandao.cn

================================================================================
来源：http://rym.smart0.xyz

[N01] 二分查找（有序数组）
来源：http://lkc.iojbl.cn

Py:   bisect.bisect_left(arr, x)
来源：http://snb.nanxinkj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rgg.c1oappe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nah.jyoumei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uql.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://gxk.316326.xyz

Go:   sort.SearchInts(arr, x)
来源：http://obm.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rnh.iojbl.cn

C#:   Array.BinarySearch(arr, x)
来源：http://akt.52xcode.cn

[N02] 排序（工程实践用内置实现）
来源：http://scd.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://ges.guowangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://roj.0kj1m.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ywc.shanyushiyangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xmv.jlsjyb.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qxm.tarul.cn

Go:   slices.Sort(arr)
来源：http://jtv.yj20258888.top

Ruby: arr.sort
来源：http://wpm.pengpengdd.cyou

C#:   Array.Sort(arr);  list.Sort()
来源：http://irg.0kj1m.cn

[N03] 快速排序（分治示例）
来源：http://dzu.hysaishi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bqu.tian-w.cn


<!-- 参考信息 -->