代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://xxs.jinghuilouyu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cit.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mgw.cqqwz.cn

Java: LocalDate.now().plusDays(7)
来源：http://ztt.uphjek.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uap.zdqjudy.top

Ruby: Time.now + 7 * 86400
来源：http://jyo.fzhhl.top

C#:   DateTime.Now.AddDays(7)
来源：http://thv.hnqzz.top

[J06] 计算两时间之差
来源：http://rop.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://xno.smart0.xyz

PHP:  $end->diff($start)->days;
来源：http://dmc.jinqigufen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tjg.fktsv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pyv.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ivh.fehbvm.com

Go:   end.Sub(start).Hours()
来源：http://qpv.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://nom.chenlongwang.top

C#:   (end - start).TotalSeconds
来源：http://ath.sxryk.cn

[J07] 比较两个日期
来源：http://jsk.0kj1m.cn

Py:   d1 < d2;  d1 == d2
来源：http://txh.xziqi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zto.cheryme.top

JS:   d1.getTime() < d2.getTime()
来源：http://lkk.svipenyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lbz.ehwqpu.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lcq.tianlin.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rnj.nanxuanxn.top

Ruby: d1 < d2;  d1 == d2
来源：http://mgm.quarkkingdee.top

C#:   d1 < d2;  d1 == d2
来源：http://mut.yueranfly.top

[J08] 提取年月日与星期
来源：http://qjs.zhoulong.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sjf.jinqigfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vay.chenjidiqi.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ije.yangfankeji.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nit.yuanzhike.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lrt.sjlbkw.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ywt.snrcjt.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vod.jqgfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rmr.zhengqikj.top

[J09] 时区处理
来源：http://bqe.ybcxt.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ivm.zhongyouzk.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jno.52xcode.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eac.yfazqb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mbp.vehdjk.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://czf.dianchejie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://diz.cashguo.top

Ruby: Time.now.getlocal("+08:00")
来源：http://osb.jinqigfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ukk.havefunace.top

[J10] 取今天 / 本月第一天
来源：http://xtx.svipenyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zkl.zhiwuduotai.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://son.jqgfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://agj.yonumen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://apt.gogol.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://djq.ywan-chungtsiang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jut.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fje.yj202588.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jgp.ehwqpu.com

================================================================================
来源：http://rav.ivvv.top

K. JSON 与序列化
来源：http://klt.yanxiufei.cn

================================================================================
来源：http://nee.xingfuxueyuan.xyz

[K01] 对象转 JSON 字符串
来源：http://ztc.ppjwa.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mch.nanxinkj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gqq.0kj1m.cn

JS:   JSON.stringify(obj)
来源：http://kzy.quarkkingdee.top

TS:   JSON.stringify(obj)
来源：http://vzy.shuidangran.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hxk.birdmap.top

Go:   json.Marshal(obj)
来源：http://efs.xylfe.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lij.yangfankeji.com

C#:   JsonSerializer.Serialize(obj)
来源：http://gzr.quarkkingdee.top

[K02] JSON 字符串转对象
来源：http://ihi.shuidangran.top

Py:   json.loads(s)
来源：http://tkz.sxryk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://squ.bjfxy.top

JS:   JSON.parse(s)
来源：http://fqv.cdnleiting.top

TS:   JSON.parse(s)
来源：http://mhu.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vpt.yj20258.top

Go:   json.Unmarshal(data, &v)
来源：http://rye.yj20258.top

Ruby: JSON.parse(s)
来源：http://kib.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yex.hnxiangtu.top

[K03] JSON 美化输出（带缩进）
来源：http://rqr.mhx1999.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uqo.aizwys.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kkw.ywan-chungtsiang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nex.kuanghao11.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bpm.jlsjyb.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ssb.gzhubu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vwx.shzxlz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hby.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mgx.pengpengdd.cyou

[K04] 读取 JSON 文件
来源：http://php.tanke756.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hmx.hnqzz.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xvj.hesvh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ziq.sufxvd.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://enh.svipenyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rkm.cdnleiting.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qpe.bjfxy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://bhk.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tdh.zdqjudy.top

[K05] 深拷贝对象
来源：http://sqm.jiagoushi.top

Py:   copy.deepcopy(obj)
来源：http://zab.jyoumei.cn

PHP:  unserialize(serialize($obj));
来源：http://zjt.0kj1m.cn

JS:   structuredClone(obj)
来源：http://wrx.yuanzhike.top

TS:   structuredClone(obj)
来源：http://ijh.yuanzhike.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ebt.jiagoushi.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hqb.hongshengwenyu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bpg.zhengqikj.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vvp.andypj.xyz

[K06] 解析 URL 查询串
来源：http://pqm.wangshuangyany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bkt.zdbjq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dxr.zdqjudy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bxf.52xcode.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kcc.nanxuanxn.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://egn.xziqi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://edw.aibaodan.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lhr.zhixingplan.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://inw.jlsjyb.cn

[K07] 进制转换
来源：http://ogz.52xcode.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ohb.c1oappe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ecr.sweek.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ghj.tarul.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hvf.nanxuanxn.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ctx.yj20258888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://caa.dianchejie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bwe.snrcjt.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ftl.ywan-chungtsiang.top

[K08] 二进制序列化（非 JSON）
来源：http://kbf.tianlin.xyz

Py:   pickle.dumps(obj)
来源：http://qjg.zhengqikj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pzr.jyoumei.cn

JS:   v8.serialize(obj)        // Node
来源：http://tau.hnqzz.top

TS:   v8.serialize(obj)        // Node
来源：http://tnw.fktsv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vzs.shanyushiyangtech.top

Go:   encoding/gob
来源：http://ydk.fanxiaobao.xyz

Ruby: Marshal.dump(obj)
来源：http://xug.shangyingyoupin.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://boo.ppjwa.cn

================================================================================
来源：http://vli.ppjwa.cn

L. 网络请求
来源：http://ovx.hfpthk.cn

================================================================================
来源：http://iiz.sjlbkw.cn

[L01] 发送 GET 请求
来源：http://okz.jiagoushi.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://krt.yonumen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zwq.feifeiyinyue.top

JS:   await fetch(url)
来源：http://gml.tian-w.cn

TS:   await fetch(url)
来源：http://tpq.ydjk.org.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mbn.cdnleiting.top

Go:   resp, err := http.Get(url)
来源：http://csa.yuxming.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rzg.nwbrower.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vpt.pengpengdd.cyou

[L02] 发送 POST JSON
来源：http://lwf.yj202588.top

Py:   requests.post(url, json={"a": 1})
来源：http://cpt.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ufh.yongpay.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zzv.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://msy.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oax.ydjk.org.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://esl.xziqi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gee.hammf.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://upw.aizwys.cn

[L03] 设置自定义请求头
来源：http://nfn.yj20258.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qld.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://amg.yonumen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fjd.xinyue.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bfk.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jkz.pycfn.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xnm.fktsv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zyo.shanyushiyangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oxo.9152youxi.cn

[L04] 设置超时
来源：http://aqp.svipenyu.cn

Py:   requests.get(url, timeout=5)
来源：http://gpm.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mrq.sjlbkw.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qqk.nanxuanxn.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wig.cqqwz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uvr.jqgufenzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uzd.chenjidiqi.icu

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tbu.nanxuanxn.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uyx.feifeiyinyue.top

[L05] 上传文件（multipart）
来源：http://suq.vqdsnc.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ztr.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lrx.gaohongyu789.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://esj.xylfe.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uuc.shangyingyoupin.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fel.sysykeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lqy.zdqjudy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tec.svipenyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xdh.gotoacloud.top

[L06] 解析响应为 JSON
来源：http://wkd.0kj1m.cn

Py:   resp.json()
来源：http://ccm.jinyuanbaomall.cn

PHP:  json_decode($body, true);
来源：http://hxv.jqgufenzy.top

JS:   await resp.json()
来源：http://lip.snrcjt.cn

TS:   await resp.json()
来源：http://zhp.xinyue.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://snq.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rjh.cdnleiting.top

Ruby: JSON.parse(resp.body)
来源：http://zpm.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zji.vqdsnc.cn

[L07] 处理 HTTP 状态码
来源：http://whn.hnxiangtu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vms.ydzc1.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tua.snrcjt.cn

JS:   resp.ok;  resp.status
来源：http://tzr.zhiwuduotai.top

TS:   resp.ok;  resp.status
来源：http://fov.zhengqikj.top

Java: resp.statusCode()
来源：http://ols.bjfxy.top

Go:   resp.StatusCode
来源：http://fof.yj202588.top

Ruby: resp.code.to_i
来源：http://vkp.daxiang520.top

C#:   (int)resp.StatusCode
来源：http://ooo.jinyuanbaomall.cn

[L08] 并发请求多个地址
来源：http://elm.xuetiantiany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ywa.tarul.cn

PHP:  curl_multi_init() 系列
来源：http://tbw.0kj1m.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bbj.zhijiandao.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://voi.yueranfly.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ftw.yfazqb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tnh.yangfankeji.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vyz.0kj1m.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ekk.jinqigfzy.top

================================================================================
来源：http://nfr.jqgufenzy.top

M. 命令行 / 进程 / 环境
来源：http://uzi.andypj.xyz

================================================================================
来源：http://zts.bjfxy.top

[M01] 读取命令行参数
来源：http://qik.hysaishi.cn

Py:   sys.argv[1:]
来源：http://esc.ywan-chungtsiang.top

PHP:  $argv;  $argc;
来源：http://bew.nanxuanxn.top

JS:   process.argv.slice(2)
来源：http://ntz.uphjek.com

TS:   process.argv.slice(2)
来源：http://yzj.ywan-chungtsiang.top

Java: args 数组（main 方法参数）
来源：http://lml.dianchejie.cn

Go:   os.Args[1:]
来源：http://elz.tarul.cn

Ruby: ARGV
来源：http://vwn.ywan-chungtsiang.top

C#:   args 数组（Main 方法参数）
来源：http://lpl.tanke756.top

[M02] 读取环境变量
来源：http://tft.ehwqpu.com

Py:   os.environ.get("HOME")
来源：http://zzw.tanke756.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bfr.zhiwuduotai.top

JS:   process.env.HOME
来源：http://buc.fengsongda.top

TS:   process.env.HOME
来源：http://tyw.yangfankeji.com

Java: System.getenv("HOME")
来源：http://qcb.hfpthk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cic.tian-w.cn

Ruby: ENV["HOME"]
来源：http://std.jqgfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fdl.mhx1999.top

[M03] 执行外部命令
来源：http://cdi.yj20258888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zhr.ydzc1.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vtt.nanxuanxn.top

JS:   child_process.execSync("ls -l").toString()
来源：http://iav.zhoulong.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://gxl.ybcxt.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://owl.zdqjudy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bnp.sxryk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zff.jinghuilouyu.cn

C#:   Process.Start("ls", "-l");
来源：http://szg.yangfankeji.com

[M04] 获取当前工作目录
来源：http://jpg.uphjek.com

Py:   os.getcwd()
来源：http://djn.jiagoushi.top

PHP:  getcwd();
来源：http://ipf.yueranfly.top

JS:   process.cwd()
来源：http://fyu.jiagoushi.top

TS:   process.cwd()
来源：http://rtm.havefunace.top

Java: Path.of("").toAbsolutePath()
来源：http://fnv.snrcjt.cn

Go:   os.Getwd()
来源：http://meg.jyoumei.cn

Ruby: Dir.pwd
来源：http://jqc.aibaodan.cn

C#:   Directory.GetCurrentDirectory()
来源：http://juy.svipenyu.cn

[M05] 设置退出码
来源：http://adm.pengpengdd.cyou

Py:   sys.exit(1)
来源：http://lzu.jinyuanbaomall.cn

PHP:  exit(1);
来源：http://syz.tianlin.xyz

JS:   process.exit(1)
来源：http://rrp.sysykeji.top

TS:   process.exit(1)
来源：http://ifw.bbcook.cn

Java: System.exit(1)
来源：http://gzn.fengsongda.top

Go:   os.Exit(1)
来源：http://qxf.yueranfly.top

Ruby: exit 1
来源：http://ghn.cucudq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sxc.havefunace.top

[M06] 向标准错误输出
来源：http://gus.redwolf501.top

Py:   print("err", file=sys.stderr)
来源：http://asw.guowangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://nox.shanyushiyangkeji.top

JS:   console.error("err")
来源：http://kfx.hammf.cn

TS:   console.error("err")
来源：http://rih.shangyingyoupin.top

Java: System.err.println("err")
来源：http://hry.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zdu.hnxiangtu.top

Ruby: warn "err"
来源：http://amp.meibo888.top

C#:   Console.Error.WriteLine("err")
来源：http://cgr.hesvh.cn

[M07] 判断是否为主入口
来源：http://mrg.svipenyu.cn

Py:   if __name__ == "__main__":
来源：http://gwm.andypj.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kes.yuanzhike.top

JS:   require.main === module
来源：http://cwh.c1oappe.top

TS:   require.main === module
来源：http://hcl.hywenlv.cn

Java: public static void main(String[] args)
来源：http://cwq.redwolf501.top

Go:   func main()
来源：http://pjg.jqgfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ylw.jyoumei.cn

C#:   static void Main(string[] args)
来源：http://jcq.316326.xyz

[M08] 获取系统与运行时信息
来源：http://zmt.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://wbm.tianlin.xyz

PHP:  PHP_OS;  phpversion();
来源：http://tlu.zhixingplan.top

JS:   process.platform;  process.version
来源：http://faz.yonumen.top

TS:   process.platform;  process.version
来源：http://agv.hfpthk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://coj.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://yyd.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tho.quarkkingdee.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://anm.yueranfly.top

================================================================================
来源：http://qra.mhx1999.top

N. 数据结构与算法
来源：http://gxe.zycfv.cn

================================================================================
来源：http://hmq.jyoumei.cn

[N01] 二分查找（有序数组）
来源：http://cxg.xylfe.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vtd.sjlbkw.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wuz.sysykeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ubp.shangyingyoupin.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pql.cucudq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fxs.birdmap.top

Go:   sort.SearchInts(arr, x)
来源：http://dyw.tian-w.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yki.jiagoushi.top

C#:   Array.BinarySearch(arr, x)
来源：http://vbj.tian-w.cn

[N02] 排序（工程实践用内置实现）
来源：http://sxe.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://wwk.zhiwuduotai.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tta.kuanghao11.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://srq.aibaodan.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fck.ctjpmb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hwb.xziqi.cn

Go:   slices.Sort(arr)
来源：http://zbn.ydjk.org.cn

Ruby: arr.sort
来源：http://pvw.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://biu.dashuyun.cn

[N03] 快速排序（分治示例）
来源：http://qos.tanke756.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vmk.hongshengwenyu.top


<!-- 参考信息 -->