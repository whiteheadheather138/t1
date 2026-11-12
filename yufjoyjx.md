代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qly.dianchejie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://snv.redwolf501.top

[J05] 时间加减（加 7 天）
来源：http://guz.cdnleiting.top

Py:   now + timedelta(days=7)
来源：http://idm.sweek.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jtp.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ckw.yfazqb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iqb.hysaishi.cn

Java: LocalDate.now().plusDays(7)
来源：http://ccb.zycfv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hdc.chenzaomai.com

Ruby: Time.now + 7 * 86400
来源：http://dpc.fktsv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vvu.0kj1m.cn

[J06] 计算两时间之差
来源：http://dqp.zhijiandao.cn

Py:   (end - start).total_seconds()
来源：http://nqs.xylfe.cn

PHP:  $end->diff($start)->days;
来源：http://hrc.daxiang520.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://exj.jiagoushi.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hrz.jinqigufen.top

Java: Duration.between(start, end).toSeconds()
来源：http://qiz.zhijiandao.cn

Go:   end.Sub(start).Hours()
来源：http://ivu.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://rhn.quarkkingdee.top

C#:   (end - start).TotalSeconds
来源：http://hqu.shanyushiyangtech.top

[J07] 比较两个日期
来源：http://zzg.52xcode.cn

Py:   d1 < d2;  d1 == d2
来源：http://fij.daxiang520.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ehk.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://jcc.tianlin.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://tlf.hesvh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bsh.hfpthk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hnk.cashguo.top

Ruby: d1 < d2;  d1 == d2
来源：http://rjb.guowangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://lxh.nanxuanxn.top

[J08] 提取年月日与星期
来源：http://hok.zhijiandao.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dtl.guannengcc.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tsa.cashguo.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://aoh.bjfxy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kfa.bbcook.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://srr.yj20258888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hzp.ctjpmb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qmb.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fkd.tianlin.xyz

[J09] 时区处理
来源：http://wdm.jinqigufen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nrz.sysykeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rlw.xuanzx.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xnq.gogol.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hdq.haohaochexian.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kyl.jqgfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://puz.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fgw.fanxiaobao.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gpu.ydjk.org.cn

[J10] 取今天 / 本月第一天
来源：http://but.hnqzz.top

Py:   date.today();  date.today().replace(day=1)
来源：http://biv.xuanzx.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vsz.redwolf501.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dhn.feifeiyinyue.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ige.gzhubu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gap.vehdjk.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rcl.316326.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xse.yj20258888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pvp.zhengqikj.top

================================================================================
来源：http://ibk.nanxuanxn.top

K. JSON 与序列化
来源：http://lge.ehwqpu.com

================================================================================
来源：http://qni.mhx1999.top

[K01] 对象转 JSON 字符串
来源：http://pas.c1oappe.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kii.hfpthk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://euf.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://lpd.ybcxt.top

TS:   JSON.stringify(obj)
来源：http://vhg.hesvh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ymn.c1oappe.top

Go:   json.Marshal(obj)
来源：http://une.ybcxt.top

Ruby: obj.to_json                                     // require "json"
来源：http://zcn.sxryk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nmf.dashuyun.cn

[K02] JSON 字符串转对象
来源：http://sgr.zhijiandao.cn

Py:   json.loads(s)
来源：http://onc.hywenlv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ipi.gogol.net.cn

JS:   JSON.parse(s)
来源：http://ytz.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://olu.tarul.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://shm.wangshuangyany.cn

Go:   json.Unmarshal(data, &v)
来源：http://cvd.gaohongyu789.top

Ruby: JSON.parse(s)
来源：http://wkw.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tgc.uphjek.com

[K03] JSON 美化输出（带缩进）
来源：http://wvc.cashguo.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dgo.cheryme.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dno.xingfuxueyuan.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://jhx.pengpengdd.cyou

TS:   JSON.stringify(obj, null, 2)
来源：http://wdu.52xcode.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jmc.haohaochexian.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kmy.xuetiantiany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://arg.cashguo.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dci.jqgfzy.top

[K04] 读取 JSON 文件
来源：http://gst.yongpay.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://coo.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wil.0kj1m.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mbk.yj202588.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qps.dianchejie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fbb.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jcs.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kxg.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hzb.uphjek.com

[K05] 深拷贝对象
来源：http://tle.zhengqikj.top

Py:   copy.deepcopy(obj)
来源：http://ahz.yongpay.top

PHP:  unserialize(serialize($obj));
来源：http://gyv.fengsongda.top

JS:   structuredClone(obj)
来源：http://gda.wangshuangyany.cn

TS:   structuredClone(obj)
来源：http://rwh.uphjek.com

Java: // 手写拷贝构造，或序列化往返
来源：http://ths.zhaomingkeji.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vqd.jqgufenzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hro.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://eec.daxiang520.top

[K06] 解析 URL 查询串
来源：http://njx.dashuyun.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://evb.yvedp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qvi.fengsongda.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vqk.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zwe.nanxuanxn.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://khi.wangshuangyany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qyz.fanxiaobao.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mcd.aizwys.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jhp.jiagoushi.top

[K07] 进制转换
来源：http://yqj.yangfankeji.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lyt.ydzc1.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hul.jinghuilouyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yie.jiagoushi.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lpy.guowangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ylo.gotoacloud.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mrn.ywan-chungtsiang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fbg.ehwqpu.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mhv.ehwqpu.com

[K08] 二进制序列化（非 JSON）
来源：http://kae.hfpthk.cn

Py:   pickle.dumps(obj)
来源：http://cof.ydzc1.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sqv.guowangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://ufw.vqdsnc.cn

TS:   v8.serialize(obj)        // Node
来源：http://fpt.chenjidiqi.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iwv.tian-w.cn

Go:   encoding/gob
来源：http://bqv.pycfn.com

Ruby: Marshal.dump(obj)
来源：http://qnw.ybcxt.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://efr.sjlbkw.cn

================================================================================
来源：http://exr.zhengqikj.top

L. 网络请求
来源：http://bid.hesvh.cn

================================================================================
来源：http://xpz.9152youxi.cn

[L01] 发送 GET 请求
来源：http://mjy.uphjek.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yuk.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iny.yj20258.top

JS:   await fetch(url)
来源：http://hpu.hongshengwenyu.top

TS:   await fetch(url)
来源：http://dok.yj20258888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qrj.yanxiufei.cn

Go:   resp, err := http.Get(url)
来源：http://mjw.zhoulong.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://nal.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gvd.sweek.top

[L02] 发送 POST JSON
来源：http://cyt.tanke756.top

Py:   requests.post(url, json={"a": 1})
来源：http://aim.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kmh.pycfn.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nlw.yueranfly.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dck.316326.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bri.yuanzhike.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://isr.zdbjq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sdg.bbcook.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tpq.snrcjt.cn

[L03] 设置自定义请求头
来源：http://kbt.ywan-chungtsiang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pow.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sln.gzhubu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pnp.meibo888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hmt.jiagoushi.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ajn.nanxinkj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://arf.c1oappe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fmv.zhixingplan.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nik.wangdashe.top

[L04] 设置超时
来源：http://pux.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://svm.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kcr.shanyushiyangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qmc.jinqigufen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zjb.quarkkingdee.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://asy.jinqigufen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fxs.daria6918.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rqv.jianghu66.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hgf.zhijiandao.cn

[L05] 上传文件（multipart）
来源：http://jxq.jinghuilouyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://enw.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tpa.sxryk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://krs.hcnkem.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kyo.jinghuilouyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xak.ywan-chungtsiang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yjo.hywenlv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lln.bjfxy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ggw.zhiwuduotai.top

[L06] 解析响应为 JSON
来源：http://fqb.fengsongda.top

Py:   resp.json()
来源：http://bwn.gogol.net.cn

PHP:  json_decode($body, true);
来源：http://uik.xziqi.cn

JS:   await resp.json()
来源：http://vcj.xylfe.cn

TS:   await resp.json()
来源：http://ocq.yueranfly.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dwm.quarkkingdee.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yza.zhiwuduotai.top

Ruby: JSON.parse(resp.body)
来源：http://onw.fengsongda.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dps.hongshengwenyu.top

[L07] 处理 HTTP 状态码
来源：http://uvs.bjfxy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pul.yuanzhike.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qgw.cashguo.top

JS:   resp.ok;  resp.status
来源：http://ltb.yangfankeji.com

TS:   resp.ok;  resp.status
来源：http://pvh.bbcook.cn

Java: resp.statusCode()
来源：http://rfc.zhengqikj.top

Go:   resp.StatusCode
来源：http://sym.yuanzhike.top

Ruby: resp.code.to_i
来源：http://eud.bjfxy.top

C#:   (int)resp.StatusCode
来源：http://gow.jqgufenzy.top

[L08] 并发请求多个地址
来源：http://xfv.yueranfly.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ify.pengpengdd.cyou

PHP:  curl_multi_init() 系列
来源：http://krt.bbcook.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zgc.sufxvd.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://omb.ydjk.org.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tam.jianghu66.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ziz.dashuyun.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://btp.shangyingyoupin.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xkz.zdbjq.cn

================================================================================
来源：http://xik.zhengqikj.top

M. 命令行 / 进程 / 环境
来源：http://hnp.birdmap.top

================================================================================
来源：http://ypn.gaohongyu789.top

[M01] 读取命令行参数
来源：http://kxe.hnqzz.top

Py:   sys.argv[1:]
来源：http://wyk.fanxiaobao.xyz

PHP:  $argv;  $argc;
来源：http://iyz.wangdashe.top

JS:   process.argv.slice(2)
来源：http://fog.zycfv.cn

TS:   process.argv.slice(2)
来源：http://pnh.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://mom.jinqigfzy.top

Go:   os.Args[1:]
来源：http://tob.sweek.top

Ruby: ARGV
来源：http://ktj.kuanghao11.cn

C#:   args 数组（Main 方法参数）
来源：http://gnm.aizwys.cn

[M02] 读取环境变量
来源：http://akr.sxryk.cn

Py:   os.environ.get("HOME")
来源：http://qvf.hongshengwenyu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ics.zhixingplan.top

JS:   process.env.HOME
来源：http://ycc.dashuyun.cn

TS:   process.env.HOME
来源：http://zfe.yanxiufei.cn

Java: System.getenv("HOME")
来源：http://fgp.zycfv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vzl.zhixingplan.top

Ruby: ENV["HOME"]
来源：http://qik.smart0.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jmx.chenlongwang.top

[M03] 执行外部命令
来源：http://eat.mhx1999.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xvh.xinyue.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yfh.wangshuangyany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qwp.redwolf501.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bux.zhongyouzk.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jgs.tarul.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jqh.gaohongyu789.top

Ruby: system("ls -l");  `ls -l`
来源：http://qdd.fengsongda.top

C#:   Process.Start("ls", "-l");
来源：http://htp.xziqi.cn

[M04] 获取当前工作目录
来源：http://xhd.cdnleiting.top

Py:   os.getcwd()
来源：http://flf.cdnleiting.top

PHP:  getcwd();
来源：http://pfs.fktsv.cn

JS:   process.cwd()
来源：http://umh.vqdsnc.cn

TS:   process.cwd()
来源：http://mbk.xylfe.cn

Java: Path.of("").toAbsolutePath()
来源：http://ygj.chenlongwang.top

Go:   os.Getwd()
来源：http://vwl.kuanghao11.cn

Ruby: Dir.pwd
来源：http://nsm.sufxvd.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iio.ctjpmb.com

[M05] 设置退出码
来源：http://lhh.pycfn.com

Py:   sys.exit(1)
来源：http://jlw.hcnkem.com

PHP:  exit(1);
来源：http://tmv.yonumen.top

JS:   process.exit(1)
来源：http://xdh.hnxiangtu.top

TS:   process.exit(1)
来源：http://jep.hysaishi.cn

Java: System.exit(1)
来源：http://bck.c1oappe.top

Go:   os.Exit(1)
来源：http://ktb.hammf.cn

Ruby: exit 1
来源：http://btv.iojbl.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rlg.fzhhl.top

[M06] 向标准错误输出
来源：http://clw.316326.xyz

Py:   print("err", file=sys.stderr)
来源：http://hdp.xuetiantiany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ege.ydjk.org.cn

JS:   console.error("err")
来源：http://cty.mhx1999.top

TS:   console.error("err")
来源：http://ytv.gotoacloud.top

Java: System.err.println("err")
来源：http://aea.aizwys.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kuf.cashguo.top

Ruby: warn "err"
来源：http://jcz.yanxiufei.cn

C#:   Console.Error.WriteLine("err")
来源：http://lli.fengsongda.top

[M07] 判断是否为主入口
来源：http://tda.nanxuanxn.top

Py:   if __name__ == "__main__":
来源：http://tru.hammf.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vsn.hongshengwenyu.top

JS:   require.main === module
来源：http://plo.jianghu66.top

TS:   require.main === module
来源：http://fgf.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://hoy.ctjpmb.com

Go:   func main()
来源：http://ubi.mhx1999.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bij.cashguo.top

C#:   static void Main(string[] args)
来源：http://jyh.jianghu66.top

[M08] 获取系统与运行时信息
来源：http://uwy.quarkkingdee.top

Py:   platform.system();  platform.python_version()
来源：http://fts.ehwqpu.com

PHP:  PHP_OS;  phpversion();
来源：http://rny.yfazqb.com

JS:   process.platform;  process.version
来源：http://kpg.snrcjt.cn

TS:   process.platform;  process.version
来源：http://dry.yuanzhike.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ovg.ywan-chungtsiang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://yij.shanyushiyangtech.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://llk.ybcxt.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fao.ybcxt.top

================================================================================
来源：http://cnn.jlsjyb.cn

N. 数据结构与算法
来源：http://xjx.cashguo.top

================================================================================
来源：http://mjl.fanxiaobao.xyz

[N01] 二分查找（有序数组）
来源：http://mtk.tarul.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kdj.dianchejie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://upu.yangfankeji.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hht.hywenlv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mmj.zdbjq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jkg.yfazqb.com

Go:   sort.SearchInts(arr, x)
来源：http://nsv.nanxinkj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://bfu.fzhhl.top

C#:   Array.BinarySearch(arr, x)
来源：http://bcw.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://xfv.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://svg.xuanzx.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wlm.fktsv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hdp.yonumen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wow.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ver.daxiang520.top

Go:   slices.Sort(arr)
来源：http://jbw.yj20258888.top


<!-- 参考信息 -->