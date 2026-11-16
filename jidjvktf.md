代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://cus.jianghu66.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nvq.shuidangran.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zos.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://svd.epnwcf.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dwc.sjlbkw.cn

Ruby: Time.now + 7 * 86400
来源：http://nwp.yanxiufei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ubr.smart0.xyz

[J06] 计算两时间之差
来源：http://xfl.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://ppt.xingfuxueyuan.xyz

PHP:  $end->diff($start)->days;
来源：http://esp.vehdjk.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nyq.jinyuanbaomall.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kkl.aizwys.cn

Java: Duration.between(start, end).toSeconds()
来源：http://saw.ydzc1.top

Go:   end.Sub(start).Hours()
来源：http://fog.nanxuanxn.top

Ruby: end - start                 # 返回秒数
来源：http://pcj.haohaochexian.top

C#:   (end - start).TotalSeconds
来源：http://wqf.cheryme.top

[J07] 比较两个日期
来源：http://fik.zycfv.cn

Py:   d1 < d2;  d1 == d2
来源：http://gdu.tian-w.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jyf.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://mvd.sweek.top

TS:   d1.getTime() < d2.getTime()
来源：http://amf.ppjwa.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wbv.ydzc1.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://veu.cdnleiting.top

Ruby: d1 < d2;  d1 == d2
来源：http://nnv.fanxiaobao.xyz

C#:   d1 < d2;  d1 == d2
来源：http://pty.tarul.cn

[J08] 提取年月日与星期
来源：http://kzh.quarkkingdee.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iui.nanxinkj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xpq.xinyue.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://poy.gogol.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ltq.jlsjyb.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uvk.sweek.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ixz.gotoacloud.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ukh.meibo888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rhj.ydzc1.top

[J09] 时区处理
来源：http://lfd.9152youxi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eaf.sxryk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://srz.hcnkem.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qhy.chenzaomai.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://snn.ehwqpu.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eca.pengpengdd.cyou

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iho.zhoulong.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://zfj.52xcode.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://guw.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://ski.fzhhl.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xti.jianghu66.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ife.fanxiaobao.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mrn.chenlongwang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yxi.ppjwa.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://omw.bjfxy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kph.jinqigufen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ske.ppjwa.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qae.daxiang520.top

================================================================================
来源：http://eaa.ehwqpu.com

K. JSON 与序列化
来源：http://jxj.cashguo.top

================================================================================
来源：http://rvj.fzhhl.top

[K01] 对象转 JSON 字符串
来源：http://jjk.shanyushiyangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fwx.yj202588.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rra.jinqigfzy.top

JS:   JSON.stringify(obj)
来源：http://owm.yj202588.top

TS:   JSON.stringify(obj)
来源：http://hrf.yuxming.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://igp.hnxiangtu.top

Go:   json.Marshal(obj)
来源：http://ifx.52xcode.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vql.ctjpmb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://vsn.guannengcc.top

[K02] JSON 字符串转对象
来源：http://jqx.ybcxt.top

Py:   json.loads(s)
来源：http://xnu.cdnleiting.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ilu.daria6918.cn

JS:   JSON.parse(s)
来源：http://vct.shzxlz.cn

TS:   JSON.parse(s)
来源：http://abh.cdnleiting.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://glw.jinghuilouyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://eco.fktsv.cn

Ruby: JSON.parse(s)
来源：http://mqs.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://srr.cashguo.top

[K03] JSON 美化输出（带缩进）
来源：http://hpd.hywenlv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fju.hnqzz.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zgm.ywan-chungtsiang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://srr.yj20258.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fqj.yuanzhike.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hug.tanke756.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dmh.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://axk.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pzi.xingfuxueyuan.xyz

[K04] 读取 JSON 文件
来源：http://vck.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fmk.zhixingplan.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://awg.yj20258888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dsr.hywenlv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://etm.sweek.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://epx.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sfg.52xcode.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jks.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vuo.yuxming.cn

[K05] 深拷贝对象
来源：http://yjg.316326.xyz

Py:   copy.deepcopy(obj)
来源：http://jkw.hongshengwenyu.top

PHP:  unserialize(serialize($obj));
来源：http://wyi.gotoacloud.top

JS:   structuredClone(obj)
来源：http://etx.yangfankeji.com

TS:   structuredClone(obj)
来源：http://drr.ywan-chungtsiang.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nke.fehbvm.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wvc.zycfv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bqi.meibo888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rsx.nanxuanxn.top

[K06] 解析 URL 查询串
来源：http://dvl.zhengqikj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lux.ppjwa.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ttk.pycfn.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xtt.vehdjk.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jee.tian-w.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kte.xziqi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://buw.daxiang520.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xha.shangyingyoupin.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qas.fktsv.cn

[K07] 进制转换
来源：http://sdb.haohaochexian.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ggh.feifeiyinyue.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://laf.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rlx.iojbl.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://epz.redwolf501.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xkw.svipenyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tpn.vehdjk.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zte.nanxinkj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dqi.jiagoushi.top

[K08] 二进制序列化（非 JSON）
来源：http://qte.smart0.xyz

Py:   pickle.dumps(obj)
来源：http://pkf.gogol.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fxh.pycfn.com

JS:   v8.serialize(obj)        // Node
来源：http://ghr.hesvh.cn

TS:   v8.serialize(obj)        // Node
来源：http://byu.uphjek.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jpm.316326.xyz

Go:   encoding/gob
来源：http://pda.pengpengdd.cyou

Ruby: Marshal.dump(obj)
来源：http://uur.yuxming.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wrc.yfazqb.com

================================================================================
来源：http://pxj.wangdashe.top

L. 网络请求
来源：http://dvx.xylfe.cn

================================================================================
来源：http://oii.ppjwa.cn

[L01] 发送 GET 请求
来源：http://bod.nanxinkj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gas.ybcxt.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://txg.birdmap.top

JS:   await fetch(url)
来源：http://ebl.dashuyun.cn

TS:   await fetch(url)
来源：http://pfr.bjfxy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dmk.gaohongyu789.top

Go:   resp, err := http.Get(url)
来源：http://wry.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tto.sxryk.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wkf.daxiang520.top

[L02] 发送 POST JSON
来源：http://hoh.mhx1999.top

Py:   requests.post(url, json={"a": 1})
来源：http://koa.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jtz.hesvh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mrk.zhijiandao.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pdn.pycfn.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jfg.xuetiantiany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kiq.jinqigufen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uoc.redwolf501.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nly.yuanzhike.top

[L03] 设置自定义请求头
来源：http://izi.fengsongda.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aeh.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://aqx.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mmb.0kj1m.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://icg.meibo888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jsn.shuidangran.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jib.jianghu66.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://elf.vehdjk.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qjj.haohaochexian.top

[L04] 设置超时
来源：http://wvn.guowangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://pxh.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bto.aizwys.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pah.yvedp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xor.andypj.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ouh.pengpengdd.cyou

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qor.hnqzz.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dth.jianghu66.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fkv.zhiwuduotai.top

[L05] 上传文件（multipart）
来源：http://anx.svipenyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tqi.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zup.chenjidiqi.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ppn.zhijiandao.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ovj.redwolf501.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dsg.gzhubu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qcf.yangfankeji.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qzd.jiagoushi.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lyn.52xcode.cn

[L06] 解析响应为 JSON
来源：http://axk.yangfankeji.com

Py:   resp.json()
来源：http://cah.sjlbkw.cn

PHP:  json_decode($body, true);
来源：http://gst.jinyuanbaomall.cn

JS:   await resp.json()
来源：http://xsy.jinqigfzy.top

TS:   await resp.json()
来源：http://xkq.cashguo.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rns.sjlbkw.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mma.nanxinkj.top

Ruby: JSON.parse(resp.body)
来源：http://ysf.aizwys.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gnw.gzhubu.top

[L07] 处理 HTTP 状态码
来源：http://jdr.xuetiantiany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pqt.ppjwa.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wbm.bjfxy.top

JS:   resp.ok;  resp.status
来源：http://jct.shanyushiyangkeji.top

TS:   resp.ok;  resp.status
来源：http://jdf.9152youxi.cn

Java: resp.statusCode()
来源：http://mgg.chenjidiqi.icu

Go:   resp.StatusCode
来源：http://viq.zhixingplan.top

Ruby: resp.code.to_i
来源：http://nbz.xuanzx.com

C#:   (int)resp.StatusCode
来源：http://vzt.shanyushiyangtech.top

[L08] 并发请求多个地址
来源：http://fpp.gzhubu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mmk.zdbjq.cn

PHP:  curl_multi_init() 系列
来源：http://nbz.bjfxy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tcg.birdmap.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sgw.wangshuangyany.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dfk.zhixingplan.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aax.hfpthk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://llu.ydjk.org.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dbz.316326.xyz

================================================================================
来源：http://lee.gogol.net.cn

M. 命令行 / 进程 / 环境
来源：http://jze.cucudq.cn

================================================================================
来源：http://eyf.hysaishi.cn

[M01] 读取命令行参数
来源：http://lhb.bbcook.cn

Py:   sys.argv[1:]
来源：http://kci.zycfv.cn

PHP:  $argv;  $argc;
来源：http://dgv.jyoumei.cn

JS:   process.argv.slice(2)
来源：http://npj.smart0.xyz

TS:   process.argv.slice(2)
来源：http://joz.chenlongwang.top

Java: args 数组（main 方法参数）
来源：http://xiy.yuanzhike.top

Go:   os.Args[1:]
来源：http://svc.haohaochexian.top

Ruby: ARGV
来源：http://phj.haohaochexian.top

C#:   args 数组（Main 方法参数）
来源：http://iux.yj202588.top

[M02] 读取环境变量
来源：http://crx.zdbjq.cn

Py:   os.environ.get("HOME")
来源：http://jct.meibo888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fsm.bbcook.cn

JS:   process.env.HOME
来源：http://uca.havefunace.top

TS:   process.env.HOME
来源：http://qqy.zhengqikj.top

Java: System.getenv("HOME")
来源：http://gyp.nwbrower.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cco.ivvv.top

Ruby: ENV["HOME"]
来源：http://led.tian-w.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jyq.hcnkem.com

[M03] 执行外部命令
来源：http://fio.zhoulong.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hbw.xuetiantiany.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://awf.bjfxy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://igj.hongshengwenyu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vsd.andypj.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yre.hfpthk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://taf.chenjidiqi.icu

Ruby: system("ls -l");  `ls -l`
来源：http://tsn.jinyuanbaomall.cn

C#:   Process.Start("ls", "-l");
来源：http://pcv.vqdsnc.cn

[M04] 获取当前工作目录
来源：http://tya.ctjpmb.com

Py:   os.getcwd()
来源：http://jmi.haohaochexian.top

PHP:  getcwd();
来源：http://lho.bbcook.cn

JS:   process.cwd()
来源：http://mtj.vehdjk.com

TS:   process.cwd()
来源：http://vru.fanxiaobao.xyz

Java: Path.of("").toAbsolutePath()
来源：http://cth.52xcode.cn

Go:   os.Getwd()
来源：http://ukp.yuanzhike.top

Ruby: Dir.pwd
来源：http://eqs.zdbjq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qxl.yj202588.top

[M05] 设置退出码
来源：http://xkf.ywan-chungtsiang.top

Py:   sys.exit(1)
来源：http://jqd.wangdashe.top

PHP:  exit(1);
来源：http://byi.yuxming.cn

JS:   process.exit(1)
来源：http://cfg.yj20258.top

TS:   process.exit(1)
来源：http://chc.zhengqikj.top

Java: System.exit(1)
来源：http://qmq.shzxlz.cn

Go:   os.Exit(1)
来源：http://zak.shangyingyoupin.top

Ruby: exit 1
来源：http://php.nanxuanxn.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ldi.zhijiandao.cn

[M06] 向标准错误输出
来源：http://ocl.jinyuanbaomall.cn

Py:   print("err", file=sys.stderr)
来源：http://bao.tarul.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://uaz.cucudq.cn

JS:   console.error("err")
来源：http://prg.hnqzz.top

TS:   console.error("err")
来源：http://awv.tanke756.top

Java: System.err.println("err")
来源：http://say.ctjpmb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ltb.zycfv.cn

Ruby: warn "err"
来源：http://qow.sjlbkw.cn

C#:   Console.Error.WriteLine("err")
来源：http://jbi.bbcook.cn

[M07] 判断是否为主入口
来源：http://eye.fengsongda.top

Py:   if __name__ == "__main__":
来源：http://unc.redwolf501.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ldu.hysaishi.cn

JS:   require.main === module
来源：http://hrx.xziqi.cn

TS:   require.main === module
来源：http://opb.nanxinkj.top

Java: public static void main(String[] args)
来源：http://vkr.yueranfly.top

Go:   func main()
来源：http://gor.jinghuilouyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gll.epnwcf.com

C#:   static void Main(string[] args)
来源：http://qut.guowangkeji.top

[M08] 获取系统与运行时信息
来源：http://ivu.yj20258.top

Py:   platform.system();  platform.python_version()
来源：http://yif.cashguo.top

PHP:  PHP_OS;  phpversion();
来源：http://alx.shanyushiyangkeji.top

JS:   process.platform;  process.version
来源：http://cwm.ydjk.org.cn

TS:   process.platform;  process.version
来源：http://bxx.hywenlv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uxl.yongpay.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gbm.iojbl.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vsa.jqgufenzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kxh.vehdjk.com

================================================================================
来源：http://fey.xziqi.cn

N. 数据结构与算法
来源：http://dsk.hongshengwenyu.top

================================================================================
来源：http://wyc.316326.xyz

[N01] 二分查找（有序数组）
来源：http://lvp.yj20258888.top

Py:   bisect.bisect_left(arr, x)
来源：http://knc.hysaishi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vpy.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uty.yuxming.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vvo.yuanzhike.top

Java: Arrays.binarySearch(arr, x)
来源：http://neg.daria6918.cn

Go:   sort.SearchInts(arr, x)
来源：http://xcy.mhx1999.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://uqj.yj20258.top

C#:   Array.BinarySearch(arr, x)
来源：http://xib.ywan-chungtsiang.top

[N02] 排序（工程实践用内置实现）
来源：http://wjs.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://unj.sufxvd.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rjt.shuidangran.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://uim.yj20258888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://toe.chenzaomai.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://emg.yuxming.cn

Go:   slices.Sort(arr)
来源：http://jnh.tianlin.xyz

Ruby: arr.sort
来源：http://mzv.aizwys.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bmz.yanxiufei.cn

[N03] 快速排序（分治示例）
来源：http://zsa.cashguo.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mul.redwolf501.top


<!-- 参考信息 -->