代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mxr.shanyushiyangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://mak.fanxiaobao.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://yxo.sweek.top

[J06] 计算两时间之差
来源：http://aeb.cashguo.top

Py:   (end - start).total_seconds()
来源：http://qpp.meibo888.top

PHP:  $end->diff($start)->days;
来源：http://fdn.yanxiufei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://adn.zycfv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nqu.ehwqpu.com

Java: Duration.between(start, end).toSeconds()
来源：http://swg.cashguo.top

Go:   end.Sub(start).Hours()
来源：http://txq.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://kbc.gaohongyu789.top

C#:   (end - start).TotalSeconds
来源：http://zmh.yanxiufei.cn

[J07] 比较两个日期
来源：http://pfp.sufxvd.cn

Py:   d1 < d2;  d1 == d2
来源：http://cll.ppjwa.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://umj.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://grk.zhixingplan.top

TS:   d1.getTime() < d2.getTime()
来源：http://orh.cucudq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dpl.xuetiantiany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tkr.ivvv.top

Ruby: d1 < d2;  d1 == d2
来源：http://qeo.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://jrl.tianlin.xyz

[J08] 提取年月日与星期
来源：http://vhh.fzhhl.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qkf.fzhhl.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wdh.ctjpmb.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lwg.aibaodan.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wni.tanke756.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pxc.gogol.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bmo.ctjpmb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cvz.gogol.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vcd.yuxming.cn

[J09] 时区处理
来源：http://got.chenzaomai.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fur.ybcxt.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://poi.daria6918.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nck.pengpengdd.cyou

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nka.xingfuxueyuan.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xko.chenjidiqi.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gsv.xingfuxueyuan.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://uoc.jiagoushi.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oil.snrcjt.cn

[J10] 取今天 / 本月第一天
来源：http://xpi.yonumen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ztq.guowangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://puo.ydjk.org.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lrk.cucudq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://viy.hnxiangtu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wjy.zycfv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tog.zhaomingkeji.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iqw.meibo888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oil.yj20258888.top

================================================================================
来源：http://yto.9152youxi.cn

K. JSON 与序列化
来源：http://rkm.zhiwuduotai.top

================================================================================
来源：http://dnf.andypj.xyz

[K01] 对象转 JSON 字符串
来源：http://nwl.shangyingyoupin.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://amn.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rsc.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://fud.ywan-chungtsiang.top

TS:   JSON.stringify(obj)
来源：http://xbp.snrcjt.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://twe.316326.xyz

Go:   json.Marshal(obj)
来源：http://gmn.bjfxy.top

Ruby: obj.to_json                                     // require "json"
来源：http://bly.yueranfly.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hqe.vehdjk.com

[K02] JSON 字符串转对象
来源：http://imo.yonumen.top

Py:   json.loads(s)
来源：http://bla.nanxinkj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tmc.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://rab.jinghuilouyu.cn

TS:   JSON.parse(s)
来源：http://uuo.fengsongda.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://akh.ehwqpu.com

Go:   json.Unmarshal(data, &v)
来源：http://uxw.daxiang520.top

Ruby: JSON.parse(s)
来源：http://hzc.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mkc.aibaodan.cn

[K03] JSON 美化输出（带缩进）
来源：http://zhk.52xcode.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ifo.c1oappe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ypq.ppjwa.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qpd.nwbrower.top

TS:   JSON.stringify(obj, null, 2)
来源：http://oon.sjlbkw.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tfs.guowangkeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bup.snrcjt.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ipm.cucudq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fsx.yueranfly.top

[K04] 读取 JSON 文件
来源：http://vww.havefunace.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ajt.svipenyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://giq.zycfv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uxs.zdbjq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://waf.xziqi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pxm.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lrk.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xux.yonumen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ycl.zhoulong.xyz

[K05] 深拷贝对象
来源：http://nps.hnqzz.top

Py:   copy.deepcopy(obj)
来源：http://haj.jlsjyb.cn

PHP:  unserialize(serialize($obj));
来源：http://ejc.redwolf501.top

JS:   structuredClone(obj)
来源：http://pzg.yonumen.top

TS:   structuredClone(obj)
来源：http://ogc.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://erl.ydzc1.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://isb.yj202588.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rid.wangdashe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://eud.sweek.top

[K06] 解析 URL 查询串
来源：http://xuj.cashguo.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bwq.hcnkem.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fzy.yanxiufei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xeh.zycfv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jiw.yvedp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://avh.zdbjq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ckc.jiagoushi.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hcf.ehwqpu.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bwp.yongpay.top

[K07] 进制转换
来源：http://wpf.chenlongwang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://inv.cqqwz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ska.52xcode.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gab.jinghuilouyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ycq.fzhhl.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zmx.yuanzhike.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ibj.tanke756.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xxh.pycfn.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qrz.mhx1999.top

[K08] 二进制序列化（非 JSON）
来源：http://pcm.guowangkeji.top

Py:   pickle.dumps(obj)
来源：http://ydm.vqdsnc.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://atf.cqqwz.cn

JS:   v8.serialize(obj)        // Node
来源：http://pbk.jlsjyb.cn

TS:   v8.serialize(obj)        // Node
来源：http://vpf.ppjwa.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ojw.vqdsnc.cn

Go:   encoding/gob
来源：http://uxv.ydzc1.top

Ruby: Marshal.dump(obj)
来源：http://nfi.snrcjt.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://urr.yj202588.top

================================================================================
来源：http://jdv.bbcook.cn

L. 网络请求
来源：http://lbf.jiagoushi.top

================================================================================
来源：http://ffm.yj20258888.top

[L01] 发送 GET 请求
来源：http://uan.jinyuanbaomall.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eho.tian-w.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jyh.chenzaomai.com

JS:   await fetch(url)
来源：http://tji.pycfn.com

TS:   await fetch(url)
来源：http://vnq.yonumen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uyu.hcnkem.com

Go:   resp, err := http.Get(url)
来源：http://tsz.jqgfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://apd.chenzaomai.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ref.cashguo.top

[L02] 发送 POST JSON
来源：http://yhd.cucudq.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dol.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://isf.gzhubu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zln.cucudq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yai.hysaishi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://reg.jyoumei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cwa.hnqzz.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nze.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tak.yfazqb.com

[L03] 设置自定义请求头
来源：http://btp.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ego.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pmk.ybcxt.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://noe.hammf.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://czn.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://afj.vqdsnc.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sbm.zhoulong.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zzi.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://toh.316326.xyz

[L04] 设置超时
来源：http://mbu.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://dsq.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://osh.0kj1m.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tvz.feifeiyinyue.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lzo.shuidangran.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rds.zhaomingkeji.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cid.ppjwa.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xfp.ppjwa.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gte.jlsjyb.cn

[L05] 上传文件（multipart）
来源：http://yjt.hammf.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kql.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://khh.sxryk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hqr.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sjc.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lkb.redwolf501.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qal.xingfuxueyuan.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qml.jlsjyb.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mdv.zhengqikj.top

[L06] 解析响应为 JSON
来源：http://zes.snrcjt.cn

Py:   resp.json()
来源：http://yww.jianghu66.top

PHP:  json_decode($body, true);
来源：http://vag.fktsv.cn

JS:   await resp.json()
来源：http://dak.tian-w.cn

TS:   await resp.json()
来源：http://rtq.mhx1999.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wyo.yfazqb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wfg.ivvv.top

Ruby: JSON.parse(resp.body)
来源：http://ksd.zhaomingkeji.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://aff.zhixingplan.top

[L07] 处理 HTTP 状态码
来源：http://eno.gzhubu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blc.nwbrower.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ujl.hnqzz.top

JS:   resp.ok;  resp.status
来源：http://dwf.hywenlv.cn

TS:   resp.ok;  resp.status
来源：http://pfr.hywenlv.cn

Java: resp.statusCode()
来源：http://hyw.shzxlz.cn

Go:   resp.StatusCode
来源：http://bry.cashguo.top

Ruby: resp.code.to_i
来源：http://uvi.smart0.xyz

C#:   (int)resp.StatusCode
来源：http://apa.snrcjt.cn

[L08] 并发请求多个地址
来源：http://hda.shuidangran.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ero.hfpthk.cn

PHP:  curl_multi_init() 系列
来源：http://mhh.yuxming.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gbv.xuanzx.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kdx.chenlongwang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://amr.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://axs.daria6918.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ens.jiagoushi.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gsk.tian-w.cn

================================================================================
来源：http://ihq.cheryme.top

M. 命令行 / 进程 / 环境
来源：http://mpr.xingfuxueyuan.xyz

================================================================================
来源：http://esc.chenjidiqi.icu

[M01] 读取命令行参数
来源：http://qef.ywan-chungtsiang.top

Py:   sys.argv[1:]
来源：http://qxo.tianlin.xyz

PHP:  $argv;  $argc;
来源：http://nni.cdnleiting.top

JS:   process.argv.slice(2)
来源：http://upu.haohaochexian.top

TS:   process.argv.slice(2)
来源：http://bcu.xingfuxueyuan.xyz

Java: args 数组（main 方法参数）
来源：http://fbg.yfazqb.com

Go:   os.Args[1:]
来源：http://mjm.zhixingplan.top

Ruby: ARGV
来源：http://ody.gogol.net.cn

C#:   args 数组（Main 方法参数）
来源：http://rrn.sweek.top

[M02] 读取环境变量
来源：http://bor.yuanzhike.top

Py:   os.environ.get("HOME")
来源：http://dqw.ivvv.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qia.xingfuxueyuan.xyz

JS:   process.env.HOME
来源：http://guj.aibaodan.cn

TS:   process.env.HOME
来源：http://zzz.xingfuxueyuan.xyz

Java: System.getenv("HOME")
来源：http://suz.aibaodan.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jvp.jianghu66.top

Ruby: ENV["HOME"]
来源：http://hcb.yongpay.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ulz.yuanzhike.top

[M03] 执行外部命令
来源：http://qxh.sweek.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lta.jqgfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://czy.yuxming.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pde.yongpay.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lsz.vehdjk.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lvh.hcnkem.com

Go:   exec.Command("ls", "-l").Output()
来源：http://efi.cucudq.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fdh.xuanzx.com

C#:   Process.Start("ls", "-l");
来源：http://ljn.zhixingplan.top

[M04] 获取当前工作目录
来源：http://oqv.dianchejie.cn

Py:   os.getcwd()
来源：http://rsr.hesvh.cn

PHP:  getcwd();
来源：http://jtg.gogol.net.cn

JS:   process.cwd()
来源：http://pek.smart0.xyz

TS:   process.cwd()
来源：http://fkh.xziqi.cn

Java: Path.of("").toAbsolutePath()
来源：http://avl.sufxvd.cn

Go:   os.Getwd()
来源：http://ptr.sysykeji.top

Ruby: Dir.pwd
来源：http://kwz.bbcook.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pja.yvedp.cn

[M05] 设置退出码
来源：http://eir.daxiang520.top

Py:   sys.exit(1)
来源：http://mgt.tanke756.top

PHP:  exit(1);
来源：http://fxk.yj20258888.top

JS:   process.exit(1)
来源：http://ete.jiagoushi.top

TS:   process.exit(1)
来源：http://wer.zdbjq.cn

Java: System.exit(1)
来源：http://zbg.jqgufenzy.top

Go:   os.Exit(1)
来源：http://dci.chenjidiqi.icu

Ruby: exit 1
来源：http://bub.zhoulong.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://npc.sysykeji.top

[M06] 向标准错误输出
来源：http://frp.52xcode.cn

Py:   print("err", file=sys.stderr)
来源：http://tim.cucudq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://onx.hesvh.cn

JS:   console.error("err")
来源：http://ber.aizwys.cn

TS:   console.error("err")
来源：http://yzb.wangshuangyany.cn

Java: System.err.println("err")
来源：http://soi.gotoacloud.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ibu.c1oappe.top

Ruby: warn "err"
来源：http://sdx.bjfxy.top

C#:   Console.Error.WriteLine("err")
来源：http://dlf.zycfv.cn

[M07] 判断是否为主入口
来源：http://cax.cucudq.cn

Py:   if __name__ == "__main__":
来源：http://cfh.zhixingplan.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://axg.0kj1m.cn

JS:   require.main === module
来源：http://wps.hnqzz.top

TS:   require.main === module
来源：http://ptx.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://skz.jinqigufen.top

Go:   func main()
来源：http://yke.jqgfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gvj.ivvv.top

C#:   static void Main(string[] args)
来源：http://sdm.iojbl.cn

[M08] 获取系统与运行时信息
来源：http://jbg.xingfuxueyuan.xyz

Py:   platform.system();  platform.python_version()
来源：http://uix.hysaishi.cn

PHP:  PHP_OS;  phpversion();
来源：http://znk.redwolf501.top

JS:   process.platform;  process.version
来源：http://hik.cheryme.top

TS:   process.platform;  process.version
来源：http://iqm.vehdjk.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mnm.jyoumei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mpj.nanxuanxn.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://arw.cucudq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sen.ppjwa.cn

================================================================================
来源：http://qbr.gotoacloud.top

N. 数据结构与算法
来源：http://lwc.c1oappe.top

================================================================================
来源：http://wys.zycfv.cn

[N01] 二分查找（有序数组）
来源：http://gya.jianghu66.top

Py:   bisect.bisect_left(arr, x)
来源：http://abh.daria6918.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ldq.gotoacloud.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ydq.daxiang520.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iyo.hfpthk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rnf.jiagoushi.top

Go:   sort.SearchInts(arr, x)
来源：http://bve.tarul.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bgk.dashuyun.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hjb.hongshengwenyu.top

[N02] 排序（工程实践用内置实现）
来源：http://bzq.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://wer.zhijiandao.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zhx.ivvv.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vzj.9152youxi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vwk.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mdd.guannengcc.top

Go:   slices.Sort(arr)
来源：http://rqk.birdmap.top

Ruby: arr.sort
来源：http://chs.yuxming.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://isj.fengsongda.top

[N03] 快速排序（分治示例）
来源：http://uin.hywenlv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wxz.cucudq.cn

PHP:  // 递归实现，或用 usort
来源：http://svs.hnxiangtu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mnz.shuidangran.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://obm.xingfuxueyuan.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rqx.nanxinkj.top


<!-- 参考信息 -->