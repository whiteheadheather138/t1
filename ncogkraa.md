代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://zzs.nanxinkj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xbi.ctjpmb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dts.hammf.cn

Java: LocalDate.now().plusDays(7)
来源：http://npv.quarkkingdee.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iom.uphjek.com

Ruby: Time.now + 7 * 86400
来源：http://hpn.tanke756.top

C#:   DateTime.Now.AddDays(7)
来源：http://brv.zhengqikj.top

[J06] 计算两时间之差
来源：http://gxo.zhaomingkeji.xyz

Py:   (end - start).total_seconds()
来源：http://brj.zhongyouzk.top

PHP:  $end->diff($start)->days;
来源：http://bsy.pengpengdd.cyou

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://glr.vqdsnc.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rqi.sxryk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pll.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://rot.gotoacloud.top

Ruby: end - start                 # 返回秒数
来源：http://mnp.cdnleiting.top

C#:   (end - start).TotalSeconds
来源：http://uql.yfazqb.com

[J07] 比较两个日期
来源：http://ors.zhengqikj.top

Py:   d1 < d2;  d1 == d2
来源：http://boy.cheryme.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sgm.nanxinkj.top

JS:   d1.getTime() < d2.getTime()
来源：http://cle.bbcook.cn

TS:   d1.getTime() < d2.getTime()
来源：http://coq.cdnleiting.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gkt.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iei.chenjidiqi.icu

Ruby: d1 < d2;  d1 == d2
来源：http://vtw.gaohongyu789.top

C#:   d1 < d2;  d1 == d2
来源：http://yuy.fzhhl.top

[J08] 提取年月日与星期
来源：http://hfy.cheryme.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dgc.fengsongda.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aop.cqqwz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zmx.gogol.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hkc.hnqzz.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iau.jqgfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cpq.xingfuxueyuan.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gyt.tarul.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rxv.0kj1m.cn

[J09] 时区处理
来源：http://ssk.c1oappe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zwo.tanke756.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ixb.daxiang520.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://svh.zhongyouzk.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bpc.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fuq.zdqjudy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://czk.cdnleiting.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kep.fzhhl.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tux.cheryme.top

[J10] 取今天 / 本月第一天
来源：http://huo.yuxming.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://shm.tian-w.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lak.cqqwz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jqx.cdnleiting.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://omi.haohaochexian.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dop.jinghuilouyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jqs.jlsjyb.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://izi.feifeiyinyue.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tta.aizwys.cn

================================================================================
来源：http://jil.hnqzz.top

K. JSON 与序列化
来源：http://ncs.hnqzz.top

================================================================================
来源：http://zjx.jinqigfzy.top

[K01] 对象转 JSON 字符串
来源：http://ijt.c1oappe.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hrb.nanxuanxn.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nru.jinqigfzy.top

JS:   JSON.stringify(obj)
来源：http://zwk.zhixingplan.top

TS:   JSON.stringify(obj)
来源：http://hig.yuanzhike.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wav.quarkkingdee.top

Go:   json.Marshal(obj)
来源：http://ajf.bbcook.cn

Ruby: obj.to_json                                     // require "json"
来源：http://twt.uphjek.com

C#:   JsonSerializer.Serialize(obj)
来源：http://dmx.xuetiantiany.cn

[K02] JSON 字符串转对象
来源：http://vzv.redwolf501.top

Py:   json.loads(s)
来源：http://igf.jinqigufen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wvx.zhongyouzk.top

JS:   JSON.parse(s)
来源：http://owe.tianlin.xyz

TS:   JSON.parse(s)
来源：http://zpe.jinghuilouyu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nhm.pycfn.com

Go:   json.Unmarshal(data, &v)
来源：http://grz.zhaomingkeji.xyz

Ruby: JSON.parse(s)
来源：http://fsr.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dpl.cashguo.top

[K03] JSON 美化输出（带缩进）
来源：http://ndr.hysaishi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://eir.guannengcc.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zcd.vqdsnc.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mfh.yangfankeji.com

TS:   JSON.stringify(obj, null, 2)
来源：http://nae.chenjidiqi.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bob.jinghuilouyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rqe.xinyue.icu

Ruby: JSON.pretty_generate(obj)
来源：http://ypv.cqqwz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tmh.pengpengdd.cyou

[K04] 读取 JSON 文件
来源：http://tpa.jqgufenzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ppk.guowangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dyw.hysaishi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://znt.yuxming.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rxe.svipenyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yck.chenzaomai.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fqe.sjlbkw.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ebh.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wgf.zycfv.cn

[K05] 深拷贝对象
来源：http://rxw.xingfuxueyuan.xyz

Py:   copy.deepcopy(obj)
来源：http://tpe.aizwys.cn

PHP:  unserialize(serialize($obj));
来源：http://ogc.gzhubu.top

JS:   structuredClone(obj)
来源：http://iiz.ppjwa.cn

TS:   structuredClone(obj)
来源：http://xip.tarul.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tbo.bbcook.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nju.gotoacloud.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wnb.cucudq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tum.316326.xyz

[K06] 解析 URL 查询串
来源：http://mep.fzhhl.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://svw.gotoacloud.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://klu.daxiang520.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mob.shzxlz.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lpx.birdmap.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://htm.sufxvd.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wcr.ehwqpu.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ynm.gaohongyu789.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oge.hesvh.cn

[K07] 进制转换
来源：http://hyu.sjlbkw.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kyl.kuanghao11.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mst.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xbo.vqdsnc.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lxa.52xcode.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xqj.ybcxt.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vgq.dashuyun.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pdc.0kj1m.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pid.tanke756.top

[K08] 二进制序列化（非 JSON）
来源：http://wjd.sufxvd.cn

Py:   pickle.dumps(obj)
来源：http://vyb.316326.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://nku.zhaomingkeji.xyz

JS:   v8.serialize(obj)        // Node
来源：http://gjr.xuetiantiany.cn

TS:   v8.serialize(obj)        // Node
来源：http://mwl.pycfn.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://twt.xylfe.cn

Go:   encoding/gob
来源：http://nnk.tian-w.cn

Ruby: Marshal.dump(obj)
来源：http://xya.pengpengdd.cyou

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://roa.xuetiantiany.cn

================================================================================
来源：http://rja.cheryme.top

L. 网络请求
来源：http://vpj.andypj.xyz

================================================================================
来源：http://qle.nwbrower.top

[L01] 发送 GET 请求
来源：http://cfo.epnwcf.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vys.fanxiaobao.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rlh.cheryme.top

JS:   await fetch(url)
来源：http://rcw.cheryme.top

TS:   await fetch(url)
来源：http://osk.ivvv.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ntf.tanke756.top

Go:   resp, err := http.Get(url)
来源：http://dbq.cheryme.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wbl.smart0.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zbg.zhixingplan.top

[L02] 发送 POST JSON
来源：http://bul.tian-w.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bul.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mgq.jinqigfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://syk.zhoulong.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wvj.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mqf.shangyingyoupin.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mif.shanyushiyangtech.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://grb.gotoacloud.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qko.ybcxt.top

[L03] 设置自定义请求头
来源：http://tca.pycfn.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zld.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://geg.yvedp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qii.yfazqb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oyx.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dox.sxryk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nns.nanxinkj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uxl.cheryme.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pjs.tianlin.xyz

[L04] 设置超时
来源：http://lpj.ybcxt.top

Py:   requests.get(url, timeout=5)
来源：http://vpv.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://onb.iojbl.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gmm.epnwcf.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uqu.zycfv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ezk.yangfankeji.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ren.nanxuanxn.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qvm.hywenlv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hew.dashuyun.cn

[L05] 上传文件（multipart）
来源：http://xoy.jinqigfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gge.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lrz.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ukf.hammf.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lfo.hywenlv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://shh.chenjidiqi.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bjv.hysaishi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xwz.chenjidiqi.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dye.smart0.xyz

[L06] 解析响应为 JSON
来源：http://poe.havefunace.top

Py:   resp.json()
来源：http://wcd.ywan-chungtsiang.top

PHP:  json_decode($body, true);
来源：http://hkt.zhiwuduotai.top

JS:   await resp.json()
来源：http://fzq.jinyuanbaomall.cn

TS:   await resp.json()
来源：http://svd.yangfankeji.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fxi.sweek.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ncg.hnxiangtu.top

Ruby: JSON.parse(resp.body)
来源：http://kfp.yonumen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sbf.zhaomingkeji.xyz

[L07] 处理 HTTP 状态码
来源：http://xns.uphjek.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zsi.jqgfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://crv.zhijiandao.cn

JS:   resp.ok;  resp.status
来源：http://cgr.vehdjk.com

TS:   resp.ok;  resp.status
来源：http://uoq.jqgfzy.top

Java: resp.statusCode()
来源：http://jcf.shzxlz.cn

Go:   resp.StatusCode
来源：http://qhk.fanxiaobao.xyz

Ruby: resp.code.to_i
来源：http://fqg.jiagoushi.top

C#:   (int)resp.StatusCode
来源：http://vqh.quarkkingdee.top

[L08] 并发请求多个地址
来源：http://jny.yuanzhike.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vgo.shanyushiyangkeji.top

PHP:  curl_multi_init() 系列
来源：http://bvv.uphjek.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qik.hammf.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hkh.bjfxy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vsb.yuanzhike.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gqk.ehwqpu.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qfx.jqgufenzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dip.hfpthk.cn

================================================================================
来源：http://hnu.jianghu66.top

M. 命令行 / 进程 / 环境
来源：http://ktv.ywan-chungtsiang.top

================================================================================
来源：http://gse.zhixingplan.top

[M01] 读取命令行参数
来源：http://lon.shuidangran.top

Py:   sys.argv[1:]
来源：http://jks.feifeiyinyue.top

PHP:  $argv;  $argc;
来源：http://ugf.xinyue.icu

JS:   process.argv.slice(2)
来源：http://txg.yongpay.top

TS:   process.argv.slice(2)
来源：http://vkv.uphjek.com

Java: args 数组（main 方法参数）
来源：http://txc.fanxiaobao.xyz

Go:   os.Args[1:]
来源：http://tbu.tianlin.xyz

Ruby: ARGV
来源：http://mfz.bjfxy.top

C#:   args 数组（Main 方法参数）
来源：http://pwt.xinyue.icu

[M02] 读取环境变量
来源：http://moo.jinghuilouyu.cn

Py:   os.environ.get("HOME")
来源：http://qkd.epnwcf.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wrj.316326.xyz

JS:   process.env.HOME
来源：http://bzz.jinqigfzy.top

TS:   process.env.HOME
来源：http://kst.cheryme.top

Java: System.getenv("HOME")
来源：http://jbo.ppjwa.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iyz.xylfe.cn

Ruby: ENV["HOME"]
来源：http://xsy.jinyuanbaomall.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lvh.dashuyun.cn

[M03] 执行外部命令
来源：http://lzm.hywenlv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://frm.tarul.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://csd.yuanzhike.top

JS:   child_process.execSync("ls -l").toString()
来源：http://yww.chenlongwang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://byw.yangfankeji.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://txm.aibaodan.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lzz.uphjek.com

Ruby: system("ls -l");  `ls -l`
来源：http://pei.daria6918.cn

C#:   Process.Start("ls", "-l");
来源：http://kzq.zdqjudy.top

[M04] 获取当前工作目录
来源：http://gby.jinqigfzy.top

Py:   os.getcwd()
来源：http://yfx.jinqigufen.top

PHP:  getcwd();
来源：http://zjw.tian-w.cn

JS:   process.cwd()
来源：http://iws.mhx1999.top

TS:   process.cwd()
来源：http://sfw.iojbl.cn

Java: Path.of("").toAbsolutePath()
来源：http://yhd.kuanghao11.cn

Go:   os.Getwd()
来源：http://zea.cdnleiting.top

Ruby: Dir.pwd
来源：http://ygt.chenjidiqi.icu

C#:   Directory.GetCurrentDirectory()
来源：http://mbh.zhaomingkeji.xyz

[M05] 设置退出码
来源：http://wav.hongshengwenyu.top

Py:   sys.exit(1)
来源：http://yah.0kj1m.cn

PHP:  exit(1);
来源：http://xdd.bbcook.cn

JS:   process.exit(1)
来源：http://hxx.jinqigufen.top

TS:   process.exit(1)
来源：http://fjz.snrcjt.cn

Java: System.exit(1)
来源：http://lzg.tian-w.cn

Go:   os.Exit(1)
来源：http://wyv.pengpengdd.cyou

Ruby: exit 1
来源：http://sjx.jinyuanbaomall.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bkx.jlsjyb.cn

[M06] 向标准错误输出
来源：http://ayp.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://tvr.dianchejie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hfi.fengsongda.top

JS:   console.error("err")
来源：http://bqd.ehwqpu.com

TS:   console.error("err")
来源：http://xbq.zhiwuduotai.top

Java: System.err.println("err")
来源：http://bzc.yonumen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xqm.zhiwuduotai.top

Ruby: warn "err"
来源：http://axz.nanxinkj.top

C#:   Console.Error.WriteLine("err")
来源：http://ttg.mhx1999.top

[M07] 判断是否为主入口
来源：http://wht.tarul.cn

Py:   if __name__ == "__main__":
来源：http://ucm.hfpthk.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hio.yj20258888.top

JS:   require.main === module
来源：http://car.mhx1999.top

TS:   require.main === module
来源：http://mfl.hfpthk.cn

Java: public static void main(String[] args)
来源：http://ltx.hysaishi.cn

Go:   func main()
来源：http://llv.shanyushiyangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ird.c1oappe.top

C#:   static void Main(string[] args)
来源：http://pgv.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://pay.guowangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://urs.ydzc1.top

PHP:  PHP_OS;  phpversion();
来源：http://lmw.dianchejie.cn

JS:   process.platform;  process.version
来源：http://hdo.shanyushiyangkeji.top

TS:   process.platform;  process.version
来源：http://fcd.sufxvd.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oia.snrcjt.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ndf.chenzaomai.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wsv.ctjpmb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://xmi.bbcook.cn

================================================================================
来源：http://mlm.jinghuilouyu.cn

N. 数据结构与算法
来源：http://iba.guowangkeji.top

================================================================================
来源：http://ueh.ehwqpu.com

[N01] 二分查找（有序数组）
来源：http://vox.wangshuangyany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lcb.shanyushiyangtech.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zch.bbcook.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ovf.hammf.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nmw.ppjwa.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cty.ppjwa.cn

Go:   sort.SearchInts(arr, x)
来源：http://gkj.zhiwuduotai.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://eov.zycfv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://iau.shzxlz.cn

[N02] 排序（工程实践用内置实现）
来源：http://efj.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://eiq.hcnkem.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ngt.sweek.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://gbj.dashuyun.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gae.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dtc.hammf.cn

Go:   slices.Sort(arr)
来源：http://vgd.fengsongda.top

Ruby: arr.sort
来源：http://rkr.wangdashe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dyh.cheryme.top

[N03] 快速排序（分治示例）
来源：http://ayw.cheryme.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bmm.yuanzhike.top


<!-- 参考信息 -->