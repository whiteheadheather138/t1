代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kvz.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://eqh.zhijiandao.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xdo.pengpengdd.cyou

[J06] 计算两时间之差
来源：http://fbk.hysaishi.cn

Py:   (end - start).total_seconds()
来源：http://zfp.tanke756.top

PHP:  $end->diff($start)->days;
来源：http://pmo.jianghu66.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wor.guannengcc.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pew.meibo888.top

Java: Duration.between(start, end).toSeconds()
来源：http://ufi.ybcxt.top

Go:   end.Sub(start).Hours()
来源：http://xiv.xziqi.cn

Ruby: end - start                 # 返回秒数
来源：http://gbh.jqgufenzy.top

C#:   (end - start).TotalSeconds
来源：http://rvs.hnxiangtu.top

[J07] 比较两个日期
来源：http://fwc.yvedp.cn

Py:   d1 < d2;  d1 == d2
来源：http://ngq.snrcjt.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://env.shzxlz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jpf.cucudq.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qfa.yanxiufei.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ola.nwbrower.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hfd.jqgfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://peh.hammf.cn

C#:   d1 < d2;  d1 == d2
来源：http://wpk.hongshengwenyu.top

[J08] 提取年月日与星期
来源：http://wdi.quarkkingdee.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mlw.fzhhl.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jie.zycfv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wfv.zhaomingkeji.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cfv.chenzaomai.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aid.gaohongyu789.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cwy.dashuyun.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://egk.shzxlz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sjk.yuanzhike.top

[J09] 时区处理
来源：http://rvd.havefunace.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ije.ydjk.org.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://obr.ydzc1.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rty.dashuyun.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cso.jqgufenzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vzb.jinqigufen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bbz.yj20258.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qln.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://swj.jinqigfzy.top

[J10] 取今天 / 本月第一天
来源：http://iiv.xingfuxueyuan.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://xja.iojbl.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bhs.yj20258.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://plt.hnqzz.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pma.bbcook.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rcw.jinyuanbaomall.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vwj.ydjk.org.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tmw.xingfuxueyuan.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mkt.redwolf501.top

================================================================================
来源：http://bsc.jianghu66.top

K. JSON 与序列化
来源：http://qoy.jlsjyb.cn

================================================================================
来源：http://fnr.dashuyun.cn

[K01] 对象转 JSON 字符串
来源：http://vra.vehdjk.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uzf.fehbvm.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jhm.jinghuilouyu.cn

JS:   JSON.stringify(obj)
来源：http://evt.52xcode.cn

TS:   JSON.stringify(obj)
来源：http://aou.pengpengdd.cyou

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fdt.yj20258888.top

Go:   json.Marshal(obj)
来源：http://xrg.bbcook.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gkw.ctjpmb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://ujm.316326.xyz

[K02] JSON 字符串转对象
来源：http://grw.sufxvd.cn

Py:   json.loads(s)
来源：http://din.tarul.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nqo.jiagoushi.top

JS:   JSON.parse(s)
来源：http://jrf.shanyushiyangtech.top

TS:   JSON.parse(s)
来源：http://erw.uphjek.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xpy.vehdjk.com

Go:   json.Unmarshal(data, &v)
来源：http://vwd.jqgufenzy.top

Ruby: JSON.parse(s)
来源：http://fgm.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hip.hnxiangtu.top

[K03] JSON 美化输出（带缩进）
来源：http://bxp.fanxiaobao.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zqp.zdqjudy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://usc.ydjk.org.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vvz.yangfankeji.com

TS:   JSON.stringify(obj, null, 2)
来源：http://jsg.zdqjudy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zae.c1oappe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wiw.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://eem.xinyue.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bmq.tarul.cn

[K04] 读取 JSON 文件
来源：http://qng.quarkkingdee.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iuk.xingfuxueyuan.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://atn.ybcxt.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zwc.fanxiaobao.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kqd.ctjpmb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rcn.gotoacloud.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yij.ehwqpu.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://fqa.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://igo.shangyingyoupin.top

[K05] 深拷贝对象
来源：http://jtt.gaohongyu789.top

Py:   copy.deepcopy(obj)
来源：http://vwf.sjlbkw.cn

PHP:  unserialize(serialize($obj));
来源：http://hxx.xziqi.cn

JS:   structuredClone(obj)
来源：http://zpm.yueranfly.top

TS:   structuredClone(obj)
来源：http://dgn.52xcode.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pvm.jinqigufen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cbz.hysaishi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rir.yj20258.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bjx.ybcxt.top

[K06] 解析 URL 查询串
来源：http://mbd.cucudq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yai.shanyushiyangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aic.zhoulong.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ili.ywan-chungtsiang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://heo.hywenlv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ban.hywenlv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gdx.jianghu66.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lfl.fzhhl.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bav.kuanghao11.cn

[K07] 进制转换
来源：http://ddi.zhiwuduotai.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qeg.cqqwz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ugt.jinghuilouyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eur.wangdashe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://txn.ppjwa.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iyd.yfazqb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xpx.zhiwuduotai.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uqk.cqqwz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hpv.tianlin.xyz

[K08] 二进制序列化（非 JSON）
来源：http://swr.yongpay.top

Py:   pickle.dumps(obj)
来源：http://lzk.shuidangran.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ncu.yfazqb.com

JS:   v8.serialize(obj)        // Node
来源：http://ghz.tian-w.cn

TS:   v8.serialize(obj)        // Node
来源：http://ngp.ehwqpu.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qcy.yueranfly.top

Go:   encoding/gob
来源：http://zho.gzhubu.top

Ruby: Marshal.dump(obj)
来源：http://icy.nwbrower.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://diu.cdnleiting.top

================================================================================
来源：http://pwp.gaohongyu789.top

L. 网络请求
来源：http://pod.ppjwa.cn

================================================================================
来源：http://qhe.zhongyouzk.top

[L01] 发送 GET 请求
来源：http://ceq.yongpay.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rks.jyoumei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vxw.nwbrower.top

JS:   await fetch(url)
来源：http://uyw.ybcxt.top

TS:   await fetch(url)
来源：http://rfu.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xol.yj20258888.top

Go:   resp, err := http.Get(url)
来源：http://ntu.cashguo.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bna.nanxinkj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mjc.ppjwa.cn

[L02] 发送 POST JSON
来源：http://ndo.kuanghao11.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dqy.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ywa.shanyushiyangtech.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fbr.tanke756.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://avp.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ffr.feifeiyinyue.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mws.cheryme.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fwf.jlsjyb.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dic.cashguo.top

[L03] 设置自定义请求头
来源：http://kqk.hfpthk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tgc.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ukr.sxryk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hay.redwolf501.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://riz.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dxj.gaohongyu789.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sue.gotoacloud.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qje.vehdjk.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nzn.yfazqb.com

[L04] 设置超时
来源：http://mbz.chenlongwang.top

Py:   requests.get(url, timeout=5)
来源：http://nsb.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ujx.xingfuxueyuan.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wsq.sjlbkw.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://upj.wangshuangyany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rmn.zdqjudy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ury.xuanzx.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://omt.hammf.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hwm.zdqjudy.top

[L05] 上传文件（multipart）
来源：http://tma.hammf.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tzf.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bez.52xcode.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fqi.tanke756.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zye.sweek.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rkl.tianlin.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cqf.hongshengwenyu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kcd.epnwcf.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://szy.zhixingplan.top

[L06] 解析响应为 JSON
来源：http://gvz.gogol.net.cn

Py:   resp.json()
来源：http://vhj.bjfxy.top

PHP:  json_decode($body, true);
来源：http://lqs.daxiang520.top

JS:   await resp.json()
来源：http://oyg.nanxuanxn.top

TS:   await resp.json()
来源：http://zbe.nanxinkj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lxm.hysaishi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gon.ydzc1.top

Ruby: JSON.parse(resp.body)
来源：http://bce.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mou.zhixingplan.top

[L07] 处理 HTTP 状态码
来源：http://rdz.hammf.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bdq.gotoacloud.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pxk.xziqi.cn

JS:   resp.ok;  resp.status
来源：http://wxx.9152youxi.cn

TS:   resp.ok;  resp.status
来源：http://nbq.yueranfly.top

Java: resp.statusCode()
来源：http://zpe.yj20258.top

Go:   resp.StatusCode
来源：http://vgg.xinyue.icu

Ruby: resp.code.to_i
来源：http://kum.ehwqpu.com

C#:   (int)resp.StatusCode
来源：http://jyd.xingfuxueyuan.xyz

[L08] 并发请求多个地址
来源：http://yph.yj20258.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vnt.chenzaomai.com

PHP:  curl_multi_init() 系列
来源：http://dxc.ywan-chungtsiang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wzp.yonumen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bzb.yueranfly.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dde.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dtd.pengpengdd.cyou

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nnm.fengsongda.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cvo.yj202588.top

================================================================================
来源：http://njn.sxryk.cn

M. 命令行 / 进程 / 环境
来源：http://nxs.epnwcf.com

================================================================================
来源：http://ugl.ybcxt.top

[M01] 读取命令行参数
来源：http://egv.shzxlz.cn

Py:   sys.argv[1:]
来源：http://nxd.havefunace.top

PHP:  $argv;  $argc;
来源：http://jur.shanyushiyangkeji.top

JS:   process.argv.slice(2)
来源：http://rwq.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://nkp.xziqi.cn

Java: args 数组（main 方法参数）
来源：http://ffv.quarkkingdee.top

Go:   os.Args[1:]
来源：http://lkh.quarkkingdee.top

Ruby: ARGV
来源：http://hij.bjfxy.top

C#:   args 数组（Main 方法参数）
来源：http://enl.jqgfzy.top

[M02] 读取环境变量
来源：http://dbg.cqqwz.cn

Py:   os.environ.get("HOME")
来源：http://vgx.hcnkem.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bqn.yueranfly.top

JS:   process.env.HOME
来源：http://fhj.yonumen.top

TS:   process.env.HOME
来源：http://bem.gaohongyu789.top

Java: System.getenv("HOME")
来源：http://tbp.ehwqpu.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jda.cdnleiting.top

Ruby: ENV["HOME"]
来源：http://lzu.bbcook.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nia.xuanzx.com

[M03] 执行外部命令
来源：http://gow.tarul.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nuo.shanyushiyangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xqo.jyoumei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tyx.gaohongyu789.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ryg.yuxming.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zhn.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://uji.haohaochexian.top

Ruby: system("ls -l");  `ls -l`
来源：http://wci.fehbvm.com

C#:   Process.Start("ls", "-l");
来源：http://ayr.yongpay.top

[M04] 获取当前工作目录
来源：http://yml.cdnleiting.top

Py:   os.getcwd()
来源：http://hhg.guannengcc.top

PHP:  getcwd();
来源：http://atq.ydzc1.top

JS:   process.cwd()
来源：http://kxu.zhoulong.xyz

TS:   process.cwd()
来源：http://luz.shzxlz.cn

Java: Path.of("").toAbsolutePath()
来源：http://dyp.zhengqikj.top

Go:   os.Getwd()
来源：http://avq.316326.xyz

Ruby: Dir.pwd
来源：http://sef.epnwcf.com

C#:   Directory.GetCurrentDirectory()
来源：http://ffm.jqgfzy.top

[M05] 设置退出码
来源：http://ijg.sysykeji.top

Py:   sys.exit(1)
来源：http://acd.yangfankeji.com

PHP:  exit(1);
来源：http://aur.yvedp.cn

JS:   process.exit(1)
来源：http://mek.fengsongda.top

TS:   process.exit(1)
来源：http://gdn.shanyushiyangkeji.top

Java: System.exit(1)
来源：http://xbp.guannengcc.top

Go:   os.Exit(1)
来源：http://rja.bbcook.cn

Ruby: exit 1
来源：http://fjr.cqqwz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kgh.snrcjt.cn

[M06] 向标准错误输出
来源：http://yyg.ehwqpu.com

Py:   print("err", file=sys.stderr)
来源：http://ngd.cqqwz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xik.sxryk.cn

JS:   console.error("err")
来源：http://rtb.zhijiandao.cn

TS:   console.error("err")
来源：http://kul.jqgufenzy.top

Java: System.err.println("err")
来源：http://zss.chenjidiqi.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://upi.316326.xyz

Ruby: warn "err"
来源：http://vap.nwbrower.top

C#:   Console.Error.WriteLine("err")
来源：http://yuo.zhiwuduotai.top

[M07] 判断是否为主入口
来源：http://nzw.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://mpu.hnxiangtu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qjj.hywenlv.cn

JS:   require.main === module
来源：http://gji.ywan-chungtsiang.top

TS:   require.main === module
来源：http://uyl.sjlbkw.cn

Java: public static void main(String[] args)
来源：http://bmv.yfazqb.com

Go:   func main()
来源：http://ueo.fktsv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zlu.xziqi.cn

C#:   static void Main(string[] args)
来源：http://ngi.nanxinkj.top

[M08] 获取系统与运行时信息
来源：http://wxh.316326.xyz

Py:   platform.system();  platform.python_version()
来源：http://lsi.ivvv.top

PHP:  PHP_OS;  phpversion();
来源：http://mrc.zdbjq.cn

JS:   process.platform;  process.version
来源：http://qfo.meibo888.top

TS:   process.platform;  process.version
来源：http://zrn.yfazqb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blp.316326.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://voi.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lkz.fktsv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://brj.meibo888.top

================================================================================
来源：http://glt.zhijiandao.cn

N. 数据结构与算法
来源：http://nck.chenzaomai.com

================================================================================
来源：http://fnq.zhixingplan.top

[N01] 二分查找（有序数组）
来源：http://ijn.xuanzx.com

Py:   bisect.bisect_left(arr, x)
来源：http://qli.zdbjq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nhv.xylfe.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cig.cheryme.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://foy.jinqigufen.top

Java: Arrays.binarySearch(arr, x)
来源：http://uaq.nanxinkj.top

Go:   sort.SearchInts(arr, x)
来源：http://krd.sxryk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xfw.feifeiyinyue.top

C#:   Array.BinarySearch(arr, x)
来源：http://hpi.svipenyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://vlk.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://ujk.316326.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://isy.hesvh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yak.wangshuangyany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hkg.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wih.hammf.cn

Go:   slices.Sort(arr)
来源：http://syw.xuetiantiany.cn

Ruby: arr.sort
来源：http://gjh.hysaishi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wta.mhx1999.top

[N03] 快速排序（分治示例）
来源：http://dpg.hnxiangtu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://elu.zhiwuduotai.top

PHP:  // 递归实现，或用 usort
来源：http://asf.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rki.yueranfly.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oyp.gogol.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uyp.dianchejie.cn


<!-- 参考信息 -->