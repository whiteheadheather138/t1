代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hmz.jlsjyb.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pti.meibo888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://les.nanxinkj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fgi.fehbvm.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xlu.zdbjq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://twl.fengsongda.top

[J05] 时间加减（加 7 天）
来源：http://fnm.chenlongwang.top

Py:   now + timedelta(days=7)
来源：http://otg.hcnkem.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://kgy.shanyushiyangtech.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kdg.zhoulong.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pjs.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://pne.iojbl.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://byn.kuanghao11.cn

Ruby: Time.now + 7 * 86400
来源：http://ifx.snrcjt.cn

C#:   DateTime.Now.AddDays(7)
来源：http://igs.gogol.net.cn

[J06] 计算两时间之差
来源：http://nmq.hnxiangtu.top

Py:   (end - start).total_seconds()
来源：http://lco.chenlongwang.top

PHP:  $end->diff($start)->days;
来源：http://qkz.gogol.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ynu.daria6918.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rnb.yj20258.top

Java: Duration.between(start, end).toSeconds()
来源：http://ttq.sysykeji.top

Go:   end.Sub(start).Hours()
来源：http://snp.ydzc1.top

Ruby: end - start                 # 返回秒数
来源：http://heu.9152youxi.cn

C#:   (end - start).TotalSeconds
来源：http://fwi.tianlin.xyz

[J07] 比较两个日期
来源：http://oyx.xingfuxueyuan.xyz

Py:   d1 < d2;  d1 == d2
来源：http://ukt.cashguo.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gob.jinqigufen.top

JS:   d1.getTime() < d2.getTime()
来源：http://akg.dianchejie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cij.xuanzx.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uip.ydzc1.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rkl.yongpay.top

Ruby: d1 < d2;  d1 == d2
来源：http://eqb.epnwcf.com

C#:   d1 < d2;  d1 == d2
来源：http://vja.hnqzz.top

[J08] 提取年月日与星期
来源：http://nix.nanxinkj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ubw.jinyuanbaomall.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cni.shanyushiyangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nnc.svipenyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yex.9152youxi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://euh.jinqigufen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ekm.vqdsnc.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://shb.zhiwuduotai.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mrd.pengpengdd.cyou

[J09] 时区处理
来源：http://hee.yuanzhike.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://deg.andypj.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mdl.jinghuilouyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nbv.52xcode.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nim.zhixingplan.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://soc.jinyuanbaomall.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hoi.316326.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://vej.hysaishi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://llj.shanyushiyangtech.top

[J10] 取今天 / 本月第一天
来源：http://jsx.tanke756.top

Py:   date.today();  date.today().replace(day=1)
来源：http://oxx.hesvh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://opi.shangyingyoupin.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bom.zdbjq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ftd.shanyushiyangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dyj.shanyushiyangtech.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://edg.shanyushiyangtech.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://aaf.meibo888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qsk.mhx1999.top

================================================================================
来源：http://wzy.jqgfzy.top

K. JSON 与序列化
来源：http://qkt.dashuyun.cn

================================================================================
来源：http://jth.yonumen.top

[K01] 对象转 JSON 字符串
来源：http://gzc.zycfv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lew.ydjk.org.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kuf.zhixingplan.top

JS:   JSON.stringify(obj)
来源：http://ajc.tanke756.top

TS:   JSON.stringify(obj)
来源：http://xvw.fzhhl.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jtc.aibaodan.cn

Go:   json.Marshal(obj)
来源：http://hdd.mhx1999.top

Ruby: obj.to_json                                     // require "json"
来源：http://cqi.sufxvd.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://klz.dashuyun.cn

[K02] JSON 字符串转对象
来源：http://ozj.ehwqpu.com

Py:   json.loads(s)
来源：http://uud.shanyushiyangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://niq.jianghu66.top

JS:   JSON.parse(s)
来源：http://buq.c1oappe.top

TS:   JSON.parse(s)
来源：http://nsi.sxryk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://eoy.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://scw.zhixingplan.top

Ruby: JSON.parse(s)
来源：http://cmd.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tda.xuetiantiany.cn

[K03] JSON 美化输出（带缩进）
来源：http://qmd.jianghu66.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://icr.zdbjq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dmf.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xah.dianchejie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tut.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vsl.cashguo.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hhj.iojbl.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ssb.meibo888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nhk.shzxlz.cn

[K04] 读取 JSON 文件
来源：http://hfg.hesvh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nyy.chenjidiqi.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rrb.pengpengdd.cyou

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rdn.9152youxi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://exa.daria6918.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lkv.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mjd.guowangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sbn.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fpn.c1oappe.top

[K05] 深拷贝对象
来源：http://eee.yfazqb.com

Py:   copy.deepcopy(obj)
来源：http://kul.yfazqb.com

PHP:  unserialize(serialize($obj));
来源：http://ldj.hywenlv.cn

JS:   structuredClone(obj)
来源：http://zsk.tanke756.top

TS:   structuredClone(obj)
来源：http://qzu.yanxiufei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zaz.andypj.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lbc.yanxiufei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oxa.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ijm.chenlongwang.top

[K06] 解析 URL 查询串
来源：http://ofz.yanxiufei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qkn.nanxinkj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tog.ivvv.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zse.yj20258.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://agj.xuetiantiany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qaf.zhoulong.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://grf.jqgfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vho.kuanghao11.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eef.yanxiufei.cn

[K07] 进制转换
来源：http://cjo.svipenyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ltd.hnqzz.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jjm.ctjpmb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mfd.vqdsnc.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jaf.zycfv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://itc.52xcode.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bpb.uphjek.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nhy.cashguo.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iwx.havefunace.top

[K08] 二进制序列化（非 JSON）
来源：http://kca.nanxuanxn.top

Py:   pickle.dumps(obj)
来源：http://ycn.aizwys.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kfx.jlsjyb.cn

JS:   v8.serialize(obj)        // Node
来源：http://iwi.cheryme.top

TS:   v8.serialize(obj)        // Node
来源：http://wcw.andypj.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ijx.sjlbkw.cn

Go:   encoding/gob
来源：http://dcn.mhx1999.top

Ruby: Marshal.dump(obj)
来源：http://ydw.fzhhl.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qjc.uphjek.com

================================================================================
来源：http://mug.hysaishi.cn

L. 网络请求
来源：http://ugq.316326.xyz

================================================================================
来源：http://joz.mhx1999.top

[L01] 发送 GET 请求
来源：http://xao.bjfxy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kwl.nanxuanxn.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kwu.hcnkem.com

JS:   await fetch(url)
来源：http://rbh.yangfankeji.com

TS:   await fetch(url)
来源：http://gge.smart0.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dyv.sysykeji.top

Go:   resp, err := http.Get(url)
来源：http://scg.shanyushiyangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jvv.quarkkingdee.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vry.ydzc1.top

[L02] 发送 POST JSON
来源：http://cgf.bjfxy.top

Py:   requests.post(url, json={"a": 1})
来源：http://fwu.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ghw.quarkkingdee.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ady.chenlongwang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tws.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qdf.sweek.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lrk.mhx1999.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uch.zhongyouzk.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ipz.daxiang520.top

[L03] 设置自定义请求头
来源：http://fvh.guowangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oul.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://moq.gzhubu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fjl.jqgfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tof.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ktd.zdqjudy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sig.zdqjudy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nrw.jinqigufen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nsz.nanxuanxn.top

[L04] 设置超时
来源：http://nvt.yonumen.top

Py:   requests.get(url, timeout=5)
来源：http://yys.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lrx.zhengqikj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cxj.yfazqb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bdm.yonumen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://csi.zhongyouzk.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hpj.sxryk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vdj.hcnkem.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://acu.zhiwuduotai.top

[L05] 上传文件（multipart）
来源：http://nis.yueranfly.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oos.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dgl.uphjek.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rlw.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://owe.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kjf.yj20258888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gxn.birdmap.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cgz.ppjwa.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tyc.xinyue.icu

[L06] 解析响应为 JSON
来源：http://fnu.jinqigufen.top

Py:   resp.json()
来源：http://feu.daxiang520.top

PHP:  json_decode($body, true);
来源：http://hpx.svipenyu.cn

JS:   await resp.json()
来源：http://ytz.yueranfly.top

TS:   await resp.json()
来源：http://gtc.yj20258.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xvw.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://aoy.ydzc1.top

Ruby: JSON.parse(resp.body)
来源：http://hzf.smart0.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ywm.sufxvd.cn

[L07] 处理 HTTP 状态码
来源：http://mar.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qkq.zhixingplan.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bul.xuetiantiany.cn

JS:   resp.ok;  resp.status
来源：http://xzv.jqgufenzy.top

TS:   resp.ok;  resp.status
来源：http://kvp.hcnkem.com

Java: resp.statusCode()
来源：http://wup.jianghu66.top

Go:   resp.StatusCode
来源：http://cau.sysykeji.top

Ruby: resp.code.to_i
来源：http://amp.ivvv.top

C#:   (int)resp.StatusCode
来源：http://jnp.sxryk.cn

[L08] 并发请求多个地址
来源：http://bln.ydzc1.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tlt.shanyushiyangkeji.top

PHP:  curl_multi_init() 系列
来源：http://feq.jiagoushi.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kad.cdnleiting.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vbz.quarkkingdee.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mua.gaohongyu789.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dke.fktsv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jfj.xuanzx.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ijf.snrcjt.cn

================================================================================
来源：http://bas.jyoumei.cn

M. 命令行 / 进程 / 环境
来源：http://zpe.cheryme.top

================================================================================
来源：http://uox.zdqjudy.top

[M01] 读取命令行参数
来源：http://bvs.sysykeji.top

Py:   sys.argv[1:]
来源：http://syn.redwolf501.top

PHP:  $argv;  $argc;
来源：http://zaa.gotoacloud.top

JS:   process.argv.slice(2)
来源：http://ufw.jinyuanbaomall.cn

TS:   process.argv.slice(2)
来源：http://ohr.yuxming.cn

Java: args 数组（main 方法参数）
来源：http://vzy.yonumen.top

Go:   os.Args[1:]
来源：http://tan.zdbjq.cn

Ruby: ARGV
来源：http://qun.52xcode.cn

C#:   args 数组（Main 方法参数）
来源：http://kps.jyoumei.cn

[M02] 读取环境变量
来源：http://dws.zhongyouzk.top

Py:   os.environ.get("HOME")
来源：http://ayc.tian-w.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zfl.bjfxy.top

JS:   process.env.HOME
来源：http://xcc.yj20258888.top

TS:   process.env.HOME
来源：http://lag.chenlongwang.top

Java: System.getenv("HOME")
来源：http://zkh.pycfn.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://awv.shzxlz.cn

Ruby: ENV["HOME"]
来源：http://ndt.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rgo.kuanghao11.cn

[M03] 执行外部命令
来源：http://oqc.ctjpmb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rfp.shuidangran.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jia.cheryme.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wer.xuetiantiany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ktr.xingfuxueyuan.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tho.52xcode.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pel.dashuyun.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zrr.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://rzo.hesvh.cn

[M04] 获取当前工作目录
来源：http://oyr.hysaishi.cn

Py:   os.getcwd()
来源：http://eal.ydzc1.top

PHP:  getcwd();
来源：http://dfi.bjfxy.top

JS:   process.cwd()
来源：http://efe.yj202588.top

TS:   process.cwd()
来源：http://fzx.zhengqikj.top

Java: Path.of("").toAbsolutePath()
来源：http://vxz.zhaomingkeji.xyz

Go:   os.Getwd()
来源：http://uwb.birdmap.top

Ruby: Dir.pwd
来源：http://htj.cashguo.top

C#:   Directory.GetCurrentDirectory()
来源：http://cxg.0kj1m.cn

[M05] 设置退出码
来源：http://afu.hysaishi.cn

Py:   sys.exit(1)
来源：http://lgf.epnwcf.com

PHP:  exit(1);
来源：http://pxj.shanyushiyangtech.top

JS:   process.exit(1)
来源：http://sgk.guowangkeji.top

TS:   process.exit(1)
来源：http://izo.jinyuanbaomall.cn

Java: System.exit(1)
来源：http://xhd.gzhubu.top

Go:   os.Exit(1)
来源：http://uoa.hnqzz.top

Ruby: exit 1
来源：http://fbd.shzxlz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vqb.fktsv.cn

[M06] 向标准错误输出
来源：http://xmd.jyoumei.cn

Py:   print("err", file=sys.stderr)
来源：http://spu.yonumen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kbm.gaohongyu789.top

JS:   console.error("err")
来源：http://ybf.hnqzz.top

TS:   console.error("err")
来源：http://mvo.tarul.cn

Java: System.err.println("err")
来源：http://mzn.zdbjq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hpf.uphjek.com

Ruby: warn "err"
来源：http://woh.vqdsnc.cn

C#:   Console.Error.WriteLine("err")
来源：http://kjj.meibo888.top

[M07] 判断是否为主入口
来源：http://bqp.zhongyouzk.top

Py:   if __name__ == "__main__":
来源：http://bhm.hammf.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nxn.hongshengwenyu.top

JS:   require.main === module
来源：http://epl.jinghuilouyu.cn

TS:   require.main === module
来源：http://hvp.xziqi.cn

Java: public static void main(String[] args)
来源：http://gra.hesvh.cn

Go:   func main()
来源：http://prg.havefunace.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dba.vqdsnc.cn

C#:   static void Main(string[] args)
来源：http://tly.epnwcf.com

[M08] 获取系统与运行时信息
来源：http://evi.kuanghao11.cn

Py:   platform.system();  platform.python_version()
来源：http://pvh.iojbl.cn

PHP:  PHP_OS;  phpversion();
来源：http://rcj.yj202588.top

JS:   process.platform;  process.version
来源：http://afg.wangdashe.top

TS:   process.platform;  process.version
来源：http://jyz.aizwys.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gxd.smart0.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://swu.hcnkem.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uen.ppjwa.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dqh.jlsjyb.cn

================================================================================
来源：http://gde.yongpay.top

N. 数据结构与算法
来源：http://jmg.havefunace.top

================================================================================
来源：http://lop.hnxiangtu.top

[N01] 二分查找（有序数组）
来源：http://opc.fehbvm.com

Py:   bisect.bisect_left(arr, x)
来源：http://uam.chenzaomai.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bfm.hywenlv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cnf.xziqi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bhg.hammf.cn

Java: Arrays.binarySearch(arr, x)
来源：http://byo.xuanzx.com

Go:   sort.SearchInts(arr, x)
来源：http://pkm.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cbj.shanyushiyangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://zhd.cdnleiting.top

[N02] 排序（工程实践用内置实现）
来源：http://fcr.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://nyu.cheryme.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rfd.zhaomingkeji.xyz


<!-- 参考信息 -->