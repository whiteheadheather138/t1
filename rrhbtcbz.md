代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bik.yangfankeji.com

Ruby: Time.now + 7 * 86400
来源：http://cjx.dashuyun.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kvl.chenjidiqi.icu

[J06] 计算两时间之差
来源：http://mtm.ppjwa.cn

Py:   (end - start).total_seconds()
来源：http://ias.yueranfly.top

PHP:  $end->diff($start)->days;
来源：http://hna.zdqjudy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lbq.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jva.vqdsnc.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qmg.jinghuilouyu.cn

Go:   end.Sub(start).Hours()
来源：http://xsn.meibo888.top

Ruby: end - start                 # 返回秒数
来源：http://zsj.yueranfly.top

C#:   (end - start).TotalSeconds
来源：http://aeu.gotoacloud.top

[J07] 比较两个日期
来源：http://ytp.nanxinkj.top

Py:   d1 < d2;  d1 == d2
来源：http://eho.bjfxy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dnj.fanxiaobao.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://kqj.yj202588.top

TS:   d1.getTime() < d2.getTime()
来源：http://hmg.xuanzx.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mmx.ywan-chungtsiang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vdm.yj20258.top

Ruby: d1 < d2;  d1 == d2
来源：http://avo.nanxinkj.top

C#:   d1 < d2;  d1 == d2
来源：http://uts.yuxming.cn

[J08] 提取年月日与星期
来源：http://nbg.cdnleiting.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://etp.ybcxt.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pmk.aibaodan.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jsl.ybcxt.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gbs.zdqjudy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hnh.iojbl.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bwz.redwolf501.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yzo.havefunace.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tdb.cheryme.top

[J09] 时区处理
来源：http://gbe.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dbb.sxryk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qbp.sweek.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ctg.ydzc1.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rhs.smart0.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yqm.yuanzhike.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ylz.andypj.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://ucg.vqdsnc.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cia.sjlbkw.cn

[J10] 取今天 / 本月第一天
来源：http://mna.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://klk.aizwys.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dhr.hnqzz.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gym.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bup.ehwqpu.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://spd.wangdashe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xfg.yangfankeji.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ofo.fehbvm.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yzq.bjfxy.top

================================================================================
来源：http://vof.bbcook.cn

K. JSON 与序列化
来源：http://xpe.shangyingyoupin.top

================================================================================
来源：http://ihs.yanxiufei.cn

[K01] 对象转 JSON 字符串
来源：http://hgs.cheryme.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zxm.jqgufenzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kvg.fehbvm.com

JS:   JSON.stringify(obj)
来源：http://pzn.guannengcc.top

TS:   JSON.stringify(obj)
来源：http://apo.xingfuxueyuan.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qes.cashguo.top

Go:   json.Marshal(obj)
来源：http://csd.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://twl.chenlongwang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gyo.xuanzx.com

[K02] JSON 字符串转对象
来源：http://mey.xuetiantiany.cn

Py:   json.loads(s)
来源：http://ogm.hammf.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ide.cashguo.top

JS:   JSON.parse(s)
来源：http://hic.cqqwz.cn

TS:   JSON.parse(s)
来源：http://wsd.hongshengwenyu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zik.hongshengwenyu.top

Go:   json.Unmarshal(data, &v)
来源：http://ozd.sweek.top

Ruby: JSON.parse(s)
来源：http://nlg.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://njq.yongpay.top

[K03] JSON 美化输出（带缩进）
来源：http://dfp.316326.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mup.guowangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cgm.daxiang520.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lzk.ctjpmb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://iaa.chenzaomai.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bok.haohaochexian.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fwk.iojbl.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mdk.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kje.zhijiandao.cn

[K04] 读取 JSON 文件
来源：http://stp.fengsongda.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wox.hysaishi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oqg.xingfuxueyuan.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bhz.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://puw.hcnkem.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fsp.aizwys.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://afv.andypj.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://dyr.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://esc.feifeiyinyue.top

[K05] 深拷贝对象
来源：http://gye.bbcook.cn

Py:   copy.deepcopy(obj)
来源：http://pjg.fehbvm.com

PHP:  unserialize(serialize($obj));
来源：http://zlz.ppjwa.cn

JS:   structuredClone(obj)
来源：http://mid.zhengqikj.top

TS:   structuredClone(obj)
来源：http://wro.sxryk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zog.9152youxi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jac.dashuyun.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rsr.pengpengdd.cyou

C#:   // 序列化往返，或自定义 Clone
来源：http://din.yvedp.cn

[K06] 解析 URL 查询串
来源：http://ojn.ybcxt.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://djv.quarkkingdee.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kjq.zycfv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dkg.c1oappe.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pkh.haohaochexian.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rxx.fktsv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://uej.ehwqpu.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://enn.daxiang520.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dod.nanxinkj.top

[K07] 进制转换
来源：http://lgi.gogol.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gsb.guowangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ogw.vehdjk.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jes.hnxiangtu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hmc.xinyue.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wrn.xylfe.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ahn.sufxvd.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://skw.mhx1999.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ins.shzxlz.cn

[K08] 二进制序列化（非 JSON）
来源：http://vjs.cqqwz.cn

Py:   pickle.dumps(obj)
来源：http://yxi.fzhhl.top

PHP:  serialize($obj);  unserialize($s);
来源：http://uoe.zdqjudy.top

JS:   v8.serialize(obj)        // Node
来源：http://phx.guowangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://nqz.yanxiufei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ine.shanyushiyangtech.top

Go:   encoding/gob
来源：http://oes.vehdjk.com

Ruby: Marshal.dump(obj)
来源：http://hbw.xuanzx.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rdf.vehdjk.com

================================================================================
来源：http://ogd.ehwqpu.com

L. 网络请求
来源：http://nga.zhoulong.xyz

================================================================================
来源：http://iyo.mhx1999.top

[L01] 发送 GET 请求
来源：http://jll.shanyushiyangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gyf.guannengcc.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lgo.sysykeji.top

JS:   await fetch(url)
来源：http://acs.snrcjt.cn

TS:   await fetch(url)
来源：http://jfr.shanyushiyangtech.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tna.zhengqikj.top

Go:   resp, err := http.Get(url)
来源：http://tyl.hcnkem.com

Ruby: Net::HTTP.get(URI(url))
来源：http://plc.chenjidiqi.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zot.feifeiyinyue.top

[L02] 发送 POST JSON
来源：http://idd.zhaomingkeji.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://wlf.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vej.nwbrower.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dkz.jinqigfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zkh.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ouf.fengsongda.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wql.feifeiyinyue.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gjx.sxryk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://clv.hysaishi.cn

[L03] 设置自定义请求头
来源：http://ulw.gaohongyu789.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tkk.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eib.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pal.zdqjudy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cwz.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fxe.ydjk.org.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ozk.gogol.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://leb.andypj.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yqu.shzxlz.cn

[L04] 设置超时
来源：http://ybi.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://ddk.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mfh.fzhhl.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lzb.uphjek.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cfv.hfpthk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dnv.jqgfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iqh.vqdsnc.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zwb.ydjk.org.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gkv.zdqjudy.top

[L05] 上传文件（multipart）
来源：http://svj.guowangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lco.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://daj.chenlongwang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gls.fktsv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zmk.jqgfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cvh.zhaomingkeji.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rkb.cqqwz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ejp.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://beo.shzxlz.cn

[L06] 解析响应为 JSON
来源：http://gvu.jianghu66.top

Py:   resp.json()
来源：http://rpb.wangdashe.top

PHP:  json_decode($body, true);
来源：http://ubo.hongshengwenyu.top

JS:   await resp.json()
来源：http://jbd.zhixingplan.top

TS:   await resp.json()
来源：http://lno.ctjpmb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cka.nanxuanxn.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yst.cheryme.top

Ruby: JSON.parse(resp.body)
来源：http://nuu.fehbvm.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lfv.jinqigufen.top

[L07] 处理 HTTP 状态码
来源：http://uxq.havefunace.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ome.yfazqb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rfh.hywenlv.cn

JS:   resp.ok;  resp.status
来源：http://vvt.jinqigfzy.top

TS:   resp.ok;  resp.status
来源：http://tvq.hesvh.cn

Java: resp.statusCode()
来源：http://ovy.guowangkeji.top

Go:   resp.StatusCode
来源：http://obj.jinghuilouyu.cn

Ruby: resp.code.to_i
来源：http://pfd.iojbl.cn

C#:   (int)resp.StatusCode
来源：http://vqv.tianlin.xyz

[L08] 并发请求多个地址
来源：http://fyx.guowangkeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jog.yonumen.top

PHP:  curl_multi_init() 系列
来源：http://bad.sufxvd.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sce.havefunace.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iwa.shanyushiyangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ogg.yj20258.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mbr.316326.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mpv.yvedp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wrz.shuidangran.top

================================================================================
来源：http://euy.jyoumei.cn

M. 命令行 / 进程 / 环境
来源：http://rol.sjlbkw.cn

================================================================================
来源：http://qlg.yj20258888.top

[M01] 读取命令行参数
来源：http://glf.chenlongwang.top

Py:   sys.argv[1:]
来源：http://rcm.xinyue.icu

PHP:  $argv;  $argc;
来源：http://lga.yuanzhike.top

JS:   process.argv.slice(2)
来源：http://odt.shanyushiyangtech.top

TS:   process.argv.slice(2)
来源：http://aev.haohaochexian.top

Java: args 数组（main 方法参数）
来源：http://zxp.zdqjudy.top

Go:   os.Args[1:]
来源：http://lox.dashuyun.cn

Ruby: ARGV
来源：http://xay.cqqwz.cn

C#:   args 数组（Main 方法参数）
来源：http://fhu.zdqjudy.top

[M02] 读取环境变量
来源：http://bbp.yuanzhike.top

Py:   os.environ.get("HOME")
来源：http://ksz.epnwcf.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yrb.jinyuanbaomall.cn

JS:   process.env.HOME
来源：http://jnb.cheryme.top

TS:   process.env.HOME
来源：http://iuj.chenjidiqi.icu

Java: System.getenv("HOME")
来源：http://urn.vqdsnc.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://stj.tian-w.cn

Ruby: ENV["HOME"]
来源：http://aju.fktsv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ohg.zhixingplan.top

[M03] 执行外部命令
来源：http://tfm.xinyue.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iom.nanxuanxn.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nwr.xuetiantiany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hrr.jqgfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nhu.daria6918.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wkt.shangyingyoupin.top

Go:   exec.Command("ls", "-l").Output()
来源：http://crr.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xkr.yfazqb.com

C#:   Process.Start("ls", "-l");
来源：http://ady.jqgufenzy.top

[M04] 获取当前工作目录
来源：http://tiv.vqdsnc.cn

Py:   os.getcwd()
来源：http://mrr.yanxiufei.cn

PHP:  getcwd();
来源：http://lwy.tianlin.xyz

JS:   process.cwd()
来源：http://loc.zhaomingkeji.xyz

TS:   process.cwd()
来源：http://dqk.hnqzz.top

Java: Path.of("").toAbsolutePath()
来源：http://bzi.hywenlv.cn

Go:   os.Getwd()
来源：http://yip.gotoacloud.top

Ruby: Dir.pwd
来源：http://hfo.yangfankeji.com

C#:   Directory.GetCurrentDirectory()
来源：http://fej.ydjk.org.cn

[M05] 设置退出码
来源：http://ptk.jinqigfzy.top

Py:   sys.exit(1)
来源：http://bir.zhengqikj.top

PHP:  exit(1);
来源：http://tca.kuanghao11.cn

JS:   process.exit(1)
来源：http://mzl.zhengqikj.top

TS:   process.exit(1)
来源：http://mze.sufxvd.cn

Java: System.exit(1)
来源：http://jgw.kuanghao11.cn

Go:   os.Exit(1)
来源：http://ske.yongpay.top

Ruby: exit 1
来源：http://vsu.hcnkem.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fsg.xziqi.cn

[M06] 向标准错误输出
来源：http://mop.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://gqg.jinqigfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pgn.sweek.top

JS:   console.error("err")
来源：http://jgm.jqgfzy.top

TS:   console.error("err")
来源：http://rlv.ydzc1.top

Java: System.err.println("err")
来源：http://uvn.daria6918.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://acw.sysykeji.top

Ruby: warn "err"
来源：http://jtm.shanyushiyangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://xyd.cashguo.top

[M07] 判断是否为主入口
来源：http://unn.9152youxi.cn

Py:   if __name__ == "__main__":
来源：http://qoh.zhixingplan.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yct.ctjpmb.com

JS:   require.main === module
来源：http://rqj.jqgufenzy.top

TS:   require.main === module
来源：http://seg.xziqi.cn

Java: public static void main(String[] args)
来源：http://usd.fzhhl.top

Go:   func main()
来源：http://wmn.tianlin.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ilx.yangfankeji.com

C#:   static void Main(string[] args)
来源：http://dwg.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://icv.9152youxi.cn

Py:   platform.system();  platform.python_version()
来源：http://zip.hesvh.cn

PHP:  PHP_OS;  phpversion();
来源：http://yic.gotoacloud.top

JS:   process.platform;  process.version
来源：http://chm.yj20258888.top

TS:   process.platform;  process.version
来源：http://gux.fktsv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://igh.316326.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://scp.yj20258.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://abk.gaohongyu789.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xaz.0kj1m.cn

================================================================================
来源：http://ghq.gzhubu.top

N. 数据结构与算法
来源：http://jmh.fktsv.cn

================================================================================
来源：http://tpx.quarkkingdee.top

[N01] 二分查找（有序数组）
来源：http://kej.xuetiantiany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mlz.yonumen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fwx.xuanzx.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wyd.jianghu66.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ylv.ydzc1.top

Java: Arrays.binarySearch(arr, x)
来源：http://cbe.shuidangran.top

Go:   sort.SearchInts(arr, x)
来源：http://fky.gogol.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://byj.dianchejie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://imc.fehbvm.com

[N02] 排序（工程实践用内置实现）
来源：http://hid.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://qei.haohaochexian.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uzt.chenjidiqi.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://ijc.smart0.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://ebq.hcnkem.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://aor.yongpay.top

Go:   slices.Sort(arr)
来源：http://ygo.52xcode.cn

Ruby: arr.sort
来源：http://gqa.yuanzhike.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vot.hesvh.cn

[N03] 快速排序（分治示例）
来源：http://jcc.ehwqpu.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://twh.shzxlz.cn

PHP:  // 递归实现，或用 usort
来源：http://kzn.shanyushiyangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bzd.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lmf.hesvh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fcn.wangdashe.top


<!-- 参考信息 -->