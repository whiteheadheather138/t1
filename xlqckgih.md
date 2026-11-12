代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wvp.xziqi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dpo.redwolf501.top

[J05] 时间加减（加 7 天）
来源：http://sfm.c1oappe.top

Py:   now + timedelta(days=7)
来源：http://zbt.havefunace.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kly.yueranfly.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qsk.cashguo.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hfe.sjlbkw.cn

Java: LocalDate.now().plusDays(7)
来源：http://wtr.jyoumei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nje.havefunace.top

Ruby: Time.now + 7 * 86400
来源：http://zka.hammf.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qyy.shzxlz.cn

[J06] 计算两时间之差
来源：http://lqb.yangfankeji.com

Py:   (end - start).total_seconds()
来源：http://fdj.vqdsnc.cn

PHP:  $end->diff($start)->days;
来源：http://zwd.tianlin.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xfw.yfazqb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pqw.chenzaomai.com

Java: Duration.between(start, end).toSeconds()
来源：http://oxi.zhijiandao.cn

Go:   end.Sub(start).Hours()
来源：http://gdr.hfpthk.cn

Ruby: end - start                 # 返回秒数
来源：http://nfw.xuanzx.com

C#:   (end - start).TotalSeconds
来源：http://dhf.xinyue.icu

[J07] 比较两个日期
来源：http://xgt.dashuyun.cn

Py:   d1 < d2;  d1 == d2
来源：http://vuj.kuanghao11.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dac.jqgfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://qmr.zhiwuduotai.top

TS:   d1.getTime() < d2.getTime()
来源：http://ssk.sxryk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vlc.fehbvm.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://onf.tarul.cn

Ruby: d1 < d2;  d1 == d2
来源：http://chg.chenjidiqi.icu

C#:   d1 < d2;  d1 == d2
来源：http://xef.nwbrower.top

[J08] 提取年月日与星期
来源：http://vyy.shanyushiyangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xzd.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mtx.feifeiyinyue.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vhb.yvedp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xcn.hnxiangtu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jvh.feifeiyinyue.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kdb.xziqi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jfv.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qmi.xuetiantiany.cn

[J09] 时区处理
来源：http://rbu.svipenyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bqt.sweek.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ddu.yueranfly.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ymd.mhx1999.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iuy.jinqigfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nrs.jianghu66.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tnu.jlsjyb.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://iga.fengsongda.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ogx.feifeiyinyue.top

[J10] 取今天 / 本月第一天
来源：http://hyt.0kj1m.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ukg.yj20258.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ybh.ctjpmb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ban.bjfxy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aol.tanke756.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wfi.yangfankeji.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qvd.xinyue.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://glo.gogol.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bvn.mhx1999.top

================================================================================
来源：http://aqk.yueranfly.top

K. JSON 与序列化
来源：http://ktn.cashguo.top

================================================================================
来源：http://wgm.chenzaomai.com

[K01] 对象转 JSON 字符串
来源：http://zkw.jqgufenzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://euu.jqgfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ynm.birdmap.top

JS:   JSON.stringify(obj)
来源：http://dqy.zdbjq.cn

TS:   JSON.stringify(obj)
来源：http://ruk.dianchejie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qnl.52xcode.cn

Go:   json.Marshal(obj)
来源：http://naa.fzhhl.top

Ruby: obj.to_json                                     // require "json"
来源：http://tnv.ydzc1.top

C#:   JsonSerializer.Serialize(obj)
来源：http://pqe.guowangkeji.top

[K02] JSON 字符串转对象
来源：http://gxc.yueranfly.top

Py:   json.loads(s)
来源：http://zgs.smart0.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qga.tian-w.cn

JS:   JSON.parse(s)
来源：http://kjn.daria6918.cn

TS:   JSON.parse(s)
来源：http://inz.xziqi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nea.daria6918.cn

Go:   json.Unmarshal(data, &v)
来源：http://rtf.epnwcf.com

Ruby: JSON.parse(s)
来源：http://jul.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://szi.ctjpmb.com

[K03] JSON 美化输出（带缩进）
来源：http://qrt.ybcxt.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mvs.zhengqikj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://olr.feifeiyinyue.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lwg.uphjek.com

TS:   JSON.stringify(obj, null, 2)
来源：http://knw.xuetiantiany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hql.cheryme.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://unl.redwolf501.top

Ruby: JSON.pretty_generate(obj)
来源：http://zsz.fktsv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xql.tianlin.xyz

[K04] 读取 JSON 文件
来源：http://uqw.redwolf501.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ter.hnqzz.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jxh.ybcxt.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nzc.yuxming.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wnl.jianghu66.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qfn.yfazqb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xce.mhx1999.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://krz.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cog.gzhubu.top

[K05] 深拷贝对象
来源：http://znf.gaohongyu789.top

Py:   copy.deepcopy(obj)
来源：http://zzb.shzxlz.cn

PHP:  unserialize(serialize($obj));
来源：http://yaf.fengsongda.top

JS:   structuredClone(obj)
来源：http://hhz.tian-w.cn

TS:   structuredClone(obj)
来源：http://ttc.zdbjq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jyd.fzhhl.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wne.cdnleiting.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wxm.guannengcc.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fkf.sysykeji.top

[K06] 解析 URL 查询串
来源：http://jfa.sxryk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://efg.wangshuangyany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pes.yanxiufei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dcs.jinqigufen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://otp.feifeiyinyue.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dvj.yfazqb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://vve.daria6918.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qum.feifeiyinyue.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gpa.hcnkem.com

[K07] 进制转换
来源：http://rhy.c1oappe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bfj.quarkkingdee.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wcq.hongshengwenyu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nlu.nanxinkj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zun.cucudq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kvq.ybcxt.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://thw.sweek.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oib.hcnkem.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sol.snrcjt.cn

[K08] 二进制序列化（非 JSON）
来源：http://yyi.jiagoushi.top

Py:   pickle.dumps(obj)
来源：http://laq.xziqi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wzc.hnqzz.top

JS:   v8.serialize(obj)        // Node
来源：http://auw.yfazqb.com

TS:   v8.serialize(obj)        // Node
来源：http://sxy.fzhhl.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mff.jlsjyb.cn

Go:   encoding/gob
来源：http://hjy.yj20258888.top

Ruby: Marshal.dump(obj)
来源：http://yuj.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lln.zhixingplan.top

================================================================================
来源：http://lye.zhoulong.xyz

L. 网络请求
来源：http://ptj.shangyingyoupin.top

================================================================================
来源：http://lzh.xingfuxueyuan.xyz

[L01] 发送 GET 请求
来源：http://bxt.zdqjudy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dwf.andypj.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mbp.hywenlv.cn

JS:   await fetch(url)
来源：http://jwi.xuetiantiany.cn

TS:   await fetch(url)
来源：http://jvr.havefunace.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vme.sjlbkw.cn

Go:   resp, err := http.Get(url)
来源：http://sbk.pengpengdd.cyou

Ruby: Net::HTTP.get(URI(url))
来源：http://xdb.xylfe.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rrg.yj202588.top

[L02] 发送 POST JSON
来源：http://mwz.bjfxy.top

Py:   requests.post(url, json={"a": 1})
来源：http://tak.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jwc.nanxuanxn.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mvs.hfpthk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dsw.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yxj.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ils.tian-w.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://swt.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://goc.gotoacloud.top

[L03] 设置自定义请求头
来源：http://qgr.gaohongyu789.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xtn.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://est.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dze.quarkkingdee.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ami.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eeb.snrcjt.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yvy.mhx1999.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zsv.yfazqb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://psw.redwolf501.top

[L04] 设置超时
来源：http://cuu.wangdashe.top

Py:   requests.get(url, timeout=5)
来源：http://yoe.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sla.fehbvm.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://akd.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bts.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rqv.fanxiaobao.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yel.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zze.chenlongwang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kzt.ywan-chungtsiang.top

[L05] 上传文件（multipart）
来源：http://tgs.vqdsnc.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iyg.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eer.chenzaomai.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uqm.hammf.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://aad.tian-w.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yue.haohaochexian.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bmf.nanxuanxn.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nni.meibo888.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jka.daxiang520.top

[L06] 解析响应为 JSON
来源：http://pym.zhongyouzk.top

Py:   resp.json()
来源：http://xpn.meibo888.top

PHP:  json_decode($body, true);
来源：http://jlj.ybcxt.top

JS:   await resp.json()
来源：http://zaq.dianchejie.cn

TS:   await resp.json()
来源：http://ftt.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vus.jinghuilouyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ezu.yj20258.top

Ruby: JSON.parse(resp.body)
来源：http://jah.smart0.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://enj.gogol.net.cn

[L07] 处理 HTTP 状态码
来源：http://vac.ydjk.org.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bsb.52xcode.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mfc.fktsv.cn

JS:   resp.ok;  resp.status
来源：http://xxq.aizwys.cn

TS:   resp.ok;  resp.status
来源：http://jpg.jinghuilouyu.cn

Java: resp.statusCode()
来源：http://yyg.bjfxy.top

Go:   resp.StatusCode
来源：http://sbs.fehbvm.com

Ruby: resp.code.to_i
来源：http://vhd.316326.xyz

C#:   (int)resp.StatusCode
来源：http://rij.zhiwuduotai.top

[L08] 并发请求多个地址
来源：http://fcu.ywan-chungtsiang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ldu.quarkkingdee.top

PHP:  curl_multi_init() 系列
来源：http://wrf.mhx1999.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ffy.cdnleiting.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lmk.c1oappe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cys.tian-w.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://chf.yangfankeji.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://srr.redwolf501.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ysp.xinyue.icu

================================================================================
来源：http://zyt.havefunace.top

M. 命令行 / 进程 / 环境
来源：http://phd.jinyuanbaomall.cn

================================================================================
来源：http://aaj.yongpay.top

[M01] 读取命令行参数
来源：http://bft.shuidangran.top

Py:   sys.argv[1:]
来源：http://qmv.birdmap.top

PHP:  $argv;  $argc;
来源：http://cpr.xziqi.cn

JS:   process.argv.slice(2)
来源：http://qep.gogol.net.cn

TS:   process.argv.slice(2)
来源：http://xdb.hnqzz.top

Java: args 数组（main 方法参数）
来源：http://nvs.jyoumei.cn

Go:   os.Args[1:]
来源：http://yqm.kuanghao11.cn

Ruby: ARGV
来源：http://trw.yvedp.cn

C#:   args 数组（Main 方法参数）
来源：http://unv.xinyue.icu

[M02] 读取环境变量
来源：http://twi.hfpthk.cn

Py:   os.environ.get("HOME")
来源：http://too.hysaishi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dci.yuxming.cn

JS:   process.env.HOME
来源：http://eqe.hfpthk.cn

TS:   process.env.HOME
来源：http://ucm.cdnleiting.top

Java: System.getenv("HOME")
来源：http://udr.aizwys.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://spk.dashuyun.cn

Ruby: ENV["HOME"]
来源：http://oan.cucudq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bxo.zhijiandao.cn

[M03] 执行外部命令
来源：http://riq.xingfuxueyuan.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dwu.jlsjyb.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uzd.shzxlz.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://quv.daxiang520.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gjn.daria6918.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xbs.cheryme.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mow.hnqzz.top

Ruby: system("ls -l");  `ls -l`
来源：http://rdi.cheryme.top

C#:   Process.Start("ls", "-l");
来源：http://ygl.hcnkem.com

[M04] 获取当前工作目录
来源：http://rcf.yvedp.cn

Py:   os.getcwd()
来源：http://qda.dashuyun.cn

PHP:  getcwd();
来源：http://lrp.jyoumei.cn

JS:   process.cwd()
来源：http://bme.daria6918.cn

TS:   process.cwd()
来源：http://ejg.haohaochexian.top

Java: Path.of("").toAbsolutePath()
来源：http://qnl.nwbrower.top

Go:   os.Getwd()
来源：http://ghx.jqgufenzy.top

Ruby: Dir.pwd
来源：http://bba.yfazqb.com

C#:   Directory.GetCurrentDirectory()
来源：http://zrb.smart0.xyz

[M05] 设置退出码
来源：http://jio.svipenyu.cn

Py:   sys.exit(1)
来源：http://yvv.fanxiaobao.xyz

PHP:  exit(1);
来源：http://fmr.sufxvd.cn

JS:   process.exit(1)
来源：http://hef.sxryk.cn

TS:   process.exit(1)
来源：http://umh.cqqwz.cn

Java: System.exit(1)
来源：http://ujt.jinghuilouyu.cn

Go:   os.Exit(1)
来源：http://cgw.fehbvm.com

Ruby: exit 1
来源：http://ppa.pengpengdd.cyou

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jci.snrcjt.cn

[M06] 向标准错误输出
来源：http://sar.nanxuanxn.top

Py:   print("err", file=sys.stderr)
来源：http://bgl.snrcjt.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zcj.zhengqikj.top

JS:   console.error("err")
来源：http://vpb.sjlbkw.cn

TS:   console.error("err")
来源：http://uwv.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://tzd.zdbjq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://whh.jinghuilouyu.cn

Ruby: warn "err"
来源：http://wsr.ydjk.org.cn

C#:   Console.Error.WriteLine("err")
来源：http://kze.yfazqb.com

[M07] 判断是否为主入口
来源：http://gsf.iojbl.cn

Py:   if __name__ == "__main__":
来源：http://bfb.dashuyun.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dia.feifeiyinyue.top

JS:   require.main === module
来源：http://xxv.redwolf501.top

TS:   require.main === module
来源：http://pkv.jianghu66.top

Java: public static void main(String[] args)
来源：http://ynn.zhongyouzk.top

Go:   func main()
来源：http://lce.yongpay.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jjg.birdmap.top

C#:   static void Main(string[] args)
来源：http://aao.ydzc1.top

[M08] 获取系统与运行时信息
来源：http://mjn.shanyushiyangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://urx.gzhubu.top

PHP:  PHP_OS;  phpversion();
来源：http://egs.zdbjq.cn

JS:   process.platform;  process.version
来源：http://zcl.hywenlv.cn

TS:   process.platform;  process.version
来源：http://eci.daria6918.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rbh.andypj.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://egk.fzhhl.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://okq.sweek.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mip.xuetiantiany.cn

================================================================================
来源：http://grw.jianghu66.top

N. 数据结构与算法
来源：http://joo.nwbrower.top

================================================================================
来源：http://ijh.shanyushiyangtech.top

[N01] 二分查找（有序数组）
来源：http://hwp.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://vqc.xuetiantiany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://daz.ydjk.org.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qjk.0kj1m.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jmr.sxryk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bqi.yueranfly.top

Go:   sort.SearchInts(arr, x)
来源：http://kjq.yvedp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kgl.shanyushiyangtech.top

C#:   Array.BinarySearch(arr, x)
来源：http://nzq.sjlbkw.cn

[N02] 排序（工程实践用内置实现）
来源：http://duv.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://kvk.zhixingplan.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cng.epnwcf.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://hnp.ehwqpu.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://bhs.gotoacloud.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oxk.zdbjq.cn

Go:   slices.Sort(arr)
来源：http://dwr.epnwcf.com


<!-- 参考信息 -->