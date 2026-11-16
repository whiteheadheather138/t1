代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://krw.meibo888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aeq.pengpengdd.cyou

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ate.jinyuanbaomall.cn

Java: LocalDate.now().plusDays(7)
来源：http://dmh.chenjidiqi.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uas.yonumen.top

Ruby: Time.now + 7 * 86400
来源：http://gwl.jinqigufen.top

C#:   DateTime.Now.AddDays(7)
来源：http://rqc.zdqjudy.top

[J06] 计算两时间之差
来源：http://lqz.yj20258888.top

Py:   (end - start).total_seconds()
来源：http://jki.ydjk.org.cn

PHP:  $end->diff($start)->days;
来源：http://vju.fzhhl.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zea.xingfuxueyuan.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mzn.zdqjudy.top

Java: Duration.between(start, end).toSeconds()
来源：http://jig.hywenlv.cn

Go:   end.Sub(start).Hours()
来源：http://itp.jinyuanbaomall.cn

Ruby: end - start                 # 返回秒数
来源：http://krv.iojbl.cn

C#:   (end - start).TotalSeconds
来源：http://toj.cdnleiting.top

[J07] 比较两个日期
来源：http://rbb.gogol.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://wum.xinyue.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dyu.ivvv.top

JS:   d1.getTime() < d2.getTime()
来源：http://spp.aibaodan.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qaa.bbcook.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fnv.0kj1m.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pzp.c1oappe.top

Ruby: d1 < d2;  d1 == d2
来源：http://yef.uphjek.com

C#:   d1 < d2;  d1 == d2
来源：http://mqx.yj202588.top

[J08] 提取年月日与星期
来源：http://nqt.yvedp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kwo.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yfz.jyoumei.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qnm.nanxinkj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yug.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uud.316326.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cyx.cheryme.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hpe.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://abz.0kj1m.cn

[J09] 时区处理
来源：http://aqy.xziqi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fmn.jianghu66.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cgt.hesvh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oap.wangshuangyany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zlt.ydzc1.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bhy.yj20258888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qsc.pengpengdd.cyou

Ruby: Time.now.getlocal("+08:00")
来源：http://exb.ywan-chungtsiang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hmm.fzhhl.top

[J10] 取今天 / 本月第一天
来源：http://pbh.yuanzhike.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qgw.aibaodan.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hae.yongpay.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zlx.bjfxy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jfh.yueranfly.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fkz.zdqjudy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mwr.bbcook.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rdd.zhongyouzk.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iql.jinqigufen.top

================================================================================
来源：http://bmx.shanyushiyangtech.top

K. JSON 与序列化
来源：http://vpu.tian-w.cn

================================================================================
来源：http://oif.chenlongwang.top

[K01] 对象转 JSON 字符串
来源：http://fuo.sxryk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mtk.ivvv.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ppj.iojbl.cn

JS:   JSON.stringify(obj)
来源：http://xyy.316326.xyz

TS:   JSON.stringify(obj)
来源：http://orl.chenjidiqi.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vsh.redwolf501.top

Go:   json.Marshal(obj)
来源：http://qez.haohaochexian.top

Ruby: obj.to_json                                     // require "json"
来源：http://jam.jinyuanbaomall.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bej.sjlbkw.cn

[K02] JSON 字符串转对象
来源：http://sil.svipenyu.cn

Py:   json.loads(s)
来源：http://odk.hammf.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wvs.xylfe.cn

JS:   JSON.parse(s)
来源：http://bst.jlsjyb.cn

TS:   JSON.parse(s)
来源：http://eoy.ppjwa.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jow.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://ana.feifeiyinyue.top

Ruby: JSON.parse(s)
来源：http://qtf.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://udb.hfpthk.cn

[K03] JSON 美化输出（带缩进）
来源：http://qoc.tianlin.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ese.smart0.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xjz.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gmn.zhongyouzk.top

TS:   JSON.stringify(obj, null, 2)
来源：http://knq.wangshuangyany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ilw.haohaochexian.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oki.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://xwl.sxryk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hvd.cashguo.top

[K04] 读取 JSON 文件
来源：http://bma.kuanghao11.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ath.dianchejie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gfz.yanxiufei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ybx.gotoacloud.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mel.zhijiandao.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pgx.c1oappe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nla.yj20258888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jkr.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uyo.jianghu66.top

[K05] 深拷贝对象
来源：http://zts.chenjidiqi.icu

Py:   copy.deepcopy(obj)
来源：http://ima.zhijiandao.cn

PHP:  unserialize(serialize($obj));
来源：http://yzm.quarkkingdee.top

JS:   structuredClone(obj)
来源：http://ocm.jinqigufen.top

TS:   structuredClone(obj)
来源：http://too.iojbl.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ayg.jiagoushi.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aev.andypj.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gra.xuanzx.com

C#:   // 序列化往返，或自定义 Clone
来源：http://uaq.xinyue.icu

[K06] 解析 URL 查询串
来源：http://stb.haohaochexian.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xjz.epnwcf.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lot.yangfankeji.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oys.nanxuanxn.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aox.tanke756.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wxb.zhoulong.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://ism.uphjek.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ceq.vehdjk.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uyf.pengpengdd.cyou

[K07] 进制转换
来源：http://gey.jinghuilouyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mei.sysykeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://der.hammf.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://koe.tarul.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cwg.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uyl.havefunace.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mpa.jqgufenzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://stn.sysykeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fko.aibaodan.cn

[K08] 二进制序列化（非 JSON）
来源：http://zvm.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://sze.nanxuanxn.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hyq.pengpengdd.cyou

JS:   v8.serialize(obj)        // Node
来源：http://szt.kuanghao11.cn

TS:   v8.serialize(obj)        // Node
来源：http://sen.0kj1m.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lmt.yfazqb.com

Go:   encoding/gob
来源：http://dgf.zycfv.cn

Ruby: Marshal.dump(obj)
来源：http://ilm.shzxlz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://djk.xylfe.cn

================================================================================
来源：http://swn.hcnkem.com

L. 网络请求
来源：http://ycv.52xcode.cn

================================================================================
来源：http://rvp.tanke756.top

[L01] 发送 GET 请求
来源：http://wqs.yj20258.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nlk.cdnleiting.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xcl.hongshengwenyu.top

JS:   await fetch(url)
来源：http://pkm.shangyingyoupin.top

TS:   await fetch(url)
来源：http://dng.ybcxt.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nny.mhx1999.top

Go:   resp, err := http.Get(url)
来源：http://kcp.ywan-chungtsiang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://iwh.shangyingyoupin.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mkb.shangyingyoupin.top

[L02] 发送 POST JSON
来源：http://dtt.guannengcc.top

Py:   requests.post(url, json={"a": 1})
来源：http://ven.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cuj.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hhn.zhiwuduotai.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ygu.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uce.shanyushiyangtech.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ovb.gogol.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xsy.c1oappe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ydr.bjfxy.top

[L03] 设置自定义请求头
来源：http://imu.chenjidiqi.icu

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xax.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gjp.svipenyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cso.sjlbkw.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oif.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ulo.yj20258888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jri.quarkkingdee.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fta.yj20258888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zpi.aibaodan.cn

[L04] 设置超时
来源：http://bqc.ctjpmb.com

Py:   requests.get(url, timeout=5)
来源：http://cxt.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pyf.hongshengwenyu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bvx.svipenyu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://luk.yongpay.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dpk.hesvh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fdw.shanyushiyangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wma.yfazqb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wra.chenjidiqi.icu

[L05] 上传文件（multipart）
来源：http://aev.shangyingyoupin.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xlz.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jrm.meibo888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xxf.aibaodan.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ynn.hfpthk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vdz.mhx1999.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hdi.316326.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qnc.zhixingplan.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zsc.zdbjq.cn

[L06] 解析响应为 JSON
来源：http://rqs.xylfe.cn

Py:   resp.json()
来源：http://awk.jinqigfzy.top

PHP:  json_decode($body, true);
来源：http://bss.cdnleiting.top

JS:   await resp.json()
来源：http://ehk.bbcook.cn

TS:   await resp.json()
来源：http://wae.jqgufenzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://efr.nwbrower.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pta.tianlin.xyz

Ruby: JSON.parse(resp.body)
来源：http://uyr.mhx1999.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mty.havefunace.top

[L07] 处理 HTTP 状态码
来源：http://tpj.ctjpmb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vff.jqgufenzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xao.quarkkingdee.top

JS:   resp.ok;  resp.status
来源：http://qnc.fktsv.cn

TS:   resp.ok;  resp.status
来源：http://wno.sufxvd.cn

Java: resp.statusCode()
来源：http://jbe.gotoacloud.top

Go:   resp.StatusCode
来源：http://wjb.dashuyun.cn

Ruby: resp.code.to_i
来源：http://wfa.birdmap.top

C#:   (int)resp.StatusCode
来源：http://uww.epnwcf.com

[L08] 并发请求多个地址
来源：http://hol.gogol.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zjj.jinghuilouyu.cn

PHP:  curl_multi_init() 系列
来源：http://gnq.hnxiangtu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ofc.bbcook.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xxe.0kj1m.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wfl.sufxvd.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ouv.jyoumei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yjf.guannengcc.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wnd.0kj1m.cn

================================================================================
来源：http://aiq.zhoulong.xyz

M. 命令行 / 进程 / 环境
来源：http://phg.zhengqikj.top

================================================================================
来源：http://geb.zdbjq.cn

[M01] 读取命令行参数
来源：http://ppf.yuxming.cn

Py:   sys.argv[1:]
来源：http://fhy.tian-w.cn

PHP:  $argv;  $argc;
来源：http://tng.jiagoushi.top

JS:   process.argv.slice(2)
来源：http://xrp.redwolf501.top

TS:   process.argv.slice(2)
来源：http://ebc.andypj.xyz

Java: args 数组（main 方法参数）
来源：http://yuo.kuanghao11.cn

Go:   os.Args[1:]
来源：http://bni.jlsjyb.cn

Ruby: ARGV
来源：http://xyq.jianghu66.top

C#:   args 数组（Main 方法参数）
来源：http://qja.yvedp.cn

[M02] 读取环境变量
来源：http://val.andypj.xyz

Py:   os.environ.get("HOME")
来源：http://zhk.shuidangran.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ixf.aizwys.cn

JS:   process.env.HOME
来源：http://ffu.tanke756.top

TS:   process.env.HOME
来源：http://lwd.xuanzx.com

Java: System.getenv("HOME")
来源：http://zkt.ydzc1.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pzf.haohaochexian.top

Ruby: ENV["HOME"]
来源：http://bvy.chenlongwang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jxo.chenlongwang.top

[M03] 执行外部命令
来源：http://hrv.ydzc1.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mxf.jinghuilouyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wll.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ugn.wangshuangyany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rnq.meibo888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://maa.bjfxy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lkw.kuanghao11.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ajr.mhx1999.top

C#:   Process.Start("ls", "-l");
来源：http://hax.cheryme.top

[M04] 获取当前工作目录
来源：http://gmf.fktsv.cn

Py:   os.getcwd()
来源：http://hlw.pengpengdd.cyou

PHP:  getcwd();
来源：http://bju.yj20258.top

JS:   process.cwd()
来源：http://ged.havefunace.top

TS:   process.cwd()
来源：http://lhd.mhx1999.top

Java: Path.of("").toAbsolutePath()
来源：http://uhh.zhixingplan.top

Go:   os.Getwd()
来源：http://eqj.quarkkingdee.top

Ruby: Dir.pwd
来源：http://qna.cheryme.top

C#:   Directory.GetCurrentDirectory()
来源：http://nsn.dianchejie.cn

[M05] 设置退出码
来源：http://unf.birdmap.top

Py:   sys.exit(1)
来源：http://amx.iojbl.cn

PHP:  exit(1);
来源：http://qju.nanxuanxn.top

JS:   process.exit(1)
来源：http://lzt.xingfuxueyuan.xyz

TS:   process.exit(1)
来源：http://noq.jyoumei.cn

Java: System.exit(1)
来源：http://hrj.andypj.xyz

Go:   os.Exit(1)
来源：http://qmb.guowangkeji.top

Ruby: exit 1
来源：http://avk.tianlin.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xvc.jiagoushi.top

[M06] 向标准错误输出
来源：http://and.fengsongda.top

Py:   print("err", file=sys.stderr)
来源：http://qsb.xziqi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://oym.hammf.cn

JS:   console.error("err")
来源：http://qjh.iojbl.cn

TS:   console.error("err")
来源：http://wku.daria6918.cn

Java: System.err.println("err")
来源：http://bky.sufxvd.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zxo.jqgufenzy.top

Ruby: warn "err"
来源：http://sru.sxryk.cn

C#:   Console.Error.WriteLine("err")
来源：http://ucu.zdbjq.cn

[M07] 判断是否为主入口
来源：http://dro.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://rfx.hcnkem.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bsz.jlsjyb.cn

JS:   require.main === module
来源：http://fcn.gaohongyu789.top

TS:   require.main === module
来源：http://nsf.cheryme.top

Java: public static void main(String[] args)
来源：http://tqg.shanyushiyangkeji.top

Go:   func main()
来源：http://yvo.ivvv.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ves.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://eul.jinqigufen.top

[M08] 获取系统与运行时信息
来源：http://tiy.bjfxy.top

Py:   platform.system();  platform.python_version()
来源：http://gbs.jinqigfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://nnx.sjlbkw.cn

JS:   process.platform;  process.version
来源：http://qfw.316326.xyz

TS:   process.platform;  process.version
来源：http://ihn.jinqigufen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yob.fehbvm.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://mfb.jianghu66.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nbl.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xan.jqgfzy.top

================================================================================
来源：http://cwn.guannengcc.top

N. 数据结构与算法
来源：http://zrv.zhongyouzk.top

================================================================================
来源：http://kzb.snrcjt.cn

[N01] 二分查找（有序数组）
来源：http://gta.cqqwz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://evm.zhijiandao.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fmc.tianlin.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jpe.yvedp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pfh.nanxuanxn.top

Java: Arrays.binarySearch(arr, x)
来源：http://xft.aibaodan.cn

Go:   sort.SearchInts(arr, x)
来源：http://dzt.sweek.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ehl.yvedp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wry.jqgfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://evh.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://pzw.zhoulong.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gok.kuanghao11.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vpa.kuanghao11.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://exd.andypj.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yae.redwolf501.top

Go:   slices.Sort(arr)
来源：http://meb.chenlongwang.top

Ruby: arr.sort
来源：http://upc.jyoumei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dzk.tarul.cn

[N03] 快速排序（分治示例）
来源：http://szp.zhongyouzk.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dgf.cashguo.top


<!-- 参考信息 -->