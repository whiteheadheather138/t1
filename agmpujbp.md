代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://emh.chenlongwang.top

Ruby: Time.now + 7 * 86400
来源：http://xix.chenjidiqi.icu

C#:   DateTime.Now.AddDays(7)
来源：http://txu.dashuyun.cn

[J06] 计算两时间之差
来源：http://aya.sxryk.cn

Py:   (end - start).total_seconds()
来源：http://fbf.aibaodan.cn

PHP:  $end->diff($start)->days;
来源：http://crk.cheryme.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xhq.wangdashe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yjg.hywenlv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ebg.nwbrower.top

Go:   end.Sub(start).Hours()
来源：http://gkm.pengpengdd.cyou

Ruby: end - start                 # 返回秒数
来源：http://dzw.bjfxy.top

C#:   (end - start).TotalSeconds
来源：http://abm.cashguo.top

[J07] 比较两个日期
来源：http://wok.hcnkem.com

Py:   d1 < d2;  d1 == d2
来源：http://rvj.jiagoushi.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dqy.ybcxt.top

JS:   d1.getTime() < d2.getTime()
来源：http://ikd.xuanzx.com

TS:   d1.getTime() < d2.getTime()
来源：http://jci.dashuyun.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lrl.ppjwa.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sxo.gaohongyu789.top

Ruby: d1 < d2;  d1 == d2
来源：http://zso.zdbjq.cn

C#:   d1 < d2;  d1 == d2
来源：http://qbe.tianlin.xyz

[J08] 提取年月日与星期
来源：http://aat.fzhhl.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dgm.jlsjyb.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fpi.cqqwz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kmu.yueranfly.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nfk.tianlin.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cgi.epnwcf.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://efu.gaohongyu789.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pgt.316326.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://use.shangyingyoupin.top

[J09] 时区处理
来源：http://ked.smart0.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rdv.fehbvm.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wie.jyoumei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dod.ppjwa.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cdc.hammf.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sub.zhoulong.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hta.gzhubu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rqe.sysykeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qak.shanyushiyangtech.top

[J10] 取今天 / 本月第一天
来源：http://urm.ybcxt.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jfx.nanxinkj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://juj.gotoacloud.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://clw.zdqjudy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pvk.ydzc1.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ofk.dashuyun.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://suo.ehwqpu.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jct.jianghu66.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ktt.ydzc1.top

================================================================================
来源：http://xat.guowangkeji.top

K. JSON 与序列化
来源：http://yej.jqgufenzy.top

================================================================================
来源：http://xuu.xylfe.cn

[K01] 对象转 JSON 字符串
来源：http://qgo.shzxlz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://khe.cucudq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cyo.sjlbkw.cn

JS:   JSON.stringify(obj)
来源：http://non.zycfv.cn

TS:   JSON.stringify(obj)
来源：http://ags.fehbvm.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vut.xylfe.cn

Go:   json.Marshal(obj)
来源：http://ejh.hnxiangtu.top

Ruby: obj.to_json                                     // require "json"
来源：http://hyi.ydzc1.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ene.zdbjq.cn

[K02] JSON 字符串转对象
来源：http://ngv.jinghuilouyu.cn

Py:   json.loads(s)
来源：http://ffa.zhaomingkeji.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vnl.jyoumei.cn

JS:   JSON.parse(s)
来源：http://djk.fanxiaobao.xyz

TS:   JSON.parse(s)
来源：http://wtu.pycfn.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://esw.52xcode.cn

Go:   json.Unmarshal(data, &v)
来源：http://ben.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://onm.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pue.hnqzz.top

[K03] JSON 美化输出（带缩进）
来源：http://wdr.nanxuanxn.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sxz.yonumen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bpm.cucudq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pxb.chenlongwang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lgu.yonumen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://epx.bjfxy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zdp.zdqjudy.top

Ruby: JSON.pretty_generate(obj)
来源：http://dyp.c1oappe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zja.jianghu66.top

[K04] 读取 JSON 文件
来源：http://azi.jianghu66.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gdi.hnxiangtu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xpd.daxiang520.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uaz.bjfxy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wln.snrcjt.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fsr.shzxlz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nii.redwolf501.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fmh.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vis.sjlbkw.cn

[K05] 深拷贝对象
来源：http://jpm.chenjidiqi.icu

Py:   copy.deepcopy(obj)
来源：http://raa.meibo888.top

PHP:  unserialize(serialize($obj));
来源：http://rfy.yonumen.top

JS:   structuredClone(obj)
来源：http://scs.zdqjudy.top

TS:   structuredClone(obj)
来源：http://rke.sufxvd.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dlq.dashuyun.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dwa.nwbrower.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://brz.haohaochexian.top

C#:   // 序列化往返，或自定义 Clone
来源：http://sxc.yj20258888.top

[K06] 解析 URL 查询串
来源：http://sav.jiagoushi.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cco.zhiwuduotai.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pxr.ybcxt.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gge.hcnkem.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rrn.fanxiaobao.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://llg.vehdjk.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://mby.nanxinkj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wtt.c1oappe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cob.quarkkingdee.top

[K07] 进制转换
来源：http://zph.hesvh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tgf.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nhy.nanxinkj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kpg.52xcode.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hqd.hammf.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kjz.hesvh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://skt.fzhhl.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ckk.pengpengdd.cyou

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vho.jiagoushi.top

[K08] 二进制序列化（非 JSON）
来源：http://xji.xziqi.cn

Py:   pickle.dumps(obj)
来源：http://ybi.redwolf501.top

PHP:  serialize($obj);  unserialize($s);
来源：http://osa.shangyingyoupin.top

JS:   v8.serialize(obj)        // Node
来源：http://jzz.fktsv.cn

TS:   v8.serialize(obj)        // Node
来源：http://fem.zdbjq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eqd.snrcjt.cn

Go:   encoding/gob
来源：http://jiy.yj20258888.top

Ruby: Marshal.dump(obj)
来源：http://kth.hcnkem.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cjl.yonumen.top

================================================================================
来源：http://xnp.yj20258.top

L. 网络请求
来源：http://zhc.chenjidiqi.icu

================================================================================
来源：http://qck.yangfankeji.com

[L01] 发送 GET 请求
来源：http://iwu.hammf.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kni.nanxuanxn.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hvg.hcnkem.com

JS:   await fetch(url)
来源：http://tdx.ydjk.org.cn

TS:   await fetch(url)
来源：http://alf.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tgk.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://uan.yongpay.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ges.dashuyun.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gwt.9152youxi.cn

[L02] 发送 POST JSON
来源：http://jss.jqgfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://ecq.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iqq.jinqigufen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lmz.ppjwa.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://roh.sweek.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bzd.jinyuanbaomall.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eva.xingfuxueyuan.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wah.fanxiaobao.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mdn.tian-w.cn

[L03] 设置自定义请求头
来源：http://sab.bbcook.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wwa.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tan.pengpengdd.cyou

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zyv.yvedp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cdj.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ihi.pengpengdd.cyou

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blu.svipenyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eaq.uphjek.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xjx.zycfv.cn

[L04] 设置超时
来源：http://zbq.hcnkem.com

Py:   requests.get(url, timeout=5)
来源：http://ywo.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kyt.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vdu.jianghu66.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fuw.vqdsnc.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hny.uphjek.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fmb.zhijiandao.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qmb.fzhhl.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sjc.hfpthk.cn

[L05] 上传文件（multipart）
来源：http://gig.dashuyun.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ysr.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qcd.yangfankeji.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lwv.nanxuanxn.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eum.fktsv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ufp.aizwys.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dul.zhengqikj.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bfv.jqgufenzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ilm.tarul.cn

[L06] 解析响应为 JSON
来源：http://ipr.bbcook.cn

Py:   resp.json()
来源：http://qyb.meibo888.top

PHP:  json_decode($body, true);
来源：http://tna.zhijiandao.cn

JS:   await resp.json()
来源：http://ykf.jiagoushi.top

TS:   await resp.json()
来源：http://hyu.xinyue.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tdo.svipenyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qer.ywan-chungtsiang.top

Ruby: JSON.parse(resp.body)
来源：http://sjr.tanke756.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fsk.guannengcc.top

[L07] 处理 HTTP 状态码
来源：http://und.cqqwz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ims.zhixingplan.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://csq.cashguo.top

JS:   resp.ok;  resp.status
来源：http://hca.haohaochexian.top

TS:   resp.ok;  resp.status
来源：http://gzc.zhengqikj.top

Java: resp.statusCode()
来源：http://eze.redwolf501.top

Go:   resp.StatusCode
来源：http://lpp.vqdsnc.cn

Ruby: resp.code.to_i
来源：http://pzh.yuanzhike.top

C#:   (int)resp.StatusCode
来源：http://hmm.tanke756.top

[L08] 并发请求多个地址
来源：http://gso.bjfxy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://htb.wangdashe.top

PHP:  curl_multi_init() 系列
来源：http://ffs.hnxiangtu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kcu.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vet.aizwys.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zjo.ivvv.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pnr.yvedp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hcq.zhoulong.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ihy.gaohongyu789.top

================================================================================
来源：http://exl.316326.xyz

M. 命令行 / 进程 / 环境
来源：http://vbv.yj20258.top

================================================================================
来源：http://kaa.cheryme.top

[M01] 读取命令行参数
来源：http://hrw.ppjwa.cn

Py:   sys.argv[1:]
来源：http://tkv.zhiwuduotai.top

PHP:  $argv;  $argc;
来源：http://kum.nanxuanxn.top

JS:   process.argv.slice(2)
来源：http://ots.hammf.cn

TS:   process.argv.slice(2)
来源：http://qov.shzxlz.cn

Java: args 数组（main 方法参数）
来源：http://sfr.cqqwz.cn

Go:   os.Args[1:]
来源：http://avn.ivvv.top

Ruby: ARGV
来源：http://qzr.iojbl.cn

C#:   args 数组（Main 方法参数）
来源：http://lpu.yangfankeji.com

[M02] 读取环境变量
来源：http://ssx.yfazqb.com

Py:   os.environ.get("HOME")
来源：http://wvk.wangshuangyany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pjh.yuanzhike.top

JS:   process.env.HOME
来源：http://dyp.jqgfzy.top

TS:   process.env.HOME
来源：http://kih.havefunace.top

Java: System.getenv("HOME")
来源：http://jcb.xuanzx.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://man.shanyushiyangkeji.top

Ruby: ENV["HOME"]
来源：http://yny.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zvj.zhixingplan.top

[M03] 执行外部命令
来源：http://sto.jyoumei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xxz.yj202588.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zne.jinqigfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zwh.gogol.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vtw.fehbvm.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vko.zhiwuduotai.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wkm.ydzc1.top

Ruby: system("ls -l");  `ls -l`
来源：http://bwy.havefunace.top

C#:   Process.Start("ls", "-l");
来源：http://pjz.sxryk.cn

[M04] 获取当前工作目录
来源：http://vtq.shuidangran.top

Py:   os.getcwd()
来源：http://rkb.chenjidiqi.icu

PHP:  getcwd();
来源：http://aup.jinqigufen.top

JS:   process.cwd()
来源：http://ffp.sysykeji.top

TS:   process.cwd()
来源：http://sgl.cucudq.cn

Java: Path.of("").toAbsolutePath()
来源：http://fvc.birdmap.top

Go:   os.Getwd()
来源：http://nzz.jinghuilouyu.cn

Ruby: Dir.pwd
来源：http://wus.hnxiangtu.top

C#:   Directory.GetCurrentDirectory()
来源：http://rtc.zdbjq.cn

[M05] 设置退出码
来源：http://xpb.xuanzx.com

Py:   sys.exit(1)
来源：http://nxy.zycfv.cn

PHP:  exit(1);
来源：http://oog.cqqwz.cn

JS:   process.exit(1)
来源：http://zsm.cucudq.cn

TS:   process.exit(1)
来源：http://hbk.yangfankeji.com

Java: System.exit(1)
来源：http://dft.daxiang520.top

Go:   os.Exit(1)
来源：http://wkk.jinyuanbaomall.cn

Ruby: exit 1
来源：http://nuq.kuanghao11.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jlv.gzhubu.top

[M06] 向标准错误输出
来源：http://ynk.zhaomingkeji.xyz

Py:   print("err", file=sys.stderr)
来源：http://pij.shuidangran.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bzb.nanxinkj.top

JS:   console.error("err")
来源：http://eql.shangyingyoupin.top

TS:   console.error("err")
来源：http://nsz.hfpthk.cn

Java: System.err.println("err")
来源：http://xsy.jinqigfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xdr.gzhubu.top

Ruby: warn "err"
来源：http://pmh.52xcode.cn

C#:   Console.Error.WriteLine("err")
来源：http://edc.shzxlz.cn

[M07] 判断是否为主入口
来源：http://ihy.hfpthk.cn

Py:   if __name__ == "__main__":
来源：http://gbg.fktsv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zsj.gotoacloud.top

JS:   require.main === module
来源：http://ain.xylfe.cn

TS:   require.main === module
来源：http://mdm.zhoulong.xyz

Java: public static void main(String[] args)
来源：http://tqq.pengpengdd.cyou

Go:   func main()
来源：http://buj.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ikx.yvedp.cn

C#:   static void Main(string[] args)
来源：http://mmr.birdmap.top

[M08] 获取系统与运行时信息
来源：http://wqc.bbcook.cn

Py:   platform.system();  platform.python_version()
来源：http://ydc.yj202588.top

PHP:  PHP_OS;  phpversion();
来源：http://hwx.zhixingplan.top

JS:   process.platform;  process.version
来源：http://wql.wangshuangyany.cn

TS:   process.platform;  process.version
来源：http://ktl.hywenlv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qec.hesvh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ekx.daria6918.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://afx.hammf.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cqk.jianghu66.top

================================================================================
来源：http://kgd.zycfv.cn

N. 数据结构与算法
来源：http://imt.jqgfzy.top

================================================================================
来源：http://ozu.zycfv.cn

[N01] 二分查找（有序数组）
来源：http://bmu.yuanzhike.top

Py:   bisect.bisect_left(arr, x)
来源：http://ccc.mhx1999.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tyb.smart0.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://leo.ctjpmb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tib.jqgufenzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://tig.ybcxt.top

Go:   sort.SearchInts(arr, x)
来源：http://jtw.smart0.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://mli.jqgufenzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://qtk.xuanzx.com

[N02] 排序（工程实践用内置实现）
来源：http://oul.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://kwx.yonumen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lmu.yj202588.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qtq.0kj1m.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rcw.ehwqpu.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yuw.mhx1999.top

Go:   slices.Sort(arr)
来源：http://kxr.aibaodan.cn

Ruby: arr.sort
来源：http://hbd.iojbl.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rbz.jqgufenzy.top

[N03] 快速排序（分治示例）
来源：http://xrz.svipenyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://thl.guowangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://lgt.fanxiaobao.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jpg.sjlbkw.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jno.cashguo.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qpw.chenlongwang.top


<!-- 参考信息 -->