代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://tlp.xuanzx.com

Go:   end.Sub(start).Hours()
来源：http://nfy.haohaochexian.top

Ruby: end - start                 # 返回秒数
来源：http://tpg.zycfv.cn

C#:   (end - start).TotalSeconds
来源：http://oqz.xuetiantiany.cn

[J07] 比较两个日期
来源：http://xwc.snrcjt.cn

Py:   d1 < d2;  d1 == d2
来源：http://hvv.zhaomingkeji.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pfe.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://txi.shanyushiyangtech.top

TS:   d1.getTime() < d2.getTime()
来源：http://ibe.mhx1999.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fqq.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kqo.chenlongwang.top

Ruby: d1 < d2;  d1 == d2
来源：http://aso.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://upj.vqdsnc.cn

[J08] 提取年月日与星期
来源：http://nuq.zdqjudy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://keb.andypj.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pbh.sysykeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ooh.ywan-chungtsiang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oaw.yongpay.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gfq.zdbjq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ktb.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hcq.0kj1m.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://emb.redwolf501.top

[J09] 时区处理
来源：http://elb.nwbrower.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uam.uphjek.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kvj.zhixingplan.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zxo.svipenyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iso.sysykeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ruy.jlsjyb.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qhq.yuanzhike.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wix.jqgfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://coz.jiagoushi.top

[J10] 取今天 / 本月第一天
来源：http://lcy.zycfv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nqa.gaohongyu789.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mvb.yonumen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dml.fktsv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xbw.shuidangran.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lau.tian-w.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dki.hesvh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ipt.jiagoushi.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jpy.zdbjq.cn

================================================================================
来源：http://jcu.iojbl.cn

K. JSON 与序列化
来源：http://jkh.yfazqb.com

================================================================================
来源：http://wiw.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://fzb.aibaodan.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mgr.iojbl.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mtu.hnqzz.top

JS:   JSON.stringify(obj)
来源：http://gvo.sufxvd.cn

TS:   JSON.stringify(obj)
来源：http://lwl.sysykeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xnu.yuxming.cn

Go:   json.Marshal(obj)
来源：http://ozr.zhoulong.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://osg.fehbvm.com

C#:   JsonSerializer.Serialize(obj)
来源：http://yrs.iojbl.cn

[K02] JSON 字符串转对象
来源：http://ihm.nwbrower.top

Py:   json.loads(s)
来源：http://azc.dianchejie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lvx.sjlbkw.cn

JS:   JSON.parse(s)
来源：http://akd.jinyuanbaomall.cn

TS:   JSON.parse(s)
来源：http://cvc.cqqwz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gse.aibaodan.cn

Go:   json.Unmarshal(data, &v)
来源：http://xrj.xingfuxueyuan.xyz

Ruby: JSON.parse(s)
来源：http://ihk.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hlc.svipenyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://qgw.ctjpmb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fzk.iojbl.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nyg.hesvh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wpx.daria6918.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ehe.jinqigufen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bwl.hammf.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bfq.fktsv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cuk.yj20258888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tyd.nwbrower.top

[K04] 读取 JSON 文件
来源：http://sqa.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://etl.daria6918.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pdl.yuxming.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dwk.zhixingplan.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vhb.jianghu66.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bdy.cashguo.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ojl.jlsjyb.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tzz.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kux.ehwqpu.com

[K05] 深拷贝对象
来源：http://ouh.shanyushiyangkeji.top

Py:   copy.deepcopy(obj)
来源：http://pio.redwolf501.top

PHP:  unserialize(serialize($obj));
来源：http://bow.ydjk.org.cn

JS:   structuredClone(obj)
来源：http://ojq.yanxiufei.cn

TS:   structuredClone(obj)
来源：http://yrr.jiagoushi.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mwx.guowangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fmy.yfazqb.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ite.jqgufenzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ibu.guowangkeji.top

[K06] 解析 URL 查询串
来源：http://gaz.yj202588.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nqy.hywenlv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rfl.pengpengdd.cyou

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qcb.316326.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ubr.shzxlz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zrv.fanxiaobao.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://zzm.aizwys.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bhg.chenlongwang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://urb.jyoumei.cn

[K07] 进制转换
来源：http://xef.xuetiantiany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bkt.ybcxt.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cqb.haohaochexian.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sgm.pengpengdd.cyou

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mpp.jlsjyb.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hxj.zhiwuduotai.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://aod.nwbrower.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nms.zhengqikj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wnt.meibo888.top

[K08] 二进制序列化（非 JSON）
来源：http://hlo.snrcjt.cn

Py:   pickle.dumps(obj)
来源：http://zxd.yangfankeji.com

PHP:  serialize($obj);  unserialize($s);
来源：http://mrn.xinyue.icu

JS:   v8.serialize(obj)        // Node
来源：http://ypo.jqgufenzy.top

TS:   v8.serialize(obj)        // Node
来源：http://chn.ydzc1.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pgz.zhixingplan.top

Go:   encoding/gob
来源：http://zmw.tian-w.cn

Ruby: Marshal.dump(obj)
来源：http://vpa.zycfv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fxm.fehbvm.com

================================================================================
来源：http://wfs.jyoumei.cn

L. 网络请求
来源：http://igc.tarul.cn

================================================================================
来源：http://luh.daxiang520.top

[L01] 发送 GET 请求
来源：http://ulb.dashuyun.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://huz.sweek.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dwr.snrcjt.cn

JS:   await fetch(url)
来源：http://eth.daria6918.cn

TS:   await fetch(url)
来源：http://lqu.yj202588.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ngf.xuanzx.com

Go:   resp, err := http.Get(url)
来源：http://fyi.xylfe.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wzz.yj20258888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://akq.shanyushiyangtech.top

[L02] 发送 POST JSON
来源：http://sas.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zwt.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ofx.zhiwuduotai.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ngr.zhengqikj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vaw.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qpg.zhongyouzk.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pln.hfpthk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ykz.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lqv.hfpthk.cn

[L03] 设置自定义请求头
来源：http://bwy.epnwcf.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://toa.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yqp.pycfn.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qmi.zhixingplan.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gbm.hammf.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iyl.cucudq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ifl.yonumen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vit.zdbjq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ayj.dianchejie.cn

[L04] 设置超时
来源：http://ucz.cdnleiting.top

Py:   requests.get(url, timeout=5)
来源：http://zrx.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lez.tianlin.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tfl.zhengqikj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://elk.aibaodan.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vlp.ywan-chungtsiang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vhm.nanxinkj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dai.meibo888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uhu.aizwys.cn

[L05] 上传文件（multipart）
来源：http://zob.sweek.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qyy.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uxd.jlsjyb.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dgf.ehwqpu.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qjm.yj202588.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://txf.bjfxy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://njv.cdnleiting.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jxe.zdqjudy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wrd.chenlongwang.top

[L06] 解析响应为 JSON
来源：http://vzm.xziqi.cn

Py:   resp.json()
来源：http://pup.aizwys.cn

PHP:  json_decode($body, true);
来源：http://php.ehwqpu.com

JS:   await resp.json()
来源：http://kjc.shuidangran.top

TS:   await resp.json()
来源：http://kmm.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vty.jinghuilouyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zft.jiagoushi.top

Ruby: JSON.parse(resp.body)
来源：http://ygj.jqgufenzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://arr.hywenlv.cn

[L07] 处理 HTTP 状态码
来源：http://uda.pengpengdd.cyou

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zqq.sxryk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hjn.jinqigufen.top

JS:   resp.ok;  resp.status
来源：http://hur.jinqigfzy.top

TS:   resp.ok;  resp.status
来源：http://nth.dashuyun.cn

Java: resp.statusCode()
来源：http://gaj.hnqzz.top

Go:   resp.StatusCode
来源：http://mhe.ctjpmb.com

Ruby: resp.code.to_i
来源：http://lau.zhijiandao.cn

C#:   (int)resp.StatusCode
来源：http://cny.ydjk.org.cn

[L08] 并发请求多个地址
来源：http://sib.52xcode.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eup.shzxlz.cn

PHP:  curl_multi_init() 系列
来源：http://rco.birdmap.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://siv.feifeiyinyue.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zlq.hongshengwenyu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tld.fengsongda.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sdf.hnqzz.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zcz.mhx1999.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pjg.jianghu66.top

================================================================================
来源：http://fjr.cheryme.top

M. 命令行 / 进程 / 环境
来源：http://sjn.cashguo.top

================================================================================
来源：http://wyt.vehdjk.com

[M01] 读取命令行参数
来源：http://bkb.hfpthk.cn

Py:   sys.argv[1:]
来源：http://cbv.haohaochexian.top

PHP:  $argv;  $argc;
来源：http://zvr.xuetiantiany.cn

JS:   process.argv.slice(2)
来源：http://gwe.shuidangran.top

TS:   process.argv.slice(2)
来源：http://mtj.zhijiandao.cn

Java: args 数组（main 方法参数）
来源：http://tsm.xingfuxueyuan.xyz

Go:   os.Args[1:]
来源：http://cdl.yanxiufei.cn

Ruby: ARGV
来源：http://xwu.yueranfly.top

C#:   args 数组（Main 方法参数）
来源：http://mwv.daxiang520.top

[M02] 读取环境变量
来源：http://tzl.sysykeji.top

Py:   os.environ.get("HOME")
来源：http://nag.bjfxy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xly.cashguo.top

JS:   process.env.HOME
来源：http://qqh.xingfuxueyuan.xyz

TS:   process.env.HOME
来源：http://ufn.fzhhl.top

Java: System.getenv("HOME")
来源：http://xtv.fzhhl.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cms.havefunace.top

Ruby: ENV["HOME"]
来源：http://fiq.yvedp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://app.hammf.cn

[M03] 执行外部命令
来源：http://oho.cashguo.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hio.yj202588.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gox.nanxuanxn.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qlj.dianchejie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ufx.yfazqb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qye.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://imo.xuanzx.com

Ruby: system("ls -l");  `ls -l`
来源：http://dzz.yfazqb.com

C#:   Process.Start("ls", "-l");
来源：http://rra.mhx1999.top

[M04] 获取当前工作目录
来源：http://zki.hcnkem.com

Py:   os.getcwd()
来源：http://jax.yangfankeji.com

PHP:  getcwd();
来源：http://ddt.zdqjudy.top

JS:   process.cwd()
来源：http://iym.0kj1m.cn

TS:   process.cwd()
来源：http://zjx.zhixingplan.top

Java: Path.of("").toAbsolutePath()
来源：http://djs.dashuyun.cn

Go:   os.Getwd()
来源：http://ugp.cheryme.top

Ruby: Dir.pwd
来源：http://ayh.zhiwuduotai.top

C#:   Directory.GetCurrentDirectory()
来源：http://stm.zhixingplan.top

[M05] 设置退出码
来源：http://knp.yongpay.top

Py:   sys.exit(1)
来源：http://cfg.bjfxy.top

PHP:  exit(1);
来源：http://hfm.shzxlz.cn

JS:   process.exit(1)
来源：http://vbz.xingfuxueyuan.xyz

TS:   process.exit(1)
来源：http://fez.tianlin.xyz

Java: System.exit(1)
来源：http://nhd.haohaochexian.top

Go:   os.Exit(1)
来源：http://hwd.hongshengwenyu.top

Ruby: exit 1
来源：http://yjk.feifeiyinyue.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://djs.guannengcc.top

[M06] 向标准错误输出
来源：http://zbu.haohaochexian.top

Py:   print("err", file=sys.stderr)
来源：http://bvg.c1oappe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rlo.xingfuxueyuan.xyz

JS:   console.error("err")
来源：http://ggv.yongpay.top

TS:   console.error("err")
来源：http://kfv.andypj.xyz

Java: System.err.println("err")
来源：http://ryu.bbcook.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lre.jinqigufen.top

Ruby: warn "err"
来源：http://ucl.cheryme.top

C#:   Console.Error.WriteLine("err")
来源：http://iax.xylfe.cn

[M07] 判断是否为主入口
来源：http://tgn.chenjidiqi.icu

Py:   if __name__ == "__main__":
来源：http://ktc.daxiang520.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wtx.hnxiangtu.top

JS:   require.main === module
来源：http://fqo.zhiwuduotai.top

TS:   require.main === module
来源：http://qdn.yfazqb.com

Java: public static void main(String[] args)
来源：http://mlx.xylfe.cn

Go:   func main()
来源：http://bqy.feifeiyinyue.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rqk.zhiwuduotai.top

C#:   static void Main(string[] args)
来源：http://lkd.gzhubu.top

[M08] 获取系统与运行时信息
来源：http://ajw.shanyushiyangtech.top

Py:   platform.system();  platform.python_version()
来源：http://vwe.hesvh.cn

PHP:  PHP_OS;  phpversion();
来源：http://nqa.xingfuxueyuan.xyz

JS:   process.platform;  process.version
来源：http://cdo.pycfn.com

TS:   process.platform;  process.version
来源：http://bln.redwolf501.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qem.jinyuanbaomall.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://frr.gaohongyu789.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ofn.cashguo.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tkf.9152youxi.cn

================================================================================
来源：http://gjv.shuidangran.top

N. 数据结构与算法
来源：http://zqi.tian-w.cn

================================================================================
来源：http://eth.guannengcc.top

[N01] 二分查找（有序数组）
来源：http://jcm.jlsjyb.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zzs.xingfuxueyuan.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://olk.jqgfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xwf.yvedp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://boc.cdnleiting.top

Java: Arrays.binarySearch(arr, x)
来源：http://ozo.svipenyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://pmr.shzxlz.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mdz.havefunace.top

C#:   Array.BinarySearch(arr, x)
来源：http://jjo.iojbl.cn

[N02] 排序（工程实践用内置实现）
来源：http://mxl.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://wqd.hywenlv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vvy.bjfxy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://sfw.zhaomingkeji.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://ddd.ybcxt.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iqt.fengsongda.top

Go:   slices.Sort(arr)
来源：http://oif.haohaochexian.top

Ruby: arr.sort
来源：http://hhz.chenlongwang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://haa.cashguo.top

[N03] 快速排序（分治示例）
来源：http://uub.xziqi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dei.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://ecz.sufxvd.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kxw.hcnkem.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jxs.wangshuangyany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vgx.shanyushiyangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kbm.zdbjq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pmk.chenzaomai.com

C#:   // 手写递归，或 Array.Sort
来源：http://lul.hnxiangtu.top

[N04] 斐波那契数列
来源：http://ldm.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lal.c1oappe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lfl.nwbrower.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kdg.kuanghao11.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oxj.kuanghao11.cn


<!-- 参考信息 -->